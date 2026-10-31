代发 wailian999

find . -name "*.tmp" -delete
来源：http://hb.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://no.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ka.asd995.cn

[R47] sed 单行替换
来源：http://af.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ym.haigaiapp.cn

[R48] awk 取指定列
来源：http://mx.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://ie.newstarts.cn

[R49] awk 带条件
来源：http://so.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aw.szxytkj.cn

[R50] awk 求和
来源：http://wn.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ab.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://nm.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ag.huixiangedu.cn

[R52] 统计行数
来源：http://wy.hnjuh.cn

wc -l a.txt
来源：http://dc.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://fv.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kq.hahajie.cn

[R54] 比较两个文件
来源：http://rt.9csxet.cn

diff a.txt b.txt
来源：http://ry.hahajie.cn

[R55] 压缩与解压
来源：http://rb.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tn.shxzskj.cn

[R56] 远程拷贝
来源：http://zn.szxytkj.cn

scp file user@host:/path/
来源：http://ec.szsharing.cn

[R57] 远程执行命令
来源：http://ys.wgjwhj.cn

ssh user@host 'uptime'
来源：http://jy.yuntaijiaju.cn

[R58] 下载文件
来源：http://mt.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rt.jctech888.com.cn

[R59] 发 POST JSON
来源：http://fk.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tt.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://jd.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hl.nszjky.cn

[R61] 磁盘占用
来源：http://xk.gzmigu.cn

df -h;  du -sh *
来源：http://ql.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://jh.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://pi.newstarts.cn

[R63] 内存与进程
来源：http://wd.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://ps.nicolike.cn

[R64] 结束进程
来源：http://wq.haigaiapp.cn

kill -9 $(pgrep -f app.py)
来源：http://tr.bookmarksfly.cn

[R65] 查看端口占用
来源：http://ez.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pw.huanxung.cn

[R66] 定时任务
来源：http://wg.haigaiapp.cn

crontab -e;  crontab -l
来源：http://vf.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://pj.huixinmuqiang.cn

openssl rand -hex 16
来源：http://be.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://wq.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://eo.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://gl.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://ck.colortex.cn

[R70] 时间戳与互转
来源：http://yv.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://ar.gzmigu.cn

[R71] 日期格式化
来源：http://ip.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ce.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://xi.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://td.hnjuh.cn

[R73] 分割大日志
来源：http://yk.szxytkj.cn

split -l 1000 big.log part_
来源：http://ag.chemitech.net.cn

[R74] 批量重命名
来源：http://im.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yx.panjiajie.cn

[R75] 导出环境变量
来源：http://yc.hnjuh.cn

export PATH="$HOME/bin:$PATH"
来源：http://vo.huixiangedu.cn

[R76] 使用临时文件
来源：http://oy.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eb.panjiajie.cn

[R77] 读取用户输入
来源：http://ff.szxytkj.cn

read -rp "请输入: " ans
来源：http://mv.asd995.cn

[R78] 交互式菜单
来源：http://ya.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fp.shxzukj.cn

[R79] 解析命令行选项
来源：http://bv.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mz.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://ib.9csxet.cn

time ./run.sh
来源：http://ri.shxzukj.cn

================================================================================
来源：http://il.szsharing.cn

S. C / C++ 专题
来源：http://wb.hahajie.cn

================================================================================
来源：http://kc.asd995.cn

[S01] C：Hello World
来源：http://gq.shxzskj.cn

#include <stdio.h>
来源：http://hs.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yq.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://kg.chemitech.net.cn

int a = 10; printf("%d\n", a);
来源：http://zq.szxytkj.cn

[S03] C：读入整数
来源：http://rd.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://oe.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://zz.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yi.hnjuh.cn

[S05] C：字符串长度
来源：http://ds.hnjuh.cn

strlen(s)
来源：http://jm.szsharing.cn

[S06] C：字符串比较
来源：http://fd.nszjky.cn

strcmp(a, b) == 0
来源：http://zh.asd995.cn

[S07] C：数组遍历求和
来源：http://ww.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ph.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://qa.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yb.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://is.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xe.panjiajie.cn

[S10] C：指针与解引用
来源：http://wq.colortex.cn

int *p = &a;  *p = 5;
来源：http://rb.521024.cn

[S11] C：逐行读文件
来源：http://po.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://yn.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qt.hahajie.cn

fclose(f);
来源：http://tu.huixiangedu.cn

[S12] C：写文件
来源：http://dm.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gu.521024.cn

[S13] C：宏定义
来源：http://hj.nicolike.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ky.szsharing.cn

[S14] C：枚举
来源：http://ha.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://xw.panjiajie.cn

[S15] C：类型转换
来源：http://qu.szxytkj.cn

(double) a / b
来源：http://xx.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://co.szxytkj.cn

x |= (1 << 3);
来源：http://us.nszjky.cn

[S17] C：安全拼接字符串
来源：http://ml.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dy.asd995.cn

[S18] C：命令行参数
来源：http://fh.bjjhwx.cn

int main(int argc, char **argv)
来源：http://qv.bjjhwx.cn

[S19] C：快速排序
来源：http://dr.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bf.haigaiapp.cn

[S20] C：二分查找
来源：http://rp.hahajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tb.hahajie.cn

[S21] C：字符类别判断
来源：http://jc.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yr.yuexingan06.cn

[S22] C：字符串转数字
来源：http://rd.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tb.jianghongdianzi.cn

[S23] C：随机数
来源：http://oy.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mu.nszjky.cn

[S24] C：获取本地时间
来源：http://ic.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ut.9csxet.cn

[S25] C：内存拷贝
来源：http://gw.gzmigu.cn

memcpy(dst, src, n);
来源：http://jz.wgjwhj.cn

[S26] C：内存清零
来源：http://sj.hahajie.cn

memset(a, 0, sizeof a);
来源：http://ix.wgjwhj.cn

[S27] C：定义常量
来源：http://zd.nszjky.cn

const double PI = 3.14159;
来源：http://oo.bjjhwx.cn

[S28] C：静态变量
来源：http://fi.jctech888.com.cn

static int counter = 0;
来源：http://gf.yuexingan06.cn

[S29] C：变参函数
来源：http://dh.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hi.huanxung.cn

[S30] C：头文件保护
来源：http://ht.huixinmuqiang.cn

#ifndef X_H
来源：http://ah.szxytkj.cn

#define X_H
来源：http://zz.asd995.cn

#endif
来源：http://if.nicolike.cn

[S31] C++：Hello World
来源：http://pb.huixiangedu.cn

#include <iostream>
来源：http://wx.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://xy.chemitech.net.cn

[S32] C++：字符串
来源：http://gw.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://zu.9csxet.cn

[S33] C++：vector 增删
来源：http://xj.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wu.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://tb.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://bj.9csxet.cn

[S35] C++：map
来源：http://ax.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gy.szsharing.cn

[S36] C++：unordered_map
来源：http://vz.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sb.nszjky.cn

[S37] C++：set
来源：http://qt.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ht.asd995.cn

[S38] C++：排序
来源：http://sq.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://sj.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://dx.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zf.yuexingan06.cn

[S40] C++：查找元素
来源：http://sx.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ci.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://em.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://en.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://pw.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://vm.szxytkj.cn

[S43] C++：智能指针
来源：http://vo.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://xt.9csxet.cn

[S44] C++：引用传参
来源：http://xj.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://vy.jctech888.com.cn

[S45] C++：lambda
来源：http://gg.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jv.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://xy.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yo.wgjwhj.cn

[S47] C++：结构化绑定遍历
来源：http://kb.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ld.521024.cn

[S48] C++：逐行读文件
来源：http://el.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pw.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://pz.gzmigu.cn

[S49] C++：写文件
来源：http://jz.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vv.nszjky.cn

[S50] C++：格式化数字
来源：http://jy.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ps.shxzukj.cn

[S51] C++：显式类型转换
来源：http://cw.jctech888.com.cn

static_cast<double>(a) / b
来源：http://my.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://ww.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://mc.bjjhwx.cn

[S53] C++：移动语义
来源：http://du.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://yt.huanxung.cn

[S54] C++：异常处理
来源：http://fx.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://al.lnxyls.cn

[S55] C++：结构化绑定
来源：http://rd.bjjhwx.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://te.asd995.cn

[S56] C++：optional
来源：http://cg.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pf.9csxet.cn

[S57] C++：编译期常量
来源：http://so.wgjwhj.cn

constexpr int N = 10;
来源：http://ya.shxzukj.cn

[S58] C++：命名空间
来源：http://lb.521024.cn

namespace ns { int f() { return 1; } }
来源：http://ve.gzmigu.cn

[S59] C++：静态断言
来源：http://ra.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ew.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://ji.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lq.9csxet.cn

================================================================================
来源：http://te.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bn.bjjhwx.cn

================================================================================
来源：http://qc.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://fx.shxzukj.cn

println("Hello")
来源：http://it.wgjwhj.cn

[T02] Kotlin：变量
来源：http://ki.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ei.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://bv.panjiajie.cn

"值: $b"
来源：http://wb.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://km.gzmigu.cn

val n: String? = null;  n?.length
来源：http://dt.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://ik.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ye.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://sb.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ha.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://oq.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fl.panjiajie.cn

[T08] Kotlin：数据类
来源：http://ey.521024.cn

data class User(val name: String, val age: Int)
来源：http://yw.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://sl.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://yc.nszjky.cn

[T10] Kotlin：默认参数
来源：http://vo.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jc.asd995.cn

[T11] Kotlin：协程
来源：http://sz.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kr.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://ph.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://dq.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://dr.9csxet.cn

val m = mapOf("a" to 1)
来源：http://xn.lnxyls.cn

[T14] Kotlin：循环
来源：http://xp.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://qb.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://fv.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://of.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://ow.yuexingan06.cn

print("Hello")
来源：http://om.newstarts.cn

[T17] Swift：变量与常量
来源：http://jm.panjiajie.cn

var a = 1;  let b = 2
来源：http://yv.asd995.cn

[T18] Swift：字符串插值
来源：http://cv.colortex.cn

"值: \(b)"
来源：http://fu.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://qt.wgjwhj.cn

if let n = opt { print(n) }
来源：http://ox.lnxyls.cn

[T20] Swift：数组操作
来源：http://nh.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://iu.bjjhwx.cn

[T21] Swift：遍历
来源：http://te.9csxet.cn

for x in a { print(x) }
来源：http://ga.lnxyls.cn

[T22] Swift：字典
来源：http://qd.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bm.jianghongdianzi.cn

[T23] Swift：函数
来源：http://fj.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bj.nszjky.cn

[T24] Swift：闭包
来源：http://fo.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qz.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://mx.asd995.cn

struct P { var x: Int }
来源：http://gz.521024.cn

[T26] Swift：类与重写
来源：http://yd.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://ug.gzmigu.cn

[T27] Swift：错误处理
来源：http://ad.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://jg.chemitech.net.cn

[T28] Swift：枚举
来源：http://ik.newstarts.cn

enum Color { case red, green }
来源：http://se.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://kf.gzmigu.cn

guard let x = opt else { return }
来源：http://np.lnxyls.cn

[T30] Swift：协议
来源：http://ac.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://jz.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://un.jctech888.com.cn

print("Hello")
来源：http://jt.nicolike.cn

[T32] Lua：局部变量
来源：http://xo.jctech888.com.cn

local a = 1
来源：http://as.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://ey.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uy.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://gc.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yi.hahajie.cn

[T35] Lua：字典表
来源：http://rr.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://sr.shtwfgs.cn

[T36] Lua：函数
来源：http://ur.gzmigu.cn

function add(a, b) return a + b end
来源：http://ql.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://kl.muxihuayi.cn

"a" .. "b"
来源：http://ey.szxytkj.cn

[T38] Lua：条件
来源：http://dq.asd995.cn

if x > 0 then print("正") end
来源：http://ju.newstarts.cn

[T39] Lua：模式匹配
来源：http://ci.lnxyls.cn

string.find(s, "%d+")
来源：http://be.newstarts.cn

[T40] Lua：元表
来源：http://ar.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://xq.shxzukj.cn

[T41] Perl：Hello World
来源：http://el.wgjwhj.cn

print "Hello\n";
来源：http://bq.huixiangedu.cn

[T42] Perl：变量类型
来源：http://mb.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ht.szsharing.cn

[T43] Perl：字符串插值
来源：http://pr.jctech888.com.cn

"值: $a"
来源：http://gg.jianghongdianzi.cn

[T44] Perl：条件
来源：http://op.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://cj.nszjky.cn

[T45] Perl：数组遍历
来源：http://zp.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://yv.hahajie.cn

[T46] Perl：哈希操作
来源：http://sk.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xy.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://qf.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ih.hnjuh.cn

[T48] Perl：正则替换
来源：http://iu.colortex.cn

$s =~ s/old/new/g;
来源：http://kh.jctech888.com.cn


<!-- 参考信息 -->