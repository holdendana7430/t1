代发 wailian999

free -h;  ps aux | grep nginx
来源：http://hg.521024.cn

[R64] 结束进程
来源：http://kz.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://go.yuexingan06.cn

[R65] 查看端口占用
来源：http://dn.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qn.shtwfgs.cn

[R66] 定时任务
来源：http://dm.521024.cn

crontab -e;  crontab -l
来源：http://af.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://sn.shxzskj.cn

openssl rand -hex 16
来源：http://ib.521024.cn

[R68] 计算文件校验值
来源：http://vm.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rw.nicolike.cn

[R69] 生成随机密码
来源：http://ag.jctech888.com.cn

head -c 16 /dev/urandom | base64
来源：http://jm.wgjwhj.cn

[R70] 时间戳与互转
来源：http://ah.panjiajie.cn

date +%s;  date -d @1700000000
来源：http://wa.9csxet.cn

[R71] 日期格式化
来源：http://nt.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jg.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://pc.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gy.nszjky.cn

[R73] 分割大日志
来源：http://ps.jctech888.com.cn

split -l 1000 big.log part_
来源：http://ds.hnjuh.cn

[R74] 批量重命名
来源：http://bl.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zu.haigaiapp.cn

[R75] 导出环境变量
来源：http://vh.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://qt.521024.cn

[R76] 使用临时文件
来源：http://kk.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gn.nicolike.cn

[R77] 读取用户输入
来源：http://pn.shxzskj.cn

read -rp "请输入: " ans
来源：http://wj.yuexingan06.cn

[R78] 交互式菜单
来源：http://hr.hahajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://da.wgjwhj.cn

[R79] 解析命令行选项
来源：http://ka.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cw.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://xd.bookmarksfly.cn

time ./run.sh
来源：http://sk.chemitech.net.cn

================================================================================
来源：http://oo.panjiajie.cn

S. C / C++ 专题
来源：http://qv.szxytkj.cn

================================================================================
来源：http://xv.lnxyls.cn

[S01] C：Hello World
来源：http://lw.colortex.cn

#include <stdio.h>
来源：http://ye.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mu.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://cw.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://ew.huixinmuqiang.cn

[S03] C：读入整数
来源：http://ld.hnjuh.cn

int x; scanf("%d", &x);
来源：http://xv.hahajie.cn

[S04] C：字符串复制
来源：http://do.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bo.szsharing.cn

[S05] C：字符串长度
来源：http://ge.newstarts.cn

strlen(s)
来源：http://br.shtwfgs.cn

[S06] C：字符串比较
来源：http://pu.newstarts.cn

strcmp(a, b) == 0
来源：http://oj.colortex.cn

[S07] C：数组遍历求和
来源：http://fw.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://on.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://bs.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ud.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://as.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yv.haigaiapp.cn

[S10] C：指针与解引用
来源：http://pq.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://bl.bjjhwx.cn

[S11] C：逐行读文件
来源：http://ci.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://jq.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yi.huixinmuqiang.cn

fclose(f);
来源：http://il.hnjuh.cn

[S12] C：写文件
来源：http://sq.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ir.9csxet.cn

[S13] C：宏定义
来源：http://gy.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yt.panjiajie.cn

[S14] C：枚举
来源：http://oe.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://yb.huixinmuqiang.cn

[S15] C：类型转换
来源：http://ml.bjjhwx.cn

(double) a / b
来源：http://zl.haigaiapp.cn

[S16] C：位操作置位
来源：http://qp.panjiajie.cn

x |= (1 << 3);
来源：http://kd.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://tg.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ap.521024.cn

[S18] C：命令行参数
来源：http://zb.hahajie.cn

int main(int argc, char **argv)
来源：http://eq.colortex.cn

[S19] C：快速排序
来源：http://lt.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oi.szxytkj.cn

[S20] C：二分查找
来源：http://gg.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xq.9csxet.cn

[S21] C：字符类别判断
来源：http://ci.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tv.hahajie.cn

[S22] C：字符串转数字
来源：http://gd.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dz.nicolike.cn

[S23] C：随机数
来源：http://lo.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ak.szxytkj.cn

[S24] C：获取本地时间
来源：http://hm.hahajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pv.muxihuayi.cn

[S25] C：内存拷贝
来源：http://rg.huanxung.cn

memcpy(dst, src, n);
来源：http://ny.newstarts.cn

[S26] C：内存清零
来源：http://tz.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://yt.hahajie.cn

[S27] C：定义常量
来源：http://fl.szsharing.cn

const double PI = 3.14159;
来源：http://tk.newstarts.cn

[S28] C：静态变量
来源：http://ac.shxzukj.cn

static int counter = 0;
来源：http://kv.asd995.cn

[S29] C：变参函数
来源：http://ym.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rm.lnxyls.cn

[S30] C：头文件保护
来源：http://om.haigaiapp.cn

#ifndef X_H
来源：http://fw.nszjky.cn

#define X_H
来源：http://fm.wgjwhj.cn

#endif
来源：http://aa.lnxyls.cn

[S31] C++：Hello World
来源：http://kf.521024.cn

#include <iostream>
来源：http://pz.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://dm.yuexingan06.cn

[S32] C++：字符串
来源：http://jf.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://is.huanxung.cn

[S33] C++：vector 增删
来源：http://dd.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qv.newstarts.cn

[S34] C++：遍历 vector
来源：http://vd.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://hs.hahajie.cn

[S35] C++：map
来源：http://cr.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kg.szxytkj.cn

[S36] C++：unordered_map
来源：http://fd.gzmigu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cg.yuexingan06.cn

[S37] C++：set
来源：http://vl.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fo.wgjwhj.cn

[S38] C++：排序
来源：http://ai.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://un.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://bi.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xb.shxzukj.cn

[S40] C++：查找元素
来源：http://ve.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rd.szsharing.cn

[S41] C++：类与构造函数
来源：http://gl.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vd.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://mz.nszjky.cn

class B : public Base { public: void f() override {} };
来源：http://ga.newstarts.cn

[S43] C++：智能指针
来源：http://lb.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://qi.szxytkj.cn

[S44] C++：引用传参
来源：http://xu.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://ne.jctech888.com.cn

[S45] C++：lambda
来源：http://bd.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sq.9csxet.cn

[S46] C++：函数模板
来源：http://wf.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cw.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://gb.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hg.9csxet.cn

[S48] C++：逐行读文件
来源：http://ug.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ir.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://id.yuexingan06.cn

[S49] C++：写文件
来源：http://gx.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nc.nicolike.cn

[S50] C++：格式化数字
来源：http://qr.huanxung.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pk.521024.cn

[S51] C++：显式类型转换
来源：http://vc.nszjky.cn

static_cast<double>(a) / b
来源：http://ar.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://vi.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://tf.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://pl.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://um.hnjuh.cn

[S54] C++：异常处理
来源：http://bd.chemitech.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tb.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://pp.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zs.521024.cn

[S56] C++：optional
来源：http://cf.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ka.newstarts.cn

[S57] C++：编译期常量
来源：http://ls.szxytkj.cn

constexpr int N = 10;
来源：http://ii.szxytkj.cn

[S58] C++：命名空间
来源：http://wg.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://nw.colortex.cn

[S59] C++：静态断言
来源：http://xn.nszjky.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nv.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://ba.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://od.521024.cn

================================================================================
来源：http://ap.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xk.huixiangedu.cn

================================================================================
来源：http://zl.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://ig.chemitech.net.cn

println("Hello")
来源：http://fi.shtwfgs.cn

[T02] Kotlin：变量
来源：http://xf.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://io.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://db.muxihuayi.cn

"值: $b"
来源：http://cj.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://em.shxzukj.cn

val n: String? = null;  n?.length
来源：http://dl.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://yf.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oa.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://lh.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lw.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://aw.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ay.huanxung.cn

[T08] Kotlin：数据类
来源：http://cf.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://bl.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://mn.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://bf.asd995.cn

[T10] Kotlin：默认参数
来源：http://zv.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://um.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://dk.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qh.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://xt.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://dv.colortex.cn

[T13] Kotlin：只读 Map
来源：http://os.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://cg.shtwfgs.cn

[T14] Kotlin：循环
来源：http://kc.colortex.cn

for (i in 1..10) println(i)
来源：http://gr.nszjky.cn

[T15] Kotlin：接口
来源：http://nr.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://dd.bjjhwx.cn

[T16] Swift：Hello World
来源：http://sy.nszjky.cn

print("Hello")
来源：http://ci.asd995.cn

[T17] Swift：变量与常量
来源：http://yg.lnxyls.cn

var a = 1;  let b = 2
来源：http://dy.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://dh.shxzukj.cn

"值: \(b)"
来源：http://sd.9csxet.cn

[T19] Swift：可选绑定
来源：http://ri.hahajie.cn

if let n = opt { print(n) }
来源：http://rk.huixiangedu.cn

[T20] Swift：数组操作
来源：http://by.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fr.chemitech.net.cn

[T21] Swift：遍历
来源：http://jy.muxihuayi.cn

for x in a { print(x) }
来源：http://xf.bjjhwx.cn

[T22] Swift：字典
来源：http://hk.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ot.shxzukj.cn

[T23] Swift：函数
来源：http://vm.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://aq.hahajie.cn

[T24] Swift：闭包
来源：http://os.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ue.muxihuayi.cn

[T25] Swift：结构体
来源：http://ha.hahajie.cn

struct P { var x: Int }
来源：http://uw.bjjhwx.cn

[T26] Swift：类与重写
来源：http://kg.szxytkj.cn

class A: Base { override func f() {} }
来源：http://wz.muxihuayi.cn

[T27] Swift：错误处理
来源：http://ro.muxihuayi.cn

do { try f() } catch { print(error) }
来源：http://ay.gzmigu.cn

[T28] Swift：枚举
来源：http://pl.colortex.cn

enum Color { case red, green }
来源：http://iz.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://bk.jctech888.com.cn

guard let x = opt else { return }
来源：http://ms.jctech888.com.cn

[T30] Swift：协议
来源：http://uc.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://xm.szxytkj.cn

[T31] Lua：Hello World
来源：http://ga.yuntaijiaju.cn

print("Hello")
来源：http://bm.panjiajie.cn

[T32] Lua：局部变量
来源：http://kc.yuntaijiaju.cn

local a = 1
来源：http://ht.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://tc.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wt.hnjuh.cn

[T34] Lua：遍历表
来源：http://ri.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pf.yuexingan06.cn

[T35] Lua：字典表
来源：http://az.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://po.hnjuh.cn

[T36] Lua：函数
来源：http://kw.yuexingan06.cn

function add(a, b) return a + b end
来源：http://mu.nszjky.cn

[T37] Lua：字符串拼接
来源：http://hh.shtwfgs.cn

"a" .. "b"
来源：http://cl.nicolike.cn

[T38] Lua：条件
来源：http://hr.wgjwhj.cn

if x > 0 then print("正") end
来源：http://it.szsharing.cn

[T39] Lua：模式匹配
来源：http://mr.colortex.cn

string.find(s, "%d+")
来源：http://vy.nicolike.cn

[T40] Lua：元表
来源：http://pz.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://mj.chemitech.net.cn

[T41] Perl：Hello World
来源：http://gb.colortex.cn

print "Hello\n";
来源：http://uf.chemitech.net.cn

[T42] Perl：变量类型
来源：http://eq.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://og.shxzukj.cn

[T43] Perl：字符串插值
来源：http://js.shxzskj.cn

"值: $a"
来源：http://zl.muxihuayi.cn

[T44] Perl：条件
来源：http://nf.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://sm.521024.cn

[T45] Perl：数组遍历
来源：http://gv.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://uf.wgjwhj.cn

[T46] Perl：哈希操作
来源：http://gv.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dh.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://ol.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gu.lnxyls.cn

[T48] Perl：正则替换
来源：http://vq.9csxet.cn

$s =~ s/old/new/g;
来源：http://pu.hahajie.cn

[T49] Perl：函数
来源：http://lu.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fs.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://xh.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fg.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://ac.gzmigu.cn

[T51] Scala：Hello World
来源：http://ot.gzmigu.cn

println("Hello")
来源：http://ou.gzmigu.cn

[T52] Scala：变量
来源：http://rj.huixiangedu.cn

val a = 1;  var b = 2
来源：http://ik.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://gc.nszjky.cn

s"值: $b"
来源：http://on.newstarts.cn

[T54] Scala：集合映射
来源：http://as.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://lz.asd995.cn

[T55] Scala：集合过滤
来源：http://ps.huixiangedu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fm.nszjky.cn

[T56] Scala：样例类
来源：http://lv.gzmigu.cn

case class User(name: String, age: Int)
来源：http://mu.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://gl.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ux.szxytkj.cn

[T58] Scala：函数定义
来源：http://zg.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wf.huixinmuqiang.cn

[T59] Scala：循环
来源：http://yj.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://yl.yuexingan06.cn

[T60] Scala：折叠
来源：http://ut.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://it.jctech888.com.cn

================================================================================
来源：http://cx.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vt.haigaiapp.cn

================================================================================
来源：http://cl.haigaiapp.cn

[U01] Py：创建虚拟环境
来源：http://yo.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://db.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://wx.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cm.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://um.yuntaijiaju.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ec.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://dg.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cd.shxzukj.cn


<!-- 参考信息 -->