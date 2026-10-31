代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zc.colortex.cn

[S21] C：字符类别判断
来源：http://ud.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sd.muxihuayi.cn

[S22] C：字符串转数字
来源：http://wn.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jc.bookmarksfly.cn

[S23] C：随机数
来源：http://fv.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cl.huanxung.cn

[S24] C：获取本地时间
来源：http://fx.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ud.lnxyls.cn

[S25] C：内存拷贝
来源：http://xh.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://nu.shxzskj.cn

[S26] C：内存清零
来源：http://xl.huanxung.cn

memset(a, 0, sizeof a);
来源：http://fv.hnjuh.cn

[S27] C：定义常量
来源：http://pu.bookmarksfly.cn

const double PI = 3.14159;
来源：http://je.huanxung.cn

[S28] C：静态变量
来源：http://fp.muxihuayi.cn

static int counter = 0;
来源：http://qh.jctech888.com.cn

[S29] C：变参函数
来源：http://vr.panjiajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gg.colortex.cn

[S30] C：头文件保护
来源：http://lj.huanxung.cn

#ifndef X_H
来源：http://gg.newstarts.cn

#define X_H
来源：http://lj.huixinmuqiang.cn

#endif
来源：http://is.szxytkj.cn

[S31] C++：Hello World
来源：http://dm.haigaiapp.cn

#include <iostream>
来源：http://za.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://pb.haigaiapp.cn

[S32] C++：字符串
来源：http://ly.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://gj.muxihuayi.cn

[S33] C++：vector 增删
来源：http://uj.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kr.lnxyls.cn

[S34] C++：遍历 vector
来源：http://vd.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://nz.nszjky.cn

[S35] C++：map
来源：http://wn.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jn.shxzukj.cn

[S36] C++：unordered_map
来源：http://yw.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ro.jianghongdianzi.cn

[S37] C++：set
来源：http://et.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pz.bjjhwx.cn

[S38] C++：排序
来源：http://rp.asd995.cn

std::sort(v.begin(), v.end());
来源：http://nh.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://sk.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mu.9csxet.cn

[S40] C++：查找元素
来源：http://rr.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sl.shxzskj.cn

[S41] C++：类与构造函数
来源：http://od.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ru.nszjky.cn

[S42] C++：继承与虚函数
来源：http://vs.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://si.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://jh.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://ws.bjjhwx.cn

[S44] C++：引用传参
来源：http://lm.asd995.cn

void inc(int &x) { ++x; }
来源：http://sc.shxzukj.cn

[S45] C++：lambda
来源：http://om.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kf.huixiangedu.cn

[S46] C++：函数模板
来源：http://jw.shxzukj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nm.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://fl.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wb.nicolike.cn

[S48] C++：逐行读文件
来源：http://ko.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cm.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://ly.nicolike.cn

[S49] C++：写文件
来源：http://md.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xv.muxihuayi.cn

[S50] C++：格式化数字
来源：http://hs.huanxung.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jc.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://km.9csxet.cn

static_cast<double>(a) / b
来源：http://ta.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://hn.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://me.szsharing.cn

[S53] C++：移动语义
来源：http://nx.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://ti.hahajie.cn

[S54] C++：异常处理
来源：http://de.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vg.bookmarksfly.cn

[S55] C++：结构化绑定
来源：http://vf.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dg.shxzukj.cn

[S56] C++：optional
来源：http://be.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ic.haigaiapp.cn

[S57] C++：编译期常量
来源：http://yo.wgjwhj.cn

constexpr int N = 10;
来源：http://wp.wgjwhj.cn

[S58] C++：命名空间
来源：http://xl.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://do.asd995.cn

[S59] C++：静态断言
来源：http://sj.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lw.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://zl.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kf.jianghongdianzi.cn

================================================================================
来源：http://zj.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nb.haigaiapp.cn

================================================================================
来源：http://yj.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://gq.shxzskj.cn

println("Hello")
来源：http://ae.hnjuh.cn

[T02] Kotlin：变量
来源：http://ny.gzmigu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ge.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://ex.bookmarksfly.cn

"值: $b"
来源：http://jy.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://te.hahajie.cn

val n: String? = null;  n?.length
来源：http://yw.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://ko.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wz.newstarts.cn

[T06] Kotlin：集合映射
来源：http://zn.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oz.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://at.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fu.szsharing.cn

[T08] Kotlin：数据类
来源：http://fg.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://sd.521024.cn

[T09] Kotlin：扩展函数
来源：http://hx.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://rw.nicolike.cn

[T10] Kotlin：默认参数
来源：http://xw.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pr.szxytkj.cn

[T11] Kotlin：协程
来源：http://hv.bookmarksfly.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ag.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://wo.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://qz.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://ze.lnxyls.cn

val m = mapOf("a" to 1)
来源：http://sl.muxihuayi.cn

[T14] Kotlin：循环
来源：http://yc.gzmigu.cn

for (i in 1..10) println(i)
来源：http://aw.hahajie.cn

[T15] Kotlin：接口
来源：http://cy.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://ii.yuexingan06.cn

[T16] Swift：Hello World
来源：http://ym.lnxyls.cn

print("Hello")
来源：http://nn.colortex.cn

[T17] Swift：变量与常量
来源：http://wt.huixiangedu.cn

var a = 1;  let b = 2
来源：http://vz.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://du.shtwfgs.cn

"值: \(b)"
来源：http://bo.szsharing.cn

[T19] Swift：可选绑定
来源：http://eh.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://kz.bookmarksfly.cn

[T20] Swift：数组操作
来源：http://py.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jj.hnjuh.cn

[T21] Swift：遍历
来源：http://cv.chemitech.net.cn

for x in a { print(x) }
来源：http://cn.szxytkj.cn

[T22] Swift：字典
来源：http://qe.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ml.shxzskj.cn

[T23] Swift：函数
来源：http://aw.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vg.asd995.cn

[T24] Swift：闭包
来源：http://hh.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vs.newstarts.cn

[T25] Swift：结构体
来源：http://mu.colortex.cn

struct P { var x: Int }
来源：http://gd.newstarts.cn

[T26] Swift：类与重写
来源：http://jx.huixiangedu.cn

class A: Base { override func f() {} }
来源：http://du.szxytkj.cn

[T27] Swift：错误处理
来源：http://mb.hahajie.cn

do { try f() } catch { print(error) }
来源：http://jm.szsharing.cn

[T28] Swift：枚举
来源：http://pz.huanxung.cn

enum Color { case red, green }
来源：http://la.hahajie.cn

[T29] Swift：guard 提前返回
来源：http://vu.colortex.cn

guard let x = opt else { return }
来源：http://uv.colortex.cn

[T30] Swift：协议
来源：http://lh.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://vb.521024.cn

[T31] Lua：Hello World
来源：http://wy.shxzukj.cn

print("Hello")
来源：http://wo.521024.cn

[T32] Lua：局部变量
来源：http://hh.nszjky.cn

local a = 1
来源：http://cu.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://zs.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rx.colortex.cn

[T34] Lua：遍历表
来源：http://lr.521024.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ds.jianghongdianzi.cn

[T35] Lua：字典表
来源：http://mf.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://wa.jianghongdianzi.cn

[T36] Lua：函数
来源：http://gb.wgjwhj.cn

function add(a, b) return a + b end
来源：http://ut.asd995.cn

[T37] Lua：字符串拼接
来源：http://qj.jianghongdianzi.cn

"a" .. "b"
来源：http://ak.muxihuayi.cn

[T38] Lua：条件
来源：http://hl.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://rk.lnxyls.cn

[T39] Lua：模式匹配
来源：http://uj.asd995.cn

string.find(s, "%d+")
来源：http://pt.521024.cn

[T40] Lua：元表
来源：http://lv.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://jh.muxihuayi.cn

[T41] Perl：Hello World
来源：http://vd.newstarts.cn

print "Hello\n";
来源：http://pa.colortex.cn

[T42] Perl：变量类型
来源：http://mj.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ey.newstarts.cn

[T43] Perl：字符串插值
来源：http://bv.asd995.cn

"值: $a"
来源：http://bz.521024.cn

[T44] Perl：条件
来源：http://pa.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://ns.panjiajie.cn

[T45] Perl：数组遍历
来源：http://pt.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://qu.newstarts.cn

[T46] Perl：哈希操作
来源：http://yl.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vo.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://nr.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qx.newstarts.cn

[T48] Perl：正则替换
来源：http://ib.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://dh.asd995.cn

[T49] Perl：函数
来源：http://mp.hahajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mv.521024.cn

[T50] Perl：逐行读文件
来源：http://me.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pi.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://rd.wgjwhj.cn

[T51] Scala：Hello World
来源：http://dc.chemitech.net.cn

println("Hello")
来源：http://ep.szsharing.cn

[T52] Scala：变量
来源：http://tm.haigaiapp.cn

val a = 1;  var b = 2
来源：http://yd.hahajie.cn

[T53] Scala：字符串插值
来源：http://xh.huanxung.cn

s"值: $b"
来源：http://zb.521024.cn

[T54] Scala：集合映射
来源：http://kr.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://mt.colortex.cn

[T55] Scala：集合过滤
来源：http://lq.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dj.huanxung.cn

[T56] Scala：样例类
来源：http://ld.huixiangedu.cn

case class User(name: String, age: Int)
来源：http://fs.colortex.cn

[T57] Scala：模式匹配
来源：http://rl.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xm.asd995.cn

[T58] Scala：函数定义
来源：http://ri.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ze.huanxung.cn

[T59] Scala：循环
来源：http://va.hahajie.cn

for (i <- 1 to 10) println(i)
来源：http://dv.huixiangedu.cn

[T60] Scala：折叠
来源：http://px.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nt.huixinmuqiang.cn

================================================================================
来源：http://kz.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dk.huixiangedu.cn

================================================================================
来源：http://rs.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://lm.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pr.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://jc.hahajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uv.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://kk.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lq.huanxung.cn

[U04] Py：变量调试打印
来源：http://zu.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ay.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://aw.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://rl.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://zq.9csxet.cn

{**a, **b}
来源：http://ey.gzmigu.cn

[U07] Py：反转字典键值
来源：http://gl.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://vi.szxytkj.cn

[U08] Py：展平二维列表
来源：http://oz.521024.cn

[y for x in nested for y in x]
来源：http://hg.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://xp.panjiajie.cn

max(d, key=d.get)
来源：http://bs.nszjky.cn

[U10] Py：按值排序字典
来源：http://ss.yuntaijiaju.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cc.521024.cn

[U11] Py：生成器表达式
来源：http://ds.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://jk.muxihuayi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sg.colortex.cn

Counter(arr).most_common(3)
来源：http://xk.bookmarksfly.cn

[U13] Py：固定长度队列
来源：http://qd.yuntaijiaju.cn

deque(maxlen=10)
来源：http://pw.shxzukj.cn

[U14] Py：分组收集到列表
来源：http://xk.newstarts.cn

defaultdict(list)
来源：http://jb.9csxet.cn

[U15] Py：高精度计时
来源：http://mt.yuexingan06.cn

t = time.perf_counter()
来源：http://wv.nszjky.cn

[U16] Py：命令行参数解析
来源：http://lf.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pn.hahajie.cn

[U17] Py：初始化日志
来源：http://pj.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://ol.bjjhwx.cn

[U18] Py：预编译正则
来源：http://vt.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://rs.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://yf.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hk.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://kx.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://ze.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://gg.bookmarksfly.cn

@contextlib.contextmanager
来源：http://kf.szsharing.cn

[U22] Py：矩阵转置
来源：http://vf.9csxet.cn

list(zip(*m))
来源：http://cz.wgjwhj.cn

[U23] Py：分块读取大文件
来源：http://zl.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ts.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://bz.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gh.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://qg.shxzukj.cn

csv.DictReader(f)
来源：http://cg.hahajie.cn

[U26] Py：并发下载
来源：http://pe.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://to.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://mk.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://wr.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://uh.newstarts.cn

UserId = int
来源：http://zc.wgjwhj.cn

[U29] Py：属性校验
来源：http://ce.huanxung.cn

@property 与 @x.setter 配合
来源：http://zm.gzmigu.cn

[U30] Py：数据类
来源：http://zg.shxzskj.cn

@dataclass(slots=True)
来源：http://dy.nicolike.cn

[U31] Py：单测
来源：http://dz.panjiajie.cn

python -m pytest -q
来源：http://wu.wgjwhj.cn

[U32] Py：代码格式化
来源：http://os.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://kr.asd995.cn

[U33] Py：打包发布
来源：http://ep.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://pa.haigaiapp.cn

[U34] Py：判断编码
来源：http://nn.szsharing.cn

chardet.detect(raw)
来源：http://vk.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://zt.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uh.asd995.cn

[U36] Py：定时任务
来源：http://gv.wgjwhj.cn

schedule.every(10).minutes.do(job)
来源：http://jq.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://zk.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sq.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://vw.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://ou.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://ib.szxytkj.cn

sys.stdout.isatty()
来源：http://em.newstarts.cn

[U40] Py：打印到标准错误
来源：http://lw.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://fg.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://rs.521024.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pn.yuexingan06.cn

[U42] PHP：PSR-4 自动加载
来源：http://oq.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dg.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://np.wgjwhj.cn

namespace App\Http;
来源：http://wy.yuntaijiaju.cn

[U44] PHP：开启严格类型
来源：http://fa.huixinmuqiang.cn

declare(strict_types=1);
来源：http://km.panjiajie.cn


<!-- 参考信息 -->