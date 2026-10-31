代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zk.nszjky.cn

[R66] 定时任务
来源：http://gb.newstarts.cn

crontab -e;  crontab -l
来源：http://yc.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://qs.nicolike.cn

openssl rand -hex 16
来源：http://vu.wgjwhj.cn

[R68] 计算文件校验值
来源：http://sw.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ep.hahajie.cn

[R69] 生成随机密码
来源：http://vd.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://ii.chemitech.net.cn

[R70] 时间戳与互转
来源：http://ty.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://aw.muxihuayi.cn

[R71] 日期格式化
来源：http://ub.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sb.9csxet.cn

[R72] 等待端口就绪
来源：http://lf.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nd.yuntaijiaju.cn

[R73] 分割大日志
来源：http://dw.panjiajie.cn

split -l 1000 big.log part_
来源：http://zi.9csxet.cn

[R74] 批量重命名
来源：http://qq.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cg.yuexingan06.cn

[R75] 导出环境变量
来源：http://bb.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://bj.wgjwhj.cn

[R76] 使用临时文件
来源：http://gq.jianghongdianzi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tw.hnjuh.cn

[R77] 读取用户输入
来源：http://yv.bjjhwx.cn

read -rp "请输入: " ans
来源：http://ik.jctech888.com.cn

[R78] 交互式菜单
来源：http://yp.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zz.bjjhwx.cn

[R79] 解析命令行选项
来源：http://nl.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ca.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://rk.wgjwhj.cn

time ./run.sh
来源：http://pp.chemitech.net.cn

================================================================================
来源：http://rp.haigaiapp.cn

S. C / C++ 专题
来源：http://nz.yuexingan06.cn

================================================================================
来源：http://ql.huixiangedu.cn

[S01] C：Hello World
来源：http://hz.huixinmuqiang.cn

#include <stdio.h>
来源：http://vo.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dr.szsharing.cn

[S02] C：变量与格式化输出
来源：http://xq.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://ov.panjiajie.cn

[S03] C：读入整数
来源：http://uh.panjiajie.cn

int x; scanf("%d", &x);
来源：http://cr.panjiajie.cn

[S04] C：字符串复制
来源：http://mq.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wd.chemitech.net.cn

[S05] C：字符串长度
来源：http://zo.9csxet.cn

strlen(s)
来源：http://np.jctech888.com.cn

[S06] C：字符串比较
来源：http://vp.newstarts.cn

strcmp(a, b) == 0
来源：http://ax.huanxung.cn

[S07] C：数组遍历求和
来源：http://xg.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ae.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://ct.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ma.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://mq.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vn.hnjuh.cn

[S10] C：指针与解引用
来源：http://xx.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://mc.wgjwhj.cn

[S11] C：逐行读文件
来源：http://vx.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://mn.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://op.colortex.cn

fclose(f);
来源：http://ab.shxzskj.cn

[S12] C：写文件
来源：http://uc.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fe.huanxung.cn

[S13] C：宏定义
来源：http://dt.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yw.colortex.cn

[S14] C：枚举
来源：http://nq.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://cv.bjjhwx.cn

[S15] C：类型转换
来源：http://os.huixiangedu.cn

(double) a / b
来源：http://jf.panjiajie.cn

[S16] C：位操作置位
来源：http://po.huanxung.cn

x |= (1 << 3);
来源：http://hy.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://cl.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rr.asd995.cn

[S18] C：命令行参数
来源：http://rr.521024.cn

int main(int argc, char **argv)
来源：http://ff.hnjuh.cn

[S19] C：快速排序
来源：http://so.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ud.jianghongdianzi.cn

[S20] C：二分查找
来源：http://tm.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kd.gzmigu.cn

[S21] C：字符类别判断
来源：http://nn.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sp.bjjhwx.cn

[S22] C：字符串转数字
来源：http://yv.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xw.huixiangedu.cn

[S23] C：随机数
来源：http://hy.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yf.hnjuh.cn

[S24] C：获取本地时间
来源：http://zj.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ad.gzmigu.cn

[S25] C：内存拷贝
来源：http://ej.szsharing.cn

memcpy(dst, src, n);
来源：http://mn.yuexingan06.cn

[S26] C：内存清零
来源：http://uk.asd995.cn

memset(a, 0, sizeof a);
来源：http://vr.lnxyls.cn

[S27] C：定义常量
来源：http://lf.szxytkj.cn

const double PI = 3.14159;
来源：http://yl.521024.cn

[S28] C：静态变量
来源：http://ul.bookmarksfly.cn

static int counter = 0;
来源：http://ve.muxihuayi.cn

[S29] C：变参函数
来源：http://bj.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lq.haigaiapp.cn

[S30] C：头文件保护
来源：http://ur.newstarts.cn

#ifndef X_H
来源：http://px.huixiangedu.cn

#define X_H
来源：http://wt.yuntaijiaju.cn

#endif
来源：http://sz.haigaiapp.cn

[S31] C++：Hello World
来源：http://sj.lnxyls.cn

#include <iostream>
来源：http://on.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://lj.wgjwhj.cn

[S32] C++：字符串
来源：http://wf.colortex.cn

std::string s = "hi";  s += "!";
来源：http://vh.huanxung.cn

[S33] C++：vector 增删
来源：http://ei.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sh.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://lg.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://xp.asd995.cn

[S35] C++：map
来源：http://em.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dg.521024.cn

[S36] C++：unordered_map
来源：http://ha.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yq.szsharing.cn

[S37] C++：set
来源：http://tx.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ly.hahajie.cn

[S38] C++：排序
来源：http://qi.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://ff.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://bg.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eh.gzmigu.cn

[S40] C++：查找元素
来源：http://gb.521024.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pz.asd995.cn

[S41] C++：类与构造函数
来源：http://ey.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oa.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://eg.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://rb.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://mm.521024.cn

auto p = std::make_unique<int>(5);
来源：http://gj.muxihuayi.cn

[S44] C++：引用传参
来源：http://ae.nicolike.cn

void inc(int &x) { ++x; }
来源：http://xp.gzmigu.cn

[S45] C++：lambda
来源：http://za.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cm.nicolike.cn

[S46] C++：函数模板
来源：http://fq.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hn.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://uc.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zs.hnjuh.cn

[S48] C++：逐行读文件
来源：http://rg.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ra.colortex.cn

while (std::getline(in, line)) { }
来源：http://hg.huixiangedu.cn

[S49] C++：写文件
来源：http://gm.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wv.muxihuayi.cn

[S50] C++：格式化数字
来源：http://ly.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fk.hahajie.cn

[S51] C++：显式类型转换
来源：http://ld.jctech888.com.cn

static_cast<double>(a) / b
来源：http://ag.521024.cn

[S52] C++：const 与 noexcept
来源：http://gz.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://qs.9csxet.cn

[S53] C++：移动语义
来源：http://vw.asd995.cn

std::vector<int> w = std::move(v);
来源：http://jh.shtwfgs.cn

[S54] C++：异常处理
来源：http://wo.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dg.521024.cn

[S55] C++：结构化绑定
来源：http://ud.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zg.szsharing.cn

[S56] C++：optional
来源：http://ku.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ty.521024.cn

[S57] C++：编译期常量
来源：http://lv.shxzskj.cn

constexpr int N = 10;
来源：http://cr.shxzukj.cn

[S58] C++：命名空间
来源：http://zs.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://pk.wgjwhj.cn

[S59] C++：静态断言
来源：http://dq.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kw.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://io.521024.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rz.gzmigu.cn

================================================================================
来源：http://uw.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qk.szxytkj.cn

================================================================================
来源：http://xq.nszjky.cn

[T01] Kotlin：Hello World
来源：http://er.szxytkj.cn

println("Hello")
来源：http://jp.shxzskj.cn

[T02] Kotlin：变量
来源：http://rc.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pd.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://of.shxzskj.cn

"值: $b"
来源：http://sy.bjjhwx.cn

[T04] Kotlin：空安全
来源：http://mm.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://ff.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://ze.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ec.nszjky.cn

[T06] Kotlin：集合映射
来源：http://ye.gzmigu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ab.nicolike.cn

[T07] Kotlin：集合过滤
来源：http://mu.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cf.panjiajie.cn

[T08] Kotlin：数据类
来源：http://jd.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://og.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://gz.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://tw.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://vo.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ds.hnjuh.cn

[T11] Kotlin：协程
来源：http://iq.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zk.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://fk.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://xi.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://ir.9csxet.cn

val m = mapOf("a" to 1)
来源：http://sq.hnjuh.cn

[T14] Kotlin：循环
来源：http://iw.yuntaijiaju.cn

for (i in 1..10) println(i)
来源：http://at.asd995.cn

[T15] Kotlin：接口
来源：http://gm.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://xk.muxihuayi.cn

[T16] Swift：Hello World
来源：http://ma.jianghongdianzi.cn

print("Hello")
来源：http://ka.colortex.cn

[T17] Swift：变量与常量
来源：http://pi.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://zj.gzmigu.cn

[T18] Swift：字符串插值
来源：http://cx.shxzukj.cn

"值: \(b)"
来源：http://on.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://hf.szxytkj.cn

if let n = opt { print(n) }
来源：http://kx.haigaiapp.cn

[T20] Swift：数组操作
来源：http://yt.colortex.cn

var a = [1, 2, 3];  a.append(4)
来源：http://un.nicolike.cn

[T21] Swift：遍历
来源：http://db.521024.cn

for x in a { print(x) }
来源：http://vs.bookmarksfly.cn

[T22] Swift：字典
来源：http://vp.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bb.colortex.cn

[T23] Swift：函数
来源：http://yc.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mq.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://hg.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vt.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://qf.hahajie.cn

struct P { var x: Int }
来源：http://xk.lnxyls.cn

[T26] Swift：类与重写
来源：http://fx.nicolike.cn

class A: Base { override func f() {} }
来源：http://ta.9csxet.cn

[T27] Swift：错误处理
来源：http://cm.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://th.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://cy.huixiangedu.cn

enum Color { case red, green }
来源：http://ii.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://fg.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://pq.panjiajie.cn

[T30] Swift：协议
来源：http://wj.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://dq.asd995.cn

[T31] Lua：Hello World
来源：http://bl.szsharing.cn

print("Hello")
来源：http://sk.bjjhwx.cn

[T32] Lua：局部变量
来源：http://gp.haigaiapp.cn

local a = 1
来源：http://ik.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://fx.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fz.shxzukj.cn

[T34] Lua：遍历表
来源：http://mw.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ci.shxzskj.cn

[T35] Lua：字典表
来源：http://ku.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://wr.jianghongdianzi.cn

[T36] Lua：函数
来源：http://ar.shxzukj.cn

function add(a, b) return a + b end
来源：http://xi.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://av.jctech888.com.cn

"a" .. "b"
来源：http://ao.hahajie.cn

[T38] Lua：条件
来源：http://os.chemitech.net.cn

if x > 0 then print("正") end
来源：http://uy.szxytkj.cn

[T39] Lua：模式匹配
来源：http://si.shxzukj.cn

string.find(s, "%d+")
来源：http://ui.gzmigu.cn

[T40] Lua：元表
来源：http://bq.szsharing.cn

setmetatable({}, { __index = base })
来源：http://tc.muxihuayi.cn

[T41] Perl：Hello World
来源：http://ky.yuntaijiaju.cn

print "Hello\n";
来源：http://gu.shxzskj.cn

[T42] Perl：变量类型
来源：http://ih.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cl.shxzskj.cn

[T43] Perl：字符串插值
来源：http://tv.jctech888.com.cn

"值: $a"
来源：http://aw.yuntaijiaju.cn

[T44] Perl：条件
来源：http://bb.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://vn.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://yi.521024.cn

for my $x (@arr) { print $x; }
来源：http://fl.hahajie.cn

[T46] Perl：哈希操作
来源：http://my.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uc.asd995.cn

[T47] Perl：正则捕获
来源：http://lk.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ko.lnxyls.cn

[T48] Perl：正则替换
来源：http://jt.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://bp.huixinmuqiang.cn

[T49] Perl：函数
来源：http://kx.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dg.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://uw.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ot.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://cx.lnxyls.cn

[T51] Scala：Hello World
来源：http://xv.nicolike.cn

println("Hello")
来源：http://yg.521024.cn

[T52] Scala：变量
来源：http://sh.newstarts.cn

val a = 1;  var b = 2
来源：http://qc.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://pu.yuntaijiaju.cn

s"值: $b"
来源：http://to.9csxet.cn

[T54] Scala：集合映射
来源：http://eo.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://qs.nicolike.cn

[T55] Scala：集合过滤
来源：http://be.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ro.szsharing.cn

[T56] Scala：样例类
来源：http://us.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://yd.szxytkj.cn

[T57] Scala：模式匹配
来源：http://fv.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rc.bjjhwx.cn

[T58] Scala：函数定义
来源：http://ze.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://re.chemitech.net.cn

[T59] Scala：循环
来源：http://je.521024.cn

for (i <- 1 to 10) println(i)
来源：http://jj.muxihuayi.cn

[T60] Scala：折叠
来源：http://dt.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fl.huixinmuqiang.cn

================================================================================
来源：http://iz.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ny.newstarts.cn

================================================================================
来源：http://ic.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://el.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tm.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://pe.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fr.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://yr.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fe.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://kt.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zh.asd995.cn

[U05] Py：列表去重且保序
来源：http://gk.9csxet.cn

list(dict.fromkeys(arr))
来源：http://aj.huixiangedu.cn

[U06] Py：合并两个字典
来源：http://ri.colortex.cn

{**a, **b}
来源：http://hj.jianghongdianzi.cn


<!-- 参考信息 -->