代发 wailian999

df -h;  du -sh *
来源：http://td.shxzukj.cn

[R62] 找最占空间的文件
来源：http://mr.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://qa.huixiangedu.cn

[R63] 内存与进程
来源：http://sx.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://bi.nszjky.cn

[R64] 结束进程
来源：http://fe.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://ct.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://ip.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://te.gzmigu.cn

[R66] 定时任务
来源：http://ar.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://ze.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://tt.chemitech.net.cn

openssl rand -hex 16
来源：http://hs.9csxet.cn

[R68] 计算文件校验值
来源：http://ks.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mf.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://ou.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://ys.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://dz.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://pv.szxytkj.cn

[R71] 日期格式化
来源：http://fq.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vv.yuexingan06.cn

[R72] 等待端口就绪
来源：http://xa.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rg.yuexingan06.cn

[R73] 分割大日志
来源：http://ak.muxihuayi.cn

split -l 1000 big.log part_
来源：http://qk.jianghongdianzi.cn

[R74] 批量重命名
来源：http://hl.9csxet.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uh.9csxet.cn

[R75] 导出环境变量
来源：http://md.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://py.bjjhwx.cn

[R76] 使用临时文件
来源：http://wp.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vi.shtwfgs.cn

[R77] 读取用户输入
来源：http://jn.szxytkj.cn

read -rp "请输入: " ans
来源：http://df.szxytkj.cn

[R78] 交互式菜单
来源：http://xp.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vh.chemitech.net.cn

[R79] 解析命令行选项
来源：http://cw.9csxet.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wk.asd995.cn

[R80] 查看脚本执行耗时
来源：http://nh.hnjuh.cn

time ./run.sh
来源：http://lx.nszjky.cn

================================================================================
来源：http://wk.shxzskj.cn

S. C / C++ 专题
来源：http://xb.muxihuayi.cn

================================================================================
来源：http://ig.shtwfgs.cn

[S01] C：Hello World
来源：http://tr.huixiangedu.cn

#include <stdio.h>
来源：http://ma.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fs.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://ub.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://js.gzmigu.cn

[S03] C：读入整数
来源：http://so.colortex.cn

int x; scanf("%d", &x);
来源：http://zx.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://wy.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tl.521024.cn

[S05] C：字符串长度
来源：http://tq.muxihuayi.cn

strlen(s)
来源：http://op.asd995.cn

[S06] C：字符串比较
来源：http://fs.huanxung.cn

strcmp(a, b) == 0
来源：http://vf.shxzukj.cn

[S07] C：数组遍历求和
来源：http://ki.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xh.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://gn.chemitech.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bh.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://tx.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ej.jctech888.com.cn

[S10] C：指针与解引用
来源：http://ei.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://zp.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://px.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://cb.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kg.haigaiapp.cn

fclose(f);
来源：http://oi.wgjwhj.cn

[S12] C：写文件
来源：http://ji.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uq.jctech888.com.cn

[S13] C：宏定义
来源：http://pa.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kz.panjiajie.cn

[S14] C：枚举
来源：http://fq.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://sp.hnjuh.cn

[S15] C：类型转换
来源：http://zd.colortex.cn

(double) a / b
来源：http://ga.colortex.cn

[S16] C：位操作置位
来源：http://ec.yuntaijiaju.cn

x |= (1 << 3);
来源：http://ie.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://fk.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cc.hnjuh.cn

[S18] C：命令行参数
来源：http://qf.nicolike.cn

int main(int argc, char **argv)
来源：http://dd.nszjky.cn

[S19] C：快速排序
来源：http://op.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://je.521024.cn

[S20] C：二分查找
来源：http://mn.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uk.hnjuh.cn

[S21] C：字符类别判断
来源：http://zm.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yt.521024.cn

[S22] C：字符串转数字
来源：http://se.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dp.shtwfgs.cn

[S23] C：随机数
来源：http://vg.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wn.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://ky.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kt.jctech888.com.cn

[S25] C：内存拷贝
来源：http://jv.panjiajie.cn

memcpy(dst, src, n);
来源：http://ve.9csxet.cn

[S26] C：内存清零
来源：http://fn.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://yh.huixiangedu.cn

[S27] C：定义常量
来源：http://bl.szsharing.cn

const double PI = 3.14159;
来源：http://co.521024.cn

[S28] C：静态变量
来源：http://js.wgjwhj.cn

static int counter = 0;
来源：http://cy.szsharing.cn

[S29] C：变参函数
来源：http://su.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iw.nicolike.cn

[S30] C：头文件保护
来源：http://qv.gzmigu.cn

#ifndef X_H
来源：http://ap.nicolike.cn

#define X_H
来源：http://gu.shxzukj.cn

#endif
来源：http://gh.lnxyls.cn

[S31] C++：Hello World
来源：http://oh.bjjhwx.cn

#include <iostream>
来源：http://em.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://ne.lnxyls.cn

[S32] C++：字符串
来源：http://jx.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://xd.chemitech.net.cn

[S33] C++：vector 增删
来源：http://fl.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zd.521024.cn

[S34] C++：遍历 vector
来源：http://xp.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://qa.huixinmuqiang.cn

[S35] C++：map
来源：http://jd.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wq.bjjhwx.cn

[S36] C++：unordered_map
来源：http://qu.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pn.bookmarksfly.cn

[S37] C++：set
来源：http://gf.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mq.szxytkj.cn

[S38] C++：排序
来源：http://tk.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://mv.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://nh.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kj.panjiajie.cn

[S40] C++：查找元素
来源：http://vg.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rz.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://jq.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mw.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://cd.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://ty.szxytkj.cn

[S43] C++：智能指针
来源：http://ew.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://jx.szxytkj.cn

[S44] C++：引用传参
来源：http://zc.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://dw.jianghongdianzi.cn

[S45] C++：lambda
来源：http://ll.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oq.muxihuayi.cn

[S46] C++：函数模板
来源：http://ln.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yu.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://up.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fe.shxzukj.cn

[S48] C++：逐行读文件
来源：http://kh.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sn.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://aj.huixiangedu.cn

[S49] C++：写文件
来源：http://xs.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jn.hnjuh.cn

[S50] C++：格式化数字
来源：http://vf.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dx.nicolike.cn

[S51] C++：显式类型转换
来源：http://pb.asd995.cn

static_cast<double>(a) / b
来源：http://vl.jianghongdianzi.cn

[S52] C++：const 与 noexcept
来源：http://bo.szsharing.cn

int size() const noexcept { return n_; }
来源：http://cp.colortex.cn

[S53] C++：移动语义
来源：http://dd.colortex.cn

std::vector<int> w = std::move(v);
来源：http://cx.szxytkj.cn

[S54] C++：异常处理
来源：http://hw.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dg.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://jg.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ai.shxzskj.cn

[S56] C++：optional
来源：http://wv.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cb.chemitech.net.cn

[S57] C++：编译期常量
来源：http://rx.bookmarksfly.cn

constexpr int N = 10;
来源：http://po.colortex.cn

[S58] C++：命名空间
来源：http://lq.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://ck.panjiajie.cn

[S59] C++：静态断言
来源：http://fw.shtwfgs.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hk.huixinmuqiang.cn

[S60] C++：遍历并删除元素
来源：http://yg.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eu.nicolike.cn

================================================================================
来源：http://nn.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vn.colortex.cn

================================================================================
来源：http://bi.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://mt.szsharing.cn

println("Hello")
来源：http://gc.jctech888.com.cn

[T02] Kotlin：变量
来源：http://za.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mc.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://jj.szsharing.cn

"值: $b"
来源：http://kq.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://yk.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://ez.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://hw.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lk.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://ek.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wj.panjiajie.cn

[T07] Kotlin：集合过滤
来源：http://vj.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lx.hnjuh.cn

[T08] Kotlin：数据类
来源：http://ib.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://sr.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://aj.colortex.cn

fun String.exclaim() = this + "!"
来源：http://qe.9csxet.cn

[T10] Kotlin：默认参数
来源：http://qb.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pn.panjiajie.cn

[T11] Kotlin：协程
来源：http://py.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ns.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://wx.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://bl.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://xf.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://fg.chemitech.net.cn

[T14] Kotlin：循环
来源：http://ap.panjiajie.cn

for (i in 1..10) println(i)
来源：http://sk.shtwfgs.cn

[T15] Kotlin：接口
来源：http://wy.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://iz.lnxyls.cn

[T16] Swift：Hello World
来源：http://fd.szsharing.cn

print("Hello")
来源：http://ko.shxzukj.cn

[T17] Swift：变量与常量
来源：http://uz.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://by.huanxung.cn

[T18] Swift：字符串插值
来源：http://vu.gzmigu.cn

"值: \(b)"
来源：http://nn.nicolike.cn

[T19] Swift：可选绑定
来源：http://qp.nicolike.cn

if let n = opt { print(n) }
来源：http://zc.shxzukj.cn

[T20] Swift：数组操作
来源：http://cw.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nf.lnxyls.cn

[T21] Swift：遍历
来源：http://tm.bjjhwx.cn

for x in a { print(x) }
来源：http://fm.nicolike.cn

[T22] Swift：字典
来源：http://cc.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qb.bjjhwx.cn

[T23] Swift：函数
来源：http://pk.wgjwhj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ge.panjiajie.cn

[T24] Swift：闭包
来源：http://kd.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ss.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://zu.hnjuh.cn

struct P { var x: Int }
来源：http://cn.huanxung.cn

[T26] Swift：类与重写
来源：http://lg.asd995.cn

class A: Base { override func f() {} }
来源：http://sl.huanxung.cn

[T27] Swift：错误处理
来源：http://fy.9csxet.cn

do { try f() } catch { print(error) }
来源：http://os.hnjuh.cn

[T28] Swift：枚举
来源：http://vc.haigaiapp.cn

enum Color { case red, green }
来源：http://no.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://pd.szsharing.cn

guard let x = opt else { return }
来源：http://tj.nszjky.cn

[T30] Swift：协议
来源：http://tq.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://oe.shtwfgs.cn

[T31] Lua：Hello World
来源：http://bh.haigaiapp.cn

print("Hello")
来源：http://mi.bjjhwx.cn

[T32] Lua：局部变量
来源：http://mk.shtwfgs.cn

local a = 1
来源：http://iu.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://vg.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zb.nicolike.cn

[T34] Lua：遍历表
来源：http://an.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pp.nszjky.cn

[T35] Lua：字典表
来源：http://bb.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://xh.521024.cn

[T36] Lua：函数
来源：http://xd.muxihuayi.cn

function add(a, b) return a + b end
来源：http://xz.huanxung.cn

[T37] Lua：字符串拼接
来源：http://ny.shxzukj.cn

"a" .. "b"
来源：http://as.panjiajie.cn

[T38] Lua：条件
来源：http://uw.shxzukj.cn

if x > 0 then print("正") end
来源：http://ki.shtwfgs.cn

[T39] Lua：模式匹配
来源：http://im.huixiangedu.cn

string.find(s, "%d+")
来源：http://gb.huanxung.cn

[T40] Lua：元表
来源：http://kj.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://ca.hahajie.cn

[T41] Perl：Hello World
来源：http://tn.hahajie.cn

print "Hello\n";
来源：http://gq.jctech888.com.cn

[T42] Perl：变量类型
来源：http://df.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://er.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://bq.hahajie.cn

"值: $a"
来源：http://ay.hnjuh.cn

[T44] Perl：条件
来源：http://jr.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://nx.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://cz.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://ys.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://vu.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fg.shxzukj.cn

[T47] Perl：正则捕获
来源：http://bn.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xu.shxzskj.cn

[T48] Perl：正则替换
来源：http://pa.shxzskj.cn

$s =~ s/old/new/g;
来源：http://ki.chemitech.net.cn

[T49] Perl：函数
来源：http://ua.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mq.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://zc.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qn.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://vu.szsharing.cn

[T51] Scala：Hello World
来源：http://hn.huixinmuqiang.cn

println("Hello")
来源：http://et.521024.cn

[T52] Scala：变量
来源：http://il.nszjky.cn

val a = 1;  var b = 2
来源：http://jp.hnjuh.cn

[T53] Scala：字符串插值
来源：http://oh.lnxyls.cn

s"值: $b"
来源：http://qu.jianghongdianzi.cn

[T54] Scala：集合映射
来源：http://ei.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://it.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://pi.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zk.chemitech.net.cn

[T56] Scala：样例类
来源：http://rj.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://kj.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://ta.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fy.jctech888.com.cn

[T58] Scala：函数定义
来源：http://wb.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bn.jctech888.com.cn

[T59] Scala：循环
来源：http://ld.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://fo.shtwfgs.cn

[T60] Scala：折叠
来源：http://pw.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yw.haigaiapp.cn

================================================================================
来源：http://oa.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://km.panjiajie.cn

================================================================================
来源：http://ei.panjiajie.cn

[U01] Py：创建虚拟环境
来源：http://nc.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://iz.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://hy.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fd.szsharing.cn


<!-- 参考信息 -->