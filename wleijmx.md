代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://xb.huixinmuqiang.cn

[R72] 等待端口就绪
来源：http://ip.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lq.chemitech.net.cn

[R73] 分割大日志
来源：http://lo.panjiajie.cn

split -l 1000 big.log part_
来源：http://fw.yuntaijiaju.cn

[R74] 批量重命名
来源：http://bl.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ru.shxzskj.cn

[R75] 导出环境变量
来源：http://xg.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://gj.huixiangedu.cn

[R76] 使用临时文件
来源：http://lg.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vo.nicolike.cn

[R77] 读取用户输入
来源：http://cv.chemitech.net.cn

read -rp "请输入: " ans
来源：http://zj.huanxung.cn

[R78] 交互式菜单
来源：http://bs.hahajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ej.panjiajie.cn

[R79] 解析命令行选项
来源：http://mo.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vu.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://mq.yuexingan06.cn

time ./run.sh
来源：http://gg.haigaiapp.cn

================================================================================
来源：http://fj.yuexingan06.cn

S. C / C++ 专题
来源：http://pa.nicolike.cn

================================================================================
来源：http://pj.bjjhwx.cn

[S01] C：Hello World
来源：http://ds.shxzukj.cn

#include <stdio.h>
来源：http://tr.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mc.asd995.cn

[S02] C：变量与格式化输出
来源：http://ls.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://kl.huixiangedu.cn

[S03] C：读入整数
来源：http://ks.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://cn.bookmarksfly.cn

[S04] C：字符串复制
来源：http://og.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://da.yuexingan06.cn

[S05] C：字符串长度
来源：http://kt.gzmigu.cn

strlen(s)
来源：http://xj.hahajie.cn

[S06] C：字符串比较
来源：http://do.521024.cn

strcmp(a, b) == 0
来源：http://ol.lnxyls.cn

[S07] C：数组遍历求和
来源：http://fj.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tu.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://va.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wl.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://nt.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ww.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://dh.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://ll.panjiajie.cn

[S11] C：逐行读文件
来源：http://hq.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://nw.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://us.asd995.cn

fclose(f);
来源：http://xe.colortex.cn

[S12] C：写文件
来源：http://jj.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ax.huixinmuqiang.cn

[S13] C：宏定义
来源：http://oe.huanxung.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bi.newstarts.cn

[S14] C：枚举
来源：http://ix.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://bc.bookmarksfly.cn

[S15] C：类型转换
来源：http://hx.yuntaijiaju.cn

(double) a / b
来源：http://ge.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://ph.wgjwhj.cn

x |= (1 << 3);
来源：http://at.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://sn.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tn.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://ne.jctech888.com.cn

int main(int argc, char **argv)
来源：http://oz.yuntaijiaju.cn

[S19] C：快速排序
来源：http://ar.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ra.yuexingan06.cn

[S20] C：二分查找
来源：http://aj.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://co.newstarts.cn

[S21] C：字符类别判断
来源：http://lq.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fh.9csxet.cn

[S22] C：字符串转数字
来源：http://un.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lw.lnxyls.cn

[S23] C：随机数
来源：http://fy.9csxet.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fa.yuexingan06.cn

[S24] C：获取本地时间
来源：http://vi.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cl.521024.cn

[S25] C：内存拷贝
来源：http://cl.nszjky.cn

memcpy(dst, src, n);
来源：http://ff.shxzukj.cn

[S26] C：内存清零
来源：http://io.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://od.lnxyls.cn

[S27] C：定义常量
来源：http://li.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://ag.huanxung.cn

[S28] C：静态变量
来源：http://kr.newstarts.cn

static int counter = 0;
来源：http://br.panjiajie.cn

[S29] C：变参函数
来源：http://ea.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bp.lnxyls.cn

[S30] C：头文件保护
来源：http://xb.lnxyls.cn

#ifndef X_H
来源：http://ba.panjiajie.cn

#define X_H
来源：http://sk.shxzukj.cn

#endif
来源：http://lc.bookmarksfly.cn

[S31] C++：Hello World
来源：http://ge.shxzskj.cn

#include <iostream>
来源：http://ez.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://qz.nicolike.cn

[S32] C++：字符串
来源：http://ej.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://ep.shtwfgs.cn

[S33] C++：vector 增删
来源：http://or.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nx.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://tp.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://oc.yuexingan06.cn

[S35] C++：map
来源：http://bt.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zq.newstarts.cn

[S36] C++：unordered_map
来源：http://at.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gj.jianghongdianzi.cn

[S37] C++：set
来源：http://yk.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://be.jctech888.com.cn

[S38] C++：排序
来源：http://cv.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://ot.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://tx.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yr.shtwfgs.cn

[S40] C++：查找元素
来源：http://dg.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cy.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://yx.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pl.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://cj.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://mi.panjiajie.cn

[S43] C++：智能指针
来源：http://xa.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://ii.szxytkj.cn

[S44] C++：引用传参
来源：http://py.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://vf.hahajie.cn

[S45] C++：lambda
来源：http://go.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://th.lnxyls.cn

[S46] C++：函数模板
来源：http://si.jianghongdianzi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wy.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://ed.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nz.szsharing.cn

[S48] C++：逐行读文件
来源：http://zl.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jr.newstarts.cn

while (std::getline(in, line)) { }
来源：http://tk.muxihuayi.cn

[S49] C++：写文件
来源：http://ro.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hf.szsharing.cn

[S50] C++：格式化数字
来源：http://rl.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wl.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://ct.shxzukj.cn

static_cast<double>(a) / b
来源：http://om.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://lb.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://de.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://ts.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://je.521024.cn

[S54] C++：异常处理
来源：http://bs.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ea.nszjky.cn

[S55] C++：结构化绑定
来源：http://ja.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xg.huanxung.cn

[S56] C++：optional
来源：http://zb.jctech888.com.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yx.colortex.cn

[S57] C++：编译期常量
来源：http://lu.hahajie.cn

constexpr int N = 10;
来源：http://jh.szsharing.cn

[S58] C++：命名空间
来源：http://jb.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://zm.huixiangedu.cn

[S59] C++：静态断言
来源：http://id.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yj.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://hl.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nx.muxihuayi.cn

================================================================================
来源：http://af.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://os.wgjwhj.cn

================================================================================
来源：http://fa.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://yu.9csxet.cn

println("Hello")
来源：http://rs.bjjhwx.cn

[T02] Kotlin：变量
来源：http://qt.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cm.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://ip.shxzskj.cn

"值: $b"
来源：http://zf.nszjky.cn

[T04] Kotlin：空安全
来源：http://xm.szxytkj.cn

val n: String? = null;  n?.length
来源：http://ns.colortex.cn

[T05] Kotlin：when 表达式
来源：http://zk.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xw.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://ae.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ad.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://nu.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://je.panjiajie.cn

[T08] Kotlin：数据类
来源：http://nr.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://ki.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://bb.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://gc.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://yt.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wh.jctech888.com.cn

[T11] Kotlin：协程
来源：http://sw.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cb.szsharing.cn

[T12] Kotlin：解构声明
来源：http://mh.haigaiapp.cn

val (a, b) = Pair(1, 2)
来源：http://wo.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://qj.hahajie.cn

val m = mapOf("a" to 1)
来源：http://qb.hahajie.cn

[T14] Kotlin：循环
来源：http://ax.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://is.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://up.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://pq.lnxyls.cn

[T16] Swift：Hello World
来源：http://vk.huanxung.cn

print("Hello")
来源：http://qx.shxzukj.cn

[T17] Swift：变量与常量
来源：http://xf.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://xd.lnxyls.cn

[T18] Swift：字符串插值
来源：http://mk.muxihuayi.cn

"值: \(b)"
来源：http://te.lnxyls.cn

[T19] Swift：可选绑定
来源：http://av.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://ve.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://uh.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qk.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://yy.szsharing.cn

for x in a { print(x) }
来源：http://zk.shtwfgs.cn

[T22] Swift：字典
来源：http://kb.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xy.newstarts.cn

[T23] Swift：函数
来源：http://lv.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bj.bookmarksfly.cn

[T24] Swift：闭包
来源：http://ua.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vs.muxihuayi.cn

[T25] Swift：结构体
来源：http://yj.shxzskj.cn

struct P { var x: Int }
来源：http://tn.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://cu.szsharing.cn

class A: Base { override func f() {} }
来源：http://dw.shtwfgs.cn

[T27] Swift：错误处理
来源：http://dw.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://um.shxzukj.cn

[T28] Swift：枚举
来源：http://mn.jctech888.com.cn

enum Color { case red, green }
来源：http://tl.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://qn.muxihuayi.cn

guard let x = opt else { return }
来源：http://om.muxihuayi.cn

[T30] Swift：协议
来源：http://ho.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://bk.panjiajie.cn

[T31] Lua：Hello World
来源：http://rd.nszjky.cn

print("Hello")
来源：http://vm.huanxung.cn

[T32] Lua：局部变量
来源：http://lh.jianghongdianzi.cn

local a = 1
来源：http://ok.panjiajie.cn

[T33] Lua：表（数组）
来源：http://kd.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zb.shxzukj.cn

[T34] Lua：遍历表
来源：http://vk.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ic.newstarts.cn

[T35] Lua：字典表
来源：http://bz.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://ru.nszjky.cn

[T36] Lua：函数
来源：http://xe.shxzukj.cn

function add(a, b) return a + b end
来源：http://gw.9csxet.cn

[T37] Lua：字符串拼接
来源：http://in.hnjuh.cn

"a" .. "b"
来源：http://js.hnjuh.cn

[T38] Lua：条件
来源：http://et.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://dd.shtwfgs.cn

[T39] Lua：模式匹配
来源：http://xu.jctech888.com.cn

string.find(s, "%d+")
来源：http://fd.colortex.cn

[T40] Lua：元表
来源：http://uj.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://fz.wgjwhj.cn

[T41] Perl：Hello World
来源：http://av.bookmarksfly.cn

print "Hello\n";
来源：http://of.jctech888.com.cn

[T42] Perl：变量类型
来源：http://nn.hnjuh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ad.panjiajie.cn

[T43] Perl：字符串插值
来源：http://ic.colortex.cn

"值: $a"
来源：http://ml.yuexingan06.cn

[T44] Perl：条件
来源：http://ha.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://pm.huixinmuqiang.cn

[T45] Perl：数组遍历
来源：http://yv.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://pw.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://gi.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pm.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://ok.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://md.muxihuayi.cn

[T48] Perl：正则替换
来源：http://lo.nicolike.cn

$s =~ s/old/new/g;
来源：http://ew.nszjky.cn

[T49] Perl：函数
来源：http://js.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://px.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://ah.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nx.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://vv.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://iv.huanxung.cn

println("Hello")
来源：http://eq.shxzukj.cn

[T52] Scala：变量
来源：http://wi.yuexingan06.cn

val a = 1;  var b = 2
来源：http://mm.colortex.cn

[T53] Scala：字符串插值
来源：http://zj.shxzukj.cn

s"值: $b"
来源：http://jk.nszjky.cn

[T54] Scala：集合映射
来源：http://kl.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://hf.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://fa.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rz.wgjwhj.cn

[T56] Scala：样例类
来源：http://lw.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://nu.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://mu.haigaiapp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pd.yuexingan06.cn

[T58] Scala：函数定义
来源：http://rv.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://av.hahajie.cn

[T59] Scala：循环
来源：http://hx.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://si.newstarts.cn

[T60] Scala：折叠
来源：http://vv.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ze.gzmigu.cn

================================================================================
来源：http://ze.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dh.szsharing.cn

================================================================================
来源：http://lu.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://ju.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ap.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://uq.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ht.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://ce.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fr.szsharing.cn

[U04] Py：变量调试打印
来源：http://sm.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qq.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://is.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://px.shxzukj.cn

[U06] Py：合并两个字典
来源：http://zl.bjjhwx.cn

{**a, **b}
来源：http://zu.gzmigu.cn

[U07] Py：反转字典键值
来源：http://cy.szsharing.cn

{v: k for k, v in d.items()}
来源：http://xe.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://du.shxzukj.cn

[y for x in nested for y in x]
来源：http://ev.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://oz.haigaiapp.cn

max(d, key=d.get)
来源：http://se.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://pj.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ww.asd995.cn

[U11] Py：生成器表达式
来源：http://mx.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://ko.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cv.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://ds.newstarts.cn


<!-- 参考信息 -->