代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ii.bookmarksfly.cn

[R54] 比较两个文件
来源：http://zc.yuexingan06.cn

diff a.txt b.txt
来源：http://nl.muxihuayi.cn

[R55] 压缩与解压
来源：http://fd.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zi.nicolike.cn

[R56] 远程拷贝
来源：http://vp.yuexingan06.cn

scp file user@host:/path/
来源：http://hu.newstarts.cn

[R57] 远程执行命令
来源：http://rs.yuexingan06.cn

ssh user@host 'uptime'
来源：http://ch.shxzskj.cn

[R58] 下载文件
来源：http://zf.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dz.asd995.cn

[R59] 发 POST JSON
来源：http://ty.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lm.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://hh.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ce.wgjwhj.cn

[R61] 磁盘占用
来源：http://zz.hahajie.cn

df -h;  du -sh *
来源：http://hr.huanxung.cn

[R62] 找最占空间的文件
来源：http://uf.asd995.cn

du -ah . | sort -rh | head -10
来源：http://li.jianghongdianzi.cn

[R63] 内存与进程
来源：http://ib.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://cq.hahajie.cn

[R64] 结束进程
来源：http://kc.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://mt.wgjwhj.cn

[R65] 查看端口占用
来源：http://cx.muxihuayi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wz.9csxet.cn

[R66] 定时任务
来源：http://ym.gzmigu.cn

crontab -e;  crontab -l
来源：http://xs.asd995.cn

[R67] 生成随机十六进制串
来源：http://rh.chemitech.net.cn

openssl rand -hex 16
来源：http://lf.wgjwhj.cn

[R68] 计算文件校验值
来源：http://jk.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cl.bookmarksfly.cn

[R69] 生成随机密码
来源：http://nh.hahajie.cn

head -c 16 /dev/urandom | base64
来源：http://dp.9csxet.cn

[R70] 时间戳与互转
来源：http://am.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://su.yuexingan06.cn

[R71] 日期格式化
来源：http://ua.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rd.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://kf.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sx.bookmarksfly.cn

[R73] 分割大日志
来源：http://uu.asd995.cn

split -l 1000 big.log part_
来源：http://ss.yuntaijiaju.cn

[R74] 批量重命名
来源：http://ex.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ag.521024.cn

[R75] 导出环境变量
来源：http://ct.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://ms.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://he.hahajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xo.chemitech.net.cn

[R77] 读取用户输入
来源：http://mf.huixiangedu.cn

read -rp "请输入: " ans
来源：http://lo.hnjuh.cn

[R78] 交互式菜单
来源：http://ns.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cu.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://yq.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bg.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://jk.nszjky.cn

time ./run.sh
来源：http://pj.szsharing.cn

================================================================================
来源：http://iu.szsharing.cn

S. C / C++ 专题
来源：http://lm.hnjuh.cn

================================================================================
来源：http://cc.hahajie.cn

[S01] C：Hello World
来源：http://em.nszjky.cn

#include <stdio.h>
来源：http://wf.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zx.huanxung.cn

[S02] C：变量与格式化输出
来源：http://bb.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://jy.shxzskj.cn

[S03] C：读入整数
来源：http://zk.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://mz.hnjuh.cn

[S04] C：字符串复制
来源：http://bi.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gu.nszjky.cn

[S05] C：字符串长度
来源：http://nq.muxihuayi.cn

strlen(s)
来源：http://dm.bookmarksfly.cn

[S06] C：字符串比较
来源：http://du.yuexingan06.cn

strcmp(a, b) == 0
来源：http://qf.521024.cn

[S07] C：数组遍历求和
来源：http://xn.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pq.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://nd.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bb.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://mx.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://or.hahajie.cn

[S10] C：指针与解引用
来源：http://bo.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://hn.huixiangedu.cn

[S11] C：逐行读文件
来源：http://km.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://tu.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lh.huanxung.cn

fclose(f);
来源：http://tp.huixinmuqiang.cn

[S12] C：写文件
来源：http://rd.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yz.yuntaijiaju.cn

[S13] C：宏定义
来源：http://ug.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zs.szxytkj.cn

[S14] C：枚举
来源：http://sf.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://zd.bjjhwx.cn

[S15] C：类型转换
来源：http://dq.huixinmuqiang.cn

(double) a / b
来源：http://bs.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://ej.szxytkj.cn

x |= (1 << 3);
来源：http://az.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://zd.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xh.shtwfgs.cn

[S18] C：命令行参数
来源：http://cv.521024.cn

int main(int argc, char **argv)
来源：http://mh.hahajie.cn

[S19] C：快速排序
来源：http://eo.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rv.shxzskj.cn

[S20] C：二分查找
来源：http://ui.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rd.shtwfgs.cn

[S21] C：字符类别判断
来源：http://cy.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xp.huixiangedu.cn

[S22] C：字符串转数字
来源：http://iu.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ke.szxytkj.cn

[S23] C：随机数
来源：http://ya.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rg.muxihuayi.cn

[S24] C：获取本地时间
来源：http://lr.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pz.colortex.cn

[S25] C：内存拷贝
来源：http://jf.shxzskj.cn

memcpy(dst, src, n);
来源：http://ql.nicolike.cn

[S26] C：内存清零
来源：http://xo.asd995.cn

memset(a, 0, sizeof a);
来源：http://ee.huixiangedu.cn

[S27] C：定义常量
来源：http://ya.panjiajie.cn

const double PI = 3.14159;
来源：http://iv.shxzskj.cn

[S28] C：静态变量
来源：http://bj.yuntaijiaju.cn

static int counter = 0;
来源：http://wg.huixiangedu.cn

[S29] C：变参函数
来源：http://qp.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oc.chemitech.net.cn

[S30] C：头文件保护
来源：http://rk.wgjwhj.cn

#ifndef X_H
来源：http://sw.panjiajie.cn

#define X_H
来源：http://gw.newstarts.cn

#endif
来源：http://fz.panjiajie.cn

[S31] C++：Hello World
来源：http://gb.haigaiapp.cn

#include <iostream>
来源：http://hg.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://mc.jctech888.com.cn

[S32] C++：字符串
来源：http://dc.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://hc.nicolike.cn

[S33] C++：vector 增删
来源：http://dd.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dn.nszjky.cn

[S34] C++：遍历 vector
来源：http://yh.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://ma.szxytkj.cn

[S35] C++：map
来源：http://co.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jm.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://vf.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pl.lnxyls.cn

[S37] C++：set
来源：http://ly.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hd.bjjhwx.cn

[S38] C++：排序
来源：http://xe.521024.cn

std::sort(v.begin(), v.end());
来源：http://vd.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://eq.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://se.chemitech.net.cn

[S40] C++：查找元素
来源：http://en.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lw.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://jv.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jv.colortex.cn

[S42] C++：继承与虚函数
来源：http://zd.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://xc.shtwfgs.cn

[S43] C++：智能指针
来源：http://mu.huixinmuqiang.cn

auto p = std::make_unique<int>(5);
来源：http://rb.newstarts.cn

[S44] C++：引用传参
来源：http://ej.asd995.cn

void inc(int &x) { ++x; }
来源：http://ed.asd995.cn

[S45] C++：lambda
来源：http://oa.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ep.huixiangedu.cn

[S46] C++：函数模板
来源：http://uu.shxzukj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uk.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://un.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://km.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://oc.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nc.colortex.cn

while (std::getline(in, line)) { }
来源：http://lt.nicolike.cn

[S49] C++：写文件
来源：http://am.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zv.nszjky.cn

[S50] C++：格式化数字
来源：http://ze.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yx.hnjuh.cn

[S51] C++：显式类型转换
来源：http://gp.asd995.cn

static_cast<double>(a) / b
来源：http://vr.jianghongdianzi.cn

[S52] C++：const 与 noexcept
来源：http://ra.lnxyls.cn

int size() const noexcept { return n_; }
来源：http://mz.shtwfgs.cn

[S53] C++：移动语义
来源：http://kh.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://rq.huixiangedu.cn

[S54] C++：异常处理
来源：http://su.muxihuayi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zu.521024.cn

[S55] C++：结构化绑定
来源：http://eg.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qp.shtwfgs.cn

[S56] C++：optional
来源：http://ik.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wv.hahajie.cn

[S57] C++：编译期常量
来源：http://kw.hnjuh.cn

constexpr int N = 10;
来源：http://fw.shtwfgs.cn

[S58] C++：命名空间
来源：http://mf.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://rx.hahajie.cn

[S59] C++：静态断言
来源：http://jy.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ie.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://ck.huixinmuqiang.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gn.jctech888.com.cn

================================================================================
来源：http://ak.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jg.huanxung.cn

================================================================================
来源：http://sr.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://ke.asd995.cn

println("Hello")
来源：http://nw.haigaiapp.cn

[T02] Kotlin：变量
来源：http://mi.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zt.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://cx.yuexingan06.cn

"值: $b"
来源：http://fc.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://fv.lnxyls.cn

val n: String? = null;  n?.length
来源：http://pt.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://gh.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://id.nicolike.cn

[T06] Kotlin：集合映射
来源：http://ai.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sh.colortex.cn

[T07] Kotlin：集合过滤
来源：http://gk.9csxet.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gs.9csxet.cn

[T08] Kotlin：数据类
来源：http://tz.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://sj.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://zi.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://aa.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://rn.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gc.shxzukj.cn

[T11] Kotlin：协程
来源：http://nw.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mh.newstarts.cn

[T12] Kotlin：解构声明
来源：http://rb.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://lk.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://fm.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://xl.nszjky.cn

[T14] Kotlin：循环
来源：http://nd.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://xh.gzmigu.cn

[T15] Kotlin：接口
来源：http://cf.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://pe.muxihuayi.cn

[T16] Swift：Hello World
来源：http://le.haigaiapp.cn

print("Hello")
来源：http://yb.muxihuayi.cn

[T17] Swift：变量与常量
来源：http://hr.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://ly.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://kg.gzmigu.cn

"值: \(b)"
来源：http://qq.hahajie.cn

[T19] Swift：可选绑定
来源：http://hn.colortex.cn

if let n = opt { print(n) }
来源：http://fj.nszjky.cn

[T20] Swift：数组操作
来源：http://cw.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rp.muxihuayi.cn

[T21] Swift：遍历
来源：http://mu.haigaiapp.cn

for x in a { print(x) }
来源：http://ky.newstarts.cn

[T22] Swift：字典
来源：http://vj.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sf.huixinmuqiang.cn

[T23] Swift：函数
来源：http://rf.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lq.huanxung.cn

[T24] Swift：闭包
来源：http://cu.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pf.huanxung.cn

[T25] Swift：结构体
来源：http://ky.nszjky.cn

struct P { var x: Int }
来源：http://bs.hahajie.cn

[T26] Swift：类与重写
来源：http://aj.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://lh.shxzukj.cn

[T27] Swift：错误处理
来源：http://qa.panjiajie.cn

do { try f() } catch { print(error) }
来源：http://tu.gzmigu.cn

[T28] Swift：枚举
来源：http://mx.jianghongdianzi.cn

enum Color { case red, green }
来源：http://gn.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://kw.hahajie.cn

guard let x = opt else { return }
来源：http://ip.521024.cn

[T30] Swift：协议
来源：http://mg.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://va.bjjhwx.cn

[T31] Lua：Hello World
来源：http://ow.9csxet.cn

print("Hello")
来源：http://ta.szsharing.cn

[T32] Lua：局部变量
来源：http://dm.haigaiapp.cn

local a = 1
来源：http://jm.newstarts.cn

[T33] Lua：表（数组）
来源：http://gy.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dp.muxihuayi.cn

[T34] Lua：遍历表
来源：http://nl.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bc.shxzukj.cn

[T35] Lua：字典表
来源：http://nk.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://ml.hnjuh.cn

[T36] Lua：函数
来源：http://bm.yuexingan06.cn

function add(a, b) return a + b end
来源：http://ks.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://jb.521024.cn

"a" .. "b"
来源：http://iv.nszjky.cn

[T38] Lua：条件
来源：http://cp.newstarts.cn

if x > 0 then print("正") end
来源：http://jq.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://my.shxzukj.cn

string.find(s, "%d+")
来源：http://ru.panjiajie.cn

[T40] Lua：元表
来源：http://hh.nicolike.cn

setmetatable({}, { __index = base })
来源：http://jd.huanxung.cn

[T41] Perl：Hello World
来源：http://hn.muxihuayi.cn

print "Hello\n";
来源：http://kr.newstarts.cn

[T42] Perl：变量类型
来源：http://yb.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://et.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://ja.lnxyls.cn

"值: $a"
来源：http://cp.huixinmuqiang.cn

[T44] Perl：条件
来源：http://ig.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://ky.shxzukj.cn

[T45] Perl：数组遍历
来源：http://ix.colortex.cn

for my $x (@arr) { print $x; }
来源：http://md.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://ru.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qe.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://fq.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zc.shxzskj.cn

[T48] Perl：正则替换
来源：http://uq.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://yp.muxihuayi.cn

[T49] Perl：函数
来源：http://vy.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ia.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://dq.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://da.szsharing.cn

while (my $line = <$fh>) { print $line; }
来源：http://ob.szxytkj.cn

[T51] Scala：Hello World
来源：http://pc.nicolike.cn

println("Hello")
来源：http://ge.jctech888.com.cn

[T52] Scala：变量
来源：http://mg.newstarts.cn

val a = 1;  var b = 2
来源：http://cg.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://bm.wgjwhj.cn

s"值: $b"
来源：http://un.nicolike.cn

[T54] Scala：集合映射
来源：http://wh.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://bl.asd995.cn

[T55] Scala：集合过滤
来源：http://er.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ga.shxzukj.cn

[T56] Scala：样例类
来源：http://ho.nicolike.cn


<!-- 参考信息 -->