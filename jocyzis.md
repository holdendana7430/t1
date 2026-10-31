代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://in.bookmarksfly.cn

[R50] awk 求和
来源：http://oe.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://oy.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://ml.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://uz.jianghongdianzi.cn

[R52] 统计行数
来源：http://eg.jianghongdianzi.cn

wc -l a.txt
来源：http://mt.hahajie.cn

[R53] 查看文件头与实时尾
来源：http://rb.colortex.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tf.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://lr.huixinmuqiang.cn

diff a.txt b.txt
来源：http://hy.bjjhwx.cn

[R55] 压缩与解压
来源：http://wo.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ns.wgjwhj.cn

[R56] 远程拷贝
来源：http://aq.jianghongdianzi.cn

scp file user@host:/path/
来源：http://qt.szsharing.cn

[R57] 远程执行命令
来源：http://ny.shxzukj.cn

ssh user@host 'uptime'
来源：http://jn.lnxyls.cn

[R58] 下载文件
来源：http://kb.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mj.yuntaijiaju.cn

[R59] 发 POST JSON
来源：http://xo.szxytkj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rk.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://jt.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ip.jctech888.com.cn

[R61] 磁盘占用
来源：http://kk.jianghongdianzi.cn

df -h;  du -sh *
来源：http://el.9csxet.cn

[R62] 找最占空间的文件
来源：http://ra.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://te.huixiangedu.cn

[R63] 内存与进程
来源：http://ca.wgjwhj.cn

free -h;  ps aux | grep nginx
来源：http://un.9csxet.cn

[R64] 结束进程
来源：http://sz.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://jn.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://nx.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yk.gzmigu.cn

[R66] 定时任务
来源：http://gr.shtwfgs.cn

crontab -e;  crontab -l
来源：http://ih.jctech888.com.cn

[R67] 生成随机十六进制串
来源：http://nd.jianghongdianzi.cn

openssl rand -hex 16
来源：http://kp.colortex.cn

[R68] 计算文件校验值
来源：http://tq.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ca.jctech888.com.cn

[R69] 生成随机密码
来源：http://zs.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://ui.szxytkj.cn

[R70] 时间戳与互转
来源：http://aw.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://pb.colortex.cn

[R71] 日期格式化
来源：http://vv.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bz.huixiangedu.cn

[R72] 等待端口就绪
来源：http://jp.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ec.lnxyls.cn

[R73] 分割大日志
来源：http://rb.haigaiapp.cn

split -l 1000 big.log part_
来源：http://ox.muxihuayi.cn

[R74] 批量重命名
来源：http://cy.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jb.muxihuayi.cn

[R75] 导出环境变量
来源：http://ao.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://ad.colortex.cn

[R76] 使用临时文件
来源：http://tp.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mq.9csxet.cn

[R77] 读取用户输入
来源：http://ln.newstarts.cn

read -rp "请输入: " ans
来源：http://rz.gzmigu.cn

[R78] 交互式菜单
来源：http://oz.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lf.huanxung.cn

[R79] 解析命令行选项
来源：http://uw.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gx.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://mi.muxihuayi.cn

time ./run.sh
来源：http://eh.shtwfgs.cn

================================================================================
来源：http://lp.chemitech.net.cn

S. C / C++ 专题
来源：http://sq.newstarts.cn

================================================================================
来源：http://yn.shxzskj.cn

[S01] C：Hello World
来源：http://ut.newstarts.cn

#include <stdio.h>
来源：http://xo.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hh.newstarts.cn

[S02] C：变量与格式化输出
来源：http://hp.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://ad.bookmarksfly.cn

[S03] C：读入整数
来源：http://xy.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://uv.hnjuh.cn

[S04] C：字符串复制
来源：http://st.huixiangedu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ep.gzmigu.cn

[S05] C：字符串长度
来源：http://az.shxzukj.cn

strlen(s)
来源：http://gx.nicolike.cn

[S06] C：字符串比较
来源：http://nq.szxytkj.cn

strcmp(a, b) == 0
来源：http://sb.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://ng.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cd.521024.cn

[S08] C：动态内存分配与释放
来源：http://ji.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://as.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://hg.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xp.szxytkj.cn

[S10] C：指针与解引用
来源：http://ra.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://be.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://hh.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://rj.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bv.bjjhwx.cn

fclose(f);
来源：http://br.huixinmuqiang.cn

[S12] C：写文件
来源：http://vz.hnjuh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xz.hahajie.cn

[S13] C：宏定义
来源：http://tq.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ki.huanxung.cn

[S14] C：枚举
来源：http://gn.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://rn.yuexingan06.cn

[S15] C：类型转换
来源：http://bv.huixinmuqiang.cn

(double) a / b
来源：http://ec.chemitech.net.cn

[S16] C：位操作置位
来源：http://nq.gzmigu.cn

x |= (1 << 3);
来源：http://xv.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://rc.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yj.shtwfgs.cn

[S18] C：命令行参数
来源：http://mu.bjjhwx.cn

int main(int argc, char **argv)
来源：http://zy.colortex.cn

[S19] C：快速排序
来源：http://gf.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zt.huanxung.cn

[S20] C：二分查找
来源：http://wq.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oa.huixiangedu.cn

[S21] C：字符类别判断
来源：http://qo.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gw.huixiangedu.cn

[S22] C：字符串转数字
来源：http://rc.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pi.hahajie.cn

[S23] C：随机数
来源：http://gu.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ch.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://vx.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sy.asd995.cn

[S25] C：内存拷贝
来源：http://db.nicolike.cn

memcpy(dst, src, n);
来源：http://rc.521024.cn

[S26] C：内存清零
来源：http://th.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://ur.shxzukj.cn

[S27] C：定义常量
来源：http://sl.bjjhwx.cn

const double PI = 3.14159;
来源：http://sa.521024.cn

[S28] C：静态变量
来源：http://xr.szxytkj.cn

static int counter = 0;
来源：http://ny.chemitech.net.cn

[S29] C：变参函数
来源：http://qi.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jm.haigaiapp.cn

[S30] C：头文件保护
来源：http://bp.gzmigu.cn

#ifndef X_H
来源：http://nj.hnjuh.cn

#define X_H
来源：http://zz.huanxung.cn

#endif
来源：http://el.szxytkj.cn

[S31] C++：Hello World
来源：http://wc.shxzukj.cn

#include <iostream>
来源：http://ub.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://tg.wgjwhj.cn

[S32] C++：字符串
来源：http://du.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://bt.hahajie.cn

[S33] C++：vector 增删
来源：http://kc.wgjwhj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dj.szsharing.cn

[S34] C++：遍历 vector
来源：http://pi.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://id.yuexingan06.cn

[S35] C++：map
来源：http://bo.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cf.hahajie.cn

[S36] C++：unordered_map
来源：http://ed.9csxet.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xw.521024.cn

[S37] C++：set
来源：http://wg.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://il.hnjuh.cn

[S38] C++：排序
来源：http://tr.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://hy.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://ml.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oq.haigaiapp.cn

[S40] C++：查找元素
来源：http://rc.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lz.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://mo.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://du.huanxung.cn

[S42] C++：继承与虚函数
来源：http://up.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://hr.huixiangedu.cn

[S43] C++：智能指针
来源：http://xm.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://xj.521024.cn

[S44] C++：引用传参
来源：http://ff.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://rr.jctech888.com.cn

[S45] C++：lambda
来源：http://xj.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://du.nicolike.cn

[S46] C++：函数模板
来源：http://kz.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ov.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://wk.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wc.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://vv.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dv.colortex.cn

while (std::getline(in, line)) { }
来源：http://wz.newstarts.cn

[S49] C++：写文件
来源：http://ba.yuexingan06.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sz.szsharing.cn

[S50] C++：格式化数字
来源：http://wv.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ln.szsharing.cn

[S51] C++：显式类型转换
来源：http://oj.haigaiapp.cn

static_cast<double>(a) / b
来源：http://nz.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://ex.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://hc.szxytkj.cn

[S53] C++：移动语义
来源：http://jn.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://lx.nszjky.cn

[S54] C++：异常处理
来源：http://nl.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cm.nszjky.cn

[S55] C++：结构化绑定
来源：http://xk.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://id.wgjwhj.cn

[S56] C++：optional
来源：http://pg.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yq.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://te.9csxet.cn

constexpr int N = 10;
来源：http://di.szxytkj.cn

[S58] C++：命名空间
来源：http://ox.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://sm.9csxet.cn

[S59] C++：静态断言
来源：http://vq.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ss.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://eq.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fj.jianghongdianzi.cn

================================================================================
来源：http://qy.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wa.szsharing.cn

================================================================================
来源：http://pg.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://aw.shxzskj.cn

println("Hello")
来源：http://lt.shxzskj.cn

[T02] Kotlin：变量
来源：http://dv.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xh.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://nc.wgjwhj.cn

"值: $b"
来源：http://to.9csxet.cn

[T04] Kotlin：空安全
来源：http://ww.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://qv.521024.cn

[T05] Kotlin：when 表达式
来源：http://or.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ac.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://sj.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ir.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://bj.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ze.nicolike.cn

[T08] Kotlin：数据类
来源：http://hn.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://nz.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://vi.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://ds.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://dt.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yb.lnxyls.cn

[T11] Kotlin：协程
来源：http://qc.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kd.huanxung.cn

[T12] Kotlin：解构声明
来源：http://zm.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://rf.shxzskj.cn

[T13] Kotlin：只读 Map
来源：http://dz.szsharing.cn

val m = mapOf("a" to 1)
来源：http://jl.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://cl.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://no.huixiangedu.cn

[T15] Kotlin：接口
来源：http://vz.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://am.shtwfgs.cn

[T16] Swift：Hello World
来源：http://ab.wgjwhj.cn

print("Hello")
来源：http://ps.hahajie.cn

[T17] Swift：变量与常量
来源：http://zw.panjiajie.cn

var a = 1;  let b = 2
来源：http://ej.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://eu.szsharing.cn

"值: \(b)"
来源：http://og.asd995.cn

[T19] Swift：可选绑定
来源：http://fs.nicolike.cn

if let n = opt { print(n) }
来源：http://ne.huanxung.cn

[T20] Swift：数组操作
来源：http://al.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oq.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://kg.asd995.cn

for x in a { print(x) }
来源：http://kc.colortex.cn

[T22] Swift：字典
来源：http://ar.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lq.wgjwhj.cn

[T23] Swift：函数
来源：http://cr.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rm.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://fc.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ek.newstarts.cn

[T25] Swift：结构体
来源：http://zk.yuexingan06.cn

struct P { var x: Int }
来源：http://se.nszjky.cn

[T26] Swift：类与重写
来源：http://pn.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://ry.shtwfgs.cn

[T27] Swift：错误处理
来源：http://wz.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://fm.newstarts.cn

[T28] Swift：枚举
来源：http://pl.hnjuh.cn

enum Color { case red, green }
来源：http://gv.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://mr.huixiangedu.cn

guard let x = opt else { return }
来源：http://ax.gzmigu.cn

[T30] Swift：协议
来源：http://ww.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://vu.newstarts.cn

[T31] Lua：Hello World
来源：http://vu.gzmigu.cn

print("Hello")
来源：http://eu.newstarts.cn

[T32] Lua：局部变量
来源：http://lj.szsharing.cn

local a = 1
来源：http://sm.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://fb.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://js.newstarts.cn

[T34] Lua：遍历表
来源：http://mg.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://us.shxzukj.cn

[T35] Lua：字典表
来源：http://it.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://gm.asd995.cn

[T36] Lua：函数
来源：http://ow.yuexingan06.cn

function add(a, b) return a + b end
来源：http://ob.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://xp.shxzukj.cn

"a" .. "b"
来源：http://gb.hahajie.cn

[T38] Lua：条件
来源：http://vu.jctech888.com.cn

if x > 0 then print("正") end
来源：http://xt.szsharing.cn

[T39] Lua：模式匹配
来源：http://zm.muxihuayi.cn

string.find(s, "%d+")
来源：http://bd.shtwfgs.cn

[T40] Lua：元表
来源：http://ql.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://db.yuexingan06.cn

[T41] Perl：Hello World
来源：http://ph.shxzukj.cn

print "Hello\n";
来源：http://eg.asd995.cn

[T42] Perl：变量类型
来源：http://wu.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tp.hnjuh.cn

[T43] Perl：字符串插值
来源：http://pe.jctech888.com.cn

"值: $a"
来源：http://rb.jctech888.com.cn

[T44] Perl：条件
来源：http://xh.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://en.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://wt.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://ah.lnxyls.cn

[T46] Perl：哈希操作
来源：http://bj.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://te.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://jl.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fs.huanxung.cn

[T48] Perl：正则替换
来源：http://ov.hahajie.cn

$s =~ s/old/new/g;
来源：http://gl.shxzskj.cn

[T49] Perl：函数
来源：http://bf.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eh.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://py.asd995.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zl.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://ua.lnxyls.cn

[T51] Scala：Hello World
来源：http://rx.huanxung.cn

println("Hello")
来源：http://wf.shxzskj.cn

[T52] Scala：变量
来源：http://uy.521024.cn


<!-- 参考信息 -->