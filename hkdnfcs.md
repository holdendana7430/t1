代发 wailian999

find . -name "*.log" -type f
来源：http://ud.nicolike.cn

[R44] 按修改时间查找
来源：http://hs.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://uw.haigaiapp.cn

[R45] 批量删除
来源：http://la.hnjuh.cn

find . -name "*.tmp" -delete
来源：http://ns.yuexingan06.cn

[R46] 递归替换文件内容
来源：http://ee.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jz.newstarts.cn

[R47] sed 单行替换
来源：http://vt.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kr.nicolike.cn

[R48] awk 取指定列
来源：http://js.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://vc.szxytkj.cn

[R49] awk 带条件
来源：http://mt.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xb.panjiajie.cn

[R50] awk 求和
来源：http://ls.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://to.newstarts.cn

[R51] 排序去重取前几
来源：http://uz.gzmigu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vb.shtwfgs.cn

[R52] 统计行数
来源：http://hy.shtwfgs.cn

wc -l a.txt
来源：http://ry.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://ik.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fe.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://dd.muxihuayi.cn

diff a.txt b.txt
来源：http://ew.9csxet.cn

[R55] 压缩与解压
来源：http://gq.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ng.huixiangedu.cn

[R56] 远程拷贝
来源：http://ob.huixinmuqiang.cn

scp file user@host:/path/
来源：http://vw.9csxet.cn

[R57] 远程执行命令
来源：http://xk.muxihuayi.cn

ssh user@host 'uptime'
来源：http://zx.muxihuayi.cn

[R58] 下载文件
来源：http://sr.jianghongdianzi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xc.gzmigu.cn

[R59] 发 POST JSON
来源：http://hh.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ql.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://on.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ou.huixiangedu.cn

[R61] 磁盘占用
来源：http://vh.nicolike.cn

df -h;  du -sh *
来源：http://xu.shxzskj.cn

[R62] 找最占空间的文件
来源：http://vw.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://vr.muxihuayi.cn

[R63] 内存与进程
来源：http://dd.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://hc.nszjky.cn

[R64] 结束进程
来源：http://ds.muxihuayi.cn

kill -9 $(pgrep -f app.py)
来源：http://ca.bookmarksfly.cn

[R65] 查看端口占用
来源：http://oa.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qg.szxytkj.cn

[R66] 定时任务
来源：http://ey.muxihuayi.cn

crontab -e;  crontab -l
来源：http://tr.521024.cn

[R67] 生成随机十六进制串
来源：http://vl.szsharing.cn

openssl rand -hex 16
来源：http://hn.panjiajie.cn

[R68] 计算文件校验值
来源：http://fz.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vu.shtwfgs.cn

[R69] 生成随机密码
来源：http://uk.521024.cn

head -c 16 /dev/urandom | base64
来源：http://jl.hnjuh.cn

[R70] 时间戳与互转
来源：http://xc.newstarts.cn

date +%s;  date -d @1700000000
来源：http://zn.huixinmuqiang.cn

[R71] 日期格式化
来源：http://if.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cz.asd995.cn

[R72] 等待端口就绪
来源：http://zs.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xh.jianghongdianzi.cn

[R73] 分割大日志
来源：http://iq.yuexingan06.cn

split -l 1000 big.log part_
来源：http://ip.shtwfgs.cn

[R74] 批量重命名
来源：http://oh.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rn.huixiangedu.cn

[R75] 导出环境变量
来源：http://gd.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://ap.hahajie.cn

[R76] 使用临时文件
来源：http://wc.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ws.shxzskj.cn

[R77] 读取用户输入
来源：http://cj.521024.cn

read -rp "请输入: " ans
来源：http://mn.gzmigu.cn

[R78] 交互式菜单
来源：http://oh.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mj.yuexingan06.cn

[R79] 解析命令行选项
来源：http://dd.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hm.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://qy.huanxung.cn

time ./run.sh
来源：http://bm.nicolike.cn

================================================================================
来源：http://kx.9csxet.cn

S. C / C++ 专题
来源：http://gm.colortex.cn

================================================================================
来源：http://ne.yuexingan06.cn

[S01] C：Hello World
来源：http://lh.jctech888.com.cn

#include <stdio.h>
来源：http://gp.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cr.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://ka.panjiajie.cn

int a = 10; printf("%d\n", a);
来源：http://ky.bjjhwx.cn

[S03] C：读入整数
来源：http://wh.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://iz.shxzukj.cn

[S04] C：字符串复制
来源：http://zi.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ds.panjiajie.cn

[S05] C：字符串长度
来源：http://dq.muxihuayi.cn

strlen(s)
来源：http://rm.muxihuayi.cn

[S06] C：字符串比较
来源：http://ql.lnxyls.cn

strcmp(a, b) == 0
来源：http://bt.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://hc.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ad.521024.cn

[S08] C：动态内存分配与释放
来源：http://xh.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://di.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://zv.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bx.newstarts.cn

[S10] C：指针与解引用
来源：http://nz.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://po.huanxung.cn

[S11] C：逐行读文件
来源：http://kw.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://lf.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ey.hahajie.cn

fclose(f);
来源：http://gz.newstarts.cn

[S12] C：写文件
来源：http://bt.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://of.nicolike.cn

[S13] C：宏定义
来源：http://lx.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wm.bjjhwx.cn

[S14] C：枚举
来源：http://on.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://yx.bjjhwx.cn

[S15] C：类型转换
来源：http://jm.szxytkj.cn

(double) a / b
来源：http://vr.huanxung.cn

[S16] C：位操作置位
来源：http://oz.gzmigu.cn

x |= (1 << 3);
来源：http://rn.colortex.cn

[S17] C：安全拼接字符串
来源：http://er.huixiangedu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wp.chemitech.net.cn

[S18] C：命令行参数
来源：http://jk.newstarts.cn

int main(int argc, char **argv)
来源：http://cv.shtwfgs.cn

[S19] C：快速排序
来源：http://rc.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wl.9csxet.cn

[S20] C：二分查找
来源：http://kb.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uu.bookmarksfly.cn

[S21] C：字符类别判断
来源：http://ip.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fo.shxzukj.cn

[S22] C：字符串转数字
来源：http://vp.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tf.shtwfgs.cn

[S23] C：随机数
来源：http://kg.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mx.chemitech.net.cn

[S24] C：获取本地时间
来源：http://oj.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rb.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://xr.colortex.cn

memcpy(dst, src, n);
来源：http://uk.shxzukj.cn

[S26] C：内存清零
来源：http://ga.szsharing.cn

memset(a, 0, sizeof a);
来源：http://gy.shxzukj.cn

[S27] C：定义常量
来源：http://nt.nszjky.cn

const double PI = 3.14159;
来源：http://ag.hahajie.cn

[S28] C：静态变量
来源：http://pz.nicolike.cn

static int counter = 0;
来源：http://xk.yuexingan06.cn

[S29] C：变参函数
来源：http://oq.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tq.nszjky.cn

[S30] C：头文件保护
来源：http://pd.panjiajie.cn

#ifndef X_H
来源：http://zj.lnxyls.cn

#define X_H
来源：http://ho.gzmigu.cn

#endif
来源：http://oq.nicolike.cn

[S31] C++：Hello World
来源：http://dt.colortex.cn

#include <iostream>
来源：http://gs.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://yh.huanxung.cn

[S32] C++：字符串
来源：http://ff.bookmarksfly.cn

std::string s = "hi";  s += "!";
来源：http://zj.huixiangedu.cn

[S33] C++：vector 增删
来源：http://rg.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pg.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://uy.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://uq.colortex.cn

[S35] C++：map
来源：http://kk.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tw.huixiangedu.cn

[S36] C++：unordered_map
来源：http://gk.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lr.huixinmuqiang.cn

[S37] C++：set
来源：http://nc.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uz.newstarts.cn

[S38] C++：排序
来源：http://jt.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://qv.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://xp.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iq.9csxet.cn

[S40] C++：查找元素
来源：http://ev.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://so.huanxung.cn

[S41] C++：类与构造函数
来源：http://vq.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://df.nszjky.cn

[S42] C++：继承与虚函数
来源：http://aq.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://hu.bookmarksfly.cn

[S43] C++：智能指针
来源：http://ba.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://ze.wgjwhj.cn

[S44] C++：引用传参
来源：http://eb.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://ub.9csxet.cn

[S45] C++：lambda
来源：http://vf.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ng.asd995.cn

[S46] C++：函数模板
来源：http://eb.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kx.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://cq.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xt.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://eu.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bz.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://wr.newstarts.cn

[S49] C++：写文件
来源：http://tr.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ig.nicolike.cn

[S50] C++：格式化数字
来源：http://uo.shxzukj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wk.hahajie.cn

[S51] C++：显式类型转换
来源：http://vg.shxzukj.cn

static_cast<double>(a) / b
来源：http://om.521024.cn

[S52] C++：const 与 noexcept
来源：http://qy.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://lp.huanxung.cn

[S53] C++：移动语义
来源：http://jr.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://qt.muxihuayi.cn

[S54] C++：异常处理
来源：http://gq.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uu.huanxung.cn

[S55] C++：结构化绑定
来源：http://mg.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dy.newstarts.cn

[S56] C++：optional
来源：http://un.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yz.gzmigu.cn

[S57] C++：编译期常量
来源：http://dr.shxzukj.cn

constexpr int N = 10;
来源：http://uc.panjiajie.cn

[S58] C++：命名空间
来源：http://uw.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://xr.lnxyls.cn

[S59] C++：静态断言
来源：http://kr.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ir.521024.cn

[S60] C++：遍历并删除元素
来源：http://rt.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://au.nicolike.cn

================================================================================
来源：http://ee.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gs.newstarts.cn

================================================================================
来源：http://cg.asd995.cn

[T01] Kotlin：Hello World
来源：http://rl.haigaiapp.cn

println("Hello")
来源：http://hb.newstarts.cn

[T02] Kotlin：变量
来源：http://xv.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pu.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://ix.jianghongdianzi.cn

"值: $b"
来源：http://gd.hnjuh.cn

[T04] Kotlin：空安全
来源：http://ku.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://qc.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://af.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ou.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://ht.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lp.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://dq.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xb.nszjky.cn

[T08] Kotlin：数据类
来源：http://rl.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://rs.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://um.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://vz.9csxet.cn

[T10] Kotlin：默认参数
来源：http://lp.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pt.haigaiapp.cn

[T11] Kotlin：协程
来源：http://as.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ps.521024.cn

[T12] Kotlin：解构声明
来源：http://iv.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://by.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://qg.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://cu.huixiangedu.cn

[T14] Kotlin：循环
来源：http://ru.lnxyls.cn

for (i in 1..10) println(i)
来源：http://ju.jctech888.com.cn

[T15] Kotlin：接口
来源：http://im.newstarts.cn

interface Shape { fun area(): Double }
来源：http://pk.szxytkj.cn

[T16] Swift：Hello World
来源：http://ek.muxihuayi.cn

print("Hello")
来源：http://zh.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://xb.hnjuh.cn

var a = 1;  let b = 2
来源：http://cf.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://fx.muxihuayi.cn

"值: \(b)"
来源：http://rt.panjiajie.cn

[T19] Swift：可选绑定
来源：http://bp.huanxung.cn

if let n = opt { print(n) }
来源：http://vp.wgjwhj.cn

[T20] Swift：数组操作
来源：http://xp.shxzskj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ll.gzmigu.cn

[T21] Swift：遍历
来源：http://qp.muxihuayi.cn

for x in a { print(x) }
来源：http://gw.szxytkj.cn

[T22] Swift：字典
来源：http://rq.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://no.yuntaijiaju.cn

[T23] Swift：函数
来源：http://xz.nicolike.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ym.huanxung.cn

[T24] Swift：闭包
来源：http://ak.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qa.shxzskj.cn

[T25] Swift：结构体
来源：http://jo.huixinmuqiang.cn

struct P { var x: Int }
来源：http://ok.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://on.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://mb.newstarts.cn

[T27] Swift：错误处理
来源：http://ka.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://sh.panjiajie.cn

[T28] Swift：枚举
来源：http://ip.haigaiapp.cn

enum Color { case red, green }
来源：http://ju.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://tl.hnjuh.cn

guard let x = opt else { return }
来源：http://mr.szsharing.cn

[T30] Swift：协议
来源：http://kg.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://bi.shxzskj.cn

[T31] Lua：Hello World
来源：http://fe.lnxyls.cn

print("Hello")
来源：http://ef.jctech888.com.cn

[T32] Lua：局部变量
来源：http://ij.chemitech.net.cn

local a = 1
来源：http://oi.shxzukj.cn

[T33] Lua：表（数组）
来源：http://lt.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tx.szsharing.cn

[T34] Lua：遍历表
来源：http://yg.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qw.wgjwhj.cn

[T35] Lua：字典表
来源：http://nc.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://ri.shxzukj.cn

[T36] Lua：函数
来源：http://nj.muxihuayi.cn

function add(a, b) return a + b end
来源：http://vj.hahajie.cn

[T37] Lua：字符串拼接
来源：http://he.panjiajie.cn

"a" .. "b"
来源：http://vn.bjjhwx.cn

[T38] Lua：条件
来源：http://yv.hahajie.cn

if x > 0 then print("正") end
来源：http://lx.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://sc.shtwfgs.cn

string.find(s, "%d+")
来源：http://zm.szsharing.cn

[T40] Lua：元表
来源：http://ll.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://ud.jctech888.com.cn

[T41] Perl：Hello World
来源：http://bg.yuntaijiaju.cn

print "Hello\n";
来源：http://lg.colortex.cn

[T42] Perl：变量类型
来源：http://lr.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zt.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://vd.lnxyls.cn

"值: $a"
来源：http://kq.hnjuh.cn

[T44] Perl：条件
来源：http://gl.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://ng.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://eo.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://la.gzmigu.cn

[T46] Perl：哈希操作
来源：http://og.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tr.chemitech.net.cn


<!-- 参考信息 -->