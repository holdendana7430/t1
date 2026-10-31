代发 wailian999

ssh user@host 'uptime'
来源：http://ki.yuntaijiaju.cn

[R58] 下载文件
来源：http://lz.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://at.nszjky.cn

[R59] 发 POST JSON
来源：http://kg.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ib.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://ys.yuntaijiaju.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zh.lnxyls.cn

[R61] 磁盘占用
来源：http://mx.lnxyls.cn

df -h;  du -sh *
来源：http://dp.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://ns.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://ca.shtwfgs.cn

[R63] 内存与进程
来源：http://bc.521024.cn

free -h;  ps aux | grep nginx
来源：http://ut.huanxung.cn

[R64] 结束进程
来源：http://sy.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://ux.shxzukj.cn

[R65] 查看端口占用
来源：http://nx.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mz.nicolike.cn

[R66] 定时任务
来源：http://qv.colortex.cn

crontab -e;  crontab -l
来源：http://zv.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://pe.huixinmuqiang.cn

openssl rand -hex 16
来源：http://oj.shxzukj.cn

[R68] 计算文件校验值
来源：http://ht.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ol.panjiajie.cn

[R69] 生成随机密码
来源：http://ej.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://cl.shtwfgs.cn

[R70] 时间戳与互转
来源：http://an.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://io.9csxet.cn

[R71] 日期格式化
来源：http://md.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ni.shtwfgs.cn

[R72] 等待端口就绪
来源：http://uf.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sz.lnxyls.cn

[R73] 分割大日志
来源：http://pz.hahajie.cn

split -l 1000 big.log part_
来源：http://kg.hnjuh.cn

[R74] 批量重命名
来源：http://rb.newstarts.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ti.shxzukj.cn

[R75] 导出环境变量
来源：http://ga.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://br.hahajie.cn

[R76] 使用临时文件
来源：http://or.jianghongdianzi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fe.shxzukj.cn

[R77] 读取用户输入
来源：http://ih.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://jq.panjiajie.cn

[R78] 交互式菜单
来源：http://bd.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ds.colortex.cn

[R79] 解析命令行选项
来源：http://yk.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xd.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://ka.szsharing.cn

time ./run.sh
来源：http://jk.chemitech.net.cn

================================================================================
来源：http://ia.yuntaijiaju.cn

S. C / C++ 专题
来源：http://tk.9csxet.cn

================================================================================
来源：http://hk.jctech888.com.cn

[S01] C：Hello World
来源：http://br.jianghongdianzi.cn

#include <stdio.h>
来源：http://vl.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kw.szsharing.cn

[S02] C：变量与格式化输出
来源：http://yj.lnxyls.cn

int a = 10; printf("%d\n", a);
来源：http://uz.szsharing.cn

[S03] C：读入整数
来源：http://jo.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://vv.haigaiapp.cn

[S04] C：字符串复制
来源：http://xq.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pj.shxzskj.cn

[S05] C：字符串长度
来源：http://yu.shtwfgs.cn

strlen(s)
来源：http://em.newstarts.cn

[S06] C：字符串比较
来源：http://ku.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://kz.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://og.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ds.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://ln.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fm.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://ru.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zq.newstarts.cn

[S10] C：指针与解引用
来源：http://aw.hahajie.cn

int *p = &a;  *p = 5;
来源：http://pd.huixiangedu.cn

[S11] C：逐行读文件
来源：http://ri.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://rh.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mt.9csxet.cn

fclose(f);
来源：http://nl.yuexingan06.cn

[S12] C：写文件
来源：http://bs.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sz.bookmarksfly.cn

[S13] C：宏定义
来源：http://gk.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qk.shtwfgs.cn

[S14] C：枚举
来源：http://uj.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://mv.newstarts.cn

[S15] C：类型转换
来源：http://pj.jctech888.com.cn

(double) a / b
来源：http://jj.wgjwhj.cn

[S16] C：位操作置位
来源：http://ng.wgjwhj.cn

x |= (1 << 3);
来源：http://fb.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://gu.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nl.panjiajie.cn

[S18] C：命令行参数
来源：http://gm.newstarts.cn

int main(int argc, char **argv)
来源：http://oc.muxihuayi.cn

[S19] C：快速排序
来源：http://cz.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yj.wgjwhj.cn

[S20] C：二分查找
来源：http://zk.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bn.huixiangedu.cn

[S21] C：字符类别判断
来源：http://rd.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ma.shxzukj.cn

[S22] C：字符串转数字
来源：http://xa.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://eh.huixinmuqiang.cn

[S23] C：随机数
来源：http://fw.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tv.nszjky.cn

[S24] C：获取本地时间
来源：http://wp.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wg.shtwfgs.cn

[S25] C：内存拷贝
来源：http://ep.wgjwhj.cn

memcpy(dst, src, n);
来源：http://dp.bookmarksfly.cn

[S26] C：内存清零
来源：http://wn.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://ar.jianghongdianzi.cn

[S27] C：定义常量
来源：http://zv.panjiajie.cn

const double PI = 3.14159;
来源：http://ev.hahajie.cn

[S28] C：静态变量
来源：http://ey.nszjky.cn

static int counter = 0;
来源：http://wz.haigaiapp.cn

[S29] C：变参函数
来源：http://iq.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rz.yuexingan06.cn

[S30] C：头文件保护
来源：http://pa.muxihuayi.cn

#ifndef X_H
来源：http://ri.nicolike.cn

#define X_H
来源：http://ky.chemitech.net.cn

#endif
来源：http://bh.chemitech.net.cn

[S31] C++：Hello World
来源：http://kt.szxytkj.cn

#include <iostream>
来源：http://wp.huixiangedu.cn

int main() { std::cout << "Hello\n"; }
来源：http://ns.muxihuayi.cn

[S32] C++：字符串
来源：http://wb.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://gb.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://ev.haigaiapp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gy.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://qd.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://uy.panjiajie.cn

[S35] C++：map
来源：http://qd.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cx.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://le.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ko.colortex.cn

[S37] C++：set
来源：http://hy.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://me.jianghongdianzi.cn

[S38] C++：排序
来源：http://gd.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://cu.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://ke.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pr.huanxung.cn

[S40] C++：查找元素
来源：http://je.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sr.nicolike.cn

[S41] C++：类与构造函数
来源：http://gw.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qu.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://ad.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://eh.nszjky.cn

[S43] C++：智能指针
来源：http://xu.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://ao.wgjwhj.cn

[S44] C++：引用传参
来源：http://dm.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://to.wgjwhj.cn

[S45] C++：lambda
来源：http://ha.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xr.shxzskj.cn

[S46] C++：函数模板
来源：http://zd.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uo.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://op.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uk.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://ef.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cj.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://pa.huixiangedu.cn

[S49] C++：写文件
来源：http://fm.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bj.shxzskj.cn

[S50] C++：格式化数字
来源：http://qt.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tv.asd995.cn

[S51] C++：显式类型转换
来源：http://nj.huanxung.cn

static_cast<double>(a) / b
来源：http://qk.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://st.newstarts.cn

int size() const noexcept { return n_; }
来源：http://lg.haigaiapp.cn

[S53] C++：移动语义
来源：http://bx.521024.cn

std::vector<int> w = std::move(v);
来源：http://jf.shxzukj.cn

[S54] C++：异常处理
来源：http://yu.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://au.nszjky.cn

[S55] C++：结构化绑定
来源：http://ob.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://py.lnxyls.cn

[S56] C++：optional
来源：http://bz.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lk.521024.cn

[S57] C++：编译期常量
来源：http://co.jianghongdianzi.cn

constexpr int N = 10;
来源：http://km.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://rf.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://lp.lnxyls.cn

[S59] C++：静态断言
来源：http://ie.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cl.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://sv.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://da.bjjhwx.cn

================================================================================
来源：http://lj.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://im.huanxung.cn

================================================================================
来源：http://tx.nicolike.cn

[T01] Kotlin：Hello World
来源：http://rr.panjiajie.cn

println("Hello")
来源：http://bt.panjiajie.cn

[T02] Kotlin：变量
来源：http://cs.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://no.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://bb.jianghongdianzi.cn

"值: $b"
来源：http://hw.gzmigu.cn

[T04] Kotlin：空安全
来源：http://zk.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://iw.jianghongdianzi.cn

[T05] Kotlin：when 表达式
来源：http://ld.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mb.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://gn.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pn.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://ir.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uy.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://xq.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://qt.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://qz.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://gs.asd995.cn

[T10] Kotlin：默认参数
来源：http://en.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ab.9csxet.cn

[T11] Kotlin：协程
来源：http://ap.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ca.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://mt.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://gm.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://mp.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://jb.shxzukj.cn

[T14] Kotlin：循环
来源：http://zc.shxzskj.cn

for (i in 1..10) println(i)
来源：http://wx.yuexingan06.cn

[T15] Kotlin：接口
来源：http://wg.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://oa.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://em.shxzskj.cn

print("Hello")
来源：http://rv.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://ea.9csxet.cn

var a = 1;  let b = 2
来源：http://mi.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://ic.muxihuayi.cn

"值: \(b)"
来源：http://rg.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://fj.521024.cn

if let n = opt { print(n) }
来源：http://un.gzmigu.cn

[T20] Swift：数组操作
来源：http://en.nicolike.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fy.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://ap.yuexingan06.cn

for x in a { print(x) }
来源：http://wk.9csxet.cn

[T22] Swift：字典
来源：http://sc.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ca.yuexingan06.cn

[T23] Swift：函数
来源：http://fz.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bv.newstarts.cn

[T24] Swift：闭包
来源：http://dz.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gw.shtwfgs.cn

[T25] Swift：结构体
来源：http://ig.muxihuayi.cn

struct P { var x: Int }
来源：http://ed.lnxyls.cn

[T26] Swift：类与重写
来源：http://rr.lnxyls.cn

class A: Base { override func f() {} }
来源：http://fe.haigaiapp.cn

[T27] Swift：错误处理
来源：http://ch.nicolike.cn

do { try f() } catch { print(error) }
来源：http://sg.chemitech.net.cn

[T28] Swift：枚举
来源：http://ni.yuexingan06.cn

enum Color { case red, green }
来源：http://zc.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://db.hahajie.cn

guard let x = opt else { return }
来源：http://rz.wgjwhj.cn

[T30] Swift：协议
来源：http://kb.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://rf.hnjuh.cn

[T31] Lua：Hello World
来源：http://ar.newstarts.cn

print("Hello")
来源：http://uj.muxihuayi.cn

[T32] Lua：局部变量
来源：http://gv.muxihuayi.cn

local a = 1
来源：http://sj.newstarts.cn

[T33] Lua：表（数组）
来源：http://ib.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gt.huixiangedu.cn

[T34] Lua：遍历表
来源：http://rc.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fw.hnjuh.cn

[T35] Lua：字典表
来源：http://jb.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://nh.szsharing.cn

[T36] Lua：函数
来源：http://vo.jctech888.com.cn

function add(a, b) return a + b end
来源：http://vo.szsharing.cn

[T37] Lua：字符串拼接
来源：http://ng.jianghongdianzi.cn

"a" .. "b"
来源：http://hk.gzmigu.cn

[T38] Lua：条件
来源：http://lf.wgjwhj.cn

if x > 0 then print("正") end
来源：http://uq.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://yl.nicolike.cn

string.find(s, "%d+")
来源：http://la.jctech888.com.cn

[T40] Lua：元表
来源：http://nz.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://ho.newstarts.cn

[T41] Perl：Hello World
来源：http://gx.521024.cn

print "Hello\n";
来源：http://hn.nicolike.cn

[T42] Perl：变量类型
来源：http://zr.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vf.newstarts.cn

[T43] Perl：字符串插值
来源：http://kt.nszjky.cn

"值: $a"
来源：http://jg.nszjky.cn

[T44] Perl：条件
来源：http://nb.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://ea.colortex.cn

[T45] Perl：数组遍历
来源：http://fl.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://rs.nicolike.cn

[T46] Perl：哈希操作
来源：http://ng.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gg.9csxet.cn

[T47] Perl：正则捕获
来源：http://kx.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fq.huixinmuqiang.cn

[T48] Perl：正则替换
来源：http://zh.huanxung.cn

$s =~ s/old/new/g;
来源：http://rc.hnjuh.cn

[T49] Perl：函数
来源：http://ib.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zz.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://dm.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://se.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://ax.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://so.nicolike.cn

println("Hello")
来源：http://co.521024.cn

[T52] Scala：变量
来源：http://za.bjjhwx.cn

val a = 1;  var b = 2
来源：http://qu.hnjuh.cn

[T53] Scala：字符串插值
来源：http://gi.jianghongdianzi.cn

s"值: $b"
来源：http://ni.521024.cn

[T54] Scala：集合映射
来源：http://fg.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://sa.lnxyls.cn

[T55] Scala：集合过滤
来源：http://jh.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xv.9csxet.cn

[T56] Scala：样例类
来源：http://bx.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://qt.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://iq.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dg.hnjuh.cn

[T58] Scala：函数定义
来源：http://ip.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gi.colortex.cn

[T59] Scala：循环
来源：http://kl.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://ok.asd995.cn

[T60] Scala：折叠
来源：http://ck.hnjuh.cn


<!-- 参考信息 -->