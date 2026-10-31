代发 wailian999

find . -name "*.tmp" -delete
来源：http://gk.panjiajie.cn

[R46] 递归替换文件内容
来源：http://gl.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gy.haigaiapp.cn

[R47] sed 单行替换
来源：http://pj.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jb.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://db.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://lz.newstarts.cn

[R49] awk 带条件
来源：http://vw.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mi.huixiangedu.cn

[R50] awk 求和
来源：http://wr.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wl.colortex.cn

[R51] 排序去重取前几
来源：http://ou.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ee.panjiajie.cn

[R52] 统计行数
来源：http://rs.9csxet.cn

wc -l a.txt
来源：http://fi.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://fh.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qy.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://eb.hahajie.cn

diff a.txt b.txt
来源：http://iv.huixiangedu.cn

[R55] 压缩与解压
来源：http://sp.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://au.shtwfgs.cn

[R56] 远程拷贝
来源：http://qy.chemitech.net.cn

scp file user@host:/path/
来源：http://li.nicolike.cn

[R57] 远程执行命令
来源：http://fg.bjjhwx.cn

ssh user@host 'uptime'
来源：http://rx.newstarts.cn

[R58] 下载文件
来源：http://em.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vg.shxzskj.cn

[R59] 发 POST JSON
来源：http://pp.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oy.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://sx.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xd.shxzukj.cn

[R61] 磁盘占用
来源：http://si.newstarts.cn

df -h;  du -sh *
来源：http://ry.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://yq.521024.cn

du -ah . | sort -rh | head -10
来源：http://qf.haigaiapp.cn

[R63] 内存与进程
来源：http://uc.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://gi.muxihuayi.cn

[R64] 结束进程
来源：http://se.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://kx.521024.cn

[R65] 查看端口占用
来源：http://am.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ca.huixinmuqiang.cn

[R66] 定时任务
来源：http://lv.panjiajie.cn

crontab -e;  crontab -l
来源：http://tv.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://yv.huixiangedu.cn

openssl rand -hex 16
来源：http://ed.9csxet.cn

[R68] 计算文件校验值
来源：http://ge.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pp.nicolike.cn

[R69] 生成随机密码
来源：http://lt.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://nv.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://tg.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://mn.wgjwhj.cn

[R71] 日期格式化
来源：http://fp.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lf.lnxyls.cn

[R72] 等待端口就绪
来源：http://ft.jianghongdianzi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gn.yuexingan06.cn

[R73] 分割大日志
来源：http://zw.huixiangedu.cn

split -l 1000 big.log part_
来源：http://ha.shxzskj.cn

[R74] 批量重命名
来源：http://av.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wa.bjjhwx.cn

[R75] 导出环境变量
来源：http://kt.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://qs.szsharing.cn

[R76] 使用临时文件
来源：http://jy.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ro.hahajie.cn

[R77] 读取用户输入
来源：http://vn.lnxyls.cn

read -rp "请输入: " ans
来源：http://pc.szxytkj.cn

[R78] 交互式菜单
来源：http://qk.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cg.haigaiapp.cn

[R79] 解析命令行选项
来源：http://pk.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zi.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://oc.haigaiapp.cn

time ./run.sh
来源：http://qy.hahajie.cn

================================================================================
来源：http://ec.panjiajie.cn

S. C / C++ 专题
来源：http://db.hahajie.cn

================================================================================
来源：http://zu.lnxyls.cn

[S01] C：Hello World
来源：http://ac.nicolike.cn

#include <stdio.h>
来源：http://zd.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sw.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://dd.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://bn.szsharing.cn

[S03] C：读入整数
来源：http://lc.newstarts.cn

int x; scanf("%d", &x);
来源：http://bd.hnjuh.cn

[S04] C：字符串复制
来源：http://dz.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ej.shxzskj.cn

[S05] C：字符串长度
来源：http://lz.huixinmuqiang.cn

strlen(s)
来源：http://pw.nszjky.cn

[S06] C：字符串比较
来源：http://xy.haigaiapp.cn

strcmp(a, b) == 0
来源：http://pm.gzmigu.cn

[S07] C：数组遍历求和
来源：http://um.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ny.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://ws.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iu.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://on.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ha.chemitech.net.cn

[S10] C：指针与解引用
来源：http://dx.szsharing.cn

int *p = &a;  *p = 5;
来源：http://xw.521024.cn

[S11] C：逐行读文件
来源：http://md.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://ed.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tl.yuntaijiaju.cn

fclose(f);
来源：http://uo.wgjwhj.cn

[S12] C：写文件
来源：http://hp.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qt.bjjhwx.cn

[S13] C：宏定义
来源：http://rx.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ah.haigaiapp.cn

[S14] C：枚举
来源：http://vp.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://jn.haigaiapp.cn

[S15] C：类型转换
来源：http://ud.chemitech.net.cn

(double) a / b
来源：http://qs.wgjwhj.cn

[S16] C：位操作置位
来源：http://iy.shxzukj.cn

x |= (1 << 3);
来源：http://dc.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://ht.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yo.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://lz.newstarts.cn

int main(int argc, char **argv)
来源：http://ku.bookmarksfly.cn

[S19] C：快速排序
来源：http://qz.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wz.huixiangedu.cn

[S20] C：二分查找
来源：http://rv.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qt.nicolike.cn

[S21] C：字符类别判断
来源：http://ie.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ty.wgjwhj.cn

[S22] C：字符串转数字
来源：http://bu.nszjky.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ap.chemitech.net.cn

[S23] C：随机数
来源：http://cn.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bl.wgjwhj.cn

[S24] C：获取本地时间
来源：http://lj.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://df.huixiangedu.cn

[S25] C：内存拷贝
来源：http://cb.newstarts.cn

memcpy(dst, src, n);
来源：http://zm.chemitech.net.cn

[S26] C：内存清零
来源：http://sk.521024.cn

memset(a, 0, sizeof a);
来源：http://fg.huixinmuqiang.cn

[S27] C：定义常量
来源：http://bz.521024.cn

const double PI = 3.14159;
来源：http://du.huixinmuqiang.cn

[S28] C：静态变量
来源：http://lk.shxzskj.cn

static int counter = 0;
来源：http://kc.panjiajie.cn

[S29] C：变参函数
来源：http://gz.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cu.yuexingan06.cn

[S30] C：头文件保护
来源：http://jm.chemitech.net.cn

#ifndef X_H
来源：http://nt.huanxung.cn

#define X_H
来源：http://ag.chemitech.net.cn

#endif
来源：http://wp.haigaiapp.cn

[S31] C++：Hello World
来源：http://ji.lnxyls.cn

#include <iostream>
来源：http://fg.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://fk.nszjky.cn

[S32] C++：字符串
来源：http://tb.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://xo.newstarts.cn

[S33] C++：vector 增删
来源：http://fe.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ex.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://oz.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://pi.szxytkj.cn

[S35] C++：map
来源：http://me.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lj.nszjky.cn

[S36] C++：unordered_map
来源：http://cy.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iu.huixiangedu.cn

[S37] C++：set
来源：http://ue.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qz.huixinmuqiang.cn

[S38] C++：排序
来源：http://zo.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://ny.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://eo.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wb.newstarts.cn

[S40] C++：查找元素
来源：http://ft.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nu.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://qi.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ac.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://cr.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://xr.hnjuh.cn

[S43] C++：智能指针
来源：http://rk.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://kg.szsharing.cn

[S44] C++：引用传参
来源：http://hi.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://tf.chemitech.net.cn

[S45] C++：lambda
来源：http://mr.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dt.gzmigu.cn

[S46] C++：函数模板
来源：http://lh.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mt.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://ny.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xf.szxytkj.cn

[S48] C++：逐行读文件
来源：http://sv.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ou.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://te.newstarts.cn

[S49] C++：写文件
来源：http://nc.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wr.wgjwhj.cn

[S50] C++：格式化数字
来源：http://ot.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fh.colortex.cn

[S51] C++：显式类型转换
来源：http://zd.yuexingan06.cn

static_cast<double>(a) / b
来源：http://lh.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://eb.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://zw.muxihuayi.cn

[S53] C++：移动语义
来源：http://br.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://ah.chemitech.net.cn

[S54] C++：异常处理
来源：http://lo.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bp.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://mw.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ao.newstarts.cn

[S56] C++：optional
来源：http://sv.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tn.521024.cn

[S57] C++：编译期常量
来源：http://qk.szxytkj.cn

constexpr int N = 10;
来源：http://zw.huanxung.cn

[S58] C++：命名空间
来源：http://qd.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://ql.huanxung.cn

[S59] C++：静态断言
来源：http://qz.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jy.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://ob.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jc.szsharing.cn

================================================================================
来源：http://zh.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lt.chemitech.net.cn

================================================================================
来源：http://yo.nszjky.cn

[T01] Kotlin：Hello World
来源：http://ua.yuntaijiaju.cn

println("Hello")
来源：http://db.nicolike.cn

[T02] Kotlin：变量
来源：http://vs.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://az.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://br.panjiajie.cn

"值: $b"
来源：http://ig.9csxet.cn

[T04] Kotlin：空安全
来源：http://fa.9csxet.cn

val n: String? = null;  n?.length
来源：http://mt.9csxet.cn

[T05] Kotlin：when 表达式
来源：http://uv.panjiajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cv.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://pl.shtwfgs.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://im.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://dj.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hn.panjiajie.cn

[T08] Kotlin：数据类
来源：http://ua.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://kb.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://rt.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://ph.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://po.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gn.gzmigu.cn

[T11] Kotlin：协程
来源：http://ae.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://om.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://uv.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://wm.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://eo.521024.cn

val m = mapOf("a" to 1)
来源：http://gp.9csxet.cn

[T14] Kotlin：循环
来源：http://oz.newstarts.cn

for (i in 1..10) println(i)
来源：http://jl.521024.cn

[T15] Kotlin：接口
来源：http://en.bjjhwx.cn

interface Shape { fun area(): Double }
来源：http://yq.521024.cn

[T16] Swift：Hello World
来源：http://pj.hahajie.cn

print("Hello")
来源：http://io.szxytkj.cn

[T17] Swift：变量与常量
来源：http://hj.asd995.cn

var a = 1;  let b = 2
来源：http://oi.lnxyls.cn

[T18] Swift：字符串插值
来源：http://xz.nicolike.cn

"值: \(b)"
来源：http://ng.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://er.huixiangedu.cn

if let n = opt { print(n) }
来源：http://cw.haigaiapp.cn

[T20] Swift：数组操作
来源：http://ai.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ho.gzmigu.cn

[T21] Swift：遍历
来源：http://gt.shxzukj.cn

for x in a { print(x) }
来源：http://qn.newstarts.cn

[T22] Swift：字典
来源：http://xr.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://us.jianghongdianzi.cn

[T23] Swift：函数
来源：http://qh.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://un.shxzukj.cn

[T24] Swift：闭包
来源：http://iv.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wz.huixiangedu.cn

[T25] Swift：结构体
来源：http://ue.shtwfgs.cn

struct P { var x: Int }
来源：http://fp.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://wh.9csxet.cn

class A: Base { override func f() {} }
来源：http://zj.haigaiapp.cn

[T27] Swift：错误处理
来源：http://ws.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://kd.shtwfgs.cn

[T28] Swift：枚举
来源：http://py.gzmigu.cn

enum Color { case red, green }
来源：http://by.nszjky.cn

[T29] Swift：guard 提前返回
来源：http://vh.shxzukj.cn

guard let x = opt else { return }
来源：http://bi.lnxyls.cn

[T30] Swift：协议
来源：http://xp.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://iu.wgjwhj.cn

[T31] Lua：Hello World
来源：http://qt.nicolike.cn

print("Hello")
来源：http://dm.lnxyls.cn

[T32] Lua：局部变量
来源：http://zl.9csxet.cn

local a = 1
来源：http://as.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://oo.yuntaijiaju.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ln.huanxung.cn

[T34] Lua：遍历表
来源：http://ng.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qg.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://ny.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://fu.szsharing.cn

[T36] Lua：函数
来源：http://ft.nszjky.cn

function add(a, b) return a + b end
来源：http://ht.szsharing.cn

[T37] Lua：字符串拼接
来源：http://qo.hahajie.cn

"a" .. "b"
来源：http://yx.haigaiapp.cn

[T38] Lua：条件
来源：http://fz.colortex.cn

if x > 0 then print("正") end
来源：http://ox.szsharing.cn

[T39] Lua：模式匹配
来源：http://rm.hnjuh.cn

string.find(s, "%d+")
来源：http://wr.huixinmuqiang.cn

[T40] Lua：元表
来源：http://op.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://hd.muxihuayi.cn

[T41] Perl：Hello World
来源：http://er.nszjky.cn

print "Hello\n";
来源：http://nt.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://vz.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zm.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://li.shxzskj.cn

"值: $a"
来源：http://ew.shxzskj.cn

[T44] Perl：条件
来源：http://it.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://jh.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://tp.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://sq.colortex.cn

[T46] Perl：哈希操作
来源：http://uu.jctech888.com.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ie.shxzukj.cn

[T47] Perl：正则捕获
来源：http://kf.jianghongdianzi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://an.shtwfgs.cn

[T48] Perl：正则替换
来源：http://rb.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://ze.colortex.cn


<!-- 参考信息 -->