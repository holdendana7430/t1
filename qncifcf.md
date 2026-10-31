代发 wailian999

memset(a, 0, sizeof a);
来源：http://xn.huixiangedu.cn

[S27] C：定义常量
来源：http://hr.nicolike.cn

const double PI = 3.14159;
来源：http://vk.panjiajie.cn

[S28] C：静态变量
来源：http://wx.wgjwhj.cn

static int counter = 0;
来源：http://yr.panjiajie.cn

[S29] C：变参函数
来源：http://af.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vd.gzmigu.cn

[S30] C：头文件保护
来源：http://so.shtwfgs.cn

#ifndef X_H
来源：http://ob.hnjuh.cn

#define X_H
来源：http://zr.huixiangedu.cn

#endif
来源：http://cm.huanxung.cn

[S31] C++：Hello World
来源：http://yh.bjjhwx.cn

#include <iostream>
来源：http://zk.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://um.bookmarksfly.cn

[S32] C++：字符串
来源：http://xl.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://oi.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://bm.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ke.newstarts.cn

[S34] C++：遍历 vector
来源：http://av.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://hz.bjjhwx.cn

[S35] C++：map
来源：http://sq.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vo.newstarts.cn

[S36] C++：unordered_map
来源：http://wi.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://on.panjiajie.cn

[S37] C++：set
来源：http://ef.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://py.jctech888.com.cn

[S38] C++：排序
来源：http://pe.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://lq.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://cn.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yl.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://cu.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kq.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://qq.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qv.521024.cn

[S42] C++：继承与虚函数
来源：http://xe.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://wk.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://nt.asd995.cn

auto p = std::make_unique<int>(5);
来源：http://xt.shxzukj.cn

[S44] C++：引用传参
来源：http://oq.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://xp.newstarts.cn

[S45] C++：lambda
来源：http://it.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nj.yuexingan06.cn

[S46] C++：函数模板
来源：http://wr.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mp.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://il.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cy.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://ix.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ij.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://yz.huixiangedu.cn

[S49] C++：写文件
来源：http://zy.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fy.jctech888.com.cn

[S50] C++：格式化数字
来源：http://hs.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vz.chemitech.net.cn

[S51] C++：显式类型转换
来源：http://wi.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://hk.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://oq.shxzukj.cn

int size() const noexcept { return n_; }
来源：http://ca.szsharing.cn

[S53] C++：移动语义
来源：http://zz.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://rr.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://ag.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ho.nszjky.cn

[S55] C++：结构化绑定
来源：http://bz.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rd.bookmarksfly.cn

[S56] C++：optional
来源：http://bv.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oc.muxihuayi.cn

[S57] C++：编译期常量
来源：http://sm.shtwfgs.cn

constexpr int N = 10;
来源：http://bq.chemitech.net.cn

[S58] C++：命名空间
来源：http://ta.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://dl.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://nx.szxytkj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ew.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://ej.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jk.521024.cn

================================================================================
来源：http://dw.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ff.newstarts.cn

================================================================================
来源：http://wf.szxytkj.cn

[T01] Kotlin：Hello World
来源：http://bv.muxihuayi.cn

println("Hello")
来源：http://xa.chemitech.net.cn

[T02] Kotlin：变量
来源：http://at.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pj.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://bi.yuntaijiaju.cn

"值: $b"
来源：http://xe.9csxet.cn

[T04] Kotlin：空安全
来源：http://qt.asd995.cn

val n: String? = null;  n?.length
来源：http://rs.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://qi.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://by.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://zm.521024.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fy.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://ys.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gz.nicolike.cn

[T08] Kotlin：数据类
来源：http://ox.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://pq.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://mo.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://cw.hahajie.cn

[T10] Kotlin：默认参数
来源：http://ee.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qh.gzmigu.cn

[T11] Kotlin：协程
来源：http://vh.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dp.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://vw.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://ej.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://mi.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://jh.shtwfgs.cn

[T14] Kotlin：循环
来源：http://kh.521024.cn

for (i in 1..10) println(i)
来源：http://wp.panjiajie.cn

[T15] Kotlin：接口
来源：http://wg.colortex.cn

interface Shape { fun area(): Double }
来源：http://yk.asd995.cn

[T16] Swift：Hello World
来源：http://up.huixiangedu.cn

print("Hello")
来源：http://kd.shxzskj.cn

[T17] Swift：变量与常量
来源：http://pq.shxzskj.cn

var a = 1;  let b = 2
来源：http://bt.9csxet.cn

[T18] Swift：字符串插值
来源：http://eo.shxzskj.cn

"值: \(b)"
来源：http://gu.hnjuh.cn

[T19] Swift：可选绑定
来源：http://vs.hnjuh.cn

if let n = opt { print(n) }
来源：http://ki.shtwfgs.cn

[T20] Swift：数组操作
来源：http://wv.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ef.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://lx.shxzukj.cn

for x in a { print(x) }
来源：http://wg.huixiangedu.cn

[T22] Swift：字典
来源：http://af.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zv.huanxung.cn

[T23] Swift：函数
来源：http://pz.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ut.shtwfgs.cn

[T24] Swift：闭包
来源：http://da.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://is.hnjuh.cn

[T25] Swift：结构体
来源：http://mh.jianghongdianzi.cn

struct P { var x: Int }
来源：http://ae.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://mf.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://nz.chemitech.net.cn

[T27] Swift：错误处理
来源：http://af.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://eu.nicolike.cn

[T28] Swift：枚举
来源：http://zn.wgjwhj.cn

enum Color { case red, green }
来源：http://hj.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://zu.nszjky.cn

guard let x = opt else { return }
来源：http://jg.shtwfgs.cn

[T30] Swift：协议
来源：http://yf.newstarts.cn

protocol Shape { func area() -> Double }
来源：http://xz.wgjwhj.cn

[T31] Lua：Hello World
来源：http://bi.szsharing.cn

print("Hello")
来源：http://dh.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://em.haigaiapp.cn

local a = 1
来源：http://vu.szsharing.cn

[T33] Lua：表（数组）
来源：http://wd.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xv.panjiajie.cn

[T34] Lua：遍历表
来源：http://mg.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qf.szxytkj.cn

[T35] Lua：字典表
来源：http://uz.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://fo.jianghongdianzi.cn

[T36] Lua：函数
来源：http://zb.szsharing.cn

function add(a, b) return a + b end
来源：http://bn.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://gx.huixinmuqiang.cn

"a" .. "b"
来源：http://ne.chemitech.net.cn

[T38] Lua：条件
来源：http://du.gzmigu.cn

if x > 0 then print("正") end
来源：http://bu.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://pu.muxihuayi.cn

string.find(s, "%d+")
来源：http://lf.521024.cn

[T40] Lua：元表
来源：http://jp.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://kk.nicolike.cn

[T41] Perl：Hello World
来源：http://jd.bookmarksfly.cn

print "Hello\n";
来源：http://ji.nszjky.cn

[T42] Perl：变量类型
来源：http://dk.hnjuh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jx.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://ox.asd995.cn

"值: $a"
来源：http://qj.haigaiapp.cn

[T44] Perl：条件
来源：http://lx.gzmigu.cn

if ($a > 0) { print "正"; }
来源：http://uc.colortex.cn

[T45] Perl：数组遍历
来源：http://et.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://dz.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://sc.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://eg.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://ru.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pi.9csxet.cn

[T48] Perl：正则替换
来源：http://sf.shtwfgs.cn

$s =~ s/old/new/g;
来源：http://te.bjjhwx.cn

[T49] Perl：函数
来源：http://ch.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ao.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://bu.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nm.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://ky.wgjwhj.cn

[T51] Scala：Hello World
来源：http://kp.lnxyls.cn

println("Hello")
来源：http://gh.yuexingan06.cn

[T52] Scala：变量
来源：http://yk.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://em.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://rj.hahajie.cn

s"值: $b"
来源：http://mj.wgjwhj.cn

[T54] Scala：集合映射
来源：http://gk.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://vk.9csxet.cn

[T55] Scala：集合过滤
来源：http://nu.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ac.521024.cn

[T56] Scala：样例类
来源：http://oj.szsharing.cn

case class User(name: String, age: Int)
来源：http://vl.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://hh.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tl.huixiangedu.cn

[T58] Scala：函数定义
来源：http://oc.huixiangedu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jo.shxzskj.cn

[T59] Scala：循环
来源：http://zs.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://is.lnxyls.cn

[T60] Scala：折叠
来源：http://vg.yuexingan06.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ov.9csxet.cn

================================================================================
来源：http://tv.yuntaijiaju.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xq.hnjuh.cn

================================================================================
来源：http://ng.hnjuh.cn

[U01] Py：创建虚拟环境
来源：http://xt.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tr.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://pm.hahajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ft.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://ky.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rq.521024.cn

[U04] Py：变量调试打印
来源：http://zn.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yd.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://id.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://rn.nszjky.cn

[U06] Py：合并两个字典
来源：http://uq.hahajie.cn

{**a, **b}
来源：http://ar.shxzukj.cn

[U07] Py：反转字典键值
来源：http://zm.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://jh.521024.cn

[U08] Py：展平二维列表
来源：http://ax.9csxet.cn

[y for x in nested for y in x]
来源：http://tk.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://qp.hahajie.cn

max(d, key=d.get)
来源：http://zl.hnjuh.cn

[U10] Py：按值排序字典
来源：http://ti.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bo.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://lx.asd995.cn

(x * 2 for x in arr)
来源：http://ia.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jy.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://ei.hahajie.cn

[U13] Py：固定长度队列
来源：http://de.9csxet.cn

deque(maxlen=10)
来源：http://zh.wgjwhj.cn

[U14] Py：分组收集到列表
来源：http://us.hahajie.cn

defaultdict(list)
来源：http://hq.haigaiapp.cn

[U15] Py：高精度计时
来源：http://qo.asd995.cn

t = time.perf_counter()
来源：http://xv.asd995.cn

[U16] Py：命令行参数解析
来源：http://sq.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vd.panjiajie.cn

[U17] Py：初始化日志
来源：http://qn.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://ot.newstarts.cn

[U18] Py：预编译正则
来源：http://sk.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://mk.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://bn.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iu.521024.cn

[U20] Py：缓存函数结果
来源：http://np.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://ef.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://ls.nszjky.cn

@contextlib.contextmanager
来源：http://qy.hahajie.cn

[U22] Py：矩阵转置
来源：http://bo.shtwfgs.cn

list(zip(*m))
来源：http://kt.gzmigu.cn

[U23] Py：分块读取大文件
来源：http://be.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xa.bookmarksfly.cn

[U24] Py：路径操作
来源：http://pr.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://di.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://mp.haigaiapp.cn

csv.DictReader(f)
来源：http://wz.huanxung.cn

[U26] Py：并发下载
来源：http://xx.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vb.huanxung.cn

[U27] Py：异步 HTTP
来源：http://pd.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://wn.nicolike.cn

[U28] Py：类型别名
来源：http://ct.colortex.cn

UserId = int
来源：http://tz.szxytkj.cn

[U29] Py：属性校验
来源：http://te.szxytkj.cn

@property 与 @x.setter 配合
来源：http://lu.gzmigu.cn

[U30] Py：数据类
来源：http://lu.yuntaijiaju.cn

@dataclass(slots=True)
来源：http://dy.hnjuh.cn

[U31] Py：单测
来源：http://uz.nszjky.cn

python -m pytest -q
来源：http://mi.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://uq.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://ra.haigaiapp.cn

[U33] Py：打包发布
来源：http://rr.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://hg.lnxyls.cn

[U34] Py：判断编码
来源：http://lt.gzmigu.cn

chardet.detect(raw)
来源：http://qh.lnxyls.cn

[U35] Py：发送邮件
来源：http://vz.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fd.jctech888.com.cn

[U36] Py：定时任务
来源：http://hm.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://tr.colortex.cn

[U37] Py：读写 Excel
来源：http://ya.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wj.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://gs.hahajie.cn

Path(__file__).resolve().parent
来源：http://aa.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://wc.jctech888.com.cn

sys.stdout.isatty()
来源：http://tw.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://yb.colortex.cn

print("err", file=sys.stderr)
来源：http://bg.yuntaijiaju.cn

[U41] PHP：初始化 Composer 项目
来源：http://ao.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vb.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://vt.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dc.gzmigu.cn

[U43] PHP：声明命名空间
来源：http://fs.shxzukj.cn

namespace App\Http;
来源：http://ps.asd995.cn

[U44] PHP：开启严格类型
来源：http://fu.jctech888.com.cn

declare(strict_types=1);
来源：http://yi.bookmarksfly.cn

[U45] PHP：类型声明与返回类型
来源：http://qi.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://he.muxihuayi.cn

[U46] PHP：可空类型
来源：http://kk.newstarts.cn

?string $name = null
来源：http://po.bjjhwx.cn

[U47] PHP：联合类型
来源：http://hr.bookmarksfly.cn

int|string $id
来源：http://of.szsharing.cn

[U48] PHP：纯枚举
来源：http://ag.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jq.shxzskj.cn

[U49] PHP：只读属性
来源：http://ji.jctech888.com.cn

public readonly string $name
来源：http://rg.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://kv.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://xd.gzmigu.cn


<!-- 参考信息 -->