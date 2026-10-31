代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cu.521024.cn

[R54] 比较两个文件
来源：http://vr.9csxet.cn

diff a.txt b.txt
来源：http://eg.9csxet.cn

[R55] 压缩与解压
来源：http://sg.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ap.lnxyls.cn

[R56] 远程拷贝
来源：http://fn.lnxyls.cn

scp file user@host:/path/
来源：http://bq.shtwfgs.cn

[R57] 远程执行命令
来源：http://ir.szxytkj.cn

ssh user@host 'uptime'
来源：http://uh.nszjky.cn

[R58] 下载文件
来源：http://jh.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://js.hahajie.cn

[R59] 发 POST JSON
来源：http://mi.szxytkj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nz.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://hj.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ij.panjiajie.cn

[R61] 磁盘占用
来源：http://yp.yuntaijiaju.cn

df -h;  du -sh *
来源：http://av.lnxyls.cn

[R62] 找最占空间的文件
来源：http://wt.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://ss.newstarts.cn

[R63] 内存与进程
来源：http://az.colortex.cn

free -h;  ps aux | grep nginx
来源：http://qk.huixinmuqiang.cn

[R64] 结束进程
来源：http://er.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://af.yuexingan06.cn

[R65] 查看端口占用
来源：http://ky.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://go.chemitech.net.cn

[R66] 定时任务
来源：http://ux.panjiajie.cn

crontab -e;  crontab -l
来源：http://sb.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://mc.jianghongdianzi.cn

openssl rand -hex 16
来源：http://oq.colortex.cn

[R68] 计算文件校验值
来源：http://qg.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://am.chemitech.net.cn

[R69] 生成随机密码
来源：http://ia.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://lm.colortex.cn

[R70] 时间戳与互转
来源：http://lw.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://by.hnjuh.cn

[R71] 日期格式化
来源：http://zn.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://if.nicolike.cn

[R72] 等待端口就绪
来源：http://fq.newstarts.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gk.asd995.cn

[R73] 分割大日志
来源：http://wt.wgjwhj.cn

split -l 1000 big.log part_
来源：http://uh.521024.cn

[R74] 批量重命名
来源：http://qv.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ze.bjjhwx.cn

[R75] 导出环境变量
来源：http://at.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://xg.jctech888.com.cn

[R76] 使用临时文件
来源：http://jp.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sr.yuexingan06.cn

[R77] 读取用户输入
来源：http://sy.huanxung.cn

read -rp "请输入: " ans
来源：http://rw.huixiangedu.cn

[R78] 交互式菜单
来源：http://xh.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://su.nicolike.cn

[R79] 解析命令行选项
来源：http://qr.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://go.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://xn.nicolike.cn

time ./run.sh
来源：http://rx.asd995.cn

================================================================================
来源：http://lz.shxzskj.cn

S. C / C++ 专题
来源：http://og.chemitech.net.cn

================================================================================
来源：http://er.huixiangedu.cn

[S01] C：Hello World
来源：http://sd.huanxung.cn

#include <stdio.h>
来源：http://nt.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ap.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://ld.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://lc.huixinmuqiang.cn

[S03] C：读入整数
来源：http://gq.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://le.hnjuh.cn

[S04] C：字符串复制
来源：http://sw.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jn.panjiajie.cn

[S05] C：字符串长度
来源：http://pt.wgjwhj.cn

strlen(s)
来源：http://eh.colortex.cn

[S06] C：字符串比较
来源：http://en.shxzskj.cn

strcmp(a, b) == 0
来源：http://jg.bookmarksfly.cn

[S07] C：数组遍历求和
来源：http://bp.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cd.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://dg.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ic.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://oe.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vr.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://la.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://fp.haigaiapp.cn

[S11] C：逐行读文件
来源：http://ne.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://tn.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qe.jianghongdianzi.cn

fclose(f);
来源：http://il.huixiangedu.cn

[S12] C：写文件
来源：http://vq.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ro.bjjhwx.cn

[S13] C：宏定义
来源：http://as.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kf.jianghongdianzi.cn

[S14] C：枚举
来源：http://hh.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://em.hahajie.cn

[S15] C：类型转换
来源：http://mo.nszjky.cn

(double) a / b
来源：http://vp.shtwfgs.cn

[S16] C：位操作置位
来源：http://nm.yuntaijiaju.cn

x |= (1 << 3);
来源：http://ci.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://kz.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dw.hahajie.cn

[S18] C：命令行参数
来源：http://lb.panjiajie.cn

int main(int argc, char **argv)
来源：http://np.shxzukj.cn

[S19] C：快速排序
来源：http://ht.gzmigu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vz.jctech888.com.cn

[S20] C：二分查找
来源：http://at.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ir.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://uy.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sv.nszjky.cn

[S22] C：字符串转数字
来源：http://qm.521024.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mo.huanxung.cn

[S23] C：随机数
来源：http://gb.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gt.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://pb.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://da.chemitech.net.cn

[S25] C：内存拷贝
来源：http://rd.huanxung.cn

memcpy(dst, src, n);
来源：http://tp.haigaiapp.cn

[S26] C：内存清零
来源：http://ko.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://jd.szxytkj.cn

[S27] C：定义常量
来源：http://yg.wgjwhj.cn

const double PI = 3.14159;
来源：http://xd.lnxyls.cn

[S28] C：静态变量
来源：http://cl.jianghongdianzi.cn

static int counter = 0;
来源：http://zs.nicolike.cn

[S29] C：变参函数
来源：http://ec.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vm.nszjky.cn

[S30] C：头文件保护
来源：http://ye.huanxung.cn

#ifndef X_H
来源：http://jt.huixinmuqiang.cn

#define X_H
来源：http://mn.szxytkj.cn

#endif
来源：http://qf.chemitech.net.cn

[S31] C++：Hello World
来源：http://gw.panjiajie.cn

#include <iostream>
来源：http://gd.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://fe.colortex.cn

[S32] C++：字符串
来源：http://ut.colortex.cn

std::string s = "hi";  s += "!";
来源：http://yt.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://uc.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oh.panjiajie.cn

[S34] C++：遍历 vector
来源：http://cx.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://zb.colortex.cn

[S35] C++：map
来源：http://kj.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hs.hnjuh.cn

[S36] C++：unordered_map
来源：http://ci.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dp.hahajie.cn

[S37] C++：set
来源：http://sl.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jt.shtwfgs.cn

[S38] C++：排序
来源：http://fn.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://rv.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://np.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://to.newstarts.cn

[S40] C++：查找元素
来源：http://lw.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fv.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://rn.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tg.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://lv.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://qg.jctech888.com.cn

[S43] C++：智能指针
来源：http://qz.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://ao.asd995.cn

[S44] C++：引用传参
来源：http://mo.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://ks.huanxung.cn

[S45] C++：lambda
来源：http://ao.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ib.bookmarksfly.cn

[S46] C++：函数模板
来源：http://hv.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qf.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://zs.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tb.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://jh.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nt.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://zg.bjjhwx.cn

[S49] C++：写文件
来源：http://yl.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tf.shxzskj.cn

[S50] C++：格式化数字
来源：http://af.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ge.szxytkj.cn

[S51] C++：显式类型转换
来源：http://fj.szxytkj.cn

static_cast<double>(a) / b
来源：http://gt.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://ak.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://ar.panjiajie.cn

[S53] C++：移动语义
来源：http://fo.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://yi.hahajie.cn

[S54] C++：异常处理
来源：http://sx.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wq.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://yw.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ql.shtwfgs.cn

[S56] C++：optional
来源：http://ws.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cp.szxytkj.cn

[S57] C++：编译期常量
来源：http://tu.nszjky.cn

constexpr int N = 10;
来源：http://jj.huixiangedu.cn

[S58] C++：命名空间
来源：http://wi.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://yn.szsharing.cn

[S59] C++：静态断言
来源：http://kc.nszjky.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wz.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://xz.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nk.shxzskj.cn

================================================================================
来源：http://ov.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rk.nicolike.cn

================================================================================
来源：http://dq.szsharing.cn

[T01] Kotlin：Hello World
来源：http://zh.shxzukj.cn

println("Hello")
来源：http://qd.colortex.cn

[T02] Kotlin：变量
来源：http://py.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zy.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://bc.panjiajie.cn

"值: $b"
来源：http://vi.nicolike.cn

[T04] Kotlin：空安全
来源：http://sm.szxytkj.cn

val n: String? = null;  n?.length
来源：http://sl.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://yy.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oi.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://hy.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://iy.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://my.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mb.nszjky.cn

[T08] Kotlin：数据类
来源：http://vz.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://xc.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://bs.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://vt.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://tw.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cq.asd995.cn

[T11] Kotlin：协程
来源：http://ol.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hx.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://yr.521024.cn

val (a, b) = Pair(1, 2)
来源：http://cw.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://fp.colortex.cn

val m = mapOf("a" to 1)
来源：http://gn.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://jx.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://mt.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://tg.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://fh.shtwfgs.cn

[T16] Swift：Hello World
来源：http://ui.yuexingan06.cn

print("Hello")
来源：http://hj.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://ss.colortex.cn

var a = 1;  let b = 2
来源：http://is.bookmarksfly.cn

[T18] Swift：字符串插值
来源：http://lu.haigaiapp.cn

"值: \(b)"
来源：http://nz.colortex.cn

[T19] Swift：可选绑定
来源：http://ie.521024.cn

if let n = opt { print(n) }
来源：http://ki.hnjuh.cn

[T20] Swift：数组操作
来源：http://xo.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rm.asd995.cn

[T21] Swift：遍历
来源：http://oj.shxzukj.cn

for x in a { print(x) }
来源：http://qz.521024.cn

[T22] Swift：字典
来源：http://lq.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vq.9csxet.cn

[T23] Swift：函数
来源：http://rq.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ql.yuexingan06.cn

[T24] Swift：闭包
来源：http://ox.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://du.9csxet.cn

[T25] Swift：结构体
来源：http://te.huanxung.cn

struct P { var x: Int }
来源：http://nm.huixinmuqiang.cn

[T26] Swift：类与重写
来源：http://bq.szsharing.cn

class A: Base { override func f() {} }
来源：http://wi.gzmigu.cn

[T27] Swift：错误处理
来源：http://lu.szxytkj.cn

do { try f() } catch { print(error) }
来源：http://dk.wgjwhj.cn

[T28] Swift：枚举
来源：http://br.shxzskj.cn

enum Color { case red, green }
来源：http://iv.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://nl.haigaiapp.cn

guard let x = opt else { return }
来源：http://gt.haigaiapp.cn

[T30] Swift：协议
来源：http://lx.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://tl.hnjuh.cn

[T31] Lua：Hello World
来源：http://nt.bjjhwx.cn

print("Hello")
来源：http://xr.huixiangedu.cn

[T32] Lua：局部变量
来源：http://lc.muxihuayi.cn

local a = 1
来源：http://pe.szxytkj.cn

[T33] Lua：表（数组）
来源：http://rb.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ba.shtwfgs.cn

[T34] Lua：遍历表
来源：http://ka.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ba.lnxyls.cn

[T35] Lua：字典表
来源：http://wd.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://mz.521024.cn

[T36] Lua：函数
来源：http://mv.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://bb.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://ce.panjiajie.cn

"a" .. "b"
来源：http://dh.jianghongdianzi.cn

[T38] Lua：条件
来源：http://zw.huixiangedu.cn

if x > 0 then print("正") end
来源：http://oo.szsharing.cn

[T39] Lua：模式匹配
来源：http://ol.shxzskj.cn

string.find(s, "%d+")
来源：http://bd.asd995.cn

[T40] Lua：元表
来源：http://cd.newstarts.cn

setmetatable({}, { __index = base })
来源：http://zt.gzmigu.cn

[T41] Perl：Hello World
来源：http://fe.shxzukj.cn

print "Hello\n";
来源：http://dz.521024.cn

[T42] Perl：变量类型
来源：http://xw.hnjuh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wp.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://ij.szsharing.cn

"值: $a"
来源：http://gb.shtwfgs.cn

[T44] Perl：条件
来源：http://tw.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://bo.newstarts.cn

[T45] Perl：数组遍历
来源：http://ru.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://jo.hahajie.cn

[T46] Perl：哈希操作
来源：http://np.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ww.gzmigu.cn

[T47] Perl：正则捕获
来源：http://xc.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sa.shxzskj.cn

[T48] Perl：正则替换
来源：http://yy.521024.cn

$s =~ s/old/new/g;
来源：http://tx.shtwfgs.cn

[T49] Perl：函数
来源：http://xl.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://im.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://dk.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vd.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://fa.newstarts.cn

[T51] Scala：Hello World
来源：http://wi.hnjuh.cn

println("Hello")
来源：http://dc.nszjky.cn

[T52] Scala：变量
来源：http://dd.huanxung.cn

val a = 1;  var b = 2
来源：http://iy.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://hw.asd995.cn

s"值: $b"
来源：http://iu.chemitech.net.cn

[T54] Scala：集合映射
来源：http://zl.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://cj.hnjuh.cn

[T55] Scala：集合过滤
来源：http://ey.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mt.huixiangedu.cn

[T56] Scala：样例类
来源：http://vu.szsharing.cn


<!-- 参考信息 -->