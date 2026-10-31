代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://ed.shtwfgs.cn

[R72] 等待端口就绪
来源：http://ue.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hg.521024.cn

[R73] 分割大日志
来源：http://mr.chemitech.net.cn

split -l 1000 big.log part_
来源：http://sf.huanxung.cn

[R74] 批量重命名
来源：http://yx.newstarts.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ty.nszjky.cn

[R75] 导出环境变量
来源：http://wv.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://hw.nicolike.cn

[R76] 使用临时文件
来源：http://yi.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ws.colortex.cn

[R77] 读取用户输入
来源：http://vb.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://un.haigaiapp.cn

[R78] 交互式菜单
来源：http://cf.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bz.colortex.cn

[R79] 解析命令行选项
来源：http://ni.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mr.521024.cn

[R80] 查看脚本执行耗时
来源：http://ex.nicolike.cn

time ./run.sh
来源：http://dt.haigaiapp.cn

================================================================================
来源：http://es.newstarts.cn

S. C / C++ 专题
来源：http://mo.521024.cn

================================================================================
来源：http://vc.bjjhwx.cn

[S01] C：Hello World
来源：http://rh.gzmigu.cn

#include <stdio.h>
来源：http://ek.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hp.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://lf.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://lx.chemitech.net.cn

[S03] C：读入整数
来源：http://gu.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://dm.colortex.cn

[S04] C：字符串复制
来源：http://ll.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mr.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://ir.newstarts.cn

strlen(s)
来源：http://so.nszjky.cn

[S06] C：字符串比较
来源：http://zi.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://cy.hnjuh.cn

[S07] C：数组遍历求和
来源：http://bj.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ps.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://es.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ts.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://vm.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jb.colortex.cn

[S10] C：指针与解引用
来源：http://xp.colortex.cn

int *p = &a;  *p = 5;
来源：http://pj.huixiangedu.cn

[S11] C：逐行读文件
来源：http://ak.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://ng.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://se.chemitech.net.cn

fclose(f);
来源：http://vl.haigaiapp.cn

[S12] C：写文件
来源：http://hr.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kk.bjjhwx.cn

[S13] C：宏定义
来源：http://xq.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ts.bookmarksfly.cn

[S14] C：枚举
来源：http://gq.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://yy.szxytkj.cn

[S15] C：类型转换
来源：http://ig.colortex.cn

(double) a / b
来源：http://oi.shtwfgs.cn

[S16] C：位操作置位
来源：http://kx.shxzukj.cn

x |= (1 << 3);
来源：http://or.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://lg.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zw.gzmigu.cn

[S18] C：命令行参数
来源：http://ve.szsharing.cn

int main(int argc, char **argv)
来源：http://pl.jianghongdianzi.cn

[S19] C：快速排序
来源：http://av.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gs.haigaiapp.cn

[S20] C：二分查找
来源：http://sh.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qc.wgjwhj.cn

[S21] C：字符类别判断
来源：http://wt.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ng.shxzukj.cn

[S22] C：字符串转数字
来源：http://go.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rh.huixinmuqiang.cn

[S23] C：随机数
来源：http://oh.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ds.lnxyls.cn

[S24] C：获取本地时间
来源：http://dr.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bg.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://tc.szxytkj.cn

memcpy(dst, src, n);
来源：http://os.shxzskj.cn

[S26] C：内存清零
来源：http://qz.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://jf.yuntaijiaju.cn

[S27] C：定义常量
来源：http://oz.yuexingan06.cn

const double PI = 3.14159;
来源：http://vj.yuntaijiaju.cn

[S28] C：静态变量
来源：http://wt.yuexingan06.cn

static int counter = 0;
来源：http://cb.yuexingan06.cn

[S29] C：变参函数
来源：http://wy.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dp.hnjuh.cn

[S30] C：头文件保护
来源：http://wv.colortex.cn

#ifndef X_H
来源：http://nl.nicolike.cn

#define X_H
来源：http://tr.bjjhwx.cn

#endif
来源：http://ad.521024.cn

[S31] C++：Hello World
来源：http://qp.haigaiapp.cn

#include <iostream>
来源：http://cg.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://hh.huanxung.cn

[S32] C++：字符串
来源：http://ix.hahajie.cn

std::string s = "hi";  s += "!";
来源：http://zh.shxzukj.cn

[S33] C++：vector 增删
来源：http://up.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vc.asd995.cn

[S34] C++：遍历 vector
来源：http://lg.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://lu.newstarts.cn

[S35] C++：map
来源：http://nd.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rp.muxihuayi.cn

[S36] C++：unordered_map
来源：http://zh.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kq.nszjky.cn

[S37] C++：set
来源：http://bv.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fw.lnxyls.cn

[S38] C++：排序
来源：http://kh.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://ed.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://pc.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mg.nszjky.cn

[S40] C++：查找元素
来源：http://yy.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ej.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://dy.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ao.huanxung.cn

[S42] C++：继承与虚函数
来源：http://fd.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://yo.shtwfgs.cn

[S43] C++：智能指针
来源：http://it.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://wx.asd995.cn

[S44] C++：引用传参
来源：http://se.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://ck.huixiangedu.cn

[S45] C++：lambda
来源：http://dy.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yt.521024.cn

[S46] C++：函数模板
来源：http://rc.yuntaijiaju.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ly.yuexingan06.cn

[S47] C++：结构化绑定遍历
来源：http://ls.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rt.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://cm.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fg.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://ga.jctech888.com.cn

[S49] C++：写文件
来源：http://ji.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bp.wgjwhj.cn

[S50] C++：格式化数字
来源：http://ki.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qz.bookmarksfly.cn

[S51] C++：显式类型转换
来源：http://vq.shxzskj.cn

static_cast<double>(a) / b
来源：http://yx.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://er.shxzukj.cn

int size() const noexcept { return n_; }
来源：http://af.haigaiapp.cn

[S53] C++：移动语义
来源：http://id.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://qx.bookmarksfly.cn

[S54] C++：异常处理
来源：http://ow.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ts.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://bp.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yl.huanxung.cn

[S56] C++：optional
来源：http://yg.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://li.gzmigu.cn

[S57] C++：编译期常量
来源：http://ql.bookmarksfly.cn

constexpr int N = 10;
来源：http://kz.9csxet.cn

[S58] C++：命名空间
来源：http://dj.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://jf.colortex.cn

[S59] C++：静态断言
来源：http://sr.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://du.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://wc.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fi.9csxet.cn

================================================================================
来源：http://ra.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qv.yuexingan06.cn

================================================================================
来源：http://bk.asd995.cn

[T01] Kotlin：Hello World
来源：http://ba.jctech888.com.cn

println("Hello")
来源：http://mv.lnxyls.cn

[T02] Kotlin：变量
来源：http://nq.gzmigu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dj.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://ew.huanxung.cn

"值: $b"
来源：http://tr.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://ar.newstarts.cn

val n: String? = null;  n?.length
来源：http://rh.asd995.cn

[T05] Kotlin：when 表达式
来源：http://rg.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://br.colortex.cn

[T06] Kotlin：集合映射
来源：http://zj.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tt.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://oh.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fs.gzmigu.cn

[T08] Kotlin：数据类
来源：http://vi.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://ur.asd995.cn

[T09] Kotlin：扩展函数
来源：http://yz.colortex.cn

fun String.exclaim() = this + "!"
来源：http://cs.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://xh.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lu.szsharing.cn

[T11] Kotlin：协程
来源：http://mk.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://iq.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://wf.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://jq.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://tl.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://nv.hahajie.cn

[T14] Kotlin：循环
来源：http://il.colortex.cn

for (i in 1..10) println(i)
来源：http://fo.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://rn.9csxet.cn

interface Shape { fun area(): Double }
来源：http://gy.szsharing.cn

[T16] Swift：Hello World
来源：http://ak.asd995.cn

print("Hello")
来源：http://vz.newstarts.cn

[T17] Swift：变量与常量
来源：http://ci.shtwfgs.cn

var a = 1;  let b = 2
来源：http://vl.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://sw.panjiajie.cn

"值: \(b)"
来源：http://kg.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://re.huanxung.cn

if let n = opt { print(n) }
来源：http://ee.yuexingan06.cn

[T20] Swift：数组操作
来源：http://ce.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ve.shtwfgs.cn

[T21] Swift：遍历
来源：http://rk.chemitech.net.cn

for x in a { print(x) }
来源：http://ys.521024.cn

[T22] Swift：字典
来源：http://tc.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ry.huanxung.cn

[T23] Swift：函数
来源：http://gh.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tk.hnjuh.cn

[T24] Swift：闭包
来源：http://py.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ck.colortex.cn

[T25] Swift：结构体
来源：http://qj.lnxyls.cn

struct P { var x: Int }
来源：http://gs.huixiangedu.cn

[T26] Swift：类与重写
来源：http://qq.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://pc.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://rq.lnxyls.cn

do { try f() } catch { print(error) }
来源：http://pg.hnjuh.cn

[T28] Swift：枚举
来源：http://jo.lnxyls.cn

enum Color { case red, green }
来源：http://ez.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://lc.colortex.cn

guard let x = opt else { return }
来源：http://if.yuntaijiaju.cn

[T30] Swift：协议
来源：http://bs.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://wu.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://ny.yuntaijiaju.cn

print("Hello")
来源：http://mg.shxzukj.cn

[T32] Lua：局部变量
来源：http://ry.huixiangedu.cn

local a = 1
来源：http://bc.9csxet.cn

[T33] Lua：表（数组）
来源：http://du.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rd.wgjwhj.cn

[T34] Lua：遍历表
来源：http://gz.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ot.panjiajie.cn

[T35] Lua：字典表
来源：http://py.nszjky.cn

local d = { a = 1 };  d.b = 2
来源：http://oq.huanxung.cn

[T36] Lua：函数
来源：http://wq.jctech888.com.cn

function add(a, b) return a + b end
来源：http://me.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://xa.huanxung.cn

"a" .. "b"
来源：http://uc.hnjuh.cn

[T38] Lua：条件
来源：http://gy.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://xk.lnxyls.cn

[T39] Lua：模式匹配
来源：http://ry.nszjky.cn

string.find(s, "%d+")
来源：http://ds.jctech888.com.cn

[T40] Lua：元表
来源：http://vv.nszjky.cn

setmetatable({}, { __index = base })
来源：http://gi.shxzukj.cn

[T41] Perl：Hello World
来源：http://op.nszjky.cn

print "Hello\n";
来源：http://sj.shtwfgs.cn

[T42] Perl：变量类型
来源：http://gn.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nk.szxytkj.cn

[T43] Perl：字符串插值
来源：http://zf.huixiangedu.cn

"值: $a"
来源：http://ae.9csxet.cn

[T44] Perl：条件
来源：http://zl.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://ef.nicolike.cn

[T45] Perl：数组遍历
来源：http://yf.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://nr.hahajie.cn

[T46] Perl：哈希操作
来源：http://yu.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mm.panjiajie.cn

[T47] Perl：正则捕获
来源：http://xs.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ef.lnxyls.cn

[T48] Perl：正则替换
来源：http://sy.panjiajie.cn

$s =~ s/old/new/g;
来源：http://ts.colortex.cn

[T49] Perl：函数
来源：http://vd.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ez.9csxet.cn

[T50] Perl：逐行读文件
来源：http://sw.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qp.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://st.hahajie.cn

[T51] Scala：Hello World
来源：http://qp.9csxet.cn

println("Hello")
来源：http://wf.panjiajie.cn

[T52] Scala：变量
来源：http://pg.shxzskj.cn

val a = 1;  var b = 2
来源：http://yu.newstarts.cn

[T53] Scala：字符串插值
来源：http://ft.9csxet.cn

s"值: $b"
来源：http://op.haigaiapp.cn

[T54] Scala：集合映射
来源：http://tf.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://gy.nszjky.cn

[T55] Scala：集合过滤
来源：http://oj.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qo.shxzukj.cn

[T56] Scala：样例类
来源：http://ss.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://ba.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://kp.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fd.nszjky.cn

[T58] Scala：函数定义
来源：http://fv.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ax.521024.cn

[T59] Scala：循环
来源：http://yj.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://aj.huanxung.cn

[T60] Scala：折叠
来源：http://ds.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kh.shxzukj.cn

================================================================================
来源：http://ne.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nn.shxzukj.cn

================================================================================
来源：http://ly.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://ak.huixinmuqiang.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tw.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://cu.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tm.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://yf.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xc.shxzskj.cn

[U04] Py：变量调试打印
来源：http://pp.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ew.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://ai.colortex.cn

list(dict.fromkeys(arr))
来源：http://nt.shxzukj.cn

[U06] Py：合并两个字典
来源：http://zq.bookmarksfly.cn

{**a, **b}
来源：http://ui.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://ac.521024.cn

{v: k for k, v in d.items()}
来源：http://rn.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://jy.muxihuayi.cn

[y for x in nested for y in x]
来源：http://he.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://cn.colortex.cn

max(d, key=d.get)
来源：http://bc.9csxet.cn

[U10] Py：按值排序字典
来源：http://lz.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wr.hnjuh.cn

[U11] Py：生成器表达式
来源：http://vf.szxytkj.cn

(x * 2 for x in arr)
来源：http://vb.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://co.shxzukj.cn

Counter(arr).most_common(3)
来源：http://qx.lnxyls.cn


<!-- 参考信息 -->