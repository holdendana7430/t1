代发 wailian999

cmd > out.log 2>&1
来源：http://ig.huanxung.cn

[R40] 追加写日志
来源：http://oa.szsharing.cn

echo "log" >> out.log
来源：http://eh.bookmarksfly.cn

[R41] 丢弃输出
来源：http://cf.9csxet.cn

cmd >/dev/null 2>&1
来源：http://qj.521024.cn

[R42] 输入重定向
来源：http://jq.bjjhwx.cn

wc -l < a.txt
来源：http://li.jctech888.com.cn

[R43] 按名字查找文件
来源：http://ta.9csxet.cn

find . -name "*.log" -type f
来源：http://ek.colortex.cn

[R44] 按修改时间查找
来源：http://vv.szxytkj.cn

find . -mtime -7 -type f
来源：http://lp.szsharing.cn

[R45] 批量删除
来源：http://vp.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://he.hahajie.cn

[R46] 递归替换文件内容
来源：http://yq.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yf.jianghongdianzi.cn

[R47] sed 单行替换
来源：http://ca.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fc.shtwfgs.cn

[R48] awk 取指定列
来源：http://ja.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://re.521024.cn

[R49] awk 带条件
来源：http://aa.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://go.szxytkj.cn

[R50] awk 求和
来源：http://og.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://za.nszjky.cn

[R51] 排序去重取前几
来源：http://xo.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ih.wgjwhj.cn

[R52] 统计行数
来源：http://si.jianghongdianzi.cn

wc -l a.txt
来源：http://up.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://bz.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://np.shxzukj.cn

[R54] 比较两个文件
来源：http://zz.hnjuh.cn

diff a.txt b.txt
来源：http://up.hahajie.cn

[R55] 压缩与解压
来源：http://lr.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cf.shxzskj.cn

[R56] 远程拷贝
来源：http://pr.shxzukj.cn

scp file user@host:/path/
来源：http://rt.shxzukj.cn

[R57] 远程执行命令
来源：http://xq.gzmigu.cn

ssh user@host 'uptime'
来源：http://ou.lnxyls.cn

[R58] 下载文件
来源：http://vy.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ym.9csxet.cn

[R59] 发 POST JSON
来源：http://qn.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mz.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://it.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bz.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://oh.yuexingan06.cn

df -h;  du -sh *
来源：http://fo.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://uu.lnxyls.cn

du -ah . | sort -rh | head -10
来源：http://vq.nszjky.cn

[R63] 内存与进程
来源：http://vx.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://ik.panjiajie.cn

[R64] 结束进程
来源：http://dt.muxihuayi.cn

kill -9 $(pgrep -f app.py)
来源：http://en.newstarts.cn

[R65] 查看端口占用
来源：http://gh.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sp.newstarts.cn

[R66] 定时任务
来源：http://hw.hahajie.cn

crontab -e;  crontab -l
来源：http://jy.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://pf.huixiangedu.cn

openssl rand -hex 16
来源：http://ry.521024.cn

[R68] 计算文件校验值
来源：http://rk.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ki.muxihuayi.cn

[R69] 生成随机密码
来源：http://mo.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://ct.shxzskj.cn

[R70] 时间戳与互转
来源：http://ub.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://qs.colortex.cn

[R71] 日期格式化
来源：http://pn.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ct.newstarts.cn

[R72] 等待端口就绪
来源：http://lt.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nu.muxihuayi.cn

[R73] 分割大日志
来源：http://bj.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://hc.huanxung.cn

[R74] 批量重命名
来源：http://tz.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oh.hahajie.cn

[R75] 导出环境变量
来源：http://qz.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://dj.bookmarksfly.cn

[R76] 使用临时文件
来源：http://vz.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qm.szxytkj.cn

[R77] 读取用户输入
来源：http://ku.gzmigu.cn

read -rp "请输入: " ans
来源：http://nt.hnjuh.cn

[R78] 交互式菜单
来源：http://xe.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://of.wgjwhj.cn

[R79] 解析命令行选项
来源：http://vx.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lw.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://sj.chemitech.net.cn

time ./run.sh
来源：http://gd.wgjwhj.cn

================================================================================
来源：http://tj.bjjhwx.cn

S. C / C++ 专题
来源：http://qc.shtwfgs.cn

================================================================================
来源：http://is.shtwfgs.cn

[S01] C：Hello World
来源：http://af.bjjhwx.cn

#include <stdio.h>
来源：http://oy.jianghongdianzi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xj.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://ix.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://lr.jctech888.com.cn

[S03] C：读入整数
来源：http://mj.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://ep.hahajie.cn

[S04] C：字符串复制
来源：http://yp.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bu.colortex.cn

[S05] C：字符串长度
来源：http://bz.gzmigu.cn

strlen(s)
来源：http://lq.bjjhwx.cn

[S06] C：字符串比较
来源：http://rw.gzmigu.cn

strcmp(a, b) == 0
来源：http://zm.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://eg.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mz.colortex.cn

[S08] C：动态内存分配与释放
来源：http://bd.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xg.bjjhwx.cn

[S09] C：结构体定义与初始化
来源：http://kk.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ys.huanxung.cn

[S10] C：指针与解引用
来源：http://du.9csxet.cn

int *p = &a;  *p = 5;
来源：http://ne.colortex.cn

[S11] C：逐行读文件
来源：http://gu.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://co.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xx.jctech888.com.cn

fclose(f);
来源：http://mu.colortex.cn

[S12] C：写文件
来源：http://dg.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pe.huanxung.cn

[S13] C：宏定义
来源：http://zu.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gm.9csxet.cn

[S14] C：枚举
来源：http://ay.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://qa.asd995.cn

[S15] C：类型转换
来源：http://fy.szxytkj.cn

(double) a / b
来源：http://uw.nszjky.cn

[S16] C：位操作置位
来源：http://jy.lnxyls.cn

x |= (1 << 3);
来源：http://cn.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://nc.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zt.szxytkj.cn

[S18] C：命令行参数
来源：http://ae.shxzskj.cn

int main(int argc, char **argv)
来源：http://og.szsharing.cn

[S19] C：快速排序
来源：http://ex.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://el.9csxet.cn

[S20] C：二分查找
来源：http://qw.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cw.521024.cn

[S21] C：字符类别判断
来源：http://gq.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lh.521024.cn

[S22] C：字符串转数字
来源：http://ub.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://se.huixiangedu.cn

[S23] C：随机数
来源：http://na.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yn.gzmigu.cn

[S24] C：获取本地时间
来源：http://kc.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gg.colortex.cn

[S25] C：内存拷贝
来源：http://gl.huanxung.cn

memcpy(dst, src, n);
来源：http://xq.huixinmuqiang.cn

[S26] C：内存清零
来源：http://ga.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://er.9csxet.cn

[S27] C：定义常量
来源：http://sh.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://wn.hnjuh.cn

[S28] C：静态变量
来源：http://tv.muxihuayi.cn

static int counter = 0;
来源：http://lg.jctech888.com.cn

[S29] C：变参函数
来源：http://cv.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jp.muxihuayi.cn

[S30] C：头文件保护
来源：http://tg.asd995.cn

#ifndef X_H
来源：http://az.bookmarksfly.cn

#define X_H
来源：http://wv.yuntaijiaju.cn

#endif
来源：http://jp.shxzskj.cn

[S31] C++：Hello World
来源：http://si.szsharing.cn

#include <iostream>
来源：http://yn.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ld.panjiajie.cn

[S32] C++：字符串
来源：http://on.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://jd.colortex.cn

[S33] C++：vector 增删
来源：http://lu.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ry.szxytkj.cn

[S34] C++：遍历 vector
来源：http://ry.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://ou.bjjhwx.cn

[S35] C++：map
来源：http://mq.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bv.lnxyls.cn

[S36] C++：unordered_map
来源：http://yj.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eh.jctech888.com.cn

[S37] C++：set
来源：http://qn.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qw.hnjuh.cn

[S38] C++：排序
来源：http://cp.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://fm.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://lj.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jk.gzmigu.cn

[S40] C++：查找元素
来源：http://er.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ei.shxzukj.cn

[S41] C++：类与构造函数
来源：http://ct.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xp.newstarts.cn

[S42] C++：继承与虚函数
来源：http://pg.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://vc.newstarts.cn

[S43] C++：智能指针
来源：http://jj.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://su.gzmigu.cn

[S44] C++：引用传参
来源：http://hs.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://yd.colortex.cn

[S45] C++：lambda
来源：http://oy.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uz.nszjky.cn

[S46] C++：函数模板
来源：http://eq.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gg.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://ve.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jj.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://du.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uc.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://ri.lnxyls.cn

[S49] C++：写文件
来源：http://nl.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fg.huanxung.cn

[S50] C++：格式化数字
来源：http://ya.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cf.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://qb.panjiajie.cn

static_cast<double>(a) / b
来源：http://ho.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://rg.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://pl.lnxyls.cn

[S53] C++：移动语义
来源：http://vo.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://vv.lnxyls.cn

[S54] C++：异常处理
来源：http://tf.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dk.nszjky.cn

[S55] C++：结构化绑定
来源：http://mf.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://py.jianghongdianzi.cn

[S56] C++：optional
来源：http://mg.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jp.shtwfgs.cn

[S57] C++：编译期常量
来源：http://qo.lnxyls.cn

constexpr int N = 10;
来源：http://we.huanxung.cn

[S58] C++：命名空间
来源：http://iw.wgjwhj.cn

namespace ns { int f() { return 1; } }
来源：http://sq.bookmarksfly.cn

[S59] C++：静态断言
来源：http://ru.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nt.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://do.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hh.huanxung.cn

================================================================================
来源：http://du.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nd.muxihuayi.cn

================================================================================
来源：http://ux.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://jm.colortex.cn

println("Hello")
来源：http://jk.9csxet.cn

[T02] Kotlin：变量
来源：http://ac.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://te.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://ca.521024.cn

"值: $b"
来源：http://lf.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://ha.hnjuh.cn

val n: String? = null;  n?.length
来源：http://pa.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://oo.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qg.shxzukj.cn

[T06] Kotlin：集合映射
来源：http://fj.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ds.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://cn.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tm.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://nr.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://de.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://qs.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://dp.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://lk.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ht.newstarts.cn

[T11] Kotlin：协程
来源：http://sf.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kq.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://wy.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://vv.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://kl.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://gx.gzmigu.cn

[T14] Kotlin：循环
来源：http://zz.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://ni.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://it.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://cx.shxzukj.cn

[T16] Swift：Hello World
来源：http://mf.shxzukj.cn

print("Hello")
来源：http://um.colortex.cn

[T17] Swift：变量与常量
来源：http://gn.yuexingan06.cn

var a = 1;  let b = 2
来源：http://lu.shxzskj.cn

[T18] Swift：字符串插值
来源：http://mo.shtwfgs.cn

"值: \(b)"
来源：http://tk.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://vc.huixiangedu.cn

if let n = opt { print(n) }
来源：http://mm.colortex.cn

[T20] Swift：数组操作
来源：http://ro.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bg.gzmigu.cn

[T21] Swift：遍历
来源：http://ym.huanxung.cn

for x in a { print(x) }
来源：http://wb.jctech888.com.cn

[T22] Swift：字典
来源：http://el.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xk.bjjhwx.cn

[T23] Swift：函数
来源：http://bt.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wg.nicolike.cn

[T24] Swift：闭包
来源：http://ee.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ru.shxzukj.cn

[T25] Swift：结构体
来源：http://cb.nszjky.cn

struct P { var x: Int }
来源：http://jz.9csxet.cn

[T26] Swift：类与重写
来源：http://jl.huanxung.cn

class A: Base { override func f() {} }
来源：http://as.haigaiapp.cn

[T27] Swift：错误处理
来源：http://fo.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://hk.huixiangedu.cn

[T28] Swift：枚举
来源：http://iz.9csxet.cn

enum Color { case red, green }
来源：http://rw.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://pe.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://vg.jctech888.com.cn

[T30] Swift：协议
来源：http://xa.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://fc.huanxung.cn

[T31] Lua：Hello World
来源：http://dc.huanxung.cn

print("Hello")
来源：http://uu.colortex.cn

[T32] Lua：局部变量
来源：http://mw.yuexingan06.cn

local a = 1
来源：http://mb.szxytkj.cn

[T33] Lua：表（数组）
来源：http://ib.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ao.asd995.cn

[T34] Lua：遍历表
来源：http://ua.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://su.nszjky.cn

[T35] Lua：字典表
来源：http://sg.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://vy.colortex.cn

[T36] Lua：函数
来源：http://zb.jctech888.com.cn

function add(a, b) return a + b end
来源：http://tn.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://qz.jianghongdianzi.cn

"a" .. "b"
来源：http://xx.newstarts.cn

[T38] Lua：条件
来源：http://id.chemitech.net.cn

if x > 0 then print("正") end
来源：http://ec.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://ra.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://kv.panjiajie.cn

[T40] Lua：元表
来源：http://ia.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://hh.nszjky.cn

[T41] Perl：Hello World
来源：http://cn.gzmigu.cn

print "Hello\n";
来源：http://es.huixiangedu.cn

[T42] Perl：变量类型
来源：http://yl.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fa.wgjwhj.cn


<!-- 参考信息 -->