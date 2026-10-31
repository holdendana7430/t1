代发 wailian999

#ifndef X_H
来源：http://dy.szxytkj.cn

#define X_H
来源：http://cl.gzmigu.cn

#endif
来源：http://zh.szxytkj.cn

[S31] C++：Hello World
来源：http://xk.521024.cn

#include <iostream>
来源：http://uz.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ld.yuntaijiaju.cn

[S32] C++：字符串
来源：http://vn.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://le.yuexingan06.cn

[S33] C++：vector 增删
来源：http://ra.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lk.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://ap.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://zw.nicolike.cn

[S35] C++：map
来源：http://my.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ui.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://ne.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sz.hahajie.cn

[S37] C++：set
来源：http://de.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wb.jctech888.com.cn

[S38] C++：排序
来源：http://zn.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://pd.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://qv.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fl.jianghongdianzi.cn

[S40] C++：查找元素
来源：http://wi.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fu.asd995.cn

[S41] C++：类与构造函数
来源：http://ga.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lf.nicolike.cn

[S42] C++：继承与虚函数
来源：http://bz.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://sv.haigaiapp.cn

[S43] C++：智能指针
来源：http://vj.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://bj.bjjhwx.cn

[S44] C++：引用传参
来源：http://la.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://qw.bookmarksfly.cn

[S45] C++：lambda
来源：http://sw.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pw.shxzukj.cn

[S46] C++：函数模板
来源：http://xe.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dz.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://tt.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cb.9csxet.cn

[S48] C++：逐行读文件
来源：http://jx.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lw.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://ho.wgjwhj.cn

[S49] C++：写文件
来源：http://xt.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ak.asd995.cn

[S50] C++：格式化数字
来源：http://ss.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kg.chemitech.net.cn

[S51] C++：显式类型转换
来源：http://ja.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://tv.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://zc.9csxet.cn

int size() const noexcept { return n_; }
来源：http://hy.szxytkj.cn

[S53] C++：移动语义
来源：http://es.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://fq.haigaiapp.cn

[S54] C++：异常处理
来源：http://nv.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mv.9csxet.cn

[S55] C++：结构化绑定
来源：http://bs.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://si.newstarts.cn

[S56] C++：optional
来源：http://mt.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ya.szxytkj.cn

[S57] C++：编译期常量
来源：http://dg.huanxung.cn

constexpr int N = 10;
来源：http://kl.shtwfgs.cn

[S58] C++：命名空间
来源：http://mt.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://mq.haigaiapp.cn

[S59] C++：静态断言
来源：http://it.shxzukj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aq.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://gg.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rn.shtwfgs.cn

================================================================================
来源：http://ow.lnxyls.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ne.9csxet.cn

================================================================================
来源：http://mv.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://vc.bookmarksfly.cn

println("Hello")
来源：http://kg.colortex.cn

[T02] Kotlin：变量
来源：http://nt.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ru.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://bc.colortex.cn

"值: $b"
来源：http://ra.nszjky.cn

[T04] Kotlin：空安全
来源：http://ij.shxzukj.cn

val n: String? = null;  n?.length
来源：http://ea.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://do.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bu.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://rx.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ff.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://nh.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gw.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://qn.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://gp.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://jp.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://zj.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://id.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ai.panjiajie.cn

[T11] Kotlin：协程
来源：http://iy.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fs.wgjwhj.cn

[T12] Kotlin：解构声明
来源：http://sj.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://tv.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://xb.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://jw.jctech888.com.cn

[T14] Kotlin：循环
来源：http://bh.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://mz.panjiajie.cn

[T15] Kotlin：接口
来源：http://vb.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://lz.huixiangedu.cn

[T16] Swift：Hello World
来源：http://it.yuntaijiaju.cn

print("Hello")
来源：http://qy.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://jy.shxzskj.cn

var a = 1;  let b = 2
来源：http://pi.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://sm.yuexingan06.cn

"值: \(b)"
来源：http://xp.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://di.9csxet.cn

if let n = opt { print(n) }
来源：http://nt.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://ld.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://he.huixiangedu.cn

[T21] Swift：遍历
来源：http://ak.panjiajie.cn

for x in a { print(x) }
来源：http://ac.yuexingan06.cn

[T22] Swift：字典
来源：http://kp.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://il.shxzskj.cn

[T23] Swift：函数
来源：http://gs.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ug.bookmarksfly.cn

[T24] Swift：闭包
来源：http://uk.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fb.asd995.cn

[T25] Swift：结构体
来源：http://pc.bookmarksfly.cn

struct P { var x: Int }
来源：http://op.hnjuh.cn

[T26] Swift：类与重写
来源：http://xv.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://rr.huanxung.cn

[T27] Swift：错误处理
来源：http://cd.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://mu.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://ws.huixinmuqiang.cn

enum Color { case red, green }
来源：http://cz.521024.cn

[T29] Swift：guard 提前返回
来源：http://uy.huanxung.cn

guard let x = opt else { return }
来源：http://ty.gzmigu.cn

[T30] Swift：协议
来源：http://qg.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://hj.nicolike.cn

[T31] Lua：Hello World
来源：http://vp.shxzskj.cn

print("Hello")
来源：http://fh.huanxung.cn

[T32] Lua：局部变量
来源：http://ic.gzmigu.cn

local a = 1
来源：http://so.9csxet.cn

[T33] Lua：表（数组）
来源：http://bk.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fu.haigaiapp.cn

[T34] Lua：遍历表
来源：http://ge.521024.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ma.yuexingan06.cn

[T35] Lua：字典表
来源：http://hj.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://xm.shxzskj.cn

[T36] Lua：函数
来源：http://zr.lnxyls.cn

function add(a, b) return a + b end
来源：http://qu.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://rh.muxihuayi.cn

"a" .. "b"
来源：http://ew.newstarts.cn

[T38] Lua：条件
来源：http://iv.wgjwhj.cn

if x > 0 then print("正") end
来源：http://bk.nicolike.cn

[T39] Lua：模式匹配
来源：http://pv.9csxet.cn

string.find(s, "%d+")
来源：http://br.huixinmuqiang.cn

[T40] Lua：元表
来源：http://ho.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://fi.panjiajie.cn

[T41] Perl：Hello World
来源：http://qe.bjjhwx.cn

print "Hello\n";
来源：http://ia.shxzskj.cn

[T42] Perl：变量类型
来源：http://re.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sm.newstarts.cn

[T43] Perl：字符串插值
来源：http://ne.muxihuayi.cn

"值: $a"
来源：http://qo.haigaiapp.cn

[T44] Perl：条件
来源：http://en.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://dh.szxytkj.cn

[T45] Perl：数组遍历
来源：http://rw.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://ae.nszjky.cn

[T46] Perl：哈希操作
来源：http://eh.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://go.hahajie.cn

[T47] Perl：正则捕获
来源：http://xs.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zd.newstarts.cn

[T48] Perl：正则替换
来源：http://un.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://ju.huixiangedu.cn

[T49] Perl：函数
来源：http://am.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ar.szsharing.cn

[T50] Perl：逐行读文件
来源：http://zq.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://du.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://wh.shtwfgs.cn

[T51] Scala：Hello World
来源：http://ro.521024.cn

println("Hello")
来源：http://db.yuexingan06.cn

[T52] Scala：变量
来源：http://lk.nicolike.cn

val a = 1;  var b = 2
来源：http://sr.521024.cn

[T53] Scala：字符串插值
来源：http://tq.szsharing.cn

s"值: $b"
来源：http://en.huixiangedu.cn

[T54] Scala：集合映射
来源：http://oh.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://js.nicolike.cn

[T55] Scala：集合过滤
来源：http://jn.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fo.chemitech.net.cn

[T56] Scala：样例类
来源：http://to.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://ju.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://ql.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xi.lnxyls.cn

[T58] Scala：函数定义
来源：http://jm.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kf.wgjwhj.cn

[T59] Scala：循环
来源：http://dk.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://yn.bjjhwx.cn

[T60] Scala：折叠
来源：http://ht.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rr.hnjuh.cn

================================================================================
来源：http://ft.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pf.yuntaijiaju.cn

================================================================================
来源：http://qu.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://uq.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://os.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://in.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zf.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://bc.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vm.hnjuh.cn

[U04] Py：变量调试打印
来源：http://wp.wgjwhj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://go.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://ve.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://fv.shxzskj.cn

[U06] Py：合并两个字典
来源：http://na.muxihuayi.cn

{**a, **b}
来源：http://wh.9csxet.cn

[U07] Py：反转字典键值
来源：http://lh.9csxet.cn

{v: k for k, v in d.items()}
来源：http://cm.521024.cn

[U08] Py：展平二维列表
来源：http://mn.9csxet.cn

[y for x in nested for y in x]
来源：http://hq.colortex.cn

[U09] Py：字典取最大值的键
来源：http://pr.bjjhwx.cn

max(d, key=d.get)
来源：http://kz.shxzukj.cn

[U10] Py：按值排序字典
来源：http://fb.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wm.szxytkj.cn

[U11] Py：生成器表达式
来源：http://ox.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://eq.asd995.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mg.hnjuh.cn

Counter(arr).most_common(3)
来源：http://yz.asd995.cn

[U13] Py：固定长度队列
来源：http://vk.panjiajie.cn

deque(maxlen=10)
来源：http://hh.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://xn.nicolike.cn

defaultdict(list)
来源：http://pm.bookmarksfly.cn

[U15] Py：高精度计时
来源：http://jk.chemitech.net.cn

t = time.perf_counter()
来源：http://be.jctech888.com.cn

[U16] Py：命令行参数解析
来源：http://qj.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ho.wgjwhj.cn

[U17] Py：初始化日志
来源：http://vo.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://lk.newstarts.cn

[U18] Py：预编译正则
来源：http://xn.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://an.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://wk.newstarts.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zf.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://kz.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://kn.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://iy.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://zk.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://dg.colortex.cn

list(zip(*m))
来源：http://pb.newstarts.cn

[U23] Py：分块读取大文件
来源：http://rw.jianghongdianzi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nj.yuexingan06.cn

[U24] Py：路径操作
来源：http://dc.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://or.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://yz.521024.cn

csv.DictReader(f)
来源：http://yk.huixinmuqiang.cn

[U26] Py：并发下载
来源：http://kb.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uk.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://yy.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://pb.521024.cn

[U28] Py：类型别名
来源：http://fj.huixiangedu.cn

UserId = int
来源：http://ge.huanxung.cn

[U29] Py：属性校验
来源：http://vk.9csxet.cn

@property 与 @x.setter 配合
来源：http://ue.hahajie.cn

[U30] Py：数据类
来源：http://vq.panjiajie.cn

@dataclass(slots=True)
来源：http://hl.newstarts.cn

[U31] Py：单测
来源：http://xx.shxzukj.cn

python -m pytest -q
来源：http://ta.chemitech.net.cn

[U32] Py：代码格式化
来源：http://sd.asd995.cn

ruff format . && ruff check --fix .
来源：http://az.colortex.cn

[U33] Py：打包发布
来源：http://cg.haigaiapp.cn

python -m build  （依赖 pyproject.toml）
来源：http://iy.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://in.shxzukj.cn

chardet.detect(raw)
来源：http://jn.chemitech.net.cn

[U35] Py：发送邮件
来源：http://qd.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eo.shxzskj.cn

[U36] Py：定时任务
来源：http://ea.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://xc.lnxyls.cn

[U37] Py：读写 Excel
来源：http://ok.asd995.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sq.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://sv.jctech888.com.cn

Path(__file__).resolve().parent
来源：http://kk.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://dr.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://ig.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://ap.huanxung.cn

print("err", file=sys.stderr)
来源：http://cm.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://ap.szsharing.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ak.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://od.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xg.jctech888.com.cn

[U43] PHP：声明命名空间
来源：http://sh.lnxyls.cn

namespace App\Http;
来源：http://qv.yuntaijiaju.cn

[U44] PHP：开启严格类型
来源：http://xa.huixiangedu.cn

declare(strict_types=1);
来源：http://ki.huanxung.cn

[U45] PHP：类型声明与返回类型
来源：http://gz.bjjhwx.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://eh.muxihuayi.cn

[U46] PHP：可空类型
来源：http://ft.hahajie.cn

?string $name = null
来源：http://us.nszjky.cn

[U47] PHP：联合类型
来源：http://fd.lnxyls.cn

int|string $id
来源：http://mp.shxzukj.cn

[U48] PHP：纯枚举
来源：http://kt.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jc.hahajie.cn

[U49] PHP：只读属性
来源：http://nx.colortex.cn

public readonly string $name
来源：http://hp.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://rx.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://ye.szxytkj.cn

[U51] PHP：数组解构
来源：http://nb.nszjky.cn

[$a, $b] = $arr;
来源：http://ot.panjiajie.cn

[U52] PHP：箭头函数
来源：http://gg.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://qk.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://ih.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://cj.hahajie.cn

[U54] PHP：空安全调用
来源：http://hf.bookmarksfly.cn

$obj?->method()
来源：http://cw.asd995.cn


<!-- 参考信息 -->