代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dx.nszjky.cn

[R54] 比较两个文件
来源：http://ih.newstarts.cn

diff a.txt b.txt
来源：http://vm.9csxet.cn

[R55] 压缩与解压
来源：http://th.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uq.haigaiapp.cn

[R56] 远程拷贝
来源：http://qw.yuntaijiaju.cn

scp file user@host:/path/
来源：http://np.huanxung.cn

[R57] 远程执行命令
来源：http://qh.yuexingan06.cn

ssh user@host 'uptime'
来源：http://iq.huixiangedu.cn

[R58] 下载文件
来源：http://ot.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ni.lnxyls.cn

[R59] 发 POST JSON
来源：http://ak.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hw.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://fg.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://so.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://lv.huixinmuqiang.cn

df -h;  du -sh *
来源：http://tb.shxzukj.cn

[R62] 找最占空间的文件
来源：http://zz.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://rl.nszjky.cn

[R63] 内存与进程
来源：http://za.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://bj.hahajie.cn

[R64] 结束进程
来源：http://ja.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://vj.haigaiapp.cn

[R65] 查看端口占用
来源：http://jv.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xf.panjiajie.cn

[R66] 定时任务
来源：http://vk.gzmigu.cn

crontab -e;  crontab -l
来源：http://zr.haigaiapp.cn

[R67] 生成随机十六进制串
来源：http://mv.szsharing.cn

openssl rand -hex 16
来源：http://gr.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://fa.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uq.shxzskj.cn

[R69] 生成随机密码
来源：http://vd.huixinmuqiang.cn

head -c 16 /dev/urandom | base64
来源：http://bz.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://bc.nicolike.cn

date +%s;  date -d @1700000000
来源：http://pb.hahajie.cn

[R71] 日期格式化
来源：http://bo.bjjhwx.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rq.panjiajie.cn

[R72] 等待端口就绪
来源：http://ol.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://az.lnxyls.cn

[R73] 分割大日志
来源：http://nc.newstarts.cn

split -l 1000 big.log part_
来源：http://fl.panjiajie.cn

[R74] 批量重命名
来源：http://cl.shxzskj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rc.yuexingan06.cn

[R75] 导出环境变量
来源：http://zp.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://ml.haigaiapp.cn

[R76] 使用临时文件
来源：http://if.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kp.9csxet.cn

[R77] 读取用户输入
来源：http://qh.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://mn.bookmarksfly.cn

[R78] 交互式菜单
来源：http://fw.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sw.nszjky.cn

[R79] 解析命令行选项
来源：http://mz.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ug.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://ib.wgjwhj.cn

time ./run.sh
来源：http://qk.huixinmuqiang.cn

================================================================================
来源：http://qj.yuntaijiaju.cn

S. C / C++ 专题
来源：http://zr.shxzukj.cn

================================================================================
来源：http://yi.hahajie.cn

[S01] C：Hello World
来源：http://fi.jianghongdianzi.cn

#include <stdio.h>
来源：http://sb.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cw.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://mx.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://dm.nszjky.cn

[S03] C：读入整数
来源：http://ef.haigaiapp.cn

int x; scanf("%d", &x);
来源：http://fm.shtwfgs.cn

[S04] C：字符串复制
来源：http://yx.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zz.bookmarksfly.cn

[S05] C：字符串长度
来源：http://ct.colortex.cn

strlen(s)
来源：http://rw.newstarts.cn

[S06] C：字符串比较
来源：http://gu.yuexingan06.cn

strcmp(a, b) == 0
来源：http://jr.nicolike.cn

[S07] C：数组遍历求和
来源：http://pi.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ey.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://jz.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uz.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://sw.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ep.9csxet.cn

[S10] C：指针与解引用
来源：http://yv.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://xm.muxihuayi.cn

[S11] C：逐行读文件
来源：http://qi.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://oo.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tr.szxytkj.cn

fclose(f);
来源：http://od.hnjuh.cn

[S12] C：写文件
来源：http://cb.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://op.shxzskj.cn

[S13] C：宏定义
来源：http://oy.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ru.nszjky.cn

[S14] C：枚举
来源：http://sn.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://ty.lnxyls.cn

[S15] C：类型转换
来源：http://kg.szsharing.cn

(double) a / b
来源：http://pv.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://aa.huanxung.cn

x |= (1 << 3);
来源：http://gp.lnxyls.cn

[S17] C：安全拼接字符串
来源：http://qm.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lc.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://fv.shxzukj.cn

int main(int argc, char **argv)
来源：http://mr.jctech888.com.cn

[S19] C：快速排序
来源：http://ym.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zr.huanxung.cn

[S20] C：二分查找
来源：http://sm.9csxet.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://su.szsharing.cn

[S21] C：字符类别判断
来源：http://at.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vd.hnjuh.cn

[S22] C：字符串转数字
来源：http://de.nszjky.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xj.shxzskj.cn

[S23] C：随机数
来源：http://wc.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tn.chemitech.net.cn

[S24] C：获取本地时间
来源：http://zg.521024.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ag.szxytkj.cn

[S25] C：内存拷贝
来源：http://iz.chemitech.net.cn

memcpy(dst, src, n);
来源：http://yf.chemitech.net.cn

[S26] C：内存清零
来源：http://tr.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://if.gzmigu.cn

[S27] C：定义常量
来源：http://pm.huanxung.cn

const double PI = 3.14159;
来源：http://lp.521024.cn

[S28] C：静态变量
来源：http://dx.shxzskj.cn

static int counter = 0;
来源：http://sg.nszjky.cn

[S29] C：变参函数
来源：http://ct.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ta.szsharing.cn

[S30] C：头文件保护
来源：http://hu.521024.cn

#ifndef X_H
来源：http://dl.panjiajie.cn

#define X_H
来源：http://xz.huixiangedu.cn

#endif
来源：http://qs.szsharing.cn

[S31] C++：Hello World
来源：http://ok.huixinmuqiang.cn

#include <iostream>
来源：http://ym.yuexingan06.cn

int main() { std::cout << "Hello\n"; }
来源：http://zj.shxzskj.cn

[S32] C++：字符串
来源：http://hr.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://zt.gzmigu.cn

[S33] C++：vector 增删
来源：http://hf.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://et.shtwfgs.cn

[S34] C++：遍历 vector
来源：http://lz.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://hv.shxzukj.cn

[S35] C++：map
来源：http://fa.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ar.jctech888.com.cn

[S36] C++：unordered_map
来源：http://ep.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://il.bjjhwx.cn

[S37] C++：set
来源：http://oo.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oj.nszjky.cn

[S38] C++：排序
来源：http://ow.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://sb.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://un.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iq.wgjwhj.cn

[S40] C++：查找元素
来源：http://cy.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xf.9csxet.cn

[S41] C++：类与构造函数
来源：http://yf.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xj.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://zr.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://mg.szxytkj.cn

[S43] C++：智能指针
来源：http://tt.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://np.panjiajie.cn

[S44] C++：引用传参
来源：http://wb.colortex.cn

void inc(int &x) { ++x; }
来源：http://ph.nicolike.cn

[S45] C++：lambda
来源：http://er.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ho.muxihuayi.cn

[S46] C++：函数模板
来源：http://lf.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uw.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://ex.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bd.gzmigu.cn

[S48] C++：逐行读文件
来源：http://zp.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jw.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://nq.asd995.cn

[S49] C++：写文件
来源：http://fu.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jq.colortex.cn

[S50] C++：格式化数字
来源：http://iu.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wa.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://eb.9csxet.cn

static_cast<double>(a) / b
来源：http://dk.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://bo.521024.cn

int size() const noexcept { return n_; }
来源：http://xu.gzmigu.cn

[S53] C++：移动语义
来源：http://gv.colortex.cn

std::vector<int> w = std::move(v);
来源：http://tb.521024.cn

[S54] C++：异常处理
来源：http://lc.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yq.lnxyls.cn

[S55] C++：结构化绑定
来源：http://dk.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mo.nszjky.cn

[S56] C++：optional
来源：http://rt.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rg.yuexingan06.cn

[S57] C++：编译期常量
来源：http://ar.colortex.cn

constexpr int N = 10;
来源：http://rt.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://qr.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://fs.shtwfgs.cn

[S59] C++：静态断言
来源：http://cz.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hx.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://mh.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ya.9csxet.cn

================================================================================
来源：http://qx.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yf.szxytkj.cn

================================================================================
来源：http://bw.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://zl.521024.cn

println("Hello")
来源：http://fk.chemitech.net.cn

[T02] Kotlin：变量
来源：http://dc.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fz.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://bt.shxzukj.cn

"值: $b"
来源：http://pd.shxzukj.cn

[T04] Kotlin：空安全
来源：http://gg.panjiajie.cn

val n: String? = null;  n?.length
来源：http://jg.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://ua.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jm.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://ux.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ms.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://as.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://at.jctech888.com.cn

[T08] Kotlin：数据类
来源：http://iv.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://mr.colortex.cn

[T09] Kotlin：扩展函数
来源：http://mw.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://fu.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://py.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ip.gzmigu.cn

[T11] Kotlin：协程
来源：http://lx.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qv.asd995.cn

[T12] Kotlin：解构声明
来源：http://id.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://pt.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://zo.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://da.nszjky.cn

[T14] Kotlin：循环
来源：http://jr.shxzskj.cn

for (i in 1..10) println(i)
来源：http://od.jctech888.com.cn

[T15] Kotlin：接口
来源：http://zs.newstarts.cn

interface Shape { fun area(): Double }
来源：http://vl.colortex.cn

[T16] Swift：Hello World
来源：http://rp.huanxung.cn

print("Hello")
来源：http://cx.hnjuh.cn

[T17] Swift：变量与常量
来源：http://sb.huixinmuqiang.cn

var a = 1;  let b = 2
来源：http://yv.colortex.cn

[T18] Swift：字符串插值
来源：http://sl.yuntaijiaju.cn

"值: \(b)"
来源：http://il.szsharing.cn

[T19] Swift：可选绑定
来源：http://bf.huanxung.cn

if let n = opt { print(n) }
来源：http://xc.jctech888.com.cn

[T20] Swift：数组操作
来源：http://nm.nicolike.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fr.nszjky.cn

[T21] Swift：遍历
来源：http://kk.szxytkj.cn

for x in a { print(x) }
来源：http://rp.panjiajie.cn

[T22] Swift：字典
来源：http://vt.huixinmuqiang.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zi.asd995.cn

[T23] Swift：函数
来源：http://fg.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://na.nicolike.cn

[T24] Swift：闭包
来源：http://vo.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nd.muxihuayi.cn

[T25] Swift：结构体
来源：http://vj.yuexingan06.cn

struct P { var x: Int }
来源：http://vs.newstarts.cn

[T26] Swift：类与重写
来源：http://sz.shxzukj.cn

class A: Base { override func f() {} }
来源：http://bx.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://ik.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://zd.521024.cn

[T28] Swift：枚举
来源：http://sd.huixinmuqiang.cn

enum Color { case red, green }
来源：http://pp.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://bh.szsharing.cn

guard let x = opt else { return }
来源：http://ie.asd995.cn

[T30] Swift：协议
来源：http://wa.colortex.cn

protocol Shape { func area() -> Double }
来源：http://hi.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://xd.newstarts.cn

print("Hello")
来源：http://gu.hahajie.cn

[T32] Lua：局部变量
来源：http://fm.wgjwhj.cn

local a = 1
来源：http://lc.chemitech.net.cn

[T33] Lua：表（数组）
来源：http://sg.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fo.hahajie.cn

[T34] Lua：遍历表
来源：http://la.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fk.shxzukj.cn

[T35] Lua：字典表
来源：http://dy.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://rc.szxytkj.cn

[T36] Lua：函数
来源：http://ia.shtwfgs.cn

function add(a, b) return a + b end
来源：http://hz.yuntaijiaju.cn

[T37] Lua：字符串拼接
来源：http://bc.shxzukj.cn

"a" .. "b"
来源：http://to.shxzskj.cn

[T38] Lua：条件
来源：http://hq.521024.cn

if x > 0 then print("正") end
来源：http://ak.yuexingan06.cn

[T39] Lua：模式匹配
来源：http://li.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://pq.shxzskj.cn

[T40] Lua：元表
来源：http://bz.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://sj.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://pl.lnxyls.cn

print "Hello\n";
来源：http://my.gzmigu.cn

[T42] Perl：变量类型
来源：http://hy.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dx.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://af.newstarts.cn

"值: $a"
来源：http://qx.huixinmuqiang.cn

[T44] Perl：条件
来源：http://wb.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://io.yuntaijiaju.cn

[T45] Perl：数组遍历
来源：http://qf.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://mn.9csxet.cn

[T46] Perl：哈希操作
来源：http://np.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hp.lnxyls.cn

[T47] Perl：正则捕获
来源：http://ao.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nb.haigaiapp.cn

[T48] Perl：正则替换
来源：http://pj.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://bj.szxytkj.cn

[T49] Perl：函数
来源：http://ja.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hx.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://yf.521024.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ze.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ye.jctech888.com.cn

[T51] Scala：Hello World
来源：http://ux.9csxet.cn

println("Hello")
来源：http://xu.muxihuayi.cn

[T52] Scala：变量
来源：http://js.asd995.cn

val a = 1;  var b = 2
来源：http://pe.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://zw.nszjky.cn

s"值: $b"
来源：http://bh.gzmigu.cn

[T54] Scala：集合映射
来源：http://jk.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://xp.asd995.cn

[T55] Scala：集合过滤
来源：http://bg.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dt.wgjwhj.cn

[T56] Scala：样例类
来源：http://sn.jctech888.com.cn


<!-- 参考信息 -->