代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://sm.huixiangedu.cn

[R48] awk 取指定列
来源：http://vs.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://jc.yuntaijiaju.cn

[R49] awk 带条件
来源：http://lq.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uc.hnjuh.cn

[R50] awk 求和
来源：http://bw.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dk.wgjwhj.cn

[R51] 排序去重取前几
来源：http://qo.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ed.bjjhwx.cn

[R52] 统计行数
来源：http://li.9csxet.cn

wc -l a.txt
来源：http://yx.colortex.cn

[R53] 查看文件头与实时尾
来源：http://mb.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fg.shxzukj.cn

[R54] 比较两个文件
来源：http://gr.huanxung.cn

diff a.txt b.txt
来源：http://iy.jianghongdianzi.cn

[R55] 压缩与解压
来源：http://oi.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gm.bjjhwx.cn

[R56] 远程拷贝
来源：http://pf.chemitech.net.cn

scp file user@host:/path/
来源：http://cl.szxytkj.cn

[R57] 远程执行命令
来源：http://ce.newstarts.cn

ssh user@host 'uptime'
来源：http://lr.wgjwhj.cn

[R58] 下载文件
来源：http://dy.colortex.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vr.asd995.cn

[R59] 发 POST JSON
来源：http://ku.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xp.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://wo.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rm.szsharing.cn

[R61] 磁盘占用
来源：http://yb.hnjuh.cn

df -h;  du -sh *
来源：http://cp.szxytkj.cn

[R62] 找最占空间的文件
来源：http://pf.521024.cn

du -ah . | sort -rh | head -10
来源：http://rw.hahajie.cn

[R63] 内存与进程
来源：http://vw.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://fw.bjjhwx.cn

[R64] 结束进程
来源：http://kz.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://ty.huanxung.cn

[R65] 查看端口占用
来源：http://za.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ds.hahajie.cn

[R66] 定时任务
来源：http://xg.huixiangedu.cn

crontab -e;  crontab -l
来源：http://bu.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://av.hnjuh.cn

openssl rand -hex 16
来源：http://yr.9csxet.cn

[R68] 计算文件校验值
来源：http://kn.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qr.panjiajie.cn

[R69] 生成随机密码
来源：http://oh.9csxet.cn

head -c 16 /dev/urandom | base64
来源：http://cb.lnxyls.cn

[R70] 时间戳与互转
来源：http://uc.huixinmuqiang.cn

date +%s;  date -d @1700000000
来源：http://ao.bjjhwx.cn

[R71] 日期格式化
来源：http://lv.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kj.huanxung.cn

[R72] 等待端口就绪
来源：http://zp.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bz.9csxet.cn

[R73] 分割大日志
来源：http://mb.yuexingan06.cn

split -l 1000 big.log part_
来源：http://xk.gzmigu.cn

[R74] 批量重命名
来源：http://eb.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qw.hnjuh.cn

[R75] 导出环境变量
来源：http://nu.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://gv.nszjky.cn

[R76] 使用临时文件
来源：http://lm.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lq.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://zw.muxihuayi.cn

read -rp "请输入: " ans
来源：http://gj.hahajie.cn

[R78] 交互式菜单
来源：http://hn.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://we.hnjuh.cn

[R79] 解析命令行选项
来源：http://gp.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://co.nszjky.cn

[R80] 查看脚本执行耗时
来源：http://fv.muxihuayi.cn

time ./run.sh
来源：http://bf.wgjwhj.cn

================================================================================
来源：http://qe.shxzukj.cn

S. C / C++ 专题
来源：http://zy.bookmarksfly.cn

================================================================================
来源：http://gg.chemitech.net.cn

[S01] C：Hello World
来源：http://lu.shxzskj.cn

#include <stdio.h>
来源：http://sj.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ro.9csxet.cn

[S02] C：变量与格式化输出
来源：http://lj.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://vg.bookmarksfly.cn

[S03] C：读入整数
来源：http://lq.huanxung.cn

int x; scanf("%d", &x);
来源：http://ho.chemitech.net.cn

[S04] C：字符串复制
来源：http://ab.nicolike.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jf.newstarts.cn

[S05] C：字符串长度
来源：http://ej.newstarts.cn

strlen(s)
来源：http://xr.panjiajie.cn

[S06] C：字符串比较
来源：http://pd.asd995.cn

strcmp(a, b) == 0
来源：http://gw.shxzukj.cn

[S07] C：数组遍历求和
来源：http://or.521024.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nb.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://lg.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lu.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://bn.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ip.wgjwhj.cn

[S10] C：指针与解引用
来源：http://uy.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://nx.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://ib.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://ff.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ai.huixinmuqiang.cn

fclose(f);
来源：http://oj.asd995.cn

[S12] C：写文件
来源：http://ov.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ug.nicolike.cn

[S13] C：宏定义
来源：http://mj.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zq.521024.cn

[S14] C：枚举
来源：http://cr.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://uo.yuntaijiaju.cn

[S15] C：类型转换
来源：http://ff.wgjwhj.cn

(double) a / b
来源：http://rx.szsharing.cn

[S16] C：位操作置位
来源：http://lw.shtwfgs.cn

x |= (1 << 3);
来源：http://om.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://gb.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fe.szxytkj.cn

[S18] C：命令行参数
来源：http://hn.bookmarksfly.cn

int main(int argc, char **argv)
来源：http://hp.muxihuayi.cn

[S19] C：快速排序
来源：http://oi.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://el.shxzukj.cn

[S20] C：二分查找
来源：http://ga.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zu.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://gv.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ie.lnxyls.cn

[S22] C：字符串转数字
来源：http://mv.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hk.bjjhwx.cn

[S23] C：随机数
来源：http://kh.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jn.nicolike.cn

[S24] C：获取本地时间
来源：http://fa.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tt.shxzukj.cn

[S25] C：内存拷贝
来源：http://cj.gzmigu.cn

memcpy(dst, src, n);
来源：http://ml.nszjky.cn

[S26] C：内存清零
来源：http://ir.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://xk.hnjuh.cn

[S27] C：定义常量
来源：http://rt.shxzukj.cn

const double PI = 3.14159;
来源：http://kb.bookmarksfly.cn

[S28] C：静态变量
来源：http://ox.haigaiapp.cn

static int counter = 0;
来源：http://xv.hahajie.cn

[S29] C：变参函数
来源：http://ab.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kn.asd995.cn

[S30] C：头文件保护
来源：http://gb.yuntaijiaju.cn

#ifndef X_H
来源：http://dd.newstarts.cn

#define X_H
来源：http://ao.hnjuh.cn

#endif
来源：http://ii.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://ro.newstarts.cn

#include <iostream>
来源：http://cg.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://uz.521024.cn

[S32] C++：字符串
来源：http://lh.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://yf.asd995.cn

[S33] C++：vector 增删
来源：http://ij.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dm.newstarts.cn

[S34] C++：遍历 vector
来源：http://ik.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://vi.chemitech.net.cn

[S35] C++：map
来源：http://xl.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fe.hnjuh.cn

[S36] C++：unordered_map
来源：http://ek.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pm.szsharing.cn

[S37] C++：set
来源：http://nl.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ug.huixinmuqiang.cn

[S38] C++：排序
来源：http://uk.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://wj.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://wp.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ck.gzmigu.cn

[S40] C++：查找元素
来源：http://wf.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ub.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://gk.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://av.newstarts.cn

[S42] C++：继承与虚函数
来源：http://pg.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://ya.gzmigu.cn

[S43] C++：智能指针
来源：http://tl.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://np.shxzskj.cn

[S44] C++：引用传参
来源：http://xf.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://se.szxytkj.cn

[S45] C++：lambda
来源：http://th.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://av.panjiajie.cn

[S46] C++：函数模板
来源：http://nq.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hs.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://yd.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qz.huanxung.cn

[S48] C++：逐行读文件
来源：http://dw.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tc.asd995.cn

while (std::getline(in, line)) { }
来源：http://kg.gzmigu.cn

[S49] C++：写文件
来源：http://gi.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pl.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://gm.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xb.panjiajie.cn

[S51] C++：显式类型转换
来源：http://do.asd995.cn

static_cast<double>(a) / b
来源：http://zl.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://qi.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://ts.lnxyls.cn

[S53] C++：移动语义
来源：http://ez.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://np.asd995.cn

[S54] C++：异常处理
来源：http://ze.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://az.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://kn.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://se.szsharing.cn

[S56] C++：optional
来源：http://xe.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ex.bjjhwx.cn

[S57] C++：编译期常量
来源：http://nt.hnjuh.cn

constexpr int N = 10;
来源：http://cg.shxzukj.cn

[S58] C++：命名空间
来源：http://wk.jianghongdianzi.cn

namespace ns { int f() { return 1; } }
来源：http://zv.jctech888.com.cn

[S59] C++：静态断言
来源：http://cp.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tr.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://sb.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bp.jianghongdianzi.cn

================================================================================
来源：http://jp.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cy.9csxet.cn

================================================================================
来源：http://ft.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://vy.huixiangedu.cn

println("Hello")
来源：http://iv.huanxung.cn

[T02] Kotlin：变量
来源：http://rx.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://aw.jianghongdianzi.cn

[T03] Kotlin：字符串模板
来源：http://ni.shxzukj.cn

"值: $b"
来源：http://zu.shxzukj.cn

[T04] Kotlin：空安全
来源：http://qb.colortex.cn

val n: String? = null;  n?.length
来源：http://qi.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://ws.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ht.huanxung.cn

[T06] Kotlin：集合映射
来源：http://bw.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ev.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://zf.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kz.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://lt.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://xt.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://fy.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://go.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://up.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vr.asd995.cn

[T11] Kotlin：协程
来源：http://yk.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ka.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://db.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://um.jctech888.com.cn

[T13] Kotlin：只读 Map
来源：http://ly.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://de.9csxet.cn

[T14] Kotlin：循环
来源：http://jz.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://ax.bjjhwx.cn

[T15] Kotlin：接口
来源：http://af.huanxung.cn

interface Shape { fun area(): Double }
来源：http://uj.yuntaijiaju.cn

[T16] Swift：Hello World
来源：http://be.lnxyls.cn

print("Hello")
来源：http://ro.gzmigu.cn

[T17] Swift：变量与常量
来源：http://ep.hnjuh.cn

var a = 1;  let b = 2
来源：http://od.colortex.cn

[T18] Swift：字符串插值
来源：http://ob.nszjky.cn

"值: \(b)"
来源：http://rn.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://qu.shxzukj.cn

if let n = opt { print(n) }
来源：http://hc.huixiangedu.cn

[T20] Swift：数组操作
来源：http://zz.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dc.bjjhwx.cn

[T21] Swift：遍历
来源：http://hk.wgjwhj.cn

for x in a { print(x) }
来源：http://fb.huanxung.cn

[T22] Swift：字典
来源：http://ow.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dg.panjiajie.cn

[T23] Swift：函数
来源：http://ab.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fb.lnxyls.cn

[T24] Swift：闭包
来源：http://si.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sw.bookmarksfly.cn

[T25] Swift：结构体
来源：http://yc.colortex.cn

struct P { var x: Int }
来源：http://nm.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://gg.huanxung.cn

class A: Base { override func f() {} }
来源：http://kb.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://az.newstarts.cn

do { try f() } catch { print(error) }
来源：http://cq.bookmarksfly.cn

[T28] Swift：枚举
来源：http://yf.shxzukj.cn

enum Color { case red, green }
来源：http://oj.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://ur.asd995.cn

guard let x = opt else { return }
来源：http://as.bjjhwx.cn

[T30] Swift：协议
来源：http://ad.colortex.cn

protocol Shape { func area() -> Double }
来源：http://qd.nicolike.cn

[T31] Lua：Hello World
来源：http://uo.wgjwhj.cn

print("Hello")
来源：http://et.nicolike.cn

[T32] Lua：局部变量
来源：http://gg.huanxung.cn

local a = 1
来源：http://th.colortex.cn

[T33] Lua：表（数组）
来源：http://ok.chemitech.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qh.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://zr.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tb.hahajie.cn

[T35] Lua：字典表
来源：http://qa.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://sh.colortex.cn

[T36] Lua：函数
来源：http://zq.hahajie.cn

function add(a, b) return a + b end
来源：http://ug.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://ns.szxytkj.cn

"a" .. "b"
来源：http://yp.hnjuh.cn

[T38] Lua：条件
来源：http://oo.521024.cn

if x > 0 then print("正") end
来源：http://ow.hahajie.cn

[T39] Lua：模式匹配
来源：http://io.bjjhwx.cn

string.find(s, "%d+")
来源：http://ar.yuexingan06.cn

[T40] Lua：元表
来源：http://oc.hahajie.cn

setmetatable({}, { __index = base })
来源：http://af.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://uw.nszjky.cn

print "Hello\n";
来源：http://rc.bjjhwx.cn

[T42] Perl：变量类型
来源：http://vj.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nf.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://ms.wgjwhj.cn

"值: $a"
来源：http://id.521024.cn

[T44] Perl：条件
来源：http://et.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://ku.9csxet.cn

[T45] Perl：数组遍历
来源：http://vd.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://ct.huanxung.cn

[T46] Perl：哈希操作
来源：http://kw.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ba.521024.cn

[T47] Perl：正则捕获
来源：http://pp.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ss.lnxyls.cn

[T48] Perl：正则替换
来源：http://xm.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://ql.colortex.cn

[T49] Perl：函数
来源：http://hm.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kc.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://ki.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zv.nicolike.cn


<!-- 参考信息 -->