代发 wailian999

free -h;  ps aux | grep nginx
来源：http://no.asd995.cn

[R64] 结束进程
来源：http://pp.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://sk.wgjwhj.cn

[R65] 查看端口占用
来源：http://dv.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oj.colortex.cn

[R66] 定时任务
来源：http://pw.haigaiapp.cn

crontab -e;  crontab -l
来源：http://rk.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://va.lnxyls.cn

openssl rand -hex 16
来源：http://nn.9csxet.cn

[R68] 计算文件校验值
来源：http://cu.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bu.colortex.cn

[R69] 生成随机密码
来源：http://jb.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://nu.lnxyls.cn

[R70] 时间戳与互转
来源：http://ms.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://ci.yuntaijiaju.cn

[R71] 日期格式化
来源：http://nc.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kd.muxihuayi.cn

[R72] 等待端口就绪
来源：http://hr.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nj.shxzukj.cn

[R73] 分割大日志
来源：http://fp.huanxung.cn

split -l 1000 big.log part_
来源：http://vl.chemitech.net.cn

[R74] 批量重命名
来源：http://yc.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://on.nicolike.cn

[R75] 导出环境变量
来源：http://py.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://hm.yuexingan06.cn

[R76] 使用临时文件
来源：http://uq.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sr.nicolike.cn

[R77] 读取用户输入
来源：http://pe.bjjhwx.cn

read -rp "请输入: " ans
来源：http://jm.szsharing.cn

[R78] 交互式菜单
来源：http://ao.hahajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ge.nszjky.cn

[R79] 解析命令行选项
来源：http://rq.yuexingan06.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://de.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://cu.nicolike.cn

time ./run.sh
来源：http://ao.colortex.cn

================================================================================
来源：http://hm.nszjky.cn

S. C / C++ 专题
来源：http://ue.yuexingan06.cn

================================================================================
来源：http://xm.shxzskj.cn

[S01] C：Hello World
来源：http://kw.colortex.cn

#include <stdio.h>
来源：http://iw.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yk.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://md.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://cw.haigaiapp.cn

[S03] C：读入整数
来源：http://na.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://py.521024.cn

[S04] C：字符串复制
来源：http://ye.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vg.bjjhwx.cn

[S05] C：字符串长度
来源：http://sj.521024.cn

strlen(s)
来源：http://ui.lnxyls.cn

[S06] C：字符串比较
来源：http://wk.shtwfgs.cn

strcmp(a, b) == 0
来源：http://ki.nszjky.cn

[S07] C：数组遍历求和
来源：http://nk.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ti.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://kg.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ti.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://tz.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cd.hahajie.cn

[S10] C：指针与解引用
来源：http://hl.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://rn.huanxung.cn

[S11] C：逐行读文件
来源：http://wd.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://jm.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rz.newstarts.cn

fclose(f);
来源：http://xh.yuexingan06.cn

[S12] C：写文件
来源：http://hy.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gv.bjjhwx.cn

[S13] C：宏定义
来源：http://ag.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uv.hahajie.cn

[S14] C：枚举
来源：http://zh.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://hx.muxihuayi.cn

[S15] C：类型转换
来源：http://kc.nszjky.cn

(double) a / b
来源：http://zr.chemitech.net.cn

[S16] C：位操作置位
来源：http://lu.nszjky.cn

x |= (1 << 3);
来源：http://es.huanxung.cn

[S17] C：安全拼接字符串
来源：http://am.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://go.muxihuayi.cn

[S18] C：命令行参数
来源：http://ba.9csxet.cn

int main(int argc, char **argv)
来源：http://jq.szxytkj.cn

[S19] C：快速排序
来源：http://se.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vw.9csxet.cn

[S20] C：二分查找
来源：http://ab.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ls.shxzskj.cn

[S21] C：字符类别判断
来源：http://wi.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://br.521024.cn

[S22] C：字符串转数字
来源：http://oo.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ml.yuntaijiaju.cn

[S23] C：随机数
来源：http://zy.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bk.shxzskj.cn

[S24] C：获取本地时间
来源：http://nq.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qa.huanxung.cn

[S25] C：内存拷贝
来源：http://po.huanxung.cn

memcpy(dst, src, n);
来源：http://ma.newstarts.cn

[S26] C：内存清零
来源：http://ol.szsharing.cn

memset(a, 0, sizeof a);
来源：http://mx.shxzukj.cn

[S27] C：定义常量
来源：http://qg.huixiangedu.cn

const double PI = 3.14159;
来源：http://nj.panjiajie.cn

[S28] C：静态变量
来源：http://we.huanxung.cn

static int counter = 0;
来源：http://iv.shtwfgs.cn

[S29] C：变参函数
来源：http://gq.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fx.huanxung.cn

[S30] C：头文件保护
来源：http://wb.shxzukj.cn

#ifndef X_H
来源：http://gt.muxihuayi.cn

#define X_H
来源：http://ej.yuntaijiaju.cn

#endif
来源：http://in.gzmigu.cn

[S31] C++：Hello World
来源：http://pv.asd995.cn

#include <iostream>
来源：http://ga.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://xd.hahajie.cn

[S32] C++：字符串
来源：http://ol.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://qn.shxzskj.cn

[S33] C++：vector 增删
来源：http://lf.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oa.lnxyls.cn

[S34] C++：遍历 vector
来源：http://fn.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://hz.haigaiapp.cn

[S35] C++：map
来源：http://gn.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vr.yuexingan06.cn

[S36] C++：unordered_map
来源：http://gg.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cx.colortex.cn

[S37] C++：set
来源：http://vz.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qq.colortex.cn

[S38] C++：排序
来源：http://nh.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://bb.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://sw.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cn.haigaiapp.cn

[S40] C++：查找元素
来源：http://ej.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nv.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://lv.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gw.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://fj.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://rs.bjjhwx.cn

[S43] C++：智能指针
来源：http://sc.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://yk.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://ga.hahajie.cn

void inc(int &x) { ++x; }
来源：http://lf.jianghongdianzi.cn

[S45] C++：lambda
来源：http://sp.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://le.nicolike.cn

[S46] C++：函数模板
来源：http://qg.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rv.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://gq.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://df.gzmigu.cn

[S48] C++：逐行读文件
来源：http://lc.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ex.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://cv.newstarts.cn

[S49] C++：写文件
来源：http://sg.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ed.hahajie.cn

[S50] C++：格式化数字
来源：http://rf.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oj.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://op.szsharing.cn

static_cast<double>(a) / b
来源：http://aw.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://cf.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://on.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://kc.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://hf.haigaiapp.cn

[S54] C++：异常处理
来源：http://jb.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rg.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://pb.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ci.yuexingan06.cn

[S56] C++：optional
来源：http://kc.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fh.yuexingan06.cn

[S57] C++：编译期常量
来源：http://ei.huixinmuqiang.cn

constexpr int N = 10;
来源：http://cp.gzmigu.cn

[S58] C++：命名空间
来源：http://ti.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://ev.shxzukj.cn

[S59] C++：静态断言
来源：http://gj.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zm.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://oy.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bh.nszjky.cn

================================================================================
来源：http://oa.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eg.hahajie.cn

================================================================================
来源：http://to.szxytkj.cn

[T01] Kotlin：Hello World
来源：http://xn.panjiajie.cn

println("Hello")
来源：http://vu.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://ea.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ea.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://ha.hnjuh.cn

"值: $b"
来源：http://ol.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://xu.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://gi.colortex.cn

[T05] Kotlin：when 表达式
来源：http://vd.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ef.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://yq.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ks.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://nm.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kr.panjiajie.cn

[T08] Kotlin：数据类
来源：http://we.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://wf.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://zy.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://dm.newstarts.cn

[T10] Kotlin：默认参数
来源：http://pw.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rb.9csxet.cn

[T11] Kotlin：协程
来源：http://rt.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xy.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://as.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://bu.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://lw.newstarts.cn

val m = mapOf("a" to 1)
来源：http://bw.newstarts.cn

[T14] Kotlin：循环
来源：http://ew.521024.cn

for (i in 1..10) println(i)
来源：http://gd.lnxyls.cn

[T15] Kotlin：接口
来源：http://ft.colortex.cn

interface Shape { fun area(): Double }
来源：http://mh.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://yp.nszjky.cn

print("Hello")
来源：http://ae.asd995.cn

[T17] Swift：变量与常量
来源：http://lj.jctech888.com.cn

var a = 1;  let b = 2
来源：http://rs.lnxyls.cn

[T18] Swift：字符串插值
来源：http://ix.shtwfgs.cn

"值: \(b)"
来源：http://mn.nszjky.cn

[T19] Swift：可选绑定
来源：http://wc.huanxung.cn

if let n = opt { print(n) }
来源：http://qe.jctech888.com.cn

[T20] Swift：数组操作
来源：http://zc.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ps.521024.cn

[T21] Swift：遍历
来源：http://jw.bjjhwx.cn

for x in a { print(x) }
来源：http://cd.haigaiapp.cn

[T22] Swift：字典
来源：http://xh.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://id.jianghongdianzi.cn

[T23] Swift：函数
来源：http://xk.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mb.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://hi.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vc.shtwfgs.cn

[T25] Swift：结构体
来源：http://va.wgjwhj.cn

struct P { var x: Int }
来源：http://qx.hnjuh.cn

[T26] Swift：类与重写
来源：http://gb.huanxung.cn

class A: Base { override func f() {} }
来源：http://vy.shxzukj.cn

[T27] Swift：错误处理
来源：http://td.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://nz.nszjky.cn

[T28] Swift：枚举
来源：http://zo.newstarts.cn

enum Color { case red, green }
来源：http://vr.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://cv.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://yv.shtwfgs.cn

[T30] Swift：协议
来源：http://em.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://kn.521024.cn

[T31] Lua：Hello World
来源：http://nv.bjjhwx.cn

print("Hello")
来源：http://lr.colortex.cn

[T32] Lua：局部变量
来源：http://pn.szsharing.cn

local a = 1
来源：http://wa.shxzukj.cn

[T33] Lua：表（数组）
来源：http://go.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sy.hahajie.cn

[T34] Lua：遍历表
来源：http://qo.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dj.muxihuayi.cn

[T35] Lua：字典表
来源：http://ej.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://cx.jianghongdianzi.cn

[T36] Lua：函数
来源：http://qi.chemitech.net.cn

function add(a, b) return a + b end
来源：http://fg.newstarts.cn

[T37] Lua：字符串拼接
来源：http://jo.yuntaijiaju.cn

"a" .. "b"
来源：http://gs.lnxyls.cn

[T38] Lua：条件
来源：http://zo.521024.cn

if x > 0 then print("正") end
来源：http://kh.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://vz.bjjhwx.cn

string.find(s, "%d+")
来源：http://ek.jianghongdianzi.cn

[T40] Lua：元表
来源：http://bs.hahajie.cn

setmetatable({}, { __index = base })
来源：http://tf.panjiajie.cn

[T41] Perl：Hello World
来源：http://ji.szxytkj.cn

print "Hello\n";
来源：http://lb.haigaiapp.cn

[T42] Perl：变量类型
来源：http://kp.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dy.newstarts.cn

[T43] Perl：字符串插值
来源：http://ea.jctech888.com.cn

"值: $a"
来源：http://gl.colortex.cn

[T44] Perl：条件
来源：http://az.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://cb.yuntaijiaju.cn

[T45] Perl：数组遍历
来源：http://aj.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://lp.asd995.cn

[T46] Perl：哈希操作
来源：http://eo.9csxet.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xp.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://we.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://se.jctech888.com.cn

[T48] Perl：正则替换
来源：http://nw.shtwfgs.cn

$s =~ s/old/new/g;
来源：http://tf.chemitech.net.cn

[T49] Perl：函数
来源：http://tn.szxytkj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fv.shtwfgs.cn

[T50] Perl：逐行读文件
来源：http://qe.newstarts.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jo.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://ac.szxytkj.cn

[T51] Scala：Hello World
来源：http://wq.szsharing.cn

println("Hello")
来源：http://vc.szsharing.cn

[T52] Scala：变量
来源：http://tp.9csxet.cn

val a = 1;  var b = 2
来源：http://tm.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://ws.wgjwhj.cn

s"值: $b"
来源：http://ya.jctech888.com.cn

[T54] Scala：集合映射
来源：http://od.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://cm.panjiajie.cn

[T55] Scala：集合过滤
来源：http://np.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qo.haigaiapp.cn

[T56] Scala：样例类
来源：http://wg.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://xs.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://tr.521024.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rm.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://gm.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kx.wgjwhj.cn

[T59] Scala：循环
来源：http://aq.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://tr.shxzskj.cn

[T60] Scala：折叠
来源：http://cv.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qg.szsharing.cn

================================================================================
来源：http://pm.szsharing.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ee.wgjwhj.cn

================================================================================
来源：http://wc.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://ga.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://it.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://ja.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jx.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://bu.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sw.huanxung.cn

[U04] Py：变量调试打印
来源：http://aq.jianghongdianzi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xq.huixiangedu.cn


<!-- 参考信息 -->