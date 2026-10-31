代发 wailian999

ssh user@host 'uptime'
来源：http://bn.chemitech.net.cn

[R58] 下载文件
来源：http://ne.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qb.shtwfgs.cn

[R59] 发 POST JSON
来源：http://dt.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jx.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://uq.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ij.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://hp.521024.cn

df -h;  du -sh *
来源：http://ux.shxzukj.cn

[R62] 找最占空间的文件
来源：http://rl.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://iz.haigaiapp.cn

[R63] 内存与进程
来源：http://zw.wgjwhj.cn

free -h;  ps aux | grep nginx
来源：http://er.huixiangedu.cn

[R64] 结束进程
来源：http://qa.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://xn.szxytkj.cn

[R65] 查看端口占用
来源：http://fe.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ou.huixiangedu.cn

[R66] 定时任务
来源：http://xl.nszjky.cn

crontab -e;  crontab -l
来源：http://mm.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://iz.jianghongdianzi.cn

openssl rand -hex 16
来源：http://wc.jctech888.com.cn

[R68] 计算文件校验值
来源：http://ce.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ft.colortex.cn

[R69] 生成随机密码
来源：http://cf.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://yr.newstarts.cn

[R70] 时间戳与互转
来源：http://js.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://ye.shxzukj.cn

[R71] 日期格式化
来源：http://gb.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zs.colortex.cn

[R72] 等待端口就绪
来源：http://bs.huixinmuqiang.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wf.asd995.cn

[R73] 分割大日志
来源：http://wt.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://ii.szsharing.cn

[R74] 批量重命名
来源：http://cb.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lx.nszjky.cn

[R75] 导出环境变量
来源：http://lf.szsharing.cn

export PATH="$HOME/bin:$PATH"
来源：http://br.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://hx.shxzukj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jk.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://ph.panjiajie.cn

read -rp "请输入: " ans
来源：http://eq.chemitech.net.cn

[R78] 交互式菜单
来源：http://om.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gz.bookmarksfly.cn

[R79] 解析命令行选项
来源：http://sc.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iy.wgjwhj.cn

[R80] 查看脚本执行耗时
来源：http://vs.huixiangedu.cn

time ./run.sh
来源：http://pc.chemitech.net.cn

================================================================================
来源：http://af.szsharing.cn

S. C / C++ 专题
来源：http://mt.shtwfgs.cn

================================================================================
来源：http://te.yuexingan06.cn

[S01] C：Hello World
来源：http://es.panjiajie.cn

#include <stdio.h>
来源：http://sl.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rc.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://tq.wgjwhj.cn

int a = 10; printf("%d\n", a);
来源：http://ju.wgjwhj.cn

[S03] C：读入整数
来源：http://it.huanxung.cn

int x; scanf("%d", &x);
来源：http://vd.muxihuayi.cn

[S04] C：字符串复制
来源：http://sq.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qv.szsharing.cn

[S05] C：字符串长度
来源：http://qf.colortex.cn

strlen(s)
来源：http://pz.newstarts.cn

[S06] C：字符串比较
来源：http://kc.szsharing.cn

strcmp(a, b) == 0
来源：http://pg.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://eb.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sr.gzmigu.cn

[S08] C：动态内存分配与释放
来源：http://im.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gc.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://tv.lnxyls.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tt.yuexingan06.cn

[S10] C：指针与解引用
来源：http://km.shxzukj.cn

int *p = &a;  *p = 5;
来源：http://os.jctech888.com.cn

[S11] C：逐行读文件
来源：http://ae.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://uu.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mg.wgjwhj.cn

fclose(f);
来源：http://ff.hahajie.cn

[S12] C：写文件
来源：http://ff.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zv.nszjky.cn

[S13] C：宏定义
来源：http://qt.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oa.szsharing.cn

[S14] C：枚举
来源：http://wh.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://bb.haigaiapp.cn

[S15] C：类型转换
来源：http://ep.jctech888.com.cn

(double) a / b
来源：http://bp.shxzskj.cn

[S16] C：位操作置位
来源：http://pd.haigaiapp.cn

x |= (1 << 3);
来源：http://lf.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://sn.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kh.yuexingan06.cn

[S18] C：命令行参数
来源：http://dp.muxihuayi.cn

int main(int argc, char **argv)
来源：http://vg.shxzskj.cn

[S19] C：快速排序
来源：http://ma.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://we.bjjhwx.cn

[S20] C：二分查找
来源：http://tg.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hb.haigaiapp.cn

[S21] C：字符类别判断
来源：http://bg.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zq.yuexingan06.cn

[S22] C：字符串转数字
来源：http://dq.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qu.bookmarksfly.cn

[S23] C：随机数
来源：http://rz.bookmarksfly.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cz.huixiangedu.cn

[S24] C：获取本地时间
来源：http://mb.hahajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zi.newstarts.cn

[S25] C：内存拷贝
来源：http://pe.nicolike.cn

memcpy(dst, src, n);
来源：http://kr.szxytkj.cn

[S26] C：内存清零
来源：http://yb.newstarts.cn

memset(a, 0, sizeof a);
来源：http://xb.521024.cn

[S27] C：定义常量
来源：http://hi.gzmigu.cn

const double PI = 3.14159;
来源：http://af.521024.cn

[S28] C：静态变量
来源：http://sr.colortex.cn

static int counter = 0;
来源：http://zl.muxihuayi.cn

[S29] C：变参函数
来源：http://tl.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lf.lnxyls.cn

[S30] C：头文件保护
来源：http://ut.asd995.cn

#ifndef X_H
来源：http://js.muxihuayi.cn

#define X_H
来源：http://rz.nszjky.cn

#endif
来源：http://zm.szsharing.cn

[S31] C++：Hello World
来源：http://ll.colortex.cn

#include <iostream>
来源：http://aa.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://zg.bjjhwx.cn

[S32] C++：字符串
来源：http://nq.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://kf.szsharing.cn

[S33] C++：vector 增删
来源：http://mr.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://au.panjiajie.cn

[S34] C++：遍历 vector
来源：http://hk.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://vy.jctech888.com.cn

[S35] C++：map
来源：http://yg.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ac.asd995.cn

[S36] C++：unordered_map
来源：http://lv.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sm.9csxet.cn

[S37] C++：set
来源：http://ax.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wn.colortex.cn

[S38] C++：排序
来源：http://oh.521024.cn

std::sort(v.begin(), v.end());
来源：http://ln.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://oh.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ru.shxzukj.cn

[S40] C++：查找元素
来源：http://ab.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nc.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://km.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ox.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://cb.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://hj.bookmarksfly.cn

[S43] C++：智能指针
来源：http://jt.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://tg.hnjuh.cn

[S44] C++：引用传参
来源：http://gg.asd995.cn

void inc(int &x) { ++x; }
来源：http://fd.jianghongdianzi.cn

[S45] C++：lambda
来源：http://mb.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://av.nicolike.cn

[S46] C++：函数模板
来源：http://lp.jianghongdianzi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jq.hahajie.cn

[S47] C++：结构化绑定遍历
来源：http://bk.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dc.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://me.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ul.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://dz.szxytkj.cn

[S49] C++：写文件
来源：http://bb.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qv.colortex.cn

[S50] C++：格式化数字
来源：http://vf.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://we.nszjky.cn

[S51] C++：显式类型转换
来源：http://cx.muxihuayi.cn

static_cast<double>(a) / b
来源：http://pq.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://nd.lnxyls.cn

int size() const noexcept { return n_; }
来源：http://ea.gzmigu.cn

[S53] C++：移动语义
来源：http://hj.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://tw.shxzskj.cn

[S54] C++：异常处理
来源：http://wl.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yf.nicolike.cn

[S55] C++：结构化绑定
来源：http://ny.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rh.haigaiapp.cn

[S56] C++：optional
来源：http://an.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xt.bjjhwx.cn

[S57] C++：编译期常量
来源：http://mp.hahajie.cn

constexpr int N = 10;
来源：http://ah.chemitech.net.cn

[S58] C++：命名空间
来源：http://mz.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://fh.lnxyls.cn

[S59] C++：静态断言
来源：http://iy.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cb.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://jk.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pg.yuexingan06.cn

================================================================================
来源：http://rd.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ww.colortex.cn

================================================================================
来源：http://cd.szxytkj.cn

[T01] Kotlin：Hello World
来源：http://tb.panjiajie.cn

println("Hello")
来源：http://kb.huixiangedu.cn

[T02] Kotlin：变量
来源：http://id.gzmigu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sh.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://rv.jctech888.com.cn

"值: $b"
来源：http://wa.nicolike.cn

[T04] Kotlin：空安全
来源：http://ks.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://cj.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://vj.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mz.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://wd.shtwfgs.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sc.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://uo.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cm.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://ci.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://gk.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://pa.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://md.asd995.cn

[T10] Kotlin：默认参数
来源：http://tb.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uz.hahajie.cn

[T11] Kotlin：协程
来源：http://my.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nu.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://zk.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://bx.shxzskj.cn

[T13] Kotlin：只读 Map
来源：http://pw.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://te.yuexingan06.cn

[T14] Kotlin：循环
来源：http://yp.huanxung.cn

for (i in 1..10) println(i)
来源：http://dv.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://gg.bjjhwx.cn

interface Shape { fun area(): Double }
来源：http://ol.wgjwhj.cn

[T16] Swift：Hello World
来源：http://ej.newstarts.cn

print("Hello")
来源：http://hy.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://bc.colortex.cn

var a = 1;  let b = 2
来源：http://mn.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://rz.bookmarksfly.cn

"值: \(b)"
来源：http://nt.gzmigu.cn

[T19] Swift：可选绑定
来源：http://bu.colortex.cn

if let n = opt { print(n) }
来源：http://vj.panjiajie.cn

[T20] Swift：数组操作
来源：http://fq.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://iw.yuexingan06.cn

[T21] Swift：遍历
来源：http://gi.muxihuayi.cn

for x in a { print(x) }
来源：http://te.szxytkj.cn

[T22] Swift：字典
来源：http://ob.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vs.asd995.cn

[T23] Swift：函数
来源：http://cr.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tw.bjjhwx.cn

[T24] Swift：闭包
来源：http://dy.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mu.hahajie.cn

[T25] Swift：结构体
来源：http://nu.wgjwhj.cn

struct P { var x: Int }
来源：http://yr.shxzskj.cn

[T26] Swift：类与重写
来源：http://nv.hnjuh.cn

class A: Base { override func f() {} }
来源：http://wi.panjiajie.cn

[T27] Swift：错误处理
来源：http://ih.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://qp.muxihuayi.cn

[T28] Swift：枚举
来源：http://kq.jianghongdianzi.cn

enum Color { case red, green }
来源：http://uq.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://eh.9csxet.cn

guard let x = opt else { return }
来源：http://xl.szxytkj.cn

[T30] Swift：协议
来源：http://di.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://kn.haigaiapp.cn

[T31] Lua：Hello World
来源：http://ne.newstarts.cn

print("Hello")
来源：http://rb.newstarts.cn

[T32] Lua：局部变量
来源：http://ki.chemitech.net.cn

local a = 1
来源：http://vh.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://oa.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hq.newstarts.cn

[T34] Lua：遍历表
来源：http://vk.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bh.nicolike.cn

[T35] Lua：字典表
来源：http://al.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://ul.szsharing.cn

[T36] Lua：函数
来源：http://pm.shxzukj.cn

function add(a, b) return a + b end
来源：http://pv.9csxet.cn

[T37] Lua：字符串拼接
来源：http://zs.bjjhwx.cn

"a" .. "b"
来源：http://ps.shtwfgs.cn

[T38] Lua：条件
来源：http://au.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://kq.huanxung.cn

[T39] Lua：模式匹配
来源：http://im.szsharing.cn

string.find(s, "%d+")
来源：http://ms.huixiangedu.cn

[T40] Lua：元表
来源：http://eg.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://yt.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://hw.szxytkj.cn

print "Hello\n";
来源：http://fi.panjiajie.cn

[T42] Perl：变量类型
来源：http://cx.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qw.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://ss.huixiangedu.cn

"值: $a"
来源：http://ps.yuntaijiaju.cn

[T44] Perl：条件
来源：http://ev.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://bj.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://pf.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://zm.shxzskj.cn

[T46] Perl：哈希操作
来源：http://zp.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yl.newstarts.cn

[T47] Perl：正则捕获
来源：http://fz.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://me.chemitech.net.cn

[T48] Perl：正则替换
来源：http://eo.huanxung.cn

$s =~ s/old/new/g;
来源：http://rb.jctech888.com.cn

[T49] Perl：函数
来源：http://mv.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nr.shtwfgs.cn

[T50] Perl：逐行读文件
来源：http://yw.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ke.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://su.szxytkj.cn

[T51] Scala：Hello World
来源：http://vy.jctech888.com.cn

println("Hello")
来源：http://ns.haigaiapp.cn

[T52] Scala：变量
来源：http://hg.chemitech.net.cn

val a = 1;  var b = 2
来源：http://rk.521024.cn

[T53] Scala：字符串插值
来源：http://mv.yuntaijiaju.cn

s"值: $b"
来源：http://vh.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://eu.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ah.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://kl.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ji.colortex.cn

[T56] Scala：样例类
来源：http://iz.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://iv.gzmigu.cn

[T57] Scala：模式匹配
来源：http://pt.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dl.colortex.cn

[T58] Scala：函数定义
来源：http://ik.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ct.colortex.cn

[T59] Scala：循环
来源：http://qz.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://wy.colortex.cn

[T60] Scala：折叠
来源：http://nc.gzmigu.cn


<!-- 参考信息 -->