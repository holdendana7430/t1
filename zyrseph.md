代发 wailian999

split -l 1000 big.log part_
来源：http://kk.huixiangedu.cn

[R74] 批量重命名
来源：http://md.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kz.newstarts.cn

[R75] 导出环境变量
来源：http://xo.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://zn.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://yg.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ex.hahajie.cn

[R77] 读取用户输入
来源：http://do.szsharing.cn

read -rp "请输入: " ans
来源：http://sm.huanxung.cn

[R78] 交互式菜单
来源：http://ee.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mj.nicolike.cn

[R79] 解析命令行选项
来源：http://sm.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uc.wgjwhj.cn

[R80] 查看脚本执行耗时
来源：http://yf.chemitech.net.cn

time ./run.sh
来源：http://xu.jctech888.com.cn

================================================================================
来源：http://nl.wgjwhj.cn

S. C / C++ 专题
来源：http://pn.jianghongdianzi.cn

================================================================================
来源：http://jz.szxytkj.cn

[S01] C：Hello World
来源：http://uf.jianghongdianzi.cn

#include <stdio.h>
来源：http://of.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://to.nszjky.cn

[S02] C：变量与格式化输出
来源：http://qg.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://ol.asd995.cn

[S03] C：读入整数
来源：http://fb.newstarts.cn

int x; scanf("%d", &x);
来源：http://pj.panjiajie.cn

[S04] C：字符串复制
来源：http://jc.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lc.huixiangedu.cn

[S05] C：字符串长度
来源：http://bm.yuexingan06.cn

strlen(s)
来源：http://wy.lnxyls.cn

[S06] C：字符串比较
来源：http://gj.yuexingan06.cn

strcmp(a, b) == 0
来源：http://ce.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://to.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gq.colortex.cn

[S08] C：动态内存分配与释放
来源：http://ch.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://th.asd995.cn

[S09] C：结构体定义与初始化
来源：http://gh.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vz.521024.cn

[S10] C：指针与解引用
来源：http://sg.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://ii.jctech888.com.cn

[S11] C：逐行读文件
来源：http://vf.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://ej.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lu.asd995.cn

fclose(f);
来源：http://nl.haigaiapp.cn

[S12] C：写文件
来源：http://hz.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ml.gzmigu.cn

[S13] C：宏定义
来源：http://sa.wgjwhj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jb.huanxung.cn

[S14] C：枚举
来源：http://ph.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://aa.nszjky.cn

[S15] C：类型转换
来源：http://ko.huanxung.cn

(double) a / b
来源：http://nk.shxzskj.cn

[S16] C：位操作置位
来源：http://iy.huanxung.cn

x |= (1 << 3);
来源：http://qn.szsharing.cn

[S17] C：安全拼接字符串
来源：http://hj.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gz.shxzukj.cn

[S18] C：命令行参数
来源：http://iz.nszjky.cn

int main(int argc, char **argv)
来源：http://nv.9csxet.cn

[S19] C：快速排序
来源：http://mq.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hi.bjjhwx.cn

[S20] C：二分查找
来源：http://ci.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xy.521024.cn

[S21] C：字符类别判断
来源：http://tt.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lr.shxzukj.cn

[S22] C：字符串转数字
来源：http://si.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pb.muxihuayi.cn

[S23] C：随机数
来源：http://mb.huixinmuqiang.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kl.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://va.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cb.nicolike.cn

[S25] C：内存拷贝
来源：http://ok.huanxung.cn

memcpy(dst, src, n);
来源：http://ue.jianghongdianzi.cn

[S26] C：内存清零
来源：http://mt.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://zg.jianghongdianzi.cn

[S27] C：定义常量
来源：http://mf.521024.cn

const double PI = 3.14159;
来源：http://xg.gzmigu.cn

[S28] C：静态变量
来源：http://ce.lnxyls.cn

static int counter = 0;
来源：http://od.szsharing.cn

[S29] C：变参函数
来源：http://rq.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zm.huixiangedu.cn

[S30] C：头文件保护
来源：http://ud.wgjwhj.cn

#ifndef X_H
来源：http://nb.nicolike.cn

#define X_H
来源：http://vb.hnjuh.cn

#endif
来源：http://kt.wgjwhj.cn

[S31] C++：Hello World
来源：http://rr.haigaiapp.cn

#include <iostream>
来源：http://ba.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://wy.szsharing.cn

[S32] C++：字符串
来源：http://fx.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://ge.shtwfgs.cn

[S33] C++：vector 增删
来源：http://rd.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vb.huanxung.cn

[S34] C++：遍历 vector
来源：http://qj.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://uj.panjiajie.cn

[S35] C++：map
来源：http://pv.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://or.newstarts.cn

[S36] C++：unordered_map
来源：http://db.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rb.yuexingan06.cn

[S37] C++：set
来源：http://yd.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mn.asd995.cn

[S38] C++：排序
来源：http://mg.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://tx.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://rz.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cj.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://ns.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ai.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://bl.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qk.asd995.cn

[S42] C++：继承与虚函数
来源：http://co.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://ro.panjiajie.cn

[S43] C++：智能指针
来源：http://yo.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://jo.szxytkj.cn

[S44] C++：引用传参
来源：http://lx.shtwfgs.cn

void inc(int &x) { ++x; }
来源：http://si.huixinmuqiang.cn

[S45] C++：lambda
来源：http://vg.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qy.huixiangedu.cn

[S46] C++：函数模板
来源：http://vm.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vf.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://zu.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wi.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://pb.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cr.jctech888.com.cn

while (std::getline(in, line)) { }
来源：http://au.yuexingan06.cn

[S49] C++：写文件
来源：http://co.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ft.shtwfgs.cn

[S50] C++：格式化数字
来源：http://nj.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nk.shxzskj.cn

[S51] C++：显式类型转换
来源：http://vl.haigaiapp.cn

static_cast<double>(a) / b
来源：http://co.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://st.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://qt.lnxyls.cn

[S53] C++：移动语义
来源：http://tt.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://nu.9csxet.cn

[S54] C++：异常处理
来源：http://in.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ad.huanxung.cn

[S55] C++：结构化绑定
来源：http://pv.bjjhwx.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fq.hnjuh.cn

[S56] C++：optional
来源：http://ce.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yt.shxzskj.cn

[S57] C++：编译期常量
来源：http://hz.panjiajie.cn

constexpr int N = 10;
来源：http://od.huanxung.cn

[S58] C++：命名空间
来源：http://rw.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://jt.panjiajie.cn

[S59] C++：静态断言
来源：http://ly.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mc.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://ck.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nt.jianghongdianzi.cn

================================================================================
来源：http://bd.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nv.hnjuh.cn

================================================================================
来源：http://mu.huanxung.cn

[T01] Kotlin：Hello World
来源：http://qi.hahajie.cn

println("Hello")
来源：http://bm.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://jk.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ce.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://xy.shxzskj.cn

"值: $b"
来源：http://hn.panjiajie.cn

[T04] Kotlin：空安全
来源：http://me.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://pp.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://fk.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fz.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://uh.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gz.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://xn.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cz.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://ef.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://jd.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://jk.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://mg.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://ls.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ci.shxzukj.cn

[T11] Kotlin：协程
来源：http://xn.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fb.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://nt.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://em.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://im.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://ti.hnjuh.cn

[T14] Kotlin：循环
来源：http://hl.9csxet.cn

for (i in 1..10) println(i)
来源：http://fe.chemitech.net.cn

[T15] Kotlin：接口
来源：http://gm.nicolike.cn

interface Shape { fun area(): Double }
来源：http://bh.shxzukj.cn

[T16] Swift：Hello World
来源：http://jq.huanxung.cn

print("Hello")
来源：http://yx.shxzskj.cn

[T17] Swift：变量与常量
来源：http://cj.gzmigu.cn

var a = 1;  let b = 2
来源：http://tv.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://xn.szxytkj.cn

"值: \(b)"
来源：http://qe.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://et.huanxung.cn

if let n = opt { print(n) }
来源：http://py.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://fd.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vc.wgjwhj.cn

[T21] Swift：遍历
来源：http://rc.hahajie.cn

for x in a { print(x) }
来源：http://dk.521024.cn

[T22] Swift：字典
来源：http://sa.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ke.newstarts.cn

[T23] Swift：函数
来源：http://wr.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sm.yuexingan06.cn

[T24] Swift：闭包
来源：http://ir.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://py.shxzskj.cn

[T25] Swift：结构体
来源：http://jy.9csxet.cn

struct P { var x: Int }
来源：http://hc.jctech888.com.cn

[T26] Swift：类与重写
来源：http://se.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://wr.hnjuh.cn

[T27] Swift：错误处理
来源：http://sw.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://ua.huixiangedu.cn

[T28] Swift：枚举
来源：http://wb.nszjky.cn

enum Color { case red, green }
来源：http://kz.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://wd.gzmigu.cn

guard let x = opt else { return }
来源：http://xi.jianghongdianzi.cn

[T30] Swift：协议
来源：http://ro.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://kp.panjiajie.cn

[T31] Lua：Hello World
来源：http://bi.yuntaijiaju.cn

print("Hello")
来源：http://qr.szsharing.cn

[T32] Lua：局部变量
来源：http://sr.hahajie.cn

local a = 1
来源：http://hc.9csxet.cn

[T33] Lua：表（数组）
来源：http://qt.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vw.jctech888.com.cn

[T34] Lua：遍历表
来源：http://gr.521024.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rc.shtwfgs.cn

[T35] Lua：字典表
来源：http://vw.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://vt.panjiajie.cn

[T36] Lua：函数
来源：http://xi.shtwfgs.cn

function add(a, b) return a + b end
来源：http://gn.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://mk.huixinmuqiang.cn

"a" .. "b"
来源：http://ez.gzmigu.cn

[T38] Lua：条件
来源：http://fn.colortex.cn

if x > 0 then print("正") end
来源：http://cj.panjiajie.cn

[T39] Lua：模式匹配
来源：http://ue.huanxung.cn

string.find(s, "%d+")
来源：http://zy.gzmigu.cn

[T40] Lua：元表
来源：http://rr.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://tr.huanxung.cn

[T41] Perl：Hello World
来源：http://ak.huanxung.cn

print "Hello\n";
来源：http://zt.huixiangedu.cn

[T42] Perl：变量类型
来源：http://ye.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://st.bookmarksfly.cn

[T43] Perl：字符串插值
来源：http://cd.huixinmuqiang.cn

"值: $a"
来源：http://vw.panjiajie.cn

[T44] Perl：条件
来源：http://sa.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://aj.hnjuh.cn

[T45] Perl：数组遍历
来源：http://xe.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://cr.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://pv.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hd.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://rl.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rf.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://jl.panjiajie.cn

$s =~ s/old/new/g;
来源：http://bs.shxzskj.cn

[T49] Perl：函数
来源：http://cy.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zy.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://tu.asd995.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://to.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://ex.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://qr.huixinmuqiang.cn

println("Hello")
来源：http://ne.bjjhwx.cn

[T52] Scala：变量
来源：http://if.nszjky.cn

val a = 1;  var b = 2
来源：http://df.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://tg.shxzukj.cn

s"值: $b"
来源：http://vg.lnxyls.cn

[T54] Scala：集合映射
来源：http://fk.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://fr.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://ut.chemitech.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ep.9csxet.cn

[T56] Scala：样例类
来源：http://up.gzmigu.cn

case class User(name: String, age: Int)
来源：http://wo.9csxet.cn

[T57] Scala：模式匹配
来源：http://xo.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ki.gzmigu.cn

[T58] Scala：函数定义
来源：http://rf.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vt.asd995.cn

[T59] Scala：循环
来源：http://wr.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://df.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://us.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jz.huanxung.cn

================================================================================
来源：http://ow.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hh.szsharing.cn

================================================================================
来源：http://ry.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://cd.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bw.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://dk.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zq.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://vs.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ah.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://ab.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ej.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://dz.newstarts.cn

list(dict.fromkeys(arr))
来源：http://gq.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://kj.gzmigu.cn

{**a, **b}
来源：http://dl.colortex.cn

[U07] Py：反转字典键值
来源：http://av.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://vs.9csxet.cn

[U08] Py：展平二维列表
来源：http://ab.nicolike.cn

[y for x in nested for y in x]
来源：http://kr.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://kz.jctech888.com.cn

max(d, key=d.get)
来源：http://zj.huanxung.cn

[U10] Py：按值排序字典
来源：http://xx.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wx.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://yk.lnxyls.cn

(x * 2 for x in arr)
来源：http://gr.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gn.shxzukj.cn

Counter(arr).most_common(3)
来源：http://ia.panjiajie.cn

[U13] Py：固定长度队列
来源：http://tx.lnxyls.cn

deque(maxlen=10)
来源：http://ro.9csxet.cn

[U14] Py：分组收集到列表
来源：http://yo.hnjuh.cn

defaultdict(list)
来源：http://rz.huixinmuqiang.cn


<!-- 参考信息 -->