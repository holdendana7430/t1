代发 wailian999

files=$(ls -1)
来源：http://hn.shxzukj.cn

[R38] 管道串联
来源：http://zr.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://av.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://mo.panjiajie.cn

cmd > out.log 2>&1
来源：http://vl.521024.cn

[R40] 追加写日志
来源：http://pw.nszjky.cn

echo "log" >> out.log
来源：http://jx.bjjhwx.cn

[R41] 丢弃输出
来源：http://eq.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://oq.huixiangedu.cn

[R42] 输入重定向
来源：http://bz.nszjky.cn

wc -l < a.txt
来源：http://bk.chemitech.net.cn

[R43] 按名字查找文件
来源：http://kf.bjjhwx.cn

find . -name "*.log" -type f
来源：http://ea.szxytkj.cn

[R44] 按修改时间查找
来源：http://pd.shxzskj.cn

find . -mtime -7 -type f
来源：http://wx.chemitech.net.cn

[R45] 批量删除
来源：http://xe.521024.cn

find . -name "*.tmp" -delete
来源：http://ea.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://cm.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gr.jctech888.com.cn

[R47] sed 单行替换
来源：http://ii.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pn.hahajie.cn

[R48] awk 取指定列
来源：http://bz.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://iq.haigaiapp.cn

[R49] awk 带条件
来源：http://jc.lnxyls.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://me.shxzukj.cn

[R50] awk 求和
来源：http://gb.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lj.szxytkj.cn

[R51] 排序去重取前几
来源：http://hi.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ow.newstarts.cn

[R52] 统计行数
来源：http://wx.lnxyls.cn

wc -l a.txt
来源：http://yd.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://fy.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yg.asd995.cn

[R54] 比较两个文件
来源：http://ie.huanxung.cn

diff a.txt b.txt
来源：http://pf.newstarts.cn

[R55] 压缩与解压
来源：http://at.chemitech.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lj.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://ty.lnxyls.cn

scp file user@host:/path/
来源：http://dz.nszjky.cn

[R57] 远程执行命令
来源：http://yh.bjjhwx.cn

ssh user@host 'uptime'
来源：http://fu.lnxyls.cn

[R58] 下载文件
来源：http://cx.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oj.shxzskj.cn

[R59] 发 POST JSON
来源：http://ie.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://og.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://ky.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nb.lnxyls.cn

[R61] 磁盘占用
来源：http://iy.hahajie.cn

df -h;  du -sh *
来源：http://zp.huixinmuqiang.cn

[R62] 找最占空间的文件
来源：http://gq.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://vv.huixinmuqiang.cn

[R63] 内存与进程
来源：http://ps.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://pw.yuexingan06.cn

[R64] 结束进程
来源：http://se.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://ks.jctech888.com.cn

[R65] 查看端口占用
来源：http://ya.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tt.haigaiapp.cn

[R66] 定时任务
来源：http://zt.panjiajie.cn

crontab -e;  crontab -l
来源：http://un.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://jv.shxzskj.cn

openssl rand -hex 16
来源：http://wr.haigaiapp.cn

[R68] 计算文件校验值
来源：http://he.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ip.bjjhwx.cn

[R69] 生成随机密码
来源：http://xb.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://tu.9csxet.cn

[R70] 时间戳与互转
来源：http://mb.huixinmuqiang.cn

date +%s;  date -d @1700000000
来源：http://vh.521024.cn

[R71] 日期格式化
来源：http://hp.newstarts.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vf.colortex.cn

[R72] 等待端口就绪
来源：http://ck.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://aj.szsharing.cn

[R73] 分割大日志
来源：http://ck.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://nq.szxytkj.cn

[R74] 批量重命名
来源：http://kv.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kd.jctech888.com.cn

[R75] 导出环境变量
来源：http://wq.wgjwhj.cn

export PATH="$HOME/bin:$PATH"
来源：http://yd.521024.cn

[R76] 使用临时文件
来源：http://an.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ve.bjjhwx.cn

[R77] 读取用户输入
来源：http://ge.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://zz.muxihuayi.cn

[R78] 交互式菜单
来源：http://df.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nv.shxzskj.cn

[R79] 解析命令行选项
来源：http://uw.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qy.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://vo.haigaiapp.cn

time ./run.sh
来源：http://to.nszjky.cn

================================================================================
来源：http://ej.wgjwhj.cn

S. C / C++ 专题
来源：http://qa.szxytkj.cn

================================================================================
来源：http://yf.panjiajie.cn

[S01] C：Hello World
来源：http://lq.muxihuayi.cn

#include <stdio.h>
来源：http://wq.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hr.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://nf.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://tc.huixinmuqiang.cn

[S03] C：读入整数
来源：http://zm.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://yc.nicolike.cn

[S04] C：字符串复制
来源：http://co.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tp.nszjky.cn

[S05] C：字符串长度
来源：http://sw.9csxet.cn

strlen(s)
来源：http://wq.huixiangedu.cn

[S06] C：字符串比较
来源：http://oz.panjiajie.cn

strcmp(a, b) == 0
来源：http://qs.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://qg.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ol.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://ze.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fr.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://tn.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nb.panjiajie.cn

[S10] C：指针与解引用
来源：http://pw.shxzukj.cn

int *p = &a;  *p = 5;
来源：http://tm.huanxung.cn

[S11] C：逐行读文件
来源：http://hf.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://pz.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ng.jctech888.com.cn

fclose(f);
来源：http://oe.shxzskj.cn

[S12] C：写文件
来源：http://hg.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lb.chemitech.net.cn

[S13] C：宏定义
来源：http://ar.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hx.lnxyls.cn

[S14] C：枚举
来源：http://tw.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://pn.newstarts.cn

[S15] C：类型转换
来源：http://gc.nszjky.cn

(double) a / b
来源：http://mm.521024.cn

[S16] C：位操作置位
来源：http://la.9csxet.cn

x |= (1 << 3);
来源：http://da.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://lj.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dp.huanxung.cn

[S18] C：命令行参数
来源：http://tq.newstarts.cn

int main(int argc, char **argv)
来源：http://dk.huixiangedu.cn

[S19] C：快速排序
来源：http://tz.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iq.yuexingan06.cn

[S20] C：二分查找
来源：http://iz.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kf.jctech888.com.cn

[S21] C：字符类别判断
来源：http://fh.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bo.nicolike.cn

[S22] C：字符串转数字
来源：http://ie.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rz.shxzukj.cn

[S23] C：随机数
来源：http://fi.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ye.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://eu.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oo.panjiajie.cn

[S25] C：内存拷贝
来源：http://an.szsharing.cn

memcpy(dst, src, n);
来源：http://ik.jianghongdianzi.cn

[S26] C：内存清零
来源：http://wq.colortex.cn

memset(a, 0, sizeof a);
来源：http://tp.huixiangedu.cn

[S27] C：定义常量
来源：http://eg.muxihuayi.cn

const double PI = 3.14159;
来源：http://gy.newstarts.cn

[S28] C：静态变量
来源：http://jc.colortex.cn

static int counter = 0;
来源：http://ub.chemitech.net.cn

[S29] C：变参函数
来源：http://jd.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ij.521024.cn

[S30] C：头文件保护
来源：http://iq.huanxung.cn

#ifndef X_H
来源：http://en.muxihuayi.cn

#define X_H
来源：http://ek.huanxung.cn

#endif
来源：http://sd.wgjwhj.cn

[S31] C++：Hello World
来源：http://br.yuexingan06.cn

#include <iostream>
来源：http://fk.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://qk.yuexingan06.cn

[S32] C++：字符串
来源：http://et.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://xi.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://bf.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nv.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://fw.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://sq.szsharing.cn

[S35] C++：map
来源：http://zt.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oi.haigaiapp.cn

[S36] C++：unordered_map
来源：http://fb.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qp.shtwfgs.cn

[S37] C++：set
来源：http://dv.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fd.chemitech.net.cn

[S38] C++：排序
来源：http://gf.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://tt.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://se.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gb.newstarts.cn

[S40] C++：查找元素
来源：http://kx.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uo.hnjuh.cn

[S41] C++：类与构造函数
来源：http://rl.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xr.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://xb.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://cp.wgjwhj.cn

[S43] C++：智能指针
来源：http://yw.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://vp.colortex.cn

[S44] C++：引用传参
来源：http://hg.newstarts.cn

void inc(int &x) { ++x; }
来源：http://fd.asd995.cn

[S45] C++：lambda
来源：http://kp.hahajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bp.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://we.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kr.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://pl.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://se.asd995.cn

[S48] C++：逐行读文件
来源：http://wj.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yg.asd995.cn

while (std::getline(in, line)) { }
来源：http://aw.9csxet.cn

[S49] C++：写文件
来源：http://rw.chemitech.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kp.muxihuayi.cn

[S50] C++：格式化数字
来源：http://ts.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ue.gzmigu.cn

[S51] C++：显式类型转换
来源：http://vs.huixiangedu.cn

static_cast<double>(a) / b
来源：http://kz.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://oc.newstarts.cn

int size() const noexcept { return n_; }
来源：http://qh.shtwfgs.cn

[S53] C++：移动语义
来源：http://fb.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://th.muxihuayi.cn

[S54] C++：异常处理
来源：http://tk.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://om.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://hv.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ej.wgjwhj.cn

[S56] C++：optional
来源：http://uy.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ee.nszjky.cn

[S57] C++：编译期常量
来源：http://uo.szxytkj.cn

constexpr int N = 10;
来源：http://tl.huanxung.cn

[S58] C++：命名空间
来源：http://ok.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://wj.shtwfgs.cn

[S59] C++：静态断言
来源：http://rq.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ud.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://vc.jianghongdianzi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ia.wgjwhj.cn

================================================================================
来源：http://gh.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://js.newstarts.cn

================================================================================
来源：http://je.nszjky.cn

[T01] Kotlin：Hello World
来源：http://tv.chemitech.net.cn

println("Hello")
来源：http://bi.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://pa.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fx.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://mj.szxytkj.cn

"值: $b"
来源：http://ay.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://jm.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://wd.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://qd.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nw.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://by.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tx.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://ie.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ky.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://ic.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://yn.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://vf.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://ah.colortex.cn

[T10] Kotlin：默认参数
来源：http://gv.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ga.lnxyls.cn

[T11] Kotlin：协程
来源：http://ie.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pt.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://ya.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://zh.colortex.cn

[T13] Kotlin：只读 Map
来源：http://dw.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://gq.wgjwhj.cn

[T14] Kotlin：循环
来源：http://ff.gzmigu.cn

for (i in 1..10) println(i)
来源：http://fa.huixiangedu.cn

[T15] Kotlin：接口
来源：http://lp.asd995.cn

interface Shape { fun area(): Double }
来源：http://wb.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://ff.panjiajie.cn

print("Hello")
来源：http://qh.colortex.cn

[T17] Swift：变量与常量
来源：http://km.jctech888.com.cn

var a = 1;  let b = 2
来源：http://or.shxzskj.cn

[T18] Swift：字符串插值
来源：http://um.panjiajie.cn

"值: \(b)"
来源：http://ev.panjiajie.cn

[T19] Swift：可选绑定
来源：http://qu.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://qs.wgjwhj.cn

[T20] Swift：数组操作
来源：http://uq.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://il.nicolike.cn

[T21] Swift：遍历
来源：http://az.panjiajie.cn

for x in a { print(x) }
来源：http://ta.521024.cn

[T22] Swift：字典
来源：http://mu.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hl.yuntaijiaju.cn

[T23] Swift：函数
来源：http://py.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yi.shxzukj.cn

[T24] Swift：闭包
来源：http://cr.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oi.521024.cn

[T25] Swift：结构体
来源：http://ny.9csxet.cn

struct P { var x: Int }
来源：http://mu.szsharing.cn

[T26] Swift：类与重写
来源：http://nm.shxzukj.cn

class A: Base { override func f() {} }
来源：http://ah.huanxung.cn

[T27] Swift：错误处理
来源：http://bf.asd995.cn

do { try f() } catch { print(error) }
来源：http://bw.szxytkj.cn

[T28] Swift：枚举
来源：http://tq.yuexingan06.cn

enum Color { case red, green }
来源：http://it.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://na.jctech888.com.cn

guard let x = opt else { return }
来源：http://ce.nszjky.cn

[T30] Swift：协议
来源：http://nn.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://pc.newstarts.cn

[T31] Lua：Hello World
来源：http://ci.haigaiapp.cn

print("Hello")
来源：http://qe.hahajie.cn

[T32] Lua：局部变量
来源：http://ey.jctech888.com.cn

local a = 1
来源：http://qt.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://wd.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bo.yuexingan06.cn

[T34] Lua：遍历表
来源：http://gl.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ff.hnjuh.cn

[T35] Lua：字典表
来源：http://fu.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://rc.huixinmuqiang.cn

[T36] Lua：函数
来源：http://sl.bjjhwx.cn

function add(a, b) return a + b end
来源：http://dp.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://no.9csxet.cn

"a" .. "b"
来源：http://ub.szsharing.cn

[T38] Lua：条件
来源：http://os.bjjhwx.cn

if x > 0 then print("正") end
来源：http://rk.szxytkj.cn

[T39] Lua：模式匹配
来源：http://cn.hahajie.cn

string.find(s, "%d+")
来源：http://yh.shxzukj.cn

[T40] Lua：元表
来源：http://bi.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://mr.wgjwhj.cn


<!-- 参考信息 -->