代发 wailian999

free -h;  ps aux | grep nginx
来源：http://qd.yuexingan06.cn

[R64] 结束进程
来源：http://tg.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://wj.bookmarksfly.cn

[R65] 查看端口占用
来源：http://rz.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eo.huixiangedu.cn

[R66] 定时任务
来源：http://kk.huixiangedu.cn

crontab -e;  crontab -l
来源：http://pp.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://rq.yuntaijiaju.cn

openssl rand -hex 16
来源：http://ny.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://mi.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ko.yuexingan06.cn

[R69] 生成随机密码
来源：http://rp.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://hb.wgjwhj.cn

[R70] 时间戳与互转
来源：http://ar.szsharing.cn

date +%s;  date -d @1700000000
来源：http://xe.gzmigu.cn

[R71] 日期格式化
来源：http://li.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ei.shtwfgs.cn

[R72] 等待端口就绪
来源：http://wm.newstarts.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ia.nszjky.cn

[R73] 分割大日志
来源：http://nt.nicolike.cn

split -l 1000 big.log part_
来源：http://ce.panjiajie.cn

[R74] 批量重命名
来源：http://py.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://je.muxihuayi.cn

[R75] 导出环境变量
来源：http://kf.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://ww.shtwfgs.cn

[R76] 使用临时文件
来源：http://ev.hahajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yl.bookmarksfly.cn

[R77] 读取用户输入
来源：http://jp.haigaiapp.cn

read -rp "请输入: " ans
来源：http://be.panjiajie.cn

[R78] 交互式菜单
来源：http://iw.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fw.colortex.cn

[R79] 解析命令行选项
来源：http://jv.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bo.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://zh.lnxyls.cn

time ./run.sh
来源：http://yq.shtwfgs.cn

================================================================================
来源：http://vw.huixinmuqiang.cn

S. C / C++ 专题
来源：http://wh.gzmigu.cn

================================================================================
来源：http://bg.huixinmuqiang.cn

[S01] C：Hello World
来源：http://lm.hahajie.cn

#include <stdio.h>
来源：http://fd.521024.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jl.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://ql.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://mh.shxzukj.cn

[S03] C：读入整数
来源：http://ar.nicolike.cn

int x; scanf("%d", &x);
来源：http://cy.521024.cn

[S04] C：字符串复制
来源：http://jm.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gm.hahajie.cn

[S05] C：字符串长度
来源：http://bu.szxytkj.cn

strlen(s)
来源：http://cq.haigaiapp.cn

[S06] C：字符串比较
来源：http://to.nszjky.cn

strcmp(a, b) == 0
来源：http://so.asd995.cn

[S07] C：数组遍历求和
来源：http://bt.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zl.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://dh.jctech888.com.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lz.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://ni.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ef.haigaiapp.cn

[S10] C：指针与解引用
来源：http://qd.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://oc.yuexingan06.cn

[S11] C：逐行读文件
来源：http://hr.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://rg.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://om.shxzukj.cn

fclose(f);
来源：http://kr.huixiangedu.cn

[S12] C：写文件
来源：http://mb.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gr.szsharing.cn

[S13] C：宏定义
来源：http://zh.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sv.asd995.cn

[S14] C：枚举
来源：http://yv.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://kj.bookmarksfly.cn

[S15] C：类型转换
来源：http://bc.9csxet.cn

(double) a / b
来源：http://xm.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://dk.szxytkj.cn

x |= (1 << 3);
来源：http://tt.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://ba.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nf.haigaiapp.cn

[S18] C：命令行参数
来源：http://ma.asd995.cn

int main(int argc, char **argv)
来源：http://wi.jianghongdianzi.cn

[S19] C：快速排序
来源：http://yk.gzmigu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cb.jianghongdianzi.cn

[S20] C：二分查找
来源：http://jl.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bc.colortex.cn

[S21] C：字符类别判断
来源：http://mv.wgjwhj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xa.shtwfgs.cn

[S22] C：字符串转数字
来源：http://kt.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://je.shxzskj.cn

[S23] C：随机数
来源：http://pj.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wd.nicolike.cn

[S24] C：获取本地时间
来源：http://ak.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uh.asd995.cn

[S25] C：内存拷贝
来源：http://ke.panjiajie.cn

memcpy(dst, src, n);
来源：http://sf.chemitech.net.cn

[S26] C：内存清零
来源：http://so.9csxet.cn

memset(a, 0, sizeof a);
来源：http://hg.huanxung.cn

[S27] C：定义常量
来源：http://ms.huanxung.cn

const double PI = 3.14159;
来源：http://it.huixiangedu.cn

[S28] C：静态变量
来源：http://mh.hahajie.cn

static int counter = 0;
来源：http://xs.yuexingan06.cn

[S29] C：变参函数
来源：http://jk.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tb.lnxyls.cn

[S30] C：头文件保护
来源：http://nm.nszjky.cn

#ifndef X_H
来源：http://sn.bookmarksfly.cn

#define X_H
来源：http://wc.bookmarksfly.cn

#endif
来源：http://ad.jctech888.com.cn

[S31] C++：Hello World
来源：http://hd.hahajie.cn

#include <iostream>
来源：http://qz.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://ne.yuexingan06.cn

[S32] C++：字符串
来源：http://qt.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://hw.asd995.cn

[S33] C++：vector 增删
来源：http://pf.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wp.hnjuh.cn

[S34] C++：遍历 vector
来源：http://es.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://wa.nszjky.cn

[S35] C++：map
来源：http://tc.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qf.szsharing.cn

[S36] C++：unordered_map
来源：http://jp.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tv.nszjky.cn

[S37] C++：set
来源：http://iq.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nz.huixinmuqiang.cn

[S38] C++：排序
来源：http://gv.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://mr.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://ur.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kr.huixiangedu.cn

[S40] C++：查找元素
来源：http://nq.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kv.gzmigu.cn

[S41] C++：类与构造函数
来源：http://iz.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fp.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://hz.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://lt.shxzukj.cn

[S43] C++：智能指针
来源：http://cr.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://ri.szxytkj.cn

[S44] C++：引用传参
来源：http://yn.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://sw.nicolike.cn

[S45] C++：lambda
来源：http://ut.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tw.asd995.cn

[S46] C++：函数模板
来源：http://hd.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cv.hahajie.cn

[S47] C++：结构化绑定遍历
来源：http://kt.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qo.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://gq.shxzskj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qr.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://rq.lnxyls.cn

[S49] C++：写文件
来源：http://sl.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nd.panjiajie.cn

[S50] C++：格式化数字
来源：http://sz.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://in.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://gj.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://ed.asd995.cn

[S52] C++：const 与 noexcept
来源：http://sh.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://fb.shxzskj.cn

[S53] C++：移动语义
来源：http://xb.521024.cn

std::vector<int> w = std::move(v);
来源：http://tx.huixiangedu.cn

[S54] C++：异常处理
来源：http://dl.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dg.nicolike.cn

[S55] C++：结构化绑定
来源：http://oa.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ut.lnxyls.cn

[S56] C++：optional
来源：http://hg.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ay.panjiajie.cn

[S57] C++：编译期常量
来源：http://uu.asd995.cn

constexpr int N = 10;
来源：http://ji.muxihuayi.cn

[S58] C++：命名空间
来源：http://ov.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://bi.bookmarksfly.cn

[S59] C++：静态断言
来源：http://dg.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ke.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://xh.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dh.shtwfgs.cn

================================================================================
来源：http://st.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lz.nszjky.cn

================================================================================
来源：http://yp.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://te.hnjuh.cn

println("Hello")
来源：http://ja.asd995.cn

[T02] Kotlin：变量
来源：http://ep.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qd.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://qs.huanxung.cn

"值: $b"
来源：http://np.lnxyls.cn

[T04] Kotlin：空安全
来源：http://hl.panjiajie.cn

val n: String? = null;  n?.length
来源：http://nm.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://bu.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qi.asd995.cn

[T06] Kotlin：集合映射
来源：http://dg.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oj.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://ib.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xu.colortex.cn

[T08] Kotlin：数据类
来源：http://ey.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://pb.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://rw.hahajie.cn

fun String.exclaim() = this + "!"
来源：http://uv.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://ay.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qa.muxihuayi.cn

[T11] Kotlin：协程
来源：http://pf.bookmarksfly.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xj.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://ls.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://yg.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://zw.9csxet.cn

val m = mapOf("a" to 1)
来源：http://gw.shtwfgs.cn

[T14] Kotlin：循环
来源：http://ls.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://yj.gzmigu.cn

[T15] Kotlin：接口
来源：http://gx.nszjky.cn

interface Shape { fun area(): Double }
来源：http://gh.521024.cn

[T16] Swift：Hello World
来源：http://gt.bookmarksfly.cn

print("Hello")
来源：http://st.shxzskj.cn

[T17] Swift：变量与常量
来源：http://nv.gzmigu.cn

var a = 1;  let b = 2
来源：http://mq.huanxung.cn

[T18] Swift：字符串插值
来源：http://tn.huixinmuqiang.cn

"值: \(b)"
来源：http://mz.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://hh.nszjky.cn

if let n = opt { print(n) }
来源：http://du.shtwfgs.cn

[T20] Swift：数组操作
来源：http://am.wgjwhj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fo.shxzskj.cn

[T21] Swift：遍历
来源：http://qe.jctech888.com.cn

for x in a { print(x) }
来源：http://lr.newstarts.cn

[T22] Swift：字典
来源：http://so.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tw.colortex.cn

[T23] Swift：函数
来源：http://au.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dr.gzmigu.cn

[T24] Swift：闭包
来源：http://ck.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sh.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://lm.huixinmuqiang.cn

struct P { var x: Int }
来源：http://dq.521024.cn

[T26] Swift：类与重写
来源：http://td.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://kz.newstarts.cn

[T27] Swift：错误处理
来源：http://id.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://nd.chemitech.net.cn

[T28] Swift：枚举
来源：http://uc.wgjwhj.cn

enum Color { case red, green }
来源：http://sh.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://vu.shxzskj.cn

guard let x = opt else { return }
来源：http://rk.szxytkj.cn

[T30] Swift：协议
来源：http://oq.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://al.jctech888.com.cn

[T31] Lua：Hello World
来源：http://rs.huanxung.cn

print("Hello")
来源：http://wy.colortex.cn

[T32] Lua：局部变量
来源：http://ec.colortex.cn

local a = 1
来源：http://ov.newstarts.cn

[T33] Lua：表（数组）
来源：http://wb.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vg.hnjuh.cn

[T34] Lua：遍历表
来源：http://zx.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ms.shxzskj.cn

[T35] Lua：字典表
来源：http://fs.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://ot.huixiangedu.cn

[T36] Lua：函数
来源：http://oh.yuexingan06.cn

function add(a, b) return a + b end
来源：http://ri.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://ia.521024.cn

"a" .. "b"
来源：http://jp.bjjhwx.cn

[T38] Lua：条件
来源：http://tk.panjiajie.cn

if x > 0 then print("正") end
来源：http://av.nicolike.cn

[T39] Lua：模式匹配
来源：http://uy.asd995.cn

string.find(s, "%d+")
来源：http://zh.shtwfgs.cn

[T40] Lua：元表
来源：http://hv.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://rp.chemitech.net.cn

[T41] Perl：Hello World
来源：http://no.hahajie.cn

print "Hello\n";
来源：http://lw.nszjky.cn

[T42] Perl：变量类型
来源：http://fe.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ir.huanxung.cn

[T43] Perl：字符串插值
来源：http://hz.huixiangedu.cn

"值: $a"
来源：http://mp.asd995.cn

[T44] Perl：条件
来源：http://ln.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://us.nszjky.cn

[T45] Perl：数组遍历
来源：http://dq.asd995.cn

for my $x (@arr) { print $x; }
来源：http://se.nszjky.cn

[T46] Perl：哈希操作
来源：http://cf.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://az.asd995.cn

[T47] Perl：正则捕获
来源：http://dp.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dc.colortex.cn

[T48] Perl：正则替换
来源：http://oh.szsharing.cn

$s =~ s/old/new/g;
来源：http://la.hahajie.cn

[T49] Perl：函数
来源：http://uc.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qc.shtwfgs.cn

[T50] Perl：逐行读文件
来源：http://xt.huanxung.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nh.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://js.huanxung.cn

[T51] Scala：Hello World
来源：http://vp.newstarts.cn

println("Hello")
来源：http://nj.haigaiapp.cn

[T52] Scala：变量
来源：http://se.colortex.cn

val a = 1;  var b = 2
来源：http://cr.nicolike.cn

[T53] Scala：字符串插值
来源：http://ah.nicolike.cn

s"值: $b"
来源：http://an.yuexingan06.cn

[T54] Scala：集合映射
来源：http://fw.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://ln.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://pl.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wl.colortex.cn

[T56] Scala：样例类
来源：http://us.huixinmuqiang.cn

case class User(name: String, age: Int)
来源：http://va.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://gi.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gw.muxihuayi.cn

[T58] Scala：函数定义
来源：http://gi.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pd.shxzskj.cn

[T59] Scala：循环
来源：http://en.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://xt.haigaiapp.cn

[T60] Scala：折叠
来源：http://om.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sj.lnxyls.cn

================================================================================
来源：http://ej.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uv.gzmigu.cn

================================================================================
来源：http://na.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://cz.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ai.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://gz.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vq.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://si.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qg.lnxyls.cn

[U04] Py：变量调试打印
来源：http://zi.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bm.muxihuayi.cn


<!-- 参考信息 -->