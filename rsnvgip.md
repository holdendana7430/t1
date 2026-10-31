代发 wailian999

files=$(ls -1)
来源：http://py.yuexingan06.cn

[R38] 管道串联
来源：http://hj.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://rn.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://uw.shxzskj.cn

cmd > out.log 2>&1
来源：http://yl.521024.cn

[R40] 追加写日志
来源：http://xf.9csxet.cn

echo "log" >> out.log
来源：http://zn.hnjuh.cn

[R41] 丢弃输出
来源：http://pp.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://wz.521024.cn

[R42] 输入重定向
来源：http://wn.jianghongdianzi.cn

wc -l < a.txt
来源：http://uf.bjjhwx.cn

[R43] 按名字查找文件
来源：http://fa.shtwfgs.cn

find . -name "*.log" -type f
来源：http://rg.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://uj.hahajie.cn

find . -mtime -7 -type f
来源：http://ma.nszjky.cn

[R45] 批量删除
来源：http://gx.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://ax.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://xh.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tc.muxihuayi.cn

[R47] sed 单行替换
来源：http://vu.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xi.asd995.cn

[R48] awk 取指定列
来源：http://hf.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://zm.huanxung.cn

[R49] awk 带条件
来源：http://hu.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yb.jctech888.com.cn

[R50] awk 求和
来源：http://kg.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dj.hahajie.cn

[R51] 排序去重取前几
来源：http://et.jianghongdianzi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lz.huanxung.cn

[R52] 统计行数
来源：http://ff.hahajie.cn

wc -l a.txt
来源：http://xq.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://sc.shxzskj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bp.yuexingan06.cn

[R54] 比较两个文件
来源：http://la.nicolike.cn

diff a.txt b.txt
来源：http://ul.asd995.cn

[R55] 压缩与解压
来源：http://bf.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xr.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://hd.szxytkj.cn

scp file user@host:/path/
来源：http://ip.haigaiapp.cn

[R57] 远程执行命令
来源：http://ut.521024.cn

ssh user@host 'uptime'
来源：http://ph.asd995.cn

[R58] 下载文件
来源：http://fd.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sf.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://vy.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ps.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://jq.hnjuh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nn.panjiajie.cn

[R61] 磁盘占用
来源：http://yw.yuexingan06.cn

df -h;  du -sh *
来源：http://kz.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://ta.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://fi.nszjky.cn

[R63] 内存与进程
来源：http://vr.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://of.szxytkj.cn

[R64] 结束进程
来源：http://xc.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://gl.gzmigu.cn

[R65] 查看端口占用
来源：http://un.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ei.szxytkj.cn

[R66] 定时任务
来源：http://yf.wgjwhj.cn

crontab -e;  crontab -l
来源：http://pq.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://bz.yuexingan06.cn

openssl rand -hex 16
来源：http://qd.jctech888.com.cn

[R68] 计算文件校验值
来源：http://id.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vk.panjiajie.cn

[R69] 生成随机密码
来源：http://nn.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://ss.newstarts.cn

[R70] 时间戳与互转
来源：http://kz.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://mw.lnxyls.cn

[R71] 日期格式化
来源：http://ot.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ny.hahajie.cn

[R72] 等待端口就绪
来源：http://sk.jianghongdianzi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://iy.szsharing.cn

[R73] 分割大日志
来源：http://me.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://fp.gzmigu.cn

[R74] 批量重命名
来源：http://qd.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://js.huanxung.cn

[R75] 导出环境变量
来源：http://zb.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://gi.bookmarksfly.cn

[R76] 使用临时文件
来源：http://jg.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zm.yuexingan06.cn

[R77] 读取用户输入
来源：http://rh.huixiangedu.cn

read -rp "请输入: " ans
来源：http://uh.panjiajie.cn

[R78] 交互式菜单
来源：http://gi.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tp.nicolike.cn

[R79] 解析命令行选项
来源：http://oc.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ul.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://wu.colortex.cn

time ./run.sh
来源：http://pe.wgjwhj.cn

================================================================================
来源：http://ef.yuntaijiaju.cn

S. C / C++ 专题
来源：http://yn.bjjhwx.cn

================================================================================
来源：http://ng.shtwfgs.cn

[S01] C：Hello World
来源：http://vr.szsharing.cn

#include <stdio.h>
来源：http://km.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://er.gzmigu.cn

[S02] C：变量与格式化输出
来源：http://wr.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://hu.hahajie.cn

[S03] C：读入整数
来源：http://lf.asd995.cn

int x; scanf("%d", &x);
来源：http://mw.shxzskj.cn

[S04] C：字符串复制
来源：http://sl.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ku.yuexingan06.cn

[S05] C：字符串长度
来源：http://wg.gzmigu.cn

strlen(s)
来源：http://ir.newstarts.cn

[S06] C：字符串比较
来源：http://de.muxihuayi.cn

strcmp(a, b) == 0
来源：http://zi.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://ty.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kd.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://rh.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ad.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://eh.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cp.panjiajie.cn

[S10] C：指针与解引用
来源：http://iv.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://gf.chemitech.net.cn

[S11] C：逐行读文件
来源：http://tw.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://yw.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vu.jctech888.com.cn

fclose(f);
来源：http://go.hnjuh.cn

[S12] C：写文件
来源：http://oj.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sk.panjiajie.cn

[S13] C：宏定义
来源：http://qn.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nw.nicolike.cn

[S14] C：枚举
来源：http://rb.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://gh.shtwfgs.cn

[S15] C：类型转换
来源：http://qh.9csxet.cn

(double) a / b
来源：http://ft.9csxet.cn

[S16] C：位操作置位
来源：http://gf.huixiangedu.cn

x |= (1 << 3);
来源：http://su.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://ve.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rg.gzmigu.cn

[S18] C：命令行参数
来源：http://zo.asd995.cn

int main(int argc, char **argv)
来源：http://vs.chemitech.net.cn

[S19] C：快速排序
来源：http://so.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ff.asd995.cn

[S20] C：二分查找
来源：http://mv.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eu.panjiajie.cn

[S21] C：字符类别判断
来源：http://gq.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cn.shxzskj.cn

[S22] C：字符串转数字
来源：http://qp.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://my.lnxyls.cn

[S23] C：随机数
来源：http://fm.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bw.asd995.cn

[S24] C：获取本地时间
来源：http://nv.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wx.shtwfgs.cn

[S25] C：内存拷贝
来源：http://ni.szsharing.cn

memcpy(dst, src, n);
来源：http://ye.huixiangedu.cn

[S26] C：内存清零
来源：http://hw.colortex.cn

memset(a, 0, sizeof a);
来源：http://ct.szsharing.cn

[S27] C：定义常量
来源：http://hl.huanxung.cn

const double PI = 3.14159;
来源：http://ny.bookmarksfly.cn

[S28] C：静态变量
来源：http://ft.colortex.cn

static int counter = 0;
来源：http://lu.lnxyls.cn

[S29] C：变参函数
来源：http://po.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rg.panjiajie.cn

[S30] C：头文件保护
来源：http://dd.muxihuayi.cn

#ifndef X_H
来源：http://mv.shtwfgs.cn

#define X_H
来源：http://ul.shxzskj.cn

#endif
来源：http://ch.521024.cn

[S31] C++：Hello World
来源：http://hv.wgjwhj.cn

#include <iostream>
来源：http://tn.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://yw.jctech888.com.cn

[S32] C++：字符串
来源：http://ij.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://up.9csxet.cn

[S33] C++：vector 增删
来源：http://ux.jctech888.com.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lo.gzmigu.cn

[S34] C++：遍历 vector
来源：http://yx.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://hx.wgjwhj.cn

[S35] C++：map
来源：http://cy.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bp.panjiajie.cn

[S36] C++：unordered_map
来源：http://bv.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rj.yuexingan06.cn

[S37] C++：set
来源：http://fp.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zu.huanxung.cn

[S38] C++：排序
来源：http://cd.asd995.cn

std::sort(v.begin(), v.end());
来源：http://pd.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://yx.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sg.szxytkj.cn

[S40] C++：查找元素
来源：http://dr.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qa.szxytkj.cn

[S41] C++：类与构造函数
来源：http://cx.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ju.nszjky.cn

[S42] C++：继承与虚函数
来源：http://tg.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://pi.szxytkj.cn

[S43] C++：智能指针
来源：http://vc.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://ig.gzmigu.cn

[S44] C++：引用传参
来源：http://bz.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://ud.wgjwhj.cn

[S45] C++：lambda
来源：http://rg.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sg.chemitech.net.cn

[S46] C++：函数模板
来源：http://qu.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tr.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://ki.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zc.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://kf.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ry.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://sk.yuntaijiaju.cn

[S49] C++：写文件
来源：http://wy.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://it.shtwfgs.cn

[S50] C++：格式化数字
来源：http://fd.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wd.lnxyls.cn

[S51] C++：显式类型转换
来源：http://oh.shxzskj.cn

static_cast<double>(a) / b
来源：http://mt.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://wk.huanxung.cn

int size() const noexcept { return n_; }
来源：http://oy.asd995.cn

[S53] C++：移动语义
来源：http://dm.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://gp.szsharing.cn

[S54] C++：异常处理
来源：http://pu.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kf.bookmarksfly.cn

[S55] C++：结构化绑定
来源：http://vz.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bl.shtwfgs.cn

[S56] C++：optional
来源：http://xn.jctech888.com.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://np.chemitech.net.cn

[S57] C++：编译期常量
来源：http://xb.yuntaijiaju.cn

constexpr int N = 10;
来源：http://hk.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://by.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://up.panjiajie.cn

[S59] C++：静态断言
来源：http://at.shtwfgs.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iq.bjjhwx.cn

[S60] C++：遍历并删除元素
来源：http://tk.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bq.newstarts.cn

================================================================================
来源：http://nh.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qb.huixinmuqiang.cn

================================================================================
来源：http://sq.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://uz.huixinmuqiang.cn

println("Hello")
来源：http://yl.wgjwhj.cn

[T02] Kotlin：变量
来源：http://si.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://es.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://at.hahajie.cn

"值: $b"
来源：http://xu.huanxung.cn

[T04] Kotlin：空安全
来源：http://eb.lnxyls.cn

val n: String? = null;  n?.length
来源：http://iw.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://eg.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pp.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://cd.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tx.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://vm.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bw.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://fb.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://gb.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://nc.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://jo.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://yi.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ya.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://xf.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wx.9csxet.cn

[T12] Kotlin：解构声明
来源：http://lg.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://jd.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://fu.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://vz.521024.cn

[T14] Kotlin：循环
来源：http://it.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://tn.wgjwhj.cn

[T15] Kotlin：接口
来源：http://mh.asd995.cn

interface Shape { fun area(): Double }
来源：http://pn.panjiajie.cn

[T16] Swift：Hello World
来源：http://er.newstarts.cn

print("Hello")
来源：http://uh.nicolike.cn

[T17] Swift：变量与常量
来源：http://ui.gzmigu.cn

var a = 1;  let b = 2
来源：http://jd.szsharing.cn

[T18] Swift：字符串插值
来源：http://vj.haigaiapp.cn

"值: \(b)"
来源：http://sd.gzmigu.cn

[T19] Swift：可选绑定
来源：http://ey.lnxyls.cn

if let n = opt { print(n) }
来源：http://wa.szxytkj.cn

[T20] Swift：数组操作
来源：http://iz.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bb.nicolike.cn

[T21] Swift：遍历
来源：http://qj.muxihuayi.cn

for x in a { print(x) }
来源：http://kq.gzmigu.cn

[T22] Swift：字典
来源：http://mb.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ub.panjiajie.cn

[T23] Swift：函数
来源：http://mx.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wj.jctech888.com.cn

[T24] Swift：闭包
来源：http://yg.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qm.nicolike.cn

[T25] Swift：结构体
来源：http://pe.521024.cn

struct P { var x: Int }
来源：http://nm.hahajie.cn

[T26] Swift：类与重写
来源：http://so.nszjky.cn

class A: Base { override func f() {} }
来源：http://tg.bjjhwx.cn

[T27] Swift：错误处理
来源：http://ng.szsharing.cn

do { try f() } catch { print(error) }
来源：http://hs.haigaiapp.cn

[T28] Swift：枚举
来源：http://jv.bookmarksfly.cn

enum Color { case red, green }
来源：http://rc.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://hc.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://bs.hahajie.cn

[T30] Swift：协议
来源：http://ut.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://ml.hnjuh.cn

[T31] Lua：Hello World
来源：http://lk.muxihuayi.cn

print("Hello")
来源：http://hg.muxihuayi.cn

[T32] Lua：局部变量
来源：http://kn.nicolike.cn

local a = 1
来源：http://rp.521024.cn

[T33] Lua：表（数组）
来源：http://nz.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ze.gzmigu.cn

[T34] Lua：遍历表
来源：http://zc.lnxyls.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tv.shxzukj.cn

[T35] Lua：字典表
来源：http://nl.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://rg.hnjuh.cn

[T36] Lua：函数
来源：http://ad.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://mw.huanxung.cn

[T37] Lua：字符串拼接
来源：http://lq.shtwfgs.cn

"a" .. "b"
来源：http://gc.yuntaijiaju.cn

[T38] Lua：条件
来源：http://wb.newstarts.cn

if x > 0 then print("正") end
来源：http://ix.hnjuh.cn

[T39] Lua：模式匹配
来源：http://wp.szxytkj.cn

string.find(s, "%d+")
来源：http://lv.panjiajie.cn

[T40] Lua：元表
来源：http://le.hahajie.cn

setmetatable({}, { __index = base })
来源：http://fr.huixinmuqiang.cn


<!-- 参考信息 -->