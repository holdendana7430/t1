代发 wailian999

df -h;  du -sh *
来源：http://uj.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://tk.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://kg.haigaiapp.cn

[R63] 内存与进程
来源：http://gv.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://er.hnjuh.cn

[R64] 结束进程
来源：http://un.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://qs.haigaiapp.cn

[R65] 查看端口占用
来源：http://tv.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qg.gzmigu.cn

[R66] 定时任务
来源：http://yx.bjjhwx.cn

crontab -e;  crontab -l
来源：http://zy.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://ur.bookmarksfly.cn

openssl rand -hex 16
来源：http://rw.chemitech.net.cn

[R68] 计算文件校验值
来源：http://rf.gzmigu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hg.9csxet.cn

[R69] 生成随机密码
来源：http://qb.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://fa.huanxung.cn

[R70] 时间戳与互转
来源：http://gu.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://pt.gzmigu.cn

[R71] 日期格式化
来源：http://bm.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rw.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://uc.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://by.huixinmuqiang.cn

[R73] 分割大日志
来源：http://no.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://zv.gzmigu.cn

[R74] 批量重命名
来源：http://ho.bookmarksfly.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ua.shxzukj.cn

[R75] 导出环境变量
来源：http://od.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://jw.panjiajie.cn

[R76] 使用临时文件
来源：http://ry.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xu.hnjuh.cn

[R77] 读取用户输入
来源：http://wh.newstarts.cn

read -rp "请输入: " ans
来源：http://rv.lnxyls.cn

[R78] 交互式菜单
来源：http://yf.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fs.asd995.cn

[R79] 解析命令行选项
来源：http://um.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lp.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://ds.yuntaijiaju.cn

time ./run.sh
来源：http://xc.nicolike.cn

================================================================================
来源：http://ke.shxzukj.cn

S. C / C++ 专题
来源：http://vk.jctech888.com.cn

================================================================================
来源：http://jz.gzmigu.cn

[S01] C：Hello World
来源：http://di.shxzskj.cn

#include <stdio.h>
来源：http://qw.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kz.9csxet.cn

[S02] C：变量与格式化输出
来源：http://lb.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://an.huanxung.cn

[S03] C：读入整数
来源：http://fb.gzmigu.cn

int x; scanf("%d", &x);
来源：http://bp.shtwfgs.cn

[S04] C：字符串复制
来源：http://jt.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://eh.newstarts.cn

[S05] C：字符串长度
来源：http://zt.wgjwhj.cn

strlen(s)
来源：http://mg.muxihuayi.cn

[S06] C：字符串比较
来源：http://kd.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://rn.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://rn.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sv.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://lr.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qk.521024.cn

[S09] C：结构体定义与初始化
来源：http://jy.lnxyls.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uh.gzmigu.cn

[S10] C：指针与解引用
来源：http://kf.szsharing.cn

int *p = &a;  *p = 5;
来源：http://nv.shxzskj.cn

[S11] C：逐行读文件
来源：http://ai.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://co.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sx.nszjky.cn

fclose(f);
来源：http://zu.chemitech.net.cn

[S12] C：写文件
来源：http://nl.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vr.gzmigu.cn

[S13] C：宏定义
来源：http://sb.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://as.huixiangedu.cn

[S14] C：枚举
来源：http://db.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://xi.gzmigu.cn

[S15] C：类型转换
来源：http://hq.jianghongdianzi.cn

(double) a / b
来源：http://ra.chemitech.net.cn

[S16] C：位操作置位
来源：http://mo.gzmigu.cn

x |= (1 << 3);
来源：http://np.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://at.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vp.bjjhwx.cn

[S18] C：命令行参数
来源：http://wn.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://jw.szxytkj.cn

[S19] C：快速排序
来源：http://pr.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ay.wgjwhj.cn

[S20] C：二分查找
来源：http://mg.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ni.chemitech.net.cn

[S21] C：字符类别判断
来源：http://pu.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bv.colortex.cn

[S22] C：字符串转数字
来源：http://li.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://up.szxytkj.cn

[S23] C：随机数
来源：http://my.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yo.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://fv.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vs.haigaiapp.cn

[S25] C：内存拷贝
来源：http://ex.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://zz.szsharing.cn

[S26] C：内存清零
来源：http://ur.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://xx.asd995.cn

[S27] C：定义常量
来源：http://bm.panjiajie.cn

const double PI = 3.14159;
来源：http://zb.wgjwhj.cn

[S28] C：静态变量
来源：http://dq.colortex.cn

static int counter = 0;
来源：http://wg.yuntaijiaju.cn

[S29] C：变参函数
来源：http://rx.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ac.wgjwhj.cn

[S30] C：头文件保护
来源：http://fh.huixinmuqiang.cn

#ifndef X_H
来源：http://dd.bookmarksfly.cn

#define X_H
来源：http://ap.jianghongdianzi.cn

#endif
来源：http://if.szsharing.cn

[S31] C++：Hello World
来源：http://ge.asd995.cn

#include <iostream>
来源：http://yl.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://pb.nszjky.cn

[S32] C++：字符串
来源：http://nr.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://wn.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://df.wgjwhj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ea.szxytkj.cn

[S34] C++：遍历 vector
来源：http://oy.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://ls.lnxyls.cn

[S35] C++：map
来源：http://ad.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lw.bjjhwx.cn

[S36] C++：unordered_map
来源：http://gh.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xu.szsharing.cn

[S37] C++：set
来源：http://qr.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://we.bjjhwx.cn

[S38] C++：排序
来源：http://gr.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://aa.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://al.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zv.newstarts.cn

[S40] C++：查找元素
来源：http://gt.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xl.huanxung.cn

[S41] C++：类与构造函数
来源：http://yb.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tp.newstarts.cn

[S42] C++：继承与虚函数
来源：http://nn.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://yz.gzmigu.cn

[S43] C++：智能指针
来源：http://qi.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://sn.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://gg.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://cn.muxihuayi.cn

[S45] C++：lambda
来源：http://mm.yuexingan06.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dr.nszjky.cn

[S46] C++：函数模板
来源：http://xt.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kq.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://mx.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rt.colortex.cn

[S48] C++：逐行读文件
来源：http://kh.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sf.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://pk.huixiangedu.cn

[S49] C++：写文件
来源：http://au.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ot.haigaiapp.cn

[S50] C++：格式化数字
来源：http://cf.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iw.nszjky.cn

[S51] C++：显式类型转换
来源：http://zi.huanxung.cn

static_cast<double>(a) / b
来源：http://tx.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://fv.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://za.chemitech.net.cn

[S53] C++：移动语义
来源：http://om.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://uk.shxzskj.cn

[S54] C++：异常处理
来源：http://qu.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cp.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://cz.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ja.9csxet.cn

[S56] C++：optional
来源：http://fg.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://co.szsharing.cn

[S57] C++：编译期常量
来源：http://da.szxytkj.cn

constexpr int N = 10;
来源：http://kd.521024.cn

[S58] C++：命名空间
来源：http://wg.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://vt.gzmigu.cn

[S59] C++：静态断言
来源：http://wa.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ap.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://rt.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sf.wgjwhj.cn

================================================================================
来源：http://qi.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ra.szxytkj.cn

================================================================================
来源：http://uv.521024.cn

[T01] Kotlin：Hello World
来源：http://sl.521024.cn

println("Hello")
来源：http://tg.lnxyls.cn

[T02] Kotlin：变量
来源：http://lh.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vo.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://bh.huixiangedu.cn

"值: $b"
来源：http://kv.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://zs.nicolike.cn

val n: String? = null;  n?.length
来源：http://lm.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://cc.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hl.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://so.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bx.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://js.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pi.gzmigu.cn

[T08] Kotlin：数据类
来源：http://eb.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://lg.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://cm.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://iy.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://jg.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wy.szxytkj.cn

[T11] Kotlin：协程
来源：http://qm.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fo.nszjky.cn

[T12] Kotlin：解构声明
来源：http://it.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://zd.521024.cn

[T13] Kotlin：只读 Map
来源：http://co.newstarts.cn

val m = mapOf("a" to 1)
来源：http://zj.asd995.cn

[T14] Kotlin：循环
来源：http://gt.shxzskj.cn

for (i in 1..10) println(i)
来源：http://ma.gzmigu.cn

[T15] Kotlin：接口
来源：http://qt.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://ai.huanxung.cn

[T16] Swift：Hello World
来源：http://vt.yuntaijiaju.cn

print("Hello")
来源：http://ty.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://aj.lnxyls.cn

var a = 1;  let b = 2
来源：http://wa.521024.cn

[T18] Swift：字符串插值
来源：http://xq.panjiajie.cn

"值: \(b)"
来源：http://sj.yuntaijiaju.cn

[T19] Swift：可选绑定
来源：http://ee.colortex.cn

if let n = opt { print(n) }
来源：http://cc.muxihuayi.cn

[T20] Swift：数组操作
来源：http://mk.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ax.bookmarksfly.cn

[T21] Swift：遍历
来源：http://vc.szsharing.cn

for x in a { print(x) }
来源：http://fo.jctech888.com.cn

[T22] Swift：字典
来源：http://vb.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dt.nicolike.cn

[T23] Swift：函数
来源：http://tx.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kh.bjjhwx.cn

[T24] Swift：闭包
来源：http://nv.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://po.panjiajie.cn

[T25] Swift：结构体
来源：http://iw.jctech888.com.cn

struct P { var x: Int }
来源：http://su.huixiangedu.cn

[T26] Swift：类与重写
来源：http://bl.shxzukj.cn

class A: Base { override func f() {} }
来源：http://lq.szxytkj.cn

[T27] Swift：错误处理
来源：http://rr.panjiajie.cn

do { try f() } catch { print(error) }
来源：http://gb.bookmarksfly.cn

[T28] Swift：枚举
来源：http://qt.chemitech.net.cn

enum Color { case red, green }
来源：http://ov.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://wm.szsharing.cn

guard let x = opt else { return }
来源：http://rz.shxzskj.cn

[T30] Swift：协议
来源：http://sq.gzmigu.cn

protocol Shape { func area() -> Double }
来源：http://mn.szsharing.cn

[T31] Lua：Hello World
来源：http://wg.huixiangedu.cn

print("Hello")
来源：http://sm.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://tj.colortex.cn

local a = 1
来源：http://ex.yuexingan06.cn

[T33] Lua：表（数组）
来源：http://vd.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gz.wgjwhj.cn

[T34] Lua：遍历表
来源：http://sd.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pu.panjiajie.cn

[T35] Lua：字典表
来源：http://mu.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://bi.newstarts.cn

[T36] Lua：函数
来源：http://xl.gzmigu.cn

function add(a, b) return a + b end
来源：http://cl.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://pi.haigaiapp.cn

"a" .. "b"
来源：http://wq.hahajie.cn

[T38] Lua：条件
来源：http://fm.colortex.cn

if x > 0 then print("正") end
来源：http://dt.asd995.cn

[T39] Lua：模式匹配
来源：http://nd.huanxung.cn

string.find(s, "%d+")
来源：http://re.lnxyls.cn

[T40] Lua：元表
来源：http://uv.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://ds.panjiajie.cn

[T41] Perl：Hello World
来源：http://qo.yuexingan06.cn

print "Hello\n";
来源：http://dj.lnxyls.cn

[T42] Perl：变量类型
来源：http://lq.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pt.nszjky.cn

[T43] Perl：字符串插值
来源：http://mp.9csxet.cn

"值: $a"
来源：http://cq.hnjuh.cn

[T44] Perl：条件
来源：http://vn.521024.cn

if ($a > 0) { print "正"; }
来源：http://th.panjiajie.cn

[T45] Perl：数组遍历
来源：http://hn.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://qd.gzmigu.cn

[T46] Perl：哈希操作
来源：http://ou.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lt.shxzukj.cn

[T47] Perl：正则捕获
来源：http://pa.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kn.bjjhwx.cn

[T48] Perl：正则替换
来源：http://ko.szxytkj.cn

$s =~ s/old/new/g;
来源：http://am.jctech888.com.cn

[T49] Perl：函数
来源：http://vm.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oq.nszjky.cn

[T50] Perl：逐行读文件
来源：http://zf.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://df.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://yk.nicolike.cn

[T51] Scala：Hello World
来源：http://gx.chemitech.net.cn

println("Hello")
来源：http://dx.jctech888.com.cn

[T52] Scala：变量
来源：http://ve.haigaiapp.cn

val a = 1;  var b = 2
来源：http://cb.shxzukj.cn

[T53] Scala：字符串插值
来源：http://kz.panjiajie.cn

s"值: $b"
来源：http://lb.shtwfgs.cn

[T54] Scala：集合映射
来源：http://wa.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://oe.lnxyls.cn

[T55] Scala：集合过滤
来源：http://mk.haigaiapp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ea.muxihuayi.cn

[T56] Scala：样例类
来源：http://nz.panjiajie.cn

case class User(name: String, age: Int)
来源：http://rw.9csxet.cn

[T57] Scala：模式匹配
来源：http://bu.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qu.szsharing.cn

[T58] Scala：函数定义
来源：http://qm.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wm.huixiangedu.cn

[T59] Scala：循环
来源：http://ni.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://vj.shtwfgs.cn

[T60] Scala：折叠
来源：http://vq.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rs.hahajie.cn

================================================================================
来源：http://yq.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pg.shxzskj.cn

================================================================================
来源：http://mj.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://cf.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gv.nszjky.cn

[U02] Py：导出 / 安装依赖
来源：http://ce.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://eu.shxzskj.cn


<!-- 参考信息 -->