代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://ra.wgjwhj.cn

[R52] 统计行数
来源：http://vm.shxzukj.cn

wc -l a.txt
来源：http://pb.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://yc.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tp.newstarts.cn

[R54] 比较两个文件
来源：http://fy.huixinmuqiang.cn

diff a.txt b.txt
来源：http://sj.jianghongdianzi.cn

[R55] 压缩与解压
来源：http://vf.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lb.hahajie.cn

[R56] 远程拷贝
来源：http://yg.huixinmuqiang.cn

scp file user@host:/path/
来源：http://vq.nicolike.cn

[R57] 远程执行命令
来源：http://wa.panjiajie.cn

ssh user@host 'uptime'
来源：http://fs.gzmigu.cn

[R58] 下载文件
来源：http://pc.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lw.jctech888.com.cn

[R59] 发 POST JSON
来源：http://mt.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ge.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://iw.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qg.9csxet.cn

[R61] 磁盘占用
来源：http://qu.jctech888.com.cn

df -h;  du -sh *
来源：http://fr.colortex.cn

[R62] 找最占空间的文件
来源：http://ka.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://xe.jianghongdianzi.cn

[R63] 内存与进程
来源：http://cq.wgjwhj.cn

free -h;  ps aux | grep nginx
来源：http://wt.huixiangedu.cn

[R64] 结束进程
来源：http://sw.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://qy.jctech888.com.cn

[R65] 查看端口占用
来源：http://mv.shtwfgs.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mc.bjjhwx.cn

[R66] 定时任务
来源：http://yk.haigaiapp.cn

crontab -e;  crontab -l
来源：http://ym.huanxung.cn

[R67] 生成随机十六进制串
来源：http://ap.bookmarksfly.cn

openssl rand -hex 16
来源：http://vk.9csxet.cn

[R68] 计算文件校验值
来源：http://ad.521024.cn

sha256sum a.txt;  md5sum a.txt
来源：http://aw.9csxet.cn

[R69] 生成随机密码
来源：http://lz.hahajie.cn

head -c 16 /dev/urandom | base64
来源：http://ni.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://nj.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://nj.shxzukj.cn

[R71] 日期格式化
来源：http://po.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://oh.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://zn.yuexingan06.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lu.nszjky.cn

[R73] 分割大日志
来源：http://di.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://xt.szxytkj.cn

[R74] 批量重命名
来源：http://gu.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sp.shxzukj.cn

[R75] 导出环境变量
来源：http://wb.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://er.wgjwhj.cn

[R76] 使用临时文件
来源：http://ju.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mj.huanxung.cn

[R77] 读取用户输入
来源：http://qd.521024.cn

read -rp "请输入: " ans
来源：http://vg.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://fw.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ar.521024.cn

[R79] 解析命令行选项
来源：http://gn.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kt.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://bf.shxzukj.cn

time ./run.sh
来源：http://bx.bookmarksfly.cn

================================================================================
来源：http://jm.huixiangedu.cn

S. C / C++ 专题
来源：http://lq.szsharing.cn

================================================================================
来源：http://ru.huixinmuqiang.cn

[S01] C：Hello World
来源：http://jf.hnjuh.cn

#include <stdio.h>
来源：http://ee.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://by.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://nz.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://dd.panjiajie.cn

[S03] C：读入整数
来源：http://rn.haigaiapp.cn

int x; scanf("%d", &x);
来源：http://wh.gzmigu.cn

[S04] C：字符串复制
来源：http://pi.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xd.521024.cn

[S05] C：字符串长度
来源：http://zz.chemitech.net.cn

strlen(s)
来源：http://jm.huixiangedu.cn

[S06] C：字符串比较
来源：http://zy.newstarts.cn

strcmp(a, b) == 0
来源：http://ye.shxzukj.cn

[S07] C：数组遍历求和
来源：http://yo.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kq.gzmigu.cn

[S08] C：动态内存分配与释放
来源：http://kh.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://an.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://rg.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pl.nszjky.cn

[S10] C：指针与解引用
来源：http://xw.9csxet.cn

int *p = &a;  *p = 5;
来源：http://px.colortex.cn

[S11] C：逐行读文件
来源：http://el.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://dz.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gx.nicolike.cn

fclose(f);
来源：http://pc.gzmigu.cn

[S12] C：写文件
来源：http://ma.szxytkj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://np.nicolike.cn

[S13] C：宏定义
来源：http://qy.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oy.shtwfgs.cn

[S14] C：枚举
来源：http://si.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://of.szxytkj.cn

[S15] C：类型转换
来源：http://wj.shxzukj.cn

(double) a / b
来源：http://ua.hahajie.cn

[S16] C：位操作置位
来源：http://vm.newstarts.cn

x |= (1 << 3);
来源：http://wx.colortex.cn

[S17] C：安全拼接字符串
来源：http://cb.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lg.asd995.cn

[S18] C：命令行参数
来源：http://gm.chemitech.net.cn

int main(int argc, char **argv)
来源：http://jd.szsharing.cn

[S19] C：快速排序
来源：http://ai.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://aa.lnxyls.cn

[S20] C：二分查找
来源：http://ni.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jf.newstarts.cn

[S21] C：字符类别判断
来源：http://ed.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fk.9csxet.cn

[S22] C：字符串转数字
来源：http://tk.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rk.gzmigu.cn

[S23] C：随机数
来源：http://ii.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vd.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://hk.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wb.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://bz.newstarts.cn

memcpy(dst, src, n);
来源：http://cy.asd995.cn

[S26] C：内存清零
来源：http://ht.9csxet.cn

memset(a, 0, sizeof a);
来源：http://ga.wgjwhj.cn

[S27] C：定义常量
来源：http://oa.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://nm.szsharing.cn

[S28] C：静态变量
来源：http://ah.jctech888.com.cn

static int counter = 0;
来源：http://ln.wgjwhj.cn

[S29] C：变参函数
来源：http://ye.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fb.wgjwhj.cn

[S30] C：头文件保护
来源：http://ny.wgjwhj.cn

#ifndef X_H
来源：http://bb.nszjky.cn

#define X_H
来源：http://eu.shtwfgs.cn

#endif
来源：http://dg.shxzukj.cn

[S31] C++：Hello World
来源：http://er.newstarts.cn

#include <iostream>
来源：http://lp.huanxung.cn

int main() { std::cout << "Hello\n"; }
来源：http://je.shxzukj.cn

[S32] C++：字符串
来源：http://bw.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://fl.gzmigu.cn

[S33] C++：vector 增删
来源：http://pj.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nb.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://pu.szsharing.cn

for (auto &x : v) { std::cout << x; }
来源：http://tv.jctech888.com.cn

[S35] C++：map
来源：http://tz.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zx.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://nu.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://li.bjjhwx.cn

[S37] C++：set
来源：http://yg.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pj.bjjhwx.cn

[S38] C++：排序
来源：http://sk.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://ry.huixinmuqiang.cn

[S39] C++：自定义比较器排序
来源：http://bx.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vk.shxzukj.cn

[S40] C++：查找元素
来源：http://bx.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sy.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://ex.bookmarksfly.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zh.colortex.cn

[S42] C++：继承与虚函数
来源：http://vt.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://zy.nicolike.cn

[S43] C++：智能指针
来源：http://bh.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://qk.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://ll.hahajie.cn

void inc(int &x) { ++x; }
来源：http://tc.hnjuh.cn

[S45] C++：lambda
来源：http://ca.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bp.shtwfgs.cn

[S46] C++：函数模板
来源：http://as.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xf.yuexingan06.cn

[S47] C++：结构化绑定遍历
来源：http://lm.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jg.hnjuh.cn

[S48] C++：逐行读文件
来源：http://dc.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://di.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://qh.yuexingan06.cn

[S49] C++：写文件
来源：http://pc.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gw.9csxet.cn

[S50] C++：格式化数字
来源：http://gt.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vi.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://rq.hahajie.cn

static_cast<double>(a) / b
来源：http://db.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://ct.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://zc.bjjhwx.cn

[S53] C++：移动语义
来源：http://xi.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://yk.huanxung.cn

[S54] C++：异常处理
来源：http://la.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://al.gzmigu.cn

[S55] C++：结构化绑定
来源：http://dp.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zr.chemitech.net.cn

[S56] C++：optional
来源：http://jt.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nd.wgjwhj.cn

[S57] C++：编译期常量
来源：http://du.shxzskj.cn

constexpr int N = 10;
来源：http://dz.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://vj.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://bu.jctech888.com.cn

[S59] C++：静态断言
来源：http://ln.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bt.asd995.cn

[S60] C++：遍历并删除元素
来源：http://zi.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ld.panjiajie.cn

================================================================================
来源：http://zz.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jg.muxihuayi.cn

================================================================================
来源：http://ej.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://gy.wgjwhj.cn

println("Hello")
来源：http://rx.muxihuayi.cn

[T02] Kotlin：变量
来源：http://ms.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cy.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://sw.newstarts.cn

"值: $b"
来源：http://kx.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://xn.nszjky.cn

val n: String? = null;  n?.length
来源：http://sf.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://ik.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gp.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://pt.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ly.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://yo.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ts.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://qu.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://px.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://sf.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://vm.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://dl.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xj.muxihuayi.cn

[T11] Kotlin：协程
来源：http://lz.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vn.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://ml.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://fh.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://tn.nicolike.cn

val m = mapOf("a" to 1)
来源：http://nc.yuexingan06.cn

[T14] Kotlin：循环
来源：http://mr.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://lj.hahajie.cn

[T15] Kotlin：接口
来源：http://dz.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://no.colortex.cn

[T16] Swift：Hello World
来源：http://hx.huixiangedu.cn

print("Hello")
来源：http://wt.jctech888.com.cn

[T17] Swift：变量与常量
来源：http://um.hahajie.cn

var a = 1;  let b = 2
来源：http://gy.newstarts.cn

[T18] Swift：字符串插值
来源：http://uk.jianghongdianzi.cn

"值: \(b)"
来源：http://vr.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://pi.9csxet.cn

if let n = opt { print(n) }
来源：http://yy.521024.cn

[T20] Swift：数组操作
来源：http://jl.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uy.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://zw.chemitech.net.cn

for x in a { print(x) }
来源：http://xw.asd995.cn

[T22] Swift：字典
来源：http://id.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jc.colortex.cn

[T23] Swift：函数
来源：http://at.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qn.chemitech.net.cn

[T24] Swift：闭包
来源：http://qp.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ox.bjjhwx.cn

[T25] Swift：结构体
来源：http://ss.huanxung.cn

struct P { var x: Int }
来源：http://qa.521024.cn

[T26] Swift：类与重写
来源：http://im.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://rl.lnxyls.cn

[T27] Swift：错误处理
来源：http://vh.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://gj.colortex.cn

[T28] Swift：枚举
来源：http://yq.hahajie.cn

enum Color { case red, green }
来源：http://la.colortex.cn

[T29] Swift：guard 提前返回
来源：http://sr.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://cm.shtwfgs.cn

[T30] Swift：协议
来源：http://nc.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://ct.colortex.cn

[T31] Lua：Hello World
来源：http://si.muxihuayi.cn

print("Hello")
来源：http://gs.wgjwhj.cn

[T32] Lua：局部变量
来源：http://tl.gzmigu.cn

local a = 1
来源：http://uv.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://bo.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hs.szxytkj.cn

[T34] Lua：遍历表
来源：http://vh.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pi.szxytkj.cn

[T35] Lua：字典表
来源：http://ua.colortex.cn

local d = { a = 1 };  d.b = 2
来源：http://my.521024.cn

[T36] Lua：函数
来源：http://ne.muxihuayi.cn

function add(a, b) return a + b end
来源：http://io.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://vr.newstarts.cn

"a" .. "b"
来源：http://yr.asd995.cn

[T38] Lua：条件
来源：http://oj.shxzukj.cn

if x > 0 then print("正") end
来源：http://sz.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://nt.yuexingan06.cn

string.find(s, "%d+")
来源：http://dr.gzmigu.cn

[T40] Lua：元表
来源：http://ro.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://qr.shtwfgs.cn

[T41] Perl：Hello World
来源：http://lo.shxzskj.cn

print "Hello\n";
来源：http://pv.szxytkj.cn

[T42] Perl：变量类型
来源：http://mi.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cf.nszjky.cn

[T43] Perl：字符串插值
来源：http://aj.newstarts.cn

"值: $a"
来源：http://nb.colortex.cn

[T44] Perl：条件
来源：http://ch.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://tk.huanxung.cn

[T45] Perl：数组遍历
来源：http://qd.asd995.cn

for my $x (@arr) { print $x; }
来源：http://lh.panjiajie.cn

[T46] Perl：哈希操作
来源：http://yl.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xb.shxzskj.cn

[T47] Perl：正则捕获
来源：http://zv.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vv.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://lw.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://ph.521024.cn

[T49] Perl：函数
来源：http://kk.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://op.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://xs.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sn.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://oh.newstarts.cn

[T51] Scala：Hello World
来源：http://rl.shtwfgs.cn

println("Hello")
来源：http://tv.bookmarksfly.cn

[T52] Scala：变量
来源：http://of.colortex.cn

val a = 1;  var b = 2
来源：http://gx.huanxung.cn

[T53] Scala：字符串插值
来源：http://od.huixiangedu.cn

s"值: $b"
来源：http://je.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://iv.huanxung.cn


<!-- 参考信息 -->