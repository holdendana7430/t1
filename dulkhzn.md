代发 wailian999

find . -name "*.log" -type f
来源：http://wj.shxzskj.cn

[R44] 按修改时间查找
来源：http://st.nicolike.cn

find . -mtime -7 -type f
来源：http://vw.huanxung.cn

[R45] 批量删除
来源：http://md.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://gm.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://wn.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pv.asd995.cn

[R47] sed 单行替换
来源：http://pj.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://on.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://fo.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://ag.wgjwhj.cn

[R49] awk 带条件
来源：http://xv.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sb.colortex.cn

[R50] awk 求和
来源：http://oo.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gw.shtwfgs.cn

[R51] 排序去重取前几
来源：http://rs.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cv.huixinmuqiang.cn

[R52] 统计行数
来源：http://zt.shtwfgs.cn

wc -l a.txt
来源：http://hj.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://ju.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xw.hnjuh.cn

[R54] 比较两个文件
来源：http://iy.panjiajie.cn

diff a.txt b.txt
来源：http://rt.chemitech.net.cn

[R55] 压缩与解压
来源：http://zg.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dh.shxzskj.cn

[R56] 远程拷贝
来源：http://uz.yuntaijiaju.cn

scp file user@host:/path/
来源：http://jt.shxzskj.cn

[R57] 远程执行命令
来源：http://fn.9csxet.cn

ssh user@host 'uptime'
来源：http://fu.huixinmuqiang.cn

[R58] 下载文件
来源：http://ik.hnjuh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jl.yuntaijiaju.cn

[R59] 发 POST JSON
来源：http://mj.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qk.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://nd.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kl.chemitech.net.cn

[R61] 磁盘占用
来源：http://zx.newstarts.cn

df -h;  du -sh *
来源：http://pb.hnjuh.cn

[R62] 找最占空间的文件
来源：http://cg.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://qk.newstarts.cn

[R63] 内存与进程
来源：http://ve.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://pz.shxzskj.cn

[R64] 结束进程
来源：http://ua.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://gf.muxihuayi.cn

[R65] 查看端口占用
来源：http://nn.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vx.szxytkj.cn

[R66] 定时任务
来源：http://wz.bjjhwx.cn

crontab -e;  crontab -l
来源：http://li.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://jj.nszjky.cn

openssl rand -hex 16
来源：http://hv.shxzskj.cn

[R68] 计算文件校验值
来源：http://es.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gs.muxihuayi.cn

[R69] 生成随机密码
来源：http://zk.jctech888.com.cn

head -c 16 /dev/urandom | base64
来源：http://kt.bjjhwx.cn

[R70] 时间戳与互转
来源：http://nj.nszjky.cn

date +%s;  date -d @1700000000
来源：http://yk.shtwfgs.cn

[R71] 日期格式化
来源：http://oz.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ty.jctech888.com.cn

[R72] 等待端口就绪
来源：http://jm.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yl.newstarts.cn

[R73] 分割大日志
来源：http://kf.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://ui.shxzskj.cn

[R74] 批量重命名
来源：http://zg.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ak.asd995.cn

[R75] 导出环境变量
来源：http://eh.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://ex.haigaiapp.cn

[R76] 使用临时文件
来源：http://gk.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jt.9csxet.cn

[R77] 读取用户输入
来源：http://gb.9csxet.cn

read -rp "请输入: " ans
来源：http://wl.hahajie.cn

[R78] 交互式菜单
来源：http://mk.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vg.panjiajie.cn

[R79] 解析命令行选项
来源：http://bn.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iu.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://vr.bjjhwx.cn

time ./run.sh
来源：http://si.jctech888.com.cn

================================================================================
来源：http://xd.521024.cn

S. C / C++ 专题
来源：http://jx.haigaiapp.cn

================================================================================
来源：http://sg.lnxyls.cn

[S01] C：Hello World
来源：http://ro.bjjhwx.cn

#include <stdio.h>
来源：http://wo.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ek.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://up.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://ra.newstarts.cn

[S03] C：读入整数
来源：http://kn.nszjky.cn

int x; scanf("%d", &x);
来源：http://lz.muxihuayi.cn

[S04] C：字符串复制
来源：http://jy.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://eh.yuexingan06.cn

[S05] C：字符串长度
来源：http://wz.asd995.cn

strlen(s)
来源：http://ek.muxihuayi.cn

[S06] C：字符串比较
来源：http://ml.nicolike.cn

strcmp(a, b) == 0
来源：http://mw.521024.cn

[S07] C：数组遍历求和
来源：http://uk.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ye.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://lp.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hl.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://hr.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ev.lnxyls.cn

[S10] C：指针与解引用
来源：http://gd.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://dj.shxzskj.cn

[S11] C：逐行读文件
来源：http://zm.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://no.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gz.nicolike.cn

fclose(f);
来源：http://yu.hahajie.cn

[S12] C：写文件
来源：http://xn.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vl.newstarts.cn

[S13] C：宏定义
来源：http://jm.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mv.shxzukj.cn

[S14] C：枚举
来源：http://oc.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://im.huixiangedu.cn

[S15] C：类型转换
来源：http://jb.yuntaijiaju.cn

(double) a / b
来源：http://lr.szsharing.cn

[S16] C：位操作置位
来源：http://et.haigaiapp.cn

x |= (1 << 3);
来源：http://js.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://ac.lnxyls.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rq.yuexingan06.cn

[S18] C：命令行参数
来源：http://io.hnjuh.cn

int main(int argc, char **argv)
来源：http://uy.asd995.cn

[S19] C：快速排序
来源：http://dq.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qj.panjiajie.cn

[S20] C：二分查找
来源：http://dr.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mx.asd995.cn

[S21] C：字符类别判断
来源：http://ad.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rw.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://pq.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jb.bookmarksfly.cn

[S23] C：随机数
来源：http://fn.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vl.hnjuh.cn

[S24] C：获取本地时间
来源：http://nq.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rl.chemitech.net.cn

[S25] C：内存拷贝
来源：http://cr.521024.cn

memcpy(dst, src, n);
来源：http://br.nszjky.cn

[S26] C：内存清零
来源：http://nf.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://un.muxihuayi.cn

[S27] C：定义常量
来源：http://kf.muxihuayi.cn

const double PI = 3.14159;
来源：http://ws.nszjky.cn

[S28] C：静态变量
来源：http://qn.hnjuh.cn

static int counter = 0;
来源：http://ug.shxzukj.cn

[S29] C：变参函数
来源：http://jf.yuexingan06.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lj.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://yr.yuexingan06.cn

#ifndef X_H
来源：http://yr.jctech888.com.cn

#define X_H
来源：http://yn.huixinmuqiang.cn

#endif
来源：http://hv.chemitech.net.cn

[S31] C++：Hello World
来源：http://hq.yuntaijiaju.cn

#include <iostream>
来源：http://rg.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://qk.yuntaijiaju.cn

[S32] C++：字符串
来源：http://sl.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://sr.lnxyls.cn

[S33] C++：vector 增删
来源：http://vm.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://es.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://gw.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://um.jctech888.com.cn

[S35] C++：map
来源：http://jn.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rx.colortex.cn

[S36] C++：unordered_map
来源：http://et.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iu.wgjwhj.cn

[S37] C++：set
来源：http://dx.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jl.shxzskj.cn

[S38] C++：排序
来源：http://bp.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://gw.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://qq.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mg.shxzukj.cn

[S40] C++：查找元素
来源：http://tk.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gn.szsharing.cn

[S41] C++：类与构造函数
来源：http://du.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wh.jctech888.com.cn

[S42] C++：继承与虚函数
来源：http://ya.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://rj.yuexingan06.cn

[S43] C++：智能指针
来源：http://wv.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://nb.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://ew.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://aa.yuntaijiaju.cn

[S45] C++：lambda
来源：http://bm.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gb.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://hh.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hu.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://hc.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://np.521024.cn

[S48] C++：逐行读文件
来源：http://wx.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://io.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://si.521024.cn

[S49] C++：写文件
来源：http://id.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sf.shxzskj.cn

[S50] C++：格式化数字
来源：http://ig.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bh.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://dw.muxihuayi.cn

static_cast<double>(a) / b
来源：http://kx.huixiangedu.cn

[S52] C++：const 与 noexcept
来源：http://sb.nicolike.cn

int size() const noexcept { return n_; }
来源：http://dv.shxzskj.cn

[S53] C++：移动语义
来源：http://zk.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://ga.hnjuh.cn

[S54] C++：异常处理
来源：http://nj.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bz.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://xo.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://me.wgjwhj.cn

[S56] C++：optional
来源：http://yn.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fy.huanxung.cn

[S57] C++：编译期常量
来源：http://ws.newstarts.cn

constexpr int N = 10;
来源：http://rk.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://yh.jianghongdianzi.cn

namespace ns { int f() { return 1; } }
来源：http://ez.shxzukj.cn

[S59] C++：静态断言
来源：http://xp.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vp.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://fw.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rh.hahajie.cn

================================================================================
来源：http://dl.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ue.szxytkj.cn

================================================================================
来源：http://zr.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://ig.szxytkj.cn

println("Hello")
来源：http://lb.szsharing.cn

[T02] Kotlin：变量
来源：http://tn.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ng.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://hl.huixiangedu.cn

"值: $b"
来源：http://ym.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://ee.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://lp.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://qv.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://um.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://mx.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fd.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://uq.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ow.bookmarksfly.cn

[T08] Kotlin：数据类
来源：http://co.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://zh.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://xr.hahajie.cn

fun String.exclaim() = this + "!"
来源：http://px.9csxet.cn

[T10] Kotlin：默认参数
来源：http://ab.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qm.chemitech.net.cn

[T11] Kotlin：协程
来源：http://bn.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mb.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://qz.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://hy.jctech888.com.cn

[T13] Kotlin：只读 Map
来源：http://gz.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://vi.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://je.shxzukj.cn

for (i in 1..10) println(i)
来源：http://hc.shxzukj.cn

[T15] Kotlin：接口
来源：http://qn.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://jk.bjjhwx.cn

[T16] Swift：Hello World
来源：http://il.asd995.cn

print("Hello")
来源：http://xw.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://we.9csxet.cn

var a = 1;  let b = 2
来源：http://eq.521024.cn

[T18] Swift：字符串插值
来源：http://cd.bjjhwx.cn

"值: \(b)"
来源：http://sa.nicolike.cn

[T19] Swift：可选绑定
来源：http://dp.chemitech.net.cn

if let n = opt { print(n) }
来源：http://ft.nszjky.cn

[T20] Swift：数组操作
来源：http://cq.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wi.gzmigu.cn

[T21] Swift：遍历
来源：http://yo.yuexingan06.cn

for x in a { print(x) }
来源：http://ip.hahajie.cn

[T22] Swift：字典
来源：http://xi.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ka.gzmigu.cn

[T23] Swift：函数
来源：http://kq.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cy.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://ml.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jj.bjjhwx.cn

[T25] Swift：结构体
来源：http://sg.hahajie.cn

struct P { var x: Int }
来源：http://rz.shtwfgs.cn

[T26] Swift：类与重写
来源：http://aa.szxytkj.cn

class A: Base { override func f() {} }
来源：http://ez.panjiajie.cn

[T27] Swift：错误处理
来源：http://fm.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://ba.szxytkj.cn

[T28] Swift：枚举
来源：http://ts.shtwfgs.cn

enum Color { case red, green }
来源：http://kn.nicolike.cn

[T29] Swift：guard 提前返回
来源：http://de.521024.cn

guard let x = opt else { return }
来源：http://dg.chemitech.net.cn

[T30] Swift：协议
来源：http://ku.newstarts.cn

protocol Shape { func area() -> Double }
来源：http://ao.9csxet.cn

[T31] Lua：Hello World
来源：http://uh.wgjwhj.cn

print("Hello")
来源：http://tb.hnjuh.cn

[T32] Lua：局部变量
来源：http://tu.chemitech.net.cn

local a = 1
来源：http://yh.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://hu.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xy.lnxyls.cn

[T34] Lua：遍历表
来源：http://lm.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vi.9csxet.cn

[T35] Lua：字典表
来源：http://cl.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://up.asd995.cn

[T36] Lua：函数
来源：http://zt.huixiangedu.cn

function add(a, b) return a + b end
来源：http://co.9csxet.cn

[T37] Lua：字符串拼接
来源：http://st.bookmarksfly.cn

"a" .. "b"
来源：http://va.gzmigu.cn

[T38] Lua：条件
来源：http://xz.bjjhwx.cn

if x > 0 then print("正") end
来源：http://lt.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://ul.szxytkj.cn

string.find(s, "%d+")
来源：http://uc.haigaiapp.cn

[T40] Lua：元表
来源：http://vk.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://sh.hnjuh.cn

[T41] Perl：Hello World
来源：http://kw.huixinmuqiang.cn

print "Hello\n";
来源：http://ch.hnjuh.cn

[T42] Perl：变量类型
来源：http://qb.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yw.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://in.shxzskj.cn

"值: $a"
来源：http://ge.hahajie.cn

[T44] Perl：条件
来源：http://cv.szsharing.cn

if ($a > 0) { print "正"; }
来源：http://jj.asd995.cn

[T45] Perl：数组遍历
来源：http://nx.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://ei.shxzskj.cn

[T46] Perl：哈希操作
来源：http://vp.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yl.shxzukj.cn


<!-- 参考信息 -->