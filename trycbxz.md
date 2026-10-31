代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yx.szxytkj.cn

[R56] 远程拷贝
来源：http://nh.haigaiapp.cn

scp file user@host:/path/
来源：http://wz.bookmarksfly.cn

[R57] 远程执行命令
来源：http://ua.chemitech.net.cn

ssh user@host 'uptime'
来源：http://og.jianghongdianzi.cn

[R58] 下载文件
来源：http://zq.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oq.bjjhwx.cn

[R59] 发 POST JSON
来源：http://wc.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qw.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://ih.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://co.hnjuh.cn

[R61] 磁盘占用
来源：http://eb.jianghongdianzi.cn

df -h;  du -sh *
来源：http://ym.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://eq.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://te.colortex.cn

[R63] 内存与进程
来源：http://rp.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://ju.bjjhwx.cn

[R64] 结束进程
来源：http://kk.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://za.szxytkj.cn

[R65] 查看端口占用
来源：http://lj.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cn.shtwfgs.cn

[R66] 定时任务
来源：http://cp.shtwfgs.cn

crontab -e;  crontab -l
来源：http://is.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://ku.jianghongdianzi.cn

openssl rand -hex 16
来源：http://ru.newstarts.cn

[R68] 计算文件校验值
来源：http://io.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bo.chemitech.net.cn

[R69] 生成随机密码
来源：http://pl.521024.cn

head -c 16 /dev/urandom | base64
来源：http://lm.9csxet.cn

[R70] 时间戳与互转
来源：http://gs.nszjky.cn

date +%s;  date -d @1700000000
来源：http://ic.jianghongdianzi.cn

[R71] 日期格式化
来源：http://zo.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qn.521024.cn

[R72] 等待端口就绪
来源：http://mg.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qn.shxzukj.cn

[R73] 分割大日志
来源：http://mb.gzmigu.cn

split -l 1000 big.log part_
来源：http://ic.newstarts.cn

[R74] 批量重命名
来源：http://ts.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dg.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://ex.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://gc.szsharing.cn

[R76] 使用临时文件
来源：http://sb.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wa.chemitech.net.cn

[R77] 读取用户输入
来源：http://hi.muxihuayi.cn

read -rp "请输入: " ans
来源：http://jo.colortex.cn

[R78] 交互式菜单
来源：http://fw.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ku.huanxung.cn

[R79] 解析命令行选项
来源：http://ff.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pq.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://tx.gzmigu.cn

time ./run.sh
来源：http://vn.panjiajie.cn

================================================================================
来源：http://qw.shtwfgs.cn

S. C / C++ 专题
来源：http://qx.shxzukj.cn

================================================================================
来源：http://zs.shtwfgs.cn

[S01] C：Hello World
来源：http://sf.nszjky.cn

#include <stdio.h>
来源：http://us.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mg.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://kf.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://nv.jctech888.com.cn

[S03] C：读入整数
来源：http://te.9csxet.cn

int x; scanf("%d", &x);
来源：http://rk.nszjky.cn

[S04] C：字符串复制
来源：http://rg.nicolike.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bz.asd995.cn

[S05] C：字符串长度
来源：http://er.shxzskj.cn

strlen(s)
来源：http://wx.nszjky.cn

[S06] C：字符串比较
来源：http://qb.colortex.cn

strcmp(a, b) == 0
来源：http://zd.9csxet.cn

[S07] C：数组遍历求和
来源：http://wz.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bd.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://ur.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://we.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://jk.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mn.hnjuh.cn

[S10] C：指针与解引用
来源：http://vu.9csxet.cn

int *p = &a;  *p = 5;
来源：http://oc.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://tt.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://jc.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ul.9csxet.cn

fclose(f);
来源：http://cn.colortex.cn

[S12] C：写文件
来源：http://kl.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ow.hahajie.cn

[S13] C：宏定义
来源：http://dp.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ug.hnjuh.cn

[S14] C：枚举
来源：http://qx.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://ut.yuntaijiaju.cn

[S15] C：类型转换
来源：http://im.panjiajie.cn

(double) a / b
来源：http://hh.colortex.cn

[S16] C：位操作置位
来源：http://oo.bjjhwx.cn

x |= (1 << 3);
来源：http://fv.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://qc.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lf.shtwfgs.cn

[S18] C：命令行参数
来源：http://rc.muxihuayi.cn

int main(int argc, char **argv)
来源：http://rq.panjiajie.cn

[S19] C：快速排序
来源：http://tu.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://em.lnxyls.cn

[S20] C：二分查找
来源：http://qp.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ns.shxzukj.cn

[S21] C：字符类别判断
来源：http://df.wgjwhj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vv.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://nb.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ls.bookmarksfly.cn

[S23] C：随机数
来源：http://ns.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zn.yuexingan06.cn

[S24] C：获取本地时间
来源：http://pu.yuexingan06.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gb.newstarts.cn

[S25] C：内存拷贝
来源：http://it.lnxyls.cn

memcpy(dst, src, n);
来源：http://lb.colortex.cn

[S26] C：内存清零
来源：http://ol.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://gx.521024.cn

[S27] C：定义常量
来源：http://jq.chemitech.net.cn

const double PI = 3.14159;
来源：http://ie.nicolike.cn

[S28] C：静态变量
来源：http://tx.hahajie.cn

static int counter = 0;
来源：http://pk.szsharing.cn

[S29] C：变参函数
来源：http://ai.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uc.bookmarksfly.cn

[S30] C：头文件保护
来源：http://gh.haigaiapp.cn

#ifndef X_H
来源：http://ap.chemitech.net.cn

#define X_H
来源：http://dt.yuntaijiaju.cn

#endif
来源：http://rw.haigaiapp.cn

[S31] C++：Hello World
来源：http://zl.lnxyls.cn

#include <iostream>
来源：http://nr.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://mx.huanxung.cn

[S32] C++：字符串
来源：http://kk.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://qv.9csxet.cn

[S33] C++：vector 增删
来源：http://dk.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jr.szsharing.cn

[S34] C++：遍历 vector
来源：http://dl.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://dc.huixiangedu.cn

[S35] C++：map
来源：http://cj.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://df.huixiangedu.cn

[S36] C++：unordered_map
来源：http://th.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wj.huixiangedu.cn

[S37] C++：set
来源：http://dp.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://od.lnxyls.cn

[S38] C++：排序
来源：http://xt.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://ca.gzmigu.cn

[S39] C++：自定义比较器排序
来源：http://as.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tn.szsharing.cn

[S40] C++：查找元素
来源：http://mj.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ky.szxytkj.cn

[S41] C++：类与构造函数
来源：http://pt.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tn.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://qc.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://ua.9csxet.cn

[S43] C++：智能指针
来源：http://cn.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://np.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://qm.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://ga.panjiajie.cn

[S45] C++：lambda
来源：http://sk.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wp.bookmarksfly.cn

[S46] C++：函数模板
来源：http://ox.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ru.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://am.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cc.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://iy.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hj.521024.cn

while (std::getline(in, line)) { }
来源：http://kq.shxzskj.cn

[S49] C++：写文件
来源：http://wg.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ig.huixiangedu.cn

[S50] C++：格式化数字
来源：http://pv.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gb.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://lp.szsharing.cn

static_cast<double>(a) / b
来源：http://bt.asd995.cn

[S52] C++：const 与 noexcept
来源：http://yq.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://yf.shtwfgs.cn

[S53] C++：移动语义
来源：http://sm.wgjwhj.cn

std::vector<int> w = std::move(v);
来源：http://ju.gzmigu.cn

[S54] C++：异常处理
来源：http://bl.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jy.shxzukj.cn

[S55] C++：结构化绑定
来源：http://mq.bjjhwx.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cs.nszjky.cn

[S56] C++：optional
来源：http://qw.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://up.lnxyls.cn

[S57] C++：编译期常量
来源：http://tz.yuexingan06.cn

constexpr int N = 10;
来源：http://ml.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://ts.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://py.newstarts.cn

[S59] C++：静态断言
来源：http://av.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://la.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://lk.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ai.newstarts.cn

================================================================================
来源：http://bq.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lr.jctech888.com.cn

================================================================================
来源：http://fl.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://zd.panjiajie.cn

println("Hello")
来源：http://pu.yuexingan06.cn

[T02] Kotlin：变量
来源：http://hn.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tc.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://na.huixinmuqiang.cn

"值: $b"
来源：http://pe.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://fr.9csxet.cn

val n: String? = null;  n?.length
来源：http://ar.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://kf.9csxet.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://td.hahajie.cn

[T06] Kotlin：集合映射
来源：http://zx.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ak.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://rq.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://eu.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://bz.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://ov.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://kz.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://in.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://mr.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kd.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://hc.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ug.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://ps.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://ky.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://zr.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://cf.chemitech.net.cn

[T14] Kotlin：循环
来源：http://fc.lnxyls.cn

for (i in 1..10) println(i)
来源：http://ji.jctech888.com.cn

[T15] Kotlin：接口
来源：http://gy.nszjky.cn

interface Shape { fun area(): Double }
来源：http://jl.shxzukj.cn

[T16] Swift：Hello World
来源：http://lt.bjjhwx.cn

print("Hello")
来源：http://yu.newstarts.cn

[T17] Swift：变量与常量
来源：http://ps.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://fj.shxzukj.cn

[T18] Swift：字符串插值
来源：http://pg.huixinmuqiang.cn

"值: \(b)"
来源：http://dn.yuntaijiaju.cn

[T19] Swift：可选绑定
来源：http://nj.hnjuh.cn

if let n = opt { print(n) }
来源：http://lt.nszjky.cn

[T20] Swift：数组操作
来源：http://ze.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ds.hahajie.cn

[T21] Swift：遍历
来源：http://jn.hnjuh.cn

for x in a { print(x) }
来源：http://qk.colortex.cn

[T22] Swift：字典
来源：http://dd.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mo.szxytkj.cn

[T23] Swift：函数
来源：http://nc.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gf.shxzskj.cn

[T24] Swift：闭包
来源：http://zf.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cz.jctech888.com.cn

[T25] Swift：结构体
来源：http://kx.9csxet.cn

struct P { var x: Int }
来源：http://ub.huixiangedu.cn

[T26] Swift：类与重写
来源：http://ev.nszjky.cn

class A: Base { override func f() {} }
来源：http://zs.yuexingan06.cn

[T27] Swift：错误处理
来源：http://al.szxytkj.cn

do { try f() } catch { print(error) }
来源：http://ch.bookmarksfly.cn

[T28] Swift：枚举
来源：http://bg.szsharing.cn

enum Color { case red, green }
来源：http://mk.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://us.newstarts.cn

guard let x = opt else { return }
来源：http://vh.shxzskj.cn

[T30] Swift：协议
来源：http://yp.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://ae.asd995.cn

[T31] Lua：Hello World
来源：http://bu.haigaiapp.cn

print("Hello")
来源：http://ll.shxzukj.cn

[T32] Lua：局部变量
来源：http://jf.chemitech.net.cn

local a = 1
来源：http://ic.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://nw.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jp.newstarts.cn

[T34] Lua：遍历表
来源：http://yz.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hc.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://ph.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://fb.huixinmuqiang.cn

[T36] Lua：函数
来源：http://mu.jctech888.com.cn

function add(a, b) return a + b end
来源：http://ck.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://ao.nicolike.cn

"a" .. "b"
来源：http://rd.bookmarksfly.cn

[T38] Lua：条件
来源：http://op.haigaiapp.cn

if x > 0 then print("正") end
来源：http://hg.newstarts.cn

[T39] Lua：模式匹配
来源：http://vo.yuexingan06.cn

string.find(s, "%d+")
来源：http://ah.jianghongdianzi.cn

[T40] Lua：元表
来源：http://oe.newstarts.cn

setmetatable({}, { __index = base })
来源：http://ml.wgjwhj.cn

[T41] Perl：Hello World
来源：http://dz.huanxung.cn

print "Hello\n";
来源：http://dv.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://mi.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zr.shxzskj.cn

[T43] Perl：字符串插值
来源：http://xw.panjiajie.cn

"值: $a"
来源：http://vm.hahajie.cn

[T44] Perl：条件
来源：http://ri.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://ui.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://ep.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://im.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://dl.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://re.hnjuh.cn

[T47] Perl：正则捕获
来源：http://yi.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rf.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://ow.lnxyls.cn

$s =~ s/old/new/g;
来源：http://oz.hnjuh.cn

[T49] Perl：函数
来源：http://eo.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tb.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://ik.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lz.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://di.9csxet.cn

[T51] Scala：Hello World
来源：http://sj.hahajie.cn

println("Hello")
来源：http://bc.jctech888.com.cn

[T52] Scala：变量
来源：http://xy.huixiangedu.cn

val a = 1;  var b = 2
来源：http://oc.szsharing.cn

[T53] Scala：字符串插值
来源：http://ye.wgjwhj.cn

s"值: $b"
来源：http://fi.chemitech.net.cn

[T54] Scala：集合映射
来源：http://lw.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://gp.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://gt.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ve.bjjhwx.cn

[T56] Scala：样例类
来源：http://ap.huanxung.cn

case class User(name: String, age: Int)
来源：http://fm.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://wl.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xh.shxzskj.cn

[T58] Scala：函数定义
来源：http://ka.panjiajie.cn


<!-- 参考信息 -->