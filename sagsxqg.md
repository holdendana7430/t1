代发 wailian999

ssh user@host 'uptime'
来源：http://bn.muxihuayi.cn

[R58] 下载文件
来源：http://mo.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://of.jctech888.com.cn

[R59] 发 POST JSON
来源：http://ra.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://va.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://mb.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ej.bookmarksfly.cn

[R61] 磁盘占用
来源：http://vf.szxytkj.cn

df -h;  du -sh *
来源：http://iq.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://bu.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://rj.shxzukj.cn

[R63] 内存与进程
来源：http://yh.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://vy.huanxung.cn

[R64] 结束进程
来源：http://rg.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://ic.shxzskj.cn

[R65] 查看端口占用
来源：http://aw.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ml.nszjky.cn

[R66] 定时任务
来源：http://eb.yuexingan06.cn

crontab -e;  crontab -l
来源：http://dp.szsharing.cn

[R67] 生成随机十六进制串
来源：http://zj.huixinmuqiang.cn

openssl rand -hex 16
来源：http://xq.yuntaijiaju.cn

[R68] 计算文件校验值
来源：http://pr.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://oe.nszjky.cn

[R69] 生成随机密码
来源：http://vr.hahajie.cn

head -c 16 /dev/urandom | base64
来源：http://qy.jianghongdianzi.cn

[R70] 时间戳与互转
来源：http://qu.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://eg.jctech888.com.cn

[R71] 日期格式化
来源：http://dh.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jf.shxzskj.cn

[R72] 等待端口就绪
来源：http://ll.jianghongdianzi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ie.panjiajie.cn

[R73] 分割大日志
来源：http://tg.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://od.muxihuayi.cn

[R74] 批量重命名
来源：http://ec.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vu.jctech888.com.cn

[R75] 导出环境变量
来源：http://um.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://jp.lnxyls.cn

[R76] 使用临时文件
来源：http://gc.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ce.chemitech.net.cn

[R77] 读取用户输入
来源：http://sw.yuexingan06.cn

read -rp "请输入: " ans
来源：http://qe.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://no.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zs.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://rx.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yi.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://bx.yuexingan06.cn

time ./run.sh
来源：http://yg.chemitech.net.cn

================================================================================
来源：http://kn.huixiangedu.cn

S. C / C++ 专题
来源：http://wf.szsharing.cn

================================================================================
来源：http://ua.huixinmuqiang.cn

[S01] C：Hello World
来源：http://oj.muxihuayi.cn

#include <stdio.h>
来源：http://ok.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yh.nicolike.cn

[S02] C：变量与格式化输出
来源：http://xa.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://es.newstarts.cn

[S03] C：读入整数
来源：http://wt.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://me.hnjuh.cn

[S04] C：字符串复制
来源：http://pw.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fl.bjjhwx.cn

[S05] C：字符串长度
来源：http://mk.szsharing.cn

strlen(s)
来源：http://ld.huixiangedu.cn

[S06] C：字符串比较
来源：http://ks.hahajie.cn

strcmp(a, b) == 0
来源：http://xk.lnxyls.cn

[S07] C：数组遍历求和
来源：http://hx.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ks.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://bf.chemitech.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ya.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://gv.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://li.muxihuayi.cn

[S10] C：指针与解引用
来源：http://hs.nicolike.cn

int *p = &a;  *p = 5;
来源：http://kf.jctech888.com.cn

[S11] C：逐行读文件
来源：http://db.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://gc.nicolike.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lu.nszjky.cn

fclose(f);
来源：http://fi.asd995.cn

[S12] C：写文件
来源：http://in.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rj.jianghongdianzi.cn

[S13] C：宏定义
来源：http://ga.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cx.wgjwhj.cn

[S14] C：枚举
来源：http://ii.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://ip.521024.cn

[S15] C：类型转换
来源：http://vu.bookmarksfly.cn

(double) a / b
来源：http://hw.nicolike.cn

[S16] C：位操作置位
来源：http://qs.shxzukj.cn

x |= (1 << 3);
来源：http://jg.hahajie.cn

[S17] C：安全拼接字符串
来源：http://ym.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vj.szxytkj.cn

[S18] C：命令行参数
来源：http://dz.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://ui.hahajie.cn

[S19] C：快速排序
来源：http://ui.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jc.9csxet.cn

[S20] C：二分查找
来源：http://gk.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://il.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://jj.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qs.colortex.cn

[S22] C：字符串转数字
来源：http://kd.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uj.newstarts.cn

[S23] C：随机数
来源：http://zt.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oq.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://jx.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://df.hahajie.cn

[S25] C：内存拷贝
来源：http://kw.chemitech.net.cn

memcpy(dst, src, n);
来源：http://hp.nszjky.cn

[S26] C：内存清零
来源：http://id.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://fe.panjiajie.cn

[S27] C：定义常量
来源：http://ni.shxzskj.cn

const double PI = 3.14159;
来源：http://yt.shtwfgs.cn

[S28] C：静态变量
来源：http://sn.hnjuh.cn

static int counter = 0;
来源：http://rb.jctech888.com.cn

[S29] C：变参函数
来源：http://cr.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xf.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://st.nszjky.cn

#ifndef X_H
来源：http://wl.huixiangedu.cn

#define X_H
来源：http://jq.yuntaijiaju.cn

#endif
来源：http://dz.521024.cn

[S31] C++：Hello World
来源：http://kn.szxytkj.cn

#include <iostream>
来源：http://uu.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://vs.panjiajie.cn

[S32] C++：字符串
来源：http://wg.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://ae.shxzukj.cn

[S33] C++：vector 增删
来源：http://zc.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hj.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://ta.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://ui.bookmarksfly.cn

[S35] C++：map
来源：http://tf.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sv.jctech888.com.cn

[S36] C++：unordered_map
来源：http://ue.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dm.nicolike.cn

[S37] C++：set
来源：http://ld.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ii.nszjky.cn

[S38] C++：排序
来源：http://up.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://ys.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://xb.bjjhwx.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ct.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://nu.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lq.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://ws.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://au.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://au.521024.cn

class B : public Base { public: void f() override {} };
来源：http://sq.hnjuh.cn

[S43] C++：智能指针
来源：http://tt.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://wq.szxytkj.cn

[S44] C++：引用传参
来源：http://dc.szsharing.cn

void inc(int &x) { ++x; }
来源：http://ac.panjiajie.cn

[S45] C++：lambda
来源：http://od.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jd.muxihuayi.cn

[S46] C++：函数模板
来源：http://lz.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ik.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://pg.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hd.panjiajie.cn

[S48] C++：逐行读文件
来源：http://wh.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zq.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://ep.muxihuayi.cn

[S49] C++：写文件
来源：http://xl.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wv.hnjuh.cn

[S50] C++：格式化数字
来源：http://to.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xk.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://sx.nicolike.cn

static_cast<double>(a) / b
来源：http://ww.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://dj.colortex.cn

int size() const noexcept { return n_; }
来源：http://rs.huixiangedu.cn

[S53] C++：移动语义
来源：http://ok.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://vg.9csxet.cn

[S54] C++：异常处理
来源：http://xq.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://en.hahajie.cn

[S55] C++：结构化绑定
来源：http://zb.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kh.lnxyls.cn

[S56] C++：optional
来源：http://ki.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://al.asd995.cn

[S57] C++：编译期常量
来源：http://nf.huixiangedu.cn

constexpr int N = 10;
来源：http://qg.shxzukj.cn

[S58] C++：命名空间
来源：http://xi.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://lb.shtwfgs.cn

[S59] C++：静态断言
来源：http://qa.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cw.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://bt.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://un.shtwfgs.cn

================================================================================
来源：http://wx.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://if.huanxung.cn

================================================================================
来源：http://qu.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://yv.lnxyls.cn

println("Hello")
来源：http://ru.521024.cn

[T02] Kotlin：变量
来源：http://dl.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xu.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://ey.521024.cn

"值: $b"
来源：http://sy.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://rz.521024.cn

val n: String? = null;  n?.length
来源：http://eg.9csxet.cn

[T05] Kotlin：when 表达式
来源：http://eg.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ks.huanxung.cn

[T06] Kotlin：集合映射
来源：http://hl.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ey.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://tr.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://iu.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://em.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://xs.bjjhwx.cn

[T09] Kotlin：扩展函数
来源：http://nd.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://je.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://eu.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ik.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://nj.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vf.szsharing.cn

[T12] Kotlin：解构声明
来源：http://vw.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://sv.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://tn.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://mg.hahajie.cn

[T14] Kotlin：循环
来源：http://gy.shxzskj.cn

for (i in 1..10) println(i)
来源：http://wg.yuexingan06.cn

[T15] Kotlin：接口
来源：http://kw.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://wg.colortex.cn

[T16] Swift：Hello World
来源：http://uz.panjiajie.cn

print("Hello")
来源：http://wn.hahajie.cn

[T17] Swift：变量与常量
来源：http://dh.shxzskj.cn

var a = 1;  let b = 2
来源：http://vu.panjiajie.cn

[T18] Swift：字符串插值
来源：http://sy.gzmigu.cn

"值: \(b)"
来源：http://ax.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://dt.asd995.cn

if let n = opt { print(n) }
来源：http://od.chemitech.net.cn

[T20] Swift：数组操作
来源：http://xx.colortex.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oi.huanxung.cn

[T21] Swift：遍历
来源：http://rs.newstarts.cn

for x in a { print(x) }
来源：http://vn.yuexingan06.cn

[T22] Swift：字典
来源：http://yq.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qy.haigaiapp.cn

[T23] Swift：函数
来源：http://kz.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wn.shxzskj.cn

[T24] Swift：闭包
来源：http://ir.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bo.huixiangedu.cn

[T25] Swift：结构体
来源：http://zt.jianghongdianzi.cn

struct P { var x: Int }
来源：http://jf.gzmigu.cn

[T26] Swift：类与重写
来源：http://rj.huixiangedu.cn

class A: Base { override func f() {} }
来源：http://qr.9csxet.cn

[T27] Swift：错误处理
来源：http://od.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://te.huixiangedu.cn

[T28] Swift：枚举
来源：http://dn.lnxyls.cn

enum Color { case red, green }
来源：http://rx.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://dm.gzmigu.cn

guard let x = opt else { return }
来源：http://dc.9csxet.cn

[T30] Swift：协议
来源：http://fp.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://tc.asd995.cn

[T31] Lua：Hello World
来源：http://dc.yuntaijiaju.cn

print("Hello")
来源：http://uo.nszjky.cn

[T32] Lua：局部变量
来源：http://ga.colortex.cn

local a = 1
来源：http://ji.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://dp.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vb.521024.cn

[T34] Lua：遍历表
来源：http://lr.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ff.szsharing.cn

[T35] Lua：字典表
来源：http://zy.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://rx.huanxung.cn

[T36] Lua：函数
来源：http://xs.szsharing.cn

function add(a, b) return a + b end
来源：http://aj.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://bn.newstarts.cn

"a" .. "b"
来源：http://lz.szxytkj.cn

[T38] Lua：条件
来源：http://ng.shxzskj.cn

if x > 0 then print("正") end
来源：http://pq.hnjuh.cn

[T39] Lua：模式匹配
来源：http://yp.shtwfgs.cn

string.find(s, "%d+")
来源：http://ea.jctech888.com.cn

[T40] Lua：元表
来源：http://mn.huixinmuqiang.cn

setmetatable({}, { __index = base })
来源：http://cr.521024.cn

[T41] Perl：Hello World
来源：http://mx.asd995.cn

print "Hello\n";
来源：http://vk.bjjhwx.cn

[T42] Perl：变量类型
来源：http://sl.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bd.nicolike.cn

[T43] Perl：字符串插值
来源：http://vz.shtwfgs.cn

"值: $a"
来源：http://io.lnxyls.cn

[T44] Perl：条件
来源：http://bz.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://on.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://qp.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://cv.huanxung.cn

[T46] Perl：哈希操作
来源：http://vx.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://om.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://fz.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://aw.muxihuayi.cn

[T48] Perl：正则替换
来源：http://ak.9csxet.cn

$s =~ s/old/new/g;
来源：http://qr.yuntaijiaju.cn

[T49] Perl：函数
来源：http://dc.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ia.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://rf.shtwfgs.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ve.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://xl.colortex.cn

[T51] Scala：Hello World
来源：http://gq.jctech888.com.cn

println("Hello")
来源：http://vx.szxytkj.cn

[T52] Scala：变量
来源：http://zi.chemitech.net.cn

val a = 1;  var b = 2
来源：http://lf.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://gl.shxzskj.cn

s"值: $b"
来源：http://ok.asd995.cn

[T54] Scala：集合映射
来源：http://nc.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://dr.asd995.cn

[T55] Scala：集合过滤
来源：http://gx.chemitech.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hf.wgjwhj.cn

[T56] Scala：样例类
来源：http://gi.szxytkj.cn

case class User(name: String, age: Int)
来源：http://rs.asd995.cn

[T57] Scala：模式匹配
来源：http://ir.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://db.huixiangedu.cn

[T58] Scala：函数定义
来源：http://lz.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xp.szsharing.cn

[T59] Scala：循环
来源：http://ph.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://zv.hahajie.cn

[T60] Scala：折叠
来源：http://ng.9csxet.cn


<!-- 参考信息 -->