代发 wailian999

#ifndef X_H
来源：http://vw.chemitech.net.cn

#define X_H
来源：http://nf.bjjhwx.cn

#endif
来源：http://od.huanxung.cn

[S31] C++：Hello World
来源：http://kp.huixiangedu.cn

#include <iostream>
来源：http://yu.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://ff.shxzskj.cn

[S32] C++：字符串
来源：http://op.hahajie.cn

std::string s = "hi";  s += "!";
来源：http://ds.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://eg.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tp.hahajie.cn

[S34] C++：遍历 vector
来源：http://ao.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://ov.szxytkj.cn

[S35] C++：map
来源：http://eu.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://co.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://fo.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wz.haigaiapp.cn

[S37] C++：set
来源：http://jx.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dl.newstarts.cn

[S38] C++：排序
来源：http://vq.colortex.cn

std::sort(v.begin(), v.end());
来源：http://bl.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://xl.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gj.huixiangedu.cn

[S40] C++：查找元素
来源：http://tv.lnxyls.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jo.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://es.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hi.jctech888.com.cn

[S42] C++：继承与虚函数
来源：http://yv.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://mc.521024.cn

[S43] C++：智能指针
来源：http://ay.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://sr.bjjhwx.cn

[S44] C++：引用传参
来源：http://rf.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://ws.9csxet.cn

[S45] C++：lambda
来源：http://bt.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://my.muxihuayi.cn

[S46] C++：函数模板
来源：http://xj.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bn.wgjwhj.cn

[S47] C++：结构化绑定遍历
来源：http://br.9csxet.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iw.lnxyls.cn

[S48] C++：逐行读文件
来源：http://fr.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nj.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://pk.jctech888.com.cn

[S49] C++：写文件
来源：http://da.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ki.szxytkj.cn

[S50] C++：格式化数字
来源：http://gu.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vw.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://dc.shxzukj.cn

static_cast<double>(a) / b
来源：http://dy.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://tm.shxzukj.cn

int size() const noexcept { return n_; }
来源：http://su.huanxung.cn

[S53] C++：移动语义
来源：http://do.asd995.cn

std::vector<int> w = std::move(v);
来源：http://jh.shxzukj.cn

[S54] C++：异常处理
来源：http://wc.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://di.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://lu.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://py.bjjhwx.cn

[S56] C++：optional
来源：http://fm.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fo.jctech888.com.cn

[S57] C++：编译期常量
来源：http://mi.huanxung.cn

constexpr int N = 10;
来源：http://sw.bjjhwx.cn

[S58] C++：命名空间
来源：http://jr.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://uy.nszjky.cn

[S59] C++：静态断言
来源：http://uw.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://al.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://fi.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qn.yuntaijiaju.cn

================================================================================
来源：http://sk.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ux.newstarts.cn

================================================================================
来源：http://rf.newstarts.cn

[T01] Kotlin：Hello World
来源：http://kd.huanxung.cn

println("Hello")
来源：http://xd.shtwfgs.cn

[T02] Kotlin：变量
来源：http://hz.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fy.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://rv.szxytkj.cn

"值: $b"
来源：http://kz.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://mq.shxzukj.cn

val n: String? = null;  n?.length
来源：http://ku.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://os.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ux.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://ti.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xh.asd995.cn

[T07] Kotlin：集合过滤
来源：http://vm.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pz.hnjuh.cn

[T08] Kotlin：数据类
来源：http://fb.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://hz.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://eo.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://zc.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://tx.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ot.lnxyls.cn

[T11] Kotlin：协程
来源：http://po.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dw.colortex.cn

[T12] Kotlin：解构声明
来源：http://mi.haigaiapp.cn

val (a, b) = Pair(1, 2)
来源：http://rx.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://cy.nszjky.cn

val m = mapOf("a" to 1)
来源：http://pe.muxihuayi.cn

[T14] Kotlin：循环
来源：http://yy.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://gd.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://rd.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://ea.huanxung.cn

[T16] Swift：Hello World
来源：http://ni.huixiangedu.cn

print("Hello")
来源：http://sl.nicolike.cn

[T17] Swift：变量与常量
来源：http://gv.nicolike.cn

var a = 1;  let b = 2
来源：http://ht.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://uu.jctech888.com.cn

"值: \(b)"
来源：http://mi.nszjky.cn

[T19] Swift：可选绑定
来源：http://mg.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://bk.gzmigu.cn

[T20] Swift：数组操作
来源：http://xv.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kb.hnjuh.cn

[T21] Swift：遍历
来源：http://lt.huixinmuqiang.cn

for x in a { print(x) }
来源：http://do.huixinmuqiang.cn

[T22] Swift：字典
来源：http://lx.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kp.huixinmuqiang.cn

[T23] Swift：函数
来源：http://td.hahajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fh.gzmigu.cn

[T24] Swift：闭包
来源：http://jy.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xs.gzmigu.cn

[T25] Swift：结构体
来源：http://ge.yuntaijiaju.cn

struct P { var x: Int }
来源：http://ep.newstarts.cn

[T26] Swift：类与重写
来源：http://ij.szsharing.cn

class A: Base { override func f() {} }
来源：http://uh.haigaiapp.cn

[T27] Swift：错误处理
来源：http://is.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://ec.jctech888.com.cn

[T28] Swift：枚举
来源：http://el.panjiajie.cn

enum Color { case red, green }
来源：http://nk.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://km.haigaiapp.cn

guard let x = opt else { return }
来源：http://bl.9csxet.cn

[T30] Swift：协议
来源：http://nl.colortex.cn

protocol Shape { func area() -> Double }
来源：http://bs.hnjuh.cn

[T31] Lua：Hello World
来源：http://jq.shtwfgs.cn

print("Hello")
来源：http://gv.hnjuh.cn

[T32] Lua：局部变量
来源：http://du.9csxet.cn

local a = 1
来源：http://vs.szsharing.cn

[T33] Lua：表（数组）
来源：http://va.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ng.panjiajie.cn

[T34] Lua：遍历表
来源：http://ou.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ej.huixiangedu.cn

[T35] Lua：字典表
来源：http://gs.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://qd.jctech888.com.cn

[T36] Lua：函数
来源：http://rh.szxytkj.cn

function add(a, b) return a + b end
来源：http://ta.521024.cn

[T37] Lua：字符串拼接
来源：http://em.nicolike.cn

"a" .. "b"
来源：http://vi.nicolike.cn

[T38] Lua：条件
来源：http://pp.gzmigu.cn

if x > 0 then print("正") end
来源：http://zw.huanxung.cn

[T39] Lua：模式匹配
来源：http://rd.huixiangedu.cn

string.find(s, "%d+")
来源：http://ph.nszjky.cn

[T40] Lua：元表
来源：http://qd.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://bo.colortex.cn

[T41] Perl：Hello World
来源：http://fr.yuexingan06.cn

print "Hello\n";
来源：http://pm.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://wm.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rx.szsharing.cn

[T43] Perl：字符串插值
来源：http://qf.hnjuh.cn

"值: $a"
来源：http://le.wgjwhj.cn

[T44] Perl：条件
来源：http://my.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://qa.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://pc.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://qg.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://fk.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://si.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://ju.lnxyls.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yx.yuexingan06.cn

[T48] Perl：正则替换
来源：http://be.colortex.cn

$s =~ s/old/new/g;
来源：http://jw.shxzskj.cn

[T49] Perl：函数
来源：http://mn.newstarts.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uz.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://vh.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xc.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://yl.bjjhwx.cn

[T51] Scala：Hello World
来源：http://ah.hnjuh.cn

println("Hello")
来源：http://yw.shxzskj.cn

[T52] Scala：变量
来源：http://vp.haigaiapp.cn

val a = 1;  var b = 2
来源：http://zr.shxzukj.cn

[T53] Scala：字符串插值
来源：http://fm.szxytkj.cn

s"值: $b"
来源：http://lp.huixiangedu.cn

[T54] Scala：集合映射
来源：http://df.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://zb.asd995.cn

[T55] Scala：集合过滤
来源：http://lf.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rk.jctech888.com.cn

[T56] Scala：样例类
来源：http://lp.shxzukj.cn

case class User(name: String, age: Int)
来源：http://mo.hnjuh.cn

[T57] Scala：模式匹配
来源：http://qr.haigaiapp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://my.shxzskj.cn

[T58] Scala：函数定义
来源：http://fa.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jo.nicolike.cn

[T59] Scala：循环
来源：http://cb.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://ca.hahajie.cn

[T60] Scala：折叠
来源：http://dr.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sd.jianghongdianzi.cn

================================================================================
来源：http://mp.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mf.shxzskj.cn

================================================================================
来源：http://bj.haigaiapp.cn

[U01] Py：创建虚拟环境
来源：http://wf.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fd.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://rw.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ne.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://cf.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://li.9csxet.cn

[U04] Py：变量调试打印
来源：http://ws.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uz.huixinmuqiang.cn

[U05] Py：列表去重且保序
来源：http://rk.huanxung.cn

list(dict.fromkeys(arr))
来源：http://ml.szxytkj.cn

[U06] Py：合并两个字典
来源：http://oy.hahajie.cn

{**a, **b}
来源：http://cm.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://uo.wgjwhj.cn

{v: k for k, v in d.items()}
来源：http://hr.shxzskj.cn

[U08] Py：展平二维列表
来源：http://xm.colortex.cn

[y for x in nested for y in x]
来源：http://dq.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://gw.szsharing.cn

max(d, key=d.get)
来源：http://ha.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://ax.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mx.nszjky.cn

[U11] Py：生成器表达式
来源：http://gv.colortex.cn

(x * 2 for x in arr)
来源：http://wv.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qe.huanxung.cn

Counter(arr).most_common(3)
来源：http://yp.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://ob.huixiangedu.cn

deque(maxlen=10)
来源：http://ev.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://ay.colortex.cn

defaultdict(list)
来源：http://xo.lnxyls.cn

[U15] Py：高精度计时
来源：http://og.hnjuh.cn

t = time.perf_counter()
来源：http://cw.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://vf.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nj.szxytkj.cn

[U17] Py：初始化日志
来源：http://xn.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://mq.gzmigu.cn

[U18] Py：预编译正则
来源：http://us.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://ig.hahajie.cn

[U19] Py：正则替换带回调
来源：http://iu.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fr.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://ob.yuntaijiaju.cn

@functools.lru_cache(maxsize=None)
来源：http://pa.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://wo.bookmarksfly.cn

@contextlib.contextmanager
来源：http://qq.szsharing.cn

[U22] Py：矩阵转置
来源：http://te.panjiajie.cn

list(zip(*m))
来源：http://pa.hnjuh.cn

[U23] Py：分块读取大文件
来源：http://ak.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qe.colortex.cn

[U24] Py：路径操作
来源：http://sn.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://om.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://je.huanxung.cn

csv.DictReader(f)
来源：http://rg.yuexingan06.cn

[U26] Py：并发下载
来源：http://jx.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ut.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://tq.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://ji.lnxyls.cn

[U28] Py：类型别名
来源：http://jd.muxihuayi.cn

UserId = int
来源：http://sb.shtwfgs.cn

[U29] Py：属性校验
来源：http://lq.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://dn.chemitech.net.cn

[U30] Py：数据类
来源：http://ju.bookmarksfly.cn

@dataclass(slots=True)
来源：http://iq.huixinmuqiang.cn

[U31] Py：单测
来源：http://cc.panjiajie.cn

python -m pytest -q
来源：http://mx.shxzukj.cn

[U32] Py：代码格式化
来源：http://xz.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://dc.szxytkj.cn

[U33] Py：打包发布
来源：http://fd.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://ju.bjjhwx.cn

[U34] Py：判断编码
来源：http://rh.asd995.cn

chardet.detect(raw)
来源：http://ys.shxzukj.cn

[U35] Py：发送邮件
来源：http://mu.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dw.yuexingan06.cn

[U36] Py：定时任务
来源：http://pg.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://co.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://xy.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qx.colortex.cn

[U38] Py：获取脚本所在目录
来源：http://vv.colortex.cn

Path(__file__).resolve().parent
来源：http://mp.colortex.cn

[U39] Py：判断是否在交互环境
来源：http://rd.nszjky.cn

sys.stdout.isatty()
来源：http://fy.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://ed.huixinmuqiang.cn

print("err", file=sys.stderr)
来源：http://jf.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://st.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://en.panjiajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://ko.bjjhwx.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bh.9csxet.cn

[U43] PHP：声明命名空间
来源：http://ge.huanxung.cn

namespace App\Http;
来源：http://ml.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://rk.wgjwhj.cn

declare(strict_types=1);
来源：http://xq.yuexingan06.cn

[U45] PHP：类型声明与返回类型
来源：http://zf.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bt.huixinmuqiang.cn

[U46] PHP：可空类型
来源：http://zm.bjjhwx.cn

?string $name = null
来源：http://hf.szsharing.cn

[U47] PHP：联合类型
来源：http://dj.yuexingan06.cn

int|string $id
来源：http://bm.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://xl.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lq.newstarts.cn

[U49] PHP：只读属性
来源：http://yn.yuntaijiaju.cn

public readonly string $name
来源：http://eq.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://gq.asd995.cn

public function __construct(private int $id) {}
来源：http://sq.lnxyls.cn

[U51] PHP：数组解构
来源：http://nv.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://ow.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://oh.panjiajie.cn

$double = fn($x) => $x * 2;
来源：http://lw.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://kc.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://uz.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://kn.nszjky.cn

$obj?->method()
来源：http://vr.newstarts.cn


<!-- 参考信息 -->