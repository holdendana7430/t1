代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://sf.panjiajie.cn

[R52] 统计行数
来源：http://jm.panjiajie.cn

wc -l a.txt
来源：http://fp.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://rq.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rl.lnxyls.cn

[R54] 比较两个文件
来源：http://ln.9csxet.cn

diff a.txt b.txt
来源：http://cn.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://ep.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qn.hahajie.cn

[R56] 远程拷贝
来源：http://fu.asd995.cn

scp file user@host:/path/
来源：http://pw.newstarts.cn

[R57] 远程执行命令
来源：http://or.bjjhwx.cn

ssh user@host 'uptime'
来源：http://tb.szxytkj.cn

[R58] 下载文件
来源：http://ly.colortex.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://da.yuexingan06.cn

[R59] 发 POST JSON
来源：http://hb.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ga.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://mh.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jn.huixiangedu.cn

[R61] 磁盘占用
来源：http://vi.hahajie.cn

df -h;  du -sh *
来源：http://rn.colortex.cn

[R62] 找最占空间的文件
来源：http://we.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://ul.jctech888.com.cn

[R63] 内存与进程
来源：http://zo.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://gw.chemitech.net.cn

[R64] 结束进程
来源：http://rk.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://vc.chemitech.net.cn

[R65] 查看端口占用
来源：http://kp.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oy.shxzskj.cn

[R66] 定时任务
来源：http://ns.chemitech.net.cn

crontab -e;  crontab -l
来源：http://na.newstarts.cn

[R67] 生成随机十六进制串
来源：http://lx.hahajie.cn

openssl rand -hex 16
来源：http://qv.lnxyls.cn

[R68] 计算文件校验值
来源：http://fb.huixiangedu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jj.huanxung.cn

[R69] 生成随机密码
来源：http://ad.521024.cn

head -c 16 /dev/urandom | base64
来源：http://zg.nszjky.cn

[R70] 时间戳与互转
来源：http://xa.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://im.gzmigu.cn

[R71] 日期格式化
来源：http://aw.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ae.gzmigu.cn

[R72] 等待端口就绪
来源：http://sr.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://an.nszjky.cn

[R73] 分割大日志
来源：http://fj.9csxet.cn

split -l 1000 big.log part_
来源：http://ua.lnxyls.cn

[R74] 批量重命名
来源：http://oh.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gc.nszjky.cn

[R75] 导出环境变量
来源：http://sx.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://vz.yuexingan06.cn

[R76] 使用临时文件
来源：http://tj.jianghongdianzi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xh.huixiangedu.cn

[R77] 读取用户输入
来源：http://lo.shxzskj.cn

read -rp "请输入: " ans
来源：http://mv.muxihuayi.cn

[R78] 交互式菜单
来源：http://xg.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ma.chemitech.net.cn

[R79] 解析命令行选项
来源：http://zm.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qi.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://hd.nicolike.cn

time ./run.sh
来源：http://jj.bookmarksfly.cn

================================================================================
来源：http://wz.nszjky.cn

S. C / C++ 专题
来源：http://yh.9csxet.cn

================================================================================
来源：http://tn.shxzskj.cn

[S01] C：Hello World
来源：http://rn.bookmarksfly.cn

#include <stdio.h>
来源：http://ls.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://li.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://eg.gzmigu.cn

int a = 10; printf("%d\n", a);
来源：http://zh.shtwfgs.cn

[S03] C：读入整数
来源：http://oy.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://hs.shtwfgs.cn

[S04] C：字符串复制
来源：http://nz.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ii.shtwfgs.cn

[S05] C：字符串长度
来源：http://kb.huixinmuqiang.cn

strlen(s)
来源：http://mt.huixiangedu.cn

[S06] C：字符串比较
来源：http://ie.jctech888.com.cn

strcmp(a, b) == 0
来源：http://nq.newstarts.cn

[S07] C：数组遍历求和
来源：http://wj.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wr.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://nw.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ir.521024.cn

[S09] C：结构体定义与初始化
来源：http://go.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pl.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://ly.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://ux.haigaiapp.cn

[S11] C：逐行读文件
来源：http://ct.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://qp.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bj.bjjhwx.cn

fclose(f);
来源：http://vn.shxzskj.cn

[S12] C：写文件
来源：http://hv.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iy.huixinmuqiang.cn

[S13] C：宏定义
来源：http://ou.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zg.newstarts.cn

[S14] C：枚举
来源：http://wz.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://kb.lnxyls.cn

[S15] C：类型转换
来源：http://rk.haigaiapp.cn

(double) a / b
来源：http://nq.panjiajie.cn

[S16] C：位操作置位
来源：http://hi.gzmigu.cn

x |= (1 << 3);
来源：http://fn.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://op.huixiangedu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gy.9csxet.cn

[S18] C：命令行参数
来源：http://xl.jctech888.com.cn

int main(int argc, char **argv)
来源：http://xx.jianghongdianzi.cn

[S19] C：快速排序
来源：http://fn.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lz.bjjhwx.cn

[S20] C：二分查找
来源：http://xb.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oa.newstarts.cn

[S21] C：字符类别判断
来源：http://sr.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xw.colortex.cn

[S22] C：字符串转数字
来源：http://ze.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://af.nszjky.cn

[S23] C：随机数
来源：http://my.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xy.asd995.cn

[S24] C：获取本地时间
来源：http://pv.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dx.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://pm.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://rx.521024.cn

[S26] C：内存清零
来源：http://jy.newstarts.cn

memset(a, 0, sizeof a);
来源：http://cd.bjjhwx.cn

[S27] C：定义常量
来源：http://mw.nszjky.cn

const double PI = 3.14159;
来源：http://cw.bookmarksfly.cn

[S28] C：静态变量
来源：http://af.wgjwhj.cn

static int counter = 0;
来源：http://sc.nszjky.cn

[S29] C：变参函数
来源：http://my.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cs.huanxung.cn

[S30] C：头文件保护
来源：http://pz.newstarts.cn

#ifndef X_H
来源：http://di.hnjuh.cn

#define X_H
来源：http://ha.chemitech.net.cn

#endif
来源：http://ft.panjiajie.cn

[S31] C++：Hello World
来源：http://xr.panjiajie.cn

#include <iostream>
来源：http://rs.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://vg.9csxet.cn

[S32] C++：字符串
来源：http://ti.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://jd.jctech888.com.cn

[S33] C++：vector 增删
来源：http://mt.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qy.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://ly.szxytkj.cn

for (auto &x : v) { std::cout << x; }
来源：http://lb.nicolike.cn

[S35] C++：map
来源：http://xg.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ir.shxzukj.cn

[S36] C++：unordered_map
来源：http://fd.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ty.bjjhwx.cn

[S37] C++：set
来源：http://iy.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mn.huanxung.cn

[S38] C++：排序
来源：http://ko.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://sd.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://aq.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sd.huanxung.cn

[S40] C++：查找元素
来源：http://xg.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://el.colortex.cn

[S41] C++：类与构造函数
来源：http://bx.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oy.hahajie.cn

[S42] C++：继承与虚函数
来源：http://dv.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://no.szsharing.cn

[S43] C++：智能指针
来源：http://us.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://wn.9csxet.cn

[S44] C++：引用传参
来源：http://wr.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://kq.bjjhwx.cn

[S45] C++：lambda
来源：http://wl.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qv.hnjuh.cn

[S46] C++：函数模板
来源：http://sr.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jj.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://lj.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fn.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://wh.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lm.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://qw.huixinmuqiang.cn

[S49] C++：写文件
来源：http://zp.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xq.newstarts.cn

[S50] C++：格式化数字
来源：http://jm.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aa.colortex.cn

[S51] C++：显式类型转换
来源：http://fh.asd995.cn

static_cast<double>(a) / b
来源：http://zl.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://tv.newstarts.cn

int size() const noexcept { return n_; }
来源：http://cm.yuexingan06.cn

[S53] C++：移动语义
来源：http://uv.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://bk.colortex.cn

[S54] C++：异常处理
来源：http://mt.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://os.gzmigu.cn

[S55] C++：结构化绑定
来源：http://rx.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ki.nszjky.cn

[S56] C++：optional
来源：http://qo.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ge.chemitech.net.cn

[S57] C++：编译期常量
来源：http://iv.bookmarksfly.cn

constexpr int N = 10;
来源：http://es.chemitech.net.cn

[S58] C++：命名空间
来源：http://lb.wgjwhj.cn

namespace ns { int f() { return 1; } }
来源：http://cn.yuexingan06.cn

[S59] C++：静态断言
来源：http://bc.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tu.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://cw.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gh.asd995.cn

================================================================================
来源：http://ga.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ln.newstarts.cn

================================================================================
来源：http://dk.hahajie.cn

[T01] Kotlin：Hello World
来源：http://ng.gzmigu.cn

println("Hello")
来源：http://fw.gzmigu.cn

[T02] Kotlin：变量
来源：http://eh.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ml.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://fw.colortex.cn

"值: $b"
来源：http://ar.nszjky.cn

[T04] Kotlin：空安全
来源：http://wv.gzmigu.cn

val n: String? = null;  n?.length
来源：http://in.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://uc.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hc.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://kf.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ia.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://oa.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ro.9csxet.cn

[T08] Kotlin：数据类
来源：http://lc.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://ps.bjjhwx.cn

[T09] Kotlin：扩展函数
来源：http://vh.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://zl.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://pw.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ni.lnxyls.cn

[T11] Kotlin：协程
来源：http://zi.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://di.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://ls.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://ff.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://gw.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://bt.hahajie.cn

[T14] Kotlin：循环
来源：http://tt.gzmigu.cn

for (i in 1..10) println(i)
来源：http://zq.shtwfgs.cn

[T15] Kotlin：接口
来源：http://gx.huanxung.cn

interface Shape { fun area(): Double }
来源：http://mq.521024.cn

[T16] Swift：Hello World
来源：http://lq.gzmigu.cn

print("Hello")
来源：http://ui.nicolike.cn

[T17] Swift：变量与常量
来源：http://bq.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://gn.asd995.cn

[T18] Swift：字符串插值
来源：http://ng.hnjuh.cn

"值: \(b)"
来源：http://nr.hahajie.cn

[T19] Swift：可选绑定
来源：http://gz.shtwfgs.cn

if let n = opt { print(n) }
来源：http://ed.huixiangedu.cn

[T20] Swift：数组操作
来源：http://qh.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qs.hahajie.cn

[T21] Swift：遍历
来源：http://nz.yuntaijiaju.cn

for x in a { print(x) }
来源：http://fe.szxytkj.cn

[T22] Swift：字典
来源：http://vp.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ce.hnjuh.cn

[T23] Swift：函数
来源：http://xx.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mh.huixiangedu.cn

[T24] Swift：闭包
来源：http://cz.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ml.wgjwhj.cn

[T25] Swift：结构体
来源：http://wt.colortex.cn

struct P { var x: Int }
来源：http://uk.haigaiapp.cn

[T26] Swift：类与重写
来源：http://xd.shxzskj.cn

class A: Base { override func f() {} }
来源：http://in.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://ru.muxihuayi.cn

do { try f() } catch { print(error) }
来源：http://eh.huixiangedu.cn

[T28] Swift：枚举
来源：http://aa.yuntaijiaju.cn

enum Color { case red, green }
来源：http://sl.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://bc.colortex.cn

guard let x = opt else { return }
来源：http://th.yuexingan06.cn

[T30] Swift：协议
来源：http://fp.yuexingan06.cn

protocol Shape { func area() -> Double }
来源：http://ba.newstarts.cn

[T31] Lua：Hello World
来源：http://by.shxzukj.cn

print("Hello")
来源：http://jo.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://nh.bjjhwx.cn

local a = 1
来源：http://yl.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://eg.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fl.haigaiapp.cn

[T34] Lua：遍历表
来源：http://vn.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://en.asd995.cn

[T35] Lua：字典表
来源：http://yq.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://uo.szsharing.cn

[T36] Lua：函数
来源：http://sa.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://zp.huanxung.cn

[T37] Lua：字符串拼接
来源：http://xe.lnxyls.cn

"a" .. "b"
来源：http://zv.muxihuayi.cn

[T38] Lua：条件
来源：http://kc.szsharing.cn

if x > 0 then print("正") end
来源：http://eq.szsharing.cn

[T39] Lua：模式匹配
来源：http://cv.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://ej.bjjhwx.cn

[T40] Lua：元表
来源：http://xf.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://ax.shxzskj.cn

[T41] Perl：Hello World
来源：http://mg.szxytkj.cn

print "Hello\n";
来源：http://ok.hnjuh.cn

[T42] Perl：变量类型
来源：http://tc.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hw.hahajie.cn

[T43] Perl：字符串插值
来源：http://pe.shxzskj.cn

"值: $a"
来源：http://tg.lnxyls.cn

[T44] Perl：条件
来源：http://un.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://qn.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://ab.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://mo.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://fc.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gv.panjiajie.cn

[T47] Perl：正则捕获
来源：http://vq.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vn.huixiangedu.cn

[T48] Perl：正则替换
来源：http://eo.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://wx.yuntaijiaju.cn

[T49] Perl：函数
来源：http://hq.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ff.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://hz.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://eg.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ph.521024.cn

[T51] Scala：Hello World
来源：http://im.colortex.cn

println("Hello")
来源：http://xq.bjjhwx.cn

[T52] Scala：变量
来源：http://cm.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://av.gzmigu.cn

[T53] Scala：字符串插值
来源：http://ib.panjiajie.cn

s"值: $b"
来源：http://hj.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://ao.haigaiapp.cn


<!-- 参考信息 -->