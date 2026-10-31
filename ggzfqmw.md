代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://vt.colortex.cn

[S02] C：变量与格式化输出
来源：http://xj.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://oz.huanxung.cn

[S03] C：读入整数
来源：http://tk.hahajie.cn

int x; scanf("%d", &x);
来源：http://vw.newstarts.cn

[S04] C：字符串复制
来源：http://dq.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hg.haigaiapp.cn

[S05] C：字符串长度
来源：http://oc.hnjuh.cn

strlen(s)
来源：http://wz.jctech888.com.cn

[S06] C：字符串比较
来源：http://ht.nszjky.cn

strcmp(a, b) == 0
来源：http://ni.nszjky.cn

[S07] C：数组遍历求和
来源：http://tj.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ei.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://ui.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qe.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://tp.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jp.huixiangedu.cn

[S10] C：指针与解引用
来源：http://hl.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://er.521024.cn

[S11] C：逐行读文件
来源：http://aq.haigaiapp.cn

FILE *f = fopen("a.txt", "r");
来源：http://ho.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://od.hahajie.cn

fclose(f);
来源：http://ux.hnjuh.cn

[S12] C：写文件
来源：http://ct.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xd.wgjwhj.cn

[S13] C：宏定义
来源：http://wb.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://df.wgjwhj.cn

[S14] C：枚举
来源：http://nt.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://ml.shxzukj.cn

[S15] C：类型转换
来源：http://bs.shxzskj.cn

(double) a / b
来源：http://yx.muxihuayi.cn

[S16] C：位操作置位
来源：http://xp.shxzskj.cn

x |= (1 << 3);
来源：http://eg.nszjky.cn

[S17] C：安全拼接字符串
来源：http://dt.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vj.hnjuh.cn

[S18] C：命令行参数
来源：http://qz.bjjhwx.cn

int main(int argc, char **argv)
来源：http://vq.muxihuayi.cn

[S19] C：快速排序
来源：http://zl.9csxet.cn

qsort(a, n, sizeof(int), cmp);
来源：http://go.newstarts.cn

[S20] C：二分查找
来源：http://gs.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bp.muxihuayi.cn

[S21] C：字符类别判断
来源：http://dx.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wv.lnxyls.cn

[S22] C：字符串转数字
来源：http://xq.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oi.chemitech.net.cn

[S23] C：随机数
来源：http://xk.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ot.panjiajie.cn

[S24] C：获取本地时间
来源：http://wj.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yh.panjiajie.cn

[S25] C：内存拷贝
来源：http://ql.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://en.yuexingan06.cn

[S26] C：内存清零
来源：http://br.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://iu.gzmigu.cn

[S27] C：定义常量
来源：http://ii.gzmigu.cn

const double PI = 3.14159;
来源：http://ep.szxytkj.cn

[S28] C：静态变量
来源：http://lb.muxihuayi.cn

static int counter = 0;
来源：http://be.hnjuh.cn

[S29] C：变参函数
来源：http://kh.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cj.lnxyls.cn

[S30] C：头文件保护
来源：http://rz.nicolike.cn

#ifndef X_H
来源：http://gq.bjjhwx.cn

#define X_H
来源：http://el.nszjky.cn

#endif
来源：http://tv.shtwfgs.cn

[S31] C++：Hello World
来源：http://gb.huanxung.cn

#include <iostream>
来源：http://sg.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://po.szxytkj.cn

[S32] C++：字符串
来源：http://aq.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://ey.newstarts.cn

[S33] C++：vector 增删
来源：http://uk.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://px.lnxyls.cn

[S34] C++：遍历 vector
来源：http://up.yuntaijiaju.cn

for (auto &x : v) { std::cout << x; }
来源：http://hl.lnxyls.cn

[S35] C++：map
来源：http://qz.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rn.huanxung.cn

[S36] C++：unordered_map
来源：http://yy.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ul.521024.cn

[S37] C++：set
来源：http://ps.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yc.bookmarksfly.cn

[S38] C++：排序
来源：http://fl.asd995.cn

std::sort(v.begin(), v.end());
来源：http://os.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://vf.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uh.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://sj.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uu.nszjky.cn

[S41] C++：类与构造函数
来源：http://gi.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ob.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://ki.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://sv.huanxung.cn

[S43] C++：智能指针
来源：http://au.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://mf.hnjuh.cn

[S44] C++：引用传参
来源：http://an.newstarts.cn

void inc(int &x) { ++x; }
来源：http://xt.gzmigu.cn

[S45] C++：lambda
来源：http://vi.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dx.shtwfgs.cn

[S46] C++：函数模板
来源：http://ba.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nl.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://eg.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ss.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://yc.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kg.huanxung.cn

while (std::getline(in, line)) { }
来源：http://kr.huixinmuqiang.cn

[S49] C++：写文件
来源：http://dw.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bl.hahajie.cn

[S50] C++：格式化数字
来源：http://ey.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cy.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://zg.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://kv.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://oa.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://ej.gzmigu.cn

[S53] C++：移动语义
来源：http://ux.colortex.cn

std::vector<int> w = std::move(v);
来源：http://jo.shxzskj.cn

[S54] C++：异常处理
来源：http://kp.chemitech.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://so.newstarts.cn

[S55] C++：结构化绑定
来源：http://qo.bjjhwx.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qo.shxzskj.cn

[S56] C++：optional
来源：http://ct.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cb.colortex.cn

[S57] C++：编译期常量
来源：http://ny.szxytkj.cn

constexpr int N = 10;
来源：http://vv.colortex.cn

[S58] C++：命名空间
来源：http://su.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://zb.yuntaijiaju.cn

[S59] C++：静态断言
来源：http://zu.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aj.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://tu.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uc.9csxet.cn

================================================================================
来源：http://fq.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qz.colortex.cn

================================================================================
来源：http://pb.nszjky.cn

[T01] Kotlin：Hello World
来源：http://ji.chemitech.net.cn

println("Hello")
来源：http://lr.gzmigu.cn

[T02] Kotlin：变量
来源：http://ac.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ws.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://gw.nicolike.cn

"值: $b"
来源：http://mn.nicolike.cn

[T04] Kotlin：空安全
来源：http://dd.panjiajie.cn

val n: String? = null;  n?.length
来源：http://lo.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://tw.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sd.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://vn.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ky.nicolike.cn

[T07] Kotlin：集合过滤
来源：http://kw.9csxet.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ul.huanxung.cn

[T08] Kotlin：数据类
来源：http://zl.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://wf.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://qt.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://uw.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://kj.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hp.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://os.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yg.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://kr.chemitech.net.cn

val (a, b) = Pair(1, 2)
来源：http://mi.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://jt.huanxung.cn

val m = mapOf("a" to 1)
来源：http://wy.nszjky.cn

[T14] Kotlin：循环
来源：http://fe.panjiajie.cn

for (i in 1..10) println(i)
来源：http://nn.szxytkj.cn

[T15] Kotlin：接口
来源：http://kt.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://uv.yuntaijiaju.cn

[T16] Swift：Hello World
来源：http://gc.hnjuh.cn

print("Hello")
来源：http://zh.asd995.cn

[T17] Swift：变量与常量
来源：http://hc.huanxung.cn

var a = 1;  let b = 2
来源：http://iy.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://zq.521024.cn

"值: \(b)"
来源：http://oz.9csxet.cn

[T19] Swift：可选绑定
来源：http://vo.panjiajie.cn

if let n = opt { print(n) }
来源：http://cn.hnjuh.cn

[T20] Swift：数组操作
来源：http://at.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ig.bjjhwx.cn

[T21] Swift：遍历
来源：http://kd.jctech888.com.cn

for x in a { print(x) }
来源：http://lc.colortex.cn

[T22] Swift：字典
来源：http://we.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ml.newstarts.cn

[T23] Swift：函数
来源：http://eg.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rb.haigaiapp.cn

[T24] Swift：闭包
来源：http://yq.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jx.hahajie.cn

[T25] Swift：结构体
来源：http://xz.nicolike.cn

struct P { var x: Int }
来源：http://sz.muxihuayi.cn

[T26] Swift：类与重写
来源：http://kp.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://lf.gzmigu.cn

[T27] Swift：错误处理
来源：http://eo.huanxung.cn

do { try f() } catch { print(error) }
来源：http://pb.nszjky.cn

[T28] Swift：枚举
来源：http://un.muxihuayi.cn

enum Color { case red, green }
来源：http://kr.shtwfgs.cn

[T29] Swift：guard 提前返回
来源：http://yc.bookmarksfly.cn

guard let x = opt else { return }
来源：http://lg.shtwfgs.cn

[T30] Swift：协议
来源：http://cc.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://cf.asd995.cn

[T31] Lua：Hello World
来源：http://ao.nicolike.cn

print("Hello")
来源：http://qu.9csxet.cn

[T32] Lua：局部变量
来源：http://iz.szsharing.cn

local a = 1
来源：http://ab.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://bw.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bk.asd995.cn

[T34] Lua：遍历表
来源：http://wb.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vk.panjiajie.cn

[T35] Lua：字典表
来源：http://lp.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://vp.nszjky.cn

[T36] Lua：函数
来源：http://zz.szxytkj.cn

function add(a, b) return a + b end
来源：http://rq.muxihuayi.cn

[T37] Lua：字符串拼接
来源：http://tc.colortex.cn

"a" .. "b"
来源：http://qd.huixinmuqiang.cn

[T38] Lua：条件
来源：http://ek.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://ps.panjiajie.cn

[T39] Lua：模式匹配
来源：http://ov.yuexingan06.cn

string.find(s, "%d+")
来源：http://va.521024.cn

[T40] Lua：元表
来源：http://dv.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://yb.huanxung.cn

[T41] Perl：Hello World
来源：http://bl.lnxyls.cn

print "Hello\n";
来源：http://ei.panjiajie.cn

[T42] Perl：变量类型
来源：http://qq.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wc.huanxung.cn

[T43] Perl：字符串插值
来源：http://ym.asd995.cn

"值: $a"
来源：http://jy.newstarts.cn

[T44] Perl：条件
来源：http://bh.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://zt.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://em.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://fi.lnxyls.cn

[T46] Perl：哈希操作
来源：http://mc.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vj.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://io.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pp.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://gf.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://la.jianghongdianzi.cn

[T49] Perl：函数
来源：http://nk.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ti.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://fu.newstarts.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ge.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://hs.colortex.cn

[T51] Scala：Hello World
来源：http://cf.bookmarksfly.cn

println("Hello")
来源：http://ls.wgjwhj.cn

[T52] Scala：变量
来源：http://ik.chemitech.net.cn

val a = 1;  var b = 2
来源：http://ex.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://hr.huixiangedu.cn

s"值: $b"
来源：http://tc.jctech888.com.cn

[T54] Scala：集合映射
来源：http://mw.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://ba.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://aw.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ds.huanxung.cn

[T56] Scala：样例类
来源：http://tf.huixiangedu.cn

case class User(name: String, age: Int)
来源：http://lh.szxytkj.cn

[T57] Scala：模式匹配
来源：http://nb.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ra.shxzukj.cn

[T58] Scala：函数定义
来源：http://bl.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hv.jianghongdianzi.cn

[T59] Scala：循环
来源：http://aw.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://xw.haigaiapp.cn

[T60] Scala：折叠
来源：http://xo.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cd.szxytkj.cn

================================================================================
来源：http://cd.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jg.jctech888.com.cn

================================================================================
来源：http://hd.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://yr.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ku.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://sw.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qg.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://gl.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fr.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://ru.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ml.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://ft.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://xo.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://yo.huixiangedu.cn

{**a, **b}
来源：http://cr.521024.cn

[U07] Py：反转字典键值
来源：http://ct.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://cf.huixinmuqiang.cn

[U08] Py：展平二维列表
来源：http://oq.lnxyls.cn

[y for x in nested for y in x]
来源：http://pe.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://qr.gzmigu.cn

max(d, key=d.get)
来源：http://gx.asd995.cn

[U10] Py：按值排序字典
来源：http://ra.szsharing.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dk.shxzskj.cn

[U11] Py：生成器表达式
来源：http://ec.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://qp.colortex.cn

[U12] Py：取出现最多的 3 个元素
来源：http://eo.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://fu.hnjuh.cn

[U13] Py：固定长度队列
来源：http://ah.chemitech.net.cn

deque(maxlen=10)
来源：http://ix.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://kd.haigaiapp.cn

defaultdict(list)
来源：http://fs.panjiajie.cn

[U15] Py：高精度计时
来源：http://kd.szsharing.cn

t = time.perf_counter()
来源：http://cn.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://qg.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://to.hahajie.cn

[U17] Py：初始化日志
来源：http://nf.yuexingan06.cn

logging.basicConfig(level=logging.INFO)
来源：http://pa.jianghongdianzi.cn

[U18] Py：预编译正则
来源：http://ul.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://kc.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://cy.huanxung.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ty.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://zn.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://ck.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://qb.shxzukj.cn

@contextlib.contextmanager
来源：http://gj.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://sc.shxzukj.cn

list(zip(*m))
来源：http://ei.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://ag.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ie.haigaiapp.cn

[U24] Py：路径操作
来源：http://em.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iw.haigaiapp.cn


<!-- 参考信息 -->