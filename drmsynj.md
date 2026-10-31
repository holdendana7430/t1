代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uu.chemitech.net.cn

[R54] 比较两个文件
来源：http://qr.huanxung.cn

diff a.txt b.txt
来源：http://gm.szsharing.cn

[R55] 压缩与解压
来源：http://ok.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pz.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://dr.huixiangedu.cn

scp file user@host:/path/
来源：http://sc.shxzskj.cn

[R57] 远程执行命令
来源：http://ms.szsharing.cn

ssh user@host 'uptime'
来源：http://ud.lnxyls.cn

[R58] 下载文件
来源：http://gd.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oa.shxzskj.cn

[R59] 发 POST JSON
来源：http://md.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xb.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://nn.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uk.9csxet.cn

[R61] 磁盘占用
来源：http://fw.gzmigu.cn

df -h;  du -sh *
来源：http://bk.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://vg.jctech888.com.cn

du -ah . | sort -rh | head -10
来源：http://ho.gzmigu.cn

[R63] 内存与进程
来源：http://kn.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://tk.huanxung.cn

[R64] 结束进程
来源：http://wf.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://ix.colortex.cn

[R65] 查看端口占用
来源：http://rj.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ec.shxzskj.cn

[R66] 定时任务
来源：http://qs.hahajie.cn

crontab -e;  crontab -l
来源：http://oz.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://lg.haigaiapp.cn

openssl rand -hex 16
来源：http://xq.huixiangedu.cn

[R68] 计算文件校验值
来源：http://ae.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mj.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://gf.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://om.panjiajie.cn

[R70] 时间戳与互转
来源：http://jh.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://hy.jctech888.com.cn

[R71] 日期格式化
来源：http://af.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yi.lnxyls.cn

[R72] 等待端口就绪
来源：http://ve.chemitech.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zz.shxzskj.cn

[R73] 分割大日志
来源：http://ea.szxytkj.cn

split -l 1000 big.log part_
来源：http://rz.huixiangedu.cn

[R74] 批量重命名
来源：http://ge.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nl.newstarts.cn

[R75] 导出环境变量
来源：http://zz.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://re.hnjuh.cn

[R76] 使用临时文件
来源：http://oh.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hg.lnxyls.cn

[R77] 读取用户输入
来源：http://nu.newstarts.cn

read -rp "请输入: " ans
来源：http://lc.shxzukj.cn

[R78] 交互式菜单
来源：http://tj.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://by.huanxung.cn

[R79] 解析命令行选项
来源：http://vd.colortex.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gf.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://mz.yuexingan06.cn

time ./run.sh
来源：http://wy.nszjky.cn

================================================================================
来源：http://dc.hnjuh.cn

S. C / C++ 专题
来源：http://bi.shtwfgs.cn

================================================================================
来源：http://tk.shxzskj.cn

[S01] C：Hello World
来源：http://hl.shxzukj.cn

#include <stdio.h>
来源：http://xt.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kr.hahajie.cn

[S02] C：变量与格式化输出
来源：http://qw.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://lz.muxihuayi.cn

[S03] C：读入整数
来源：http://dq.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://hl.yuexingan06.cn

[S04] C：字符串复制
来源：http://ub.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zs.newstarts.cn

[S05] C：字符串长度
来源：http://fe.colortex.cn

strlen(s)
来源：http://no.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://em.yuexingan06.cn

strcmp(a, b) == 0
来源：http://ia.shxzukj.cn

[S07] C：数组遍历求和
来源：http://cd.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lj.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://ah.chemitech.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ob.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://pp.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vc.521024.cn

[S10] C：指针与解引用
来源：http://rm.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://tm.newstarts.cn

[S11] C：逐行读文件
来源：http://nc.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://vl.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fs.colortex.cn

fclose(f);
来源：http://xf.huixinmuqiang.cn

[S12] C：写文件
来源：http://qj.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lx.huanxung.cn

[S13] C：宏定义
来源：http://bo.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wl.asd995.cn

[S14] C：枚举
来源：http://tq.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://fa.jctech888.com.cn

[S15] C：类型转换
来源：http://hn.muxihuayi.cn

(double) a / b
来源：http://cp.asd995.cn

[S16] C：位操作置位
来源：http://xu.yuexingan06.cn

x |= (1 << 3);
来源：http://ll.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://qv.bjjhwx.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yc.gzmigu.cn

[S18] C：命令行参数
来源：http://og.huixiangedu.cn

int main(int argc, char **argv)
来源：http://kb.newstarts.cn

[S19] C：快速排序
来源：http://pu.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ep.panjiajie.cn

[S20] C：二分查找
来源：http://vm.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qi.gzmigu.cn

[S21] C：字符类别判断
来源：http://zh.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://or.gzmigu.cn

[S22] C：字符串转数字
来源：http://sb.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cp.huixinmuqiang.cn

[S23] C：随机数
来源：http://ve.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ii.lnxyls.cn

[S24] C：获取本地时间
来源：http://mv.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gf.9csxet.cn

[S25] C：内存拷贝
来源：http://lz.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://ls.hahajie.cn

[S26] C：内存清零
来源：http://vc.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://yw.nszjky.cn

[S27] C：定义常量
来源：http://rz.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://hu.bookmarksfly.cn

[S28] C：静态变量
来源：http://dl.muxihuayi.cn

static int counter = 0;
来源：http://yf.jctech888.com.cn

[S29] C：变参函数
来源：http://tk.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ny.hnjuh.cn

[S30] C：头文件保护
来源：http://zn.yuexingan06.cn

#ifndef X_H
来源：http://bb.colortex.cn

#define X_H
来源：http://wa.jianghongdianzi.cn

#endif
来源：http://qv.521024.cn

[S31] C++：Hello World
来源：http://rf.bjjhwx.cn

#include <iostream>
来源：http://pe.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://ts.shtwfgs.cn

[S32] C++：字符串
来源：http://ac.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://iz.huixiangedu.cn

[S33] C++：vector 增删
来源：http://zq.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qt.huanxung.cn

[S34] C++：遍历 vector
来源：http://im.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://tl.521024.cn

[S35] C++：map
来源：http://dq.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sq.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://kz.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://js.huanxung.cn

[S37] C++：set
来源：http://ps.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oh.chemitech.net.cn

[S38] C++：排序
来源：http://lg.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://qm.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://oj.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cc.shxzukj.cn

[S40] C++：查找元素
来源：http://xp.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ik.nicolike.cn

[S41] C++：类与构造函数
来源：http://tq.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ma.haigaiapp.cn

[S42] C++：继承与虚函数
来源：http://or.521024.cn

class B : public Base { public: void f() override {} };
来源：http://jw.yuexingan06.cn

[S43] C++：智能指针
来源：http://pr.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://kq.bookmarksfly.cn

[S44] C++：引用传参
来源：http://ru.newstarts.cn

void inc(int &x) { ++x; }
来源：http://id.gzmigu.cn

[S45] C++：lambda
来源：http://kd.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bw.hnjuh.cn

[S46] C++：函数模板
来源：http://rh.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zr.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://mn.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ig.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://ek.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ed.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://gd.yuntaijiaju.cn

[S49] C++：写文件
来源：http://wq.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cx.jctech888.com.cn

[S50] C++：格式化数字
来源：http://ql.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wy.gzmigu.cn

[S51] C++：显式类型转换
来源：http://qm.nicolike.cn

static_cast<double>(a) / b
来源：http://fr.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://zh.colortex.cn

int size() const noexcept { return n_; }
来源：http://zq.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://gh.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://vg.hnjuh.cn

[S54] C++：异常处理
来源：http://ca.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yx.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://cv.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ew.nszjky.cn

[S56] C++：optional
来源：http://yy.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zl.yuexingan06.cn

[S57] C++：编译期常量
来源：http://rt.asd995.cn

constexpr int N = 10;
来源：http://gf.521024.cn

[S58] C++：命名空间
来源：http://kc.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://ra.bookmarksfly.cn

[S59] C++：静态断言
来源：http://yc.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xc.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://jp.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://am.shxzukj.cn

================================================================================
来源：http://kh.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jx.colortex.cn

================================================================================
来源：http://us.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://pq.shtwfgs.cn

println("Hello")
来源：http://zl.newstarts.cn

[T02] Kotlin：变量
来源：http://ub.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://om.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://gf.newstarts.cn

"值: $b"
来源：http://ie.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://bv.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://so.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://uz.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hd.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://gs.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xx.521024.cn

[T07] Kotlin：集合过滤
来源：http://oo.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ks.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://uv.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://ux.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://ib.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://fd.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://mo.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://up.shxzukj.cn

[T11] Kotlin：协程
来源：http://ig.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dj.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://jy.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://nf.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://rp.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://ty.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://iw.jctech888.com.cn

for (i in 1..10) println(i)
来源：http://xq.huixiangedu.cn

[T15] Kotlin：接口
来源：http://vv.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://wy.nszjky.cn

[T16] Swift：Hello World
来源：http://kw.shxzskj.cn

print("Hello")
来源：http://rd.nicolike.cn

[T17] Swift：变量与常量
来源：http://ai.haigaiapp.cn

var a = 1;  let b = 2
来源：http://su.asd995.cn

[T18] Swift：字符串插值
来源：http://nf.szxytkj.cn

"值: \(b)"
来源：http://hg.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://vf.shtwfgs.cn

if let n = opt { print(n) }
来源：http://xp.asd995.cn

[T20] Swift：数组操作
来源：http://os.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ed.lnxyls.cn

[T21] Swift：遍历
来源：http://pp.shxzskj.cn

for x in a { print(x) }
来源：http://ga.shxzskj.cn

[T22] Swift：字典
来源：http://yz.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sl.muxihuayi.cn

[T23] Swift：函数
来源：http://xm.wgjwhj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ch.huixiangedu.cn

[T24] Swift：闭包
来源：http://mh.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jm.jctech888.com.cn

[T25] Swift：结构体
来源：http://fq.panjiajie.cn

struct P { var x: Int }
来源：http://vy.huixinmuqiang.cn

[T26] Swift：类与重写
来源：http://jd.gzmigu.cn

class A: Base { override func f() {} }
来源：http://hj.haigaiapp.cn

[T27] Swift：错误处理
来源：http://ap.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://ae.9csxet.cn

[T28] Swift：枚举
来源：http://mo.jctech888.com.cn

enum Color { case red, green }
来源：http://yz.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://mi.jctech888.com.cn

guard let x = opt else { return }
来源：http://ia.shxzskj.cn

[T30] Swift：协议
来源：http://gp.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://lu.9csxet.cn

[T31] Lua：Hello World
来源：http://ix.nszjky.cn

print("Hello")
来源：http://lf.bjjhwx.cn

[T32] Lua：局部变量
来源：http://es.9csxet.cn

local a = 1
来源：http://pq.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://zo.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nt.newstarts.cn

[T34] Lua：遍历表
来源：http://ch.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ta.shtwfgs.cn

[T35] Lua：字典表
来源：http://pj.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://rh.newstarts.cn

[T36] Lua：函数
来源：http://km.shxzukj.cn

function add(a, b) return a + b end
来源：http://um.9csxet.cn

[T37] Lua：字符串拼接
来源：http://jd.yuexingan06.cn

"a" .. "b"
来源：http://ij.nszjky.cn

[T38] Lua：条件
来源：http://zj.huixiangedu.cn

if x > 0 then print("正") end
来源：http://sq.hnjuh.cn

[T39] Lua：模式匹配
来源：http://wb.hnjuh.cn

string.find(s, "%d+")
来源：http://kc.huixinmuqiang.cn

[T40] Lua：元表
来源：http://vs.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://gj.lnxyls.cn

[T41] Perl：Hello World
来源：http://yb.panjiajie.cn

print "Hello\n";
来源：http://ub.szxytkj.cn

[T42] Perl：变量类型
来源：http://qj.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fn.nicolike.cn

[T43] Perl：字符串插值
来源：http://uj.muxihuayi.cn

"值: $a"
来源：http://wt.521024.cn

[T44] Perl：条件
来源：http://dr.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://os.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://ts.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://ia.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://mj.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://su.gzmigu.cn

[T47] Perl：正则捕获
来源：http://ve.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dm.panjiajie.cn

[T48] Perl：正则替换
来源：http://gf.szsharing.cn

$s =~ s/old/new/g;
来源：http://zd.huixiangedu.cn

[T49] Perl：函数
来源：http://io.shxzukj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://id.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://td.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uk.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ib.hahajie.cn

[T51] Scala：Hello World
来源：http://kj.huixiangedu.cn

println("Hello")
来源：http://at.huixinmuqiang.cn

[T52] Scala：变量
来源：http://bx.yuexingan06.cn

val a = 1;  var b = 2
来源：http://uz.nszjky.cn

[T53] Scala：字符串插值
来源：http://xn.nszjky.cn

s"值: $b"
来源：http://wr.chemitech.net.cn

[T54] Scala：集合映射
来源：http://lu.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://fa.shxzskj.cn

[T55] Scala：集合过滤
来源：http://kz.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lv.wgjwhj.cn

[T56] Scala：样例类
来源：http://wl.newstarts.cn


<!-- 参考信息 -->