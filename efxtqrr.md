代发 wailian999

split -l 1000 big.log part_
来源：http://qb.nicolike.cn

[R74] 批量重命名
来源：http://pm.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mo.haigaiapp.cn

[R75] 导出环境变量
来源：http://xf.hnjuh.cn

export PATH="$HOME/bin:$PATH"
来源：http://br.colortex.cn

[R76] 使用临时文件
来源：http://em.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ln.gzmigu.cn

[R77] 读取用户输入
来源：http://ge.asd995.cn

read -rp "请输入: " ans
来源：http://ip.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://yt.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nb.gzmigu.cn

[R79] 解析命令行选项
来源：http://al.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zv.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://qn.chemitech.net.cn

time ./run.sh
来源：http://ra.wgjwhj.cn

================================================================================
来源：http://dq.newstarts.cn

S. C / C++ 专题
来源：http://nn.asd995.cn

================================================================================
来源：http://tz.bookmarksfly.cn

[S01] C：Hello World
来源：http://yf.huixinmuqiang.cn

#include <stdio.h>
来源：http://zq.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jj.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://nh.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://lv.shxzukj.cn

[S03] C：读入整数
来源：http://ou.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://th.bjjhwx.cn

[S04] C：字符串复制
来源：http://ow.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mh.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://pw.hnjuh.cn

strlen(s)
来源：http://zv.szxytkj.cn

[S06] C：字符串比较
来源：http://lo.9csxet.cn

strcmp(a, b) == 0
来源：http://pe.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://nl.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qh.gzmigu.cn

[S08] C：动态内存分配与释放
来源：http://tm.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kg.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://tp.hnjuh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dr.huanxung.cn

[S10] C：指针与解引用
来源：http://qc.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://qo.chemitech.net.cn

[S11] C：逐行读文件
来源：http://dl.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://jq.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ke.panjiajie.cn

fclose(f);
来源：http://ec.panjiajie.cn

[S12] C：写文件
来源：http://yl.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ye.9csxet.cn

[S13] C：宏定义
来源：http://cc.newstarts.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zy.bjjhwx.cn

[S14] C：枚举
来源：http://uf.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://qv.shxzskj.cn

[S15] C：类型转换
来源：http://ol.szxytkj.cn

(double) a / b
来源：http://zn.szxytkj.cn

[S16] C：位操作置位
来源：http://jn.haigaiapp.cn

x |= (1 << 3);
来源：http://hl.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://cn.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mu.hnjuh.cn

[S18] C：命令行参数
来源：http://sb.huanxung.cn

int main(int argc, char **argv)
来源：http://ig.szsharing.cn

[S19] C：快速排序
来源：http://sf.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ij.yuexingan06.cn

[S20] C：二分查找
来源：http://mg.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mh.muxihuayi.cn

[S21] C：字符类别判断
来源：http://dw.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hk.shxzskj.cn

[S22] C：字符串转数字
来源：http://ky.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://og.nszjky.cn

[S23] C：随机数
来源：http://nb.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sf.nicolike.cn

[S24] C：获取本地时间
来源：http://np.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cv.muxihuayi.cn

[S25] C：内存拷贝
来源：http://un.panjiajie.cn

memcpy(dst, src, n);
来源：http://jf.nicolike.cn

[S26] C：内存清零
来源：http://xk.szsharing.cn

memset(a, 0, sizeof a);
来源：http://on.newstarts.cn

[S27] C：定义常量
来源：http://fq.huixiangedu.cn

const double PI = 3.14159;
来源：http://db.yuntaijiaju.cn

[S28] C：静态变量
来源：http://ev.yuexingan06.cn

static int counter = 0;
来源：http://lw.bookmarksfly.cn

[S29] C：变参函数
来源：http://xz.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mu.muxihuayi.cn

[S30] C：头文件保护
来源：http://xm.colortex.cn

#ifndef X_H
来源：http://da.jctech888.com.cn

#define X_H
来源：http://fq.muxihuayi.cn

#endif
来源：http://ux.huixiangedu.cn

[S31] C++：Hello World
来源：http://io.haigaiapp.cn

#include <iostream>
来源：http://fz.bookmarksfly.cn

int main() { std::cout << "Hello\n"; }
来源：http://fc.shtwfgs.cn

[S32] C++：字符串
来源：http://sh.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://vx.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://cb.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vj.muxihuayi.cn

[S34] C++：遍历 vector
来源：http://tv.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://dg.jianghongdianzi.cn

[S35] C++：map
来源：http://zo.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mh.hahajie.cn

[S36] C++：unordered_map
来源：http://sg.9csxet.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ot.yuntaijiaju.cn

[S37] C++：set
来源：http://yi.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://op.yuexingan06.cn

[S38] C++：排序
来源：http://dy.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://id.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://ex.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://il.huanxung.cn

[S40] C++：查找元素
来源：http://vm.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://do.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://ku.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cr.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://vz.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://nf.shxzukj.cn

[S43] C++：智能指针
来源：http://bw.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://pc.chemitech.net.cn

[S44] C++：引用传参
来源：http://ow.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://nj.shtwfgs.cn

[S45] C++：lambda
来源：http://qi.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://na.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://xt.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cz.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://bq.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qi.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://rd.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xv.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://an.yuntaijiaju.cn

[S49] C++：写文件
来源：http://lb.colortex.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rd.lnxyls.cn

[S50] C++：格式化数字
来源：http://yi.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zc.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://ec.szsharing.cn

static_cast<double>(a) / b
来源：http://jh.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://lf.szsharing.cn

int size() const noexcept { return n_; }
来源：http://ul.huanxung.cn

[S53] C++：移动语义
来源：http://gy.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://wv.hahajie.cn

[S54] C++：异常处理
来源：http://bk.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vn.nszjky.cn

[S55] C++：结构化绑定
来源：http://ag.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rt.huixiangedu.cn

[S56] C++：optional
来源：http://fv.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mu.szsharing.cn

[S57] C++：编译期常量
来源：http://hc.huanxung.cn

constexpr int N = 10;
来源：http://cl.521024.cn

[S58] C++：命名空间
来源：http://mg.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://bf.haigaiapp.cn

[S59] C++：静态断言
来源：http://vz.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xx.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://ld.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qd.chemitech.net.cn

================================================================================
来源：http://iq.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vo.jianghongdianzi.cn

================================================================================
来源：http://ja.bjjhwx.cn

[T01] Kotlin：Hello World
来源：http://ut.bookmarksfly.cn

println("Hello")
来源：http://wl.nszjky.cn

[T02] Kotlin：变量
来源：http://re.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mf.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://od.lnxyls.cn

"值: $b"
来源：http://uy.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://th.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://sj.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://zb.colortex.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ic.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://et.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pj.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://rg.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vy.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://qp.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://yu.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://yu.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://ns.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://na.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ok.hnjuh.cn

[T11] Kotlin：协程
来源：http://vv.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://me.szsharing.cn

[T12] Kotlin：解构声明
来源：http://at.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://lu.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://dq.huanxung.cn

val m = mapOf("a" to 1)
来源：http://qe.nicolike.cn

[T14] Kotlin：循环
来源：http://vw.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://bt.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://bo.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://bp.bjjhwx.cn

[T16] Swift：Hello World
来源：http://ti.nicolike.cn

print("Hello")
来源：http://aq.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://vs.newstarts.cn

var a = 1;  let b = 2
来源：http://wg.shxzskj.cn

[T18] Swift：字符串插值
来源：http://ki.gzmigu.cn

"值: \(b)"
来源：http://ua.huanxung.cn

[T19] Swift：可选绑定
来源：http://hj.shtwfgs.cn

if let n = opt { print(n) }
来源：http://zq.szxytkj.cn

[T20] Swift：数组操作
来源：http://pq.wgjwhj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://od.jctech888.com.cn

[T21] Swift：遍历
来源：http://ci.panjiajie.cn

for x in a { print(x) }
来源：http://xn.hahajie.cn

[T22] Swift：字典
来源：http://bq.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tw.lnxyls.cn

[T23] Swift：函数
来源：http://ri.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tk.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://kz.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bj.521024.cn

[T25] Swift：结构体
来源：http://wi.9csxet.cn

struct P { var x: Int }
来源：http://nx.szxytkj.cn

[T26] Swift：类与重写
来源：http://cw.asd995.cn

class A: Base { override func f() {} }
来源：http://zo.lnxyls.cn

[T27] Swift：错误处理
来源：http://te.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://xp.lnxyls.cn

[T28] Swift：枚举
来源：http://ug.muxihuayi.cn

enum Color { case red, green }
来源：http://yd.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://se.nicolike.cn

guard let x = opt else { return }
来源：http://yi.panjiajie.cn

[T30] Swift：协议
来源：http://ca.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://ep.haigaiapp.cn

[T31] Lua：Hello World
来源：http://kv.shtwfgs.cn

print("Hello")
来源：http://si.lnxyls.cn

[T32] Lua：局部变量
来源：http://kq.nszjky.cn

local a = 1
来源：http://br.huanxung.cn

[T33] Lua：表（数组）
来源：http://nz.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zd.huixiangedu.cn

[T34] Lua：遍历表
来源：http://tf.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ya.hahajie.cn

[T35] Lua：字典表
来源：http://og.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://xi.jianghongdianzi.cn

[T36] Lua：函数
来源：http://rp.shtwfgs.cn

function add(a, b) return a + b end
来源：http://qb.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://qc.szsharing.cn

"a" .. "b"
来源：http://rd.hnjuh.cn

[T38] Lua：条件
来源：http://va.9csxet.cn

if x > 0 then print("正") end
来源：http://ow.yuexingan06.cn

[T39] Lua：模式匹配
来源：http://hy.hahajie.cn

string.find(s, "%d+")
来源：http://tx.shtwfgs.cn

[T40] Lua：元表
来源：http://mo.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://jc.szxytkj.cn

[T41] Perl：Hello World
来源：http://ec.huixinmuqiang.cn

print "Hello\n";
来源：http://cp.wgjwhj.cn

[T42] Perl：变量类型
来源：http://bu.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ov.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://bi.wgjwhj.cn

"值: $a"
来源：http://lr.jianghongdianzi.cn

[T44] Perl：条件
来源：http://pa.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://wr.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://iu.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://md.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://kf.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fr.hnjuh.cn

[T47] Perl：正则捕获
来源：http://zt.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kc.hahajie.cn

[T48] Perl：正则替换
来源：http://ox.panjiajie.cn

$s =~ s/old/new/g;
来源：http://sr.521024.cn

[T49] Perl：函数
来源：http://fj.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qi.nszjky.cn

[T50] Perl：逐行读文件
来源：http://yl.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xx.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://dq.hnjuh.cn

[T51] Scala：Hello World
来源：http://nk.hnjuh.cn

println("Hello")
来源：http://gv.chemitech.net.cn

[T52] Scala：变量
来源：http://et.haigaiapp.cn

val a = 1;  var b = 2
来源：http://gf.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://su.hnjuh.cn

s"值: $b"
来源：http://ev.huanxung.cn

[T54] Scala：集合映射
来源：http://ne.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://xa.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://ab.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kb.muxihuayi.cn

[T56] Scala：样例类
来源：http://by.huixiangedu.cn

case class User(name: String, age: Int)
来源：http://jj.lnxyls.cn

[T57] Scala：模式匹配
来源：http://fm.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gj.shtwfgs.cn

[T58] Scala：函数定义
来源：http://mc.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ac.521024.cn

[T59] Scala：循环
来源：http://xv.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://xa.yuexingan06.cn

[T60] Scala：折叠
来源：http://yh.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wy.lnxyls.cn

================================================================================
来源：http://bi.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gx.9csxet.cn

================================================================================
来源：http://fy.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://ur.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pz.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://ae.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tq.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://jq.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wq.hahajie.cn

[U04] Py：变量调试打印
来源：http://io.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ky.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://kg.521024.cn

list(dict.fromkeys(arr))
来源：http://wm.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://ho.haigaiapp.cn

{**a, **b}
来源：http://qs.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://ih.gzmigu.cn

{v: k for k, v in d.items()}
来源：http://bz.lnxyls.cn

[U08] Py：展平二维列表
来源：http://vt.szxytkj.cn

[y for x in nested for y in x]
来源：http://vf.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://yl.huixinmuqiang.cn

max(d, key=d.get)
来源：http://xj.bjjhwx.cn

[U10] Py：按值排序字典
来源：http://yi.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bz.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://lz.szxytkj.cn

(x * 2 for x in arr)
来源：http://ii.colortex.cn

[U12] Py：取出现最多的 3 个元素
来源：http://aa.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://qt.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://et.hahajie.cn

deque(maxlen=10)
来源：http://dt.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://em.huixiangedu.cn

defaultdict(list)
来源：http://fk.muxihuayi.cn


<!-- 参考信息 -->