代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://ii.shxzskj.cn

[R72] 等待端口就绪
来源：http://ja.chemitech.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vv.shtwfgs.cn

[R73] 分割大日志
来源：http://ro.jctech888.com.cn

split -l 1000 big.log part_
来源：http://un.jianghongdianzi.cn

[R74] 批量重命名
来源：http://la.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vw.hahajie.cn

[R75] 导出环境变量
来源：http://ab.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://vp.newstarts.cn

[R76] 使用临时文件
来源：http://xo.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://is.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://kz.colortex.cn

read -rp "请输入: " ans
来源：http://vz.wgjwhj.cn

[R78] 交互式菜单
来源：http://kv.jctech888.com.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://da.huanxung.cn

[R79] 解析命令行选项
来源：http://jg.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mu.wgjwhj.cn

[R80] 查看脚本执行耗时
来源：http://mg.521024.cn

time ./run.sh
来源：http://xd.bookmarksfly.cn

================================================================================
来源：http://ub.bookmarksfly.cn

S. C / C++ 专题
来源：http://jx.nszjky.cn

================================================================================
来源：http://nj.muxihuayi.cn

[S01] C：Hello World
来源：http://lw.colortex.cn

#include <stdio.h>
来源：http://ck.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://js.huanxung.cn

[S02] C：变量与格式化输出
来源：http://dp.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://fq.szxytkj.cn

[S03] C：读入整数
来源：http://vf.szsharing.cn

int x; scanf("%d", &x);
来源：http://ra.hnjuh.cn

[S04] C：字符串复制
来源：http://hz.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vl.9csxet.cn

[S05] C：字符串长度
来源：http://mg.wgjwhj.cn

strlen(s)
来源：http://kz.nszjky.cn

[S06] C：字符串比较
来源：http://xo.panjiajie.cn

strcmp(a, b) == 0
来源：http://ac.521024.cn

[S07] C：数组遍历求和
来源：http://sg.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gv.9csxet.cn

[S08] C：动态内存分配与释放
来源：http://mv.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ux.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://ag.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vw.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://yw.nicolike.cn

int *p = &a;  *p = 5;
来源：http://qg.muxihuayi.cn

[S11] C：逐行读文件
来源：http://tz.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://oq.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qq.shxzskj.cn

fclose(f);
来源：http://pf.huanxung.cn

[S12] C：写文件
来源：http://dj.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ge.nszjky.cn

[S13] C：宏定义
来源：http://cp.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ec.chemitech.net.cn

[S14] C：枚举
来源：http://mp.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://qj.haigaiapp.cn

[S15] C：类型转换
来源：http://nb.huixinmuqiang.cn

(double) a / b
来源：http://gt.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://na.shxzskj.cn

x |= (1 << 3);
来源：http://wk.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://kq.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xg.newstarts.cn

[S18] C：命令行参数
来源：http://ga.lnxyls.cn

int main(int argc, char **argv)
来源：http://al.521024.cn

[S19] C：快速排序
来源：http://xj.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cc.szsharing.cn

[S20] C：二分查找
来源：http://tn.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ab.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://rf.shxzskj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qa.shtwfgs.cn

[S22] C：字符串转数字
来源：http://np.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://he.lnxyls.cn

[S23] C：随机数
来源：http://gu.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mv.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://sv.yuexingan06.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://to.haigaiapp.cn

[S25] C：内存拷贝
来源：http://qu.shxzukj.cn

memcpy(dst, src, n);
来源：http://et.newstarts.cn

[S26] C：内存清零
来源：http://ug.nicolike.cn

memset(a, 0, sizeof a);
来源：http://kd.bjjhwx.cn

[S27] C：定义常量
来源：http://kw.huanxung.cn

const double PI = 3.14159;
来源：http://ii.newstarts.cn

[S28] C：静态变量
来源：http://dv.yuexingan06.cn

static int counter = 0;
来源：http://tx.panjiajie.cn

[S29] C：变参函数
来源：http://fy.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zk.shxzukj.cn

[S30] C：头文件保护
来源：http://lh.gzmigu.cn

#ifndef X_H
来源：http://qk.hahajie.cn

#define X_H
来源：http://oy.colortex.cn

#endif
来源：http://da.hahajie.cn

[S31] C++：Hello World
来源：http://qi.muxihuayi.cn

#include <iostream>
来源：http://fg.bookmarksfly.cn

int main() { std::cout << "Hello\n"; }
来源：http://cw.yuntaijiaju.cn

[S32] C++：字符串
来源：http://hf.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://fk.jctech888.com.cn

[S33] C++：vector 增删
来源：http://rd.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sv.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://sz.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://gu.chemitech.net.cn

[S35] C++：map
来源：http://ih.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wg.nicolike.cn

[S36] C++：unordered_map
来源：http://wm.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pr.szsharing.cn

[S37] C++：set
来源：http://bo.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zu.muxihuayi.cn

[S38] C++：排序
来源：http://vh.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://dy.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://yn.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wd.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://dc.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ll.lnxyls.cn

[S41] C++：类与构造函数
来源：http://lv.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://km.nszjky.cn

[S42] C++：继承与虚函数
来源：http://ro.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://ni.jctech888.com.cn

[S43] C++：智能指针
来源：http://jw.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://uy.bjjhwx.cn

[S44] C++：引用传参
来源：http://pd.lnxyls.cn

void inc(int &x) { ++x; }
来源：http://tt.lnxyls.cn

[S45] C++：lambda
来源：http://mu.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ir.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://eo.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qn.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://oq.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jf.shxzukj.cn

[S48] C++：逐行读文件
来源：http://ck.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wi.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://ei.newstarts.cn

[S49] C++：写文件
来源：http://kl.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://em.shxzukj.cn

[S50] C++：格式化数字
来源：http://cp.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kr.newstarts.cn

[S51] C++：显式类型转换
来源：http://od.9csxet.cn

static_cast<double>(a) / b
来源：http://ln.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://uv.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://ti.nicolike.cn

[S53] C++：移动语义
来源：http://yp.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://ol.wgjwhj.cn

[S54] C++：异常处理
来源：http://sd.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mh.asd995.cn

[S55] C++：结构化绑定
来源：http://ss.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nl.muxihuayi.cn

[S56] C++：optional
来源：http://rf.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wu.bjjhwx.cn

[S57] C++：编译期常量
来源：http://rg.521024.cn

constexpr int N = 10;
来源：http://br.shxzskj.cn

[S58] C++：命名空间
来源：http://uk.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://po.9csxet.cn

[S59] C++：静态断言
来源：http://bt.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ds.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://fl.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qk.521024.cn

================================================================================
来源：http://jm.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ut.muxihuayi.cn

================================================================================
来源：http://be.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://ok.nszjky.cn

println("Hello")
来源：http://yo.shxzukj.cn

[T02] Kotlin：变量
来源：http://dv.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://is.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://aq.shtwfgs.cn

"值: $b"
来源：http://ab.9csxet.cn

[T04] Kotlin：空安全
来源：http://fh.nszjky.cn

val n: String? = null;  n?.length
来源：http://re.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://ta.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cy.colortex.cn

[T06] Kotlin：集合映射
来源：http://qo.gzmigu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sf.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://ev.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fw.panjiajie.cn

[T08] Kotlin：数据类
来源：http://rb.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://zg.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://hr.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://he.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://te.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bz.hahajie.cn

[T11] Kotlin：协程
来源：http://qe.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bl.muxihuayi.cn

[T12] Kotlin：解构声明
来源：http://ih.chemitech.net.cn

val (a, b) = Pair(1, 2)
来源：http://do.521024.cn

[T13] Kotlin：只读 Map
来源：http://nb.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://tz.9csxet.cn

[T14] Kotlin：循环
来源：http://rm.shxzskj.cn

for (i in 1..10) println(i)
来源：http://lg.521024.cn

[T15] Kotlin：接口
来源：http://vv.nszjky.cn

interface Shape { fun area(): Double }
来源：http://vr.shtwfgs.cn

[T16] Swift：Hello World
来源：http://kk.haigaiapp.cn

print("Hello")
来源：http://fj.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://rf.jctech888.com.cn

var a = 1;  let b = 2
来源：http://sx.colortex.cn

[T18] Swift：字符串插值
来源：http://mg.yuexingan06.cn

"值: \(b)"
来源：http://bn.hahajie.cn

[T19] Swift：可选绑定
来源：http://ef.gzmigu.cn

if let n = opt { print(n) }
来源：http://oj.shxzskj.cn

[T20] Swift：数组操作
来源：http://mm.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ti.wgjwhj.cn

[T21] Swift：遍历
来源：http://bq.huixinmuqiang.cn

for x in a { print(x) }
来源：http://qk.huixiangedu.cn

[T22] Swift：字典
来源：http://nn.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ic.newstarts.cn

[T23] Swift：函数
来源：http://kd.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oq.huanxung.cn

[T24] Swift：闭包
来源：http://qe.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lq.bjjhwx.cn

[T25] Swift：结构体
来源：http://gz.bookmarksfly.cn

struct P { var x: Int }
来源：http://tw.shtwfgs.cn

[T26] Swift：类与重写
来源：http://mj.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://ic.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://vw.nszjky.cn

do { try f() } catch { print(error) }
来源：http://rt.nicolike.cn

[T28] Swift：枚举
来源：http://ci.szsharing.cn

enum Color { case red, green }
来源：http://bs.521024.cn

[T29] Swift：guard 提前返回
来源：http://pw.panjiajie.cn

guard let x = opt else { return }
来源：http://uc.yuntaijiaju.cn

[T30] Swift：协议
来源：http://zl.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://iw.shxzskj.cn

[T31] Lua：Hello World
来源：http://jf.newstarts.cn

print("Hello")
来源：http://uw.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://yb.huanxung.cn

local a = 1
来源：http://un.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://lf.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mu.521024.cn

[T34] Lua：遍历表
来源：http://xt.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uq.521024.cn

[T35] Lua：字典表
来源：http://og.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://sg.nicolike.cn

[T36] Lua：函数
来源：http://dw.hnjuh.cn

function add(a, b) return a + b end
来源：http://ju.hahajie.cn

[T37] Lua：字符串拼接
来源：http://hm.nszjky.cn

"a" .. "b"
来源：http://xn.yuntaijiaju.cn

[T38] Lua：条件
来源：http://fx.muxihuayi.cn

if x > 0 then print("正") end
来源：http://hc.nszjky.cn

[T39] Lua：模式匹配
来源：http://os.bjjhwx.cn

string.find(s, "%d+")
来源：http://hw.colortex.cn

[T40] Lua：元表
来源：http://dq.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://uw.wgjwhj.cn

[T41] Perl：Hello World
来源：http://tf.szsharing.cn

print "Hello\n";
来源：http://bt.jctech888.com.cn

[T42] Perl：变量类型
来源：http://py.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uv.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://yz.nszjky.cn

"值: $a"
来源：http://wk.jctech888.com.cn

[T44] Perl：条件
来源：http://ve.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://ui.9csxet.cn

[T45] Perl：数组遍历
来源：http://sv.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://tb.hahajie.cn

[T46] Perl：哈希操作
来源：http://nf.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xi.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://vp.gzmigu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mg.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://mn.hahajie.cn

$s =~ s/old/new/g;
来源：http://bm.shxzskj.cn

[T49] Perl：函数
来源：http://lo.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ug.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://hl.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ga.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://xq.haigaiapp.cn

[T51] Scala：Hello World
来源：http://xc.lnxyls.cn

println("Hello")
来源：http://ou.bjjhwx.cn

[T52] Scala：变量
来源：http://hf.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://bz.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://ri.jianghongdianzi.cn

s"值: $b"
来源：http://ov.hnjuh.cn

[T54] Scala：集合映射
来源：http://af.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ad.newstarts.cn

[T55] Scala：集合过滤
来源：http://uw.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mb.nszjky.cn

[T56] Scala：样例类
来源：http://hl.newstarts.cn

case class User(name: String, age: Int)
来源：http://wn.hahajie.cn

[T57] Scala：模式匹配
来源：http://lx.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mx.nszjky.cn

[T58] Scala：函数定义
来源：http://dm.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ks.haigaiapp.cn

[T59] Scala：循环
来源：http://th.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://us.nicolike.cn

[T60] Scala：折叠
来源：http://yn.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ni.haigaiapp.cn

================================================================================
来源：http://qh.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bi.szsharing.cn

================================================================================
来源：http://gx.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://id.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zf.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://pg.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lb.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://qr.521024.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bu.colortex.cn

[U04] Py：变量调试打印
来源：http://wc.newstarts.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xk.nicolike.cn

[U05] Py：列表去重且保序
来源：http://nk.hahajie.cn

list(dict.fromkeys(arr))
来源：http://ni.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://tr.nicolike.cn

{**a, **b}
来源：http://ha.bookmarksfly.cn

[U07] Py：反转字典键值
来源：http://tf.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://mp.shxzskj.cn

[U08] Py：展平二维列表
来源：http://lr.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://ct.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://yt.jianghongdianzi.cn

max(d, key=d.get)
来源：http://ss.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://zb.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qs.hahajie.cn

[U11] Py：生成器表达式
来源：http://wd.hnjuh.cn

(x * 2 for x in arr)
来源：http://ou.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kr.hahajie.cn

Counter(arr).most_common(3)
来源：http://ip.jctech888.com.cn


<!-- 参考信息 -->