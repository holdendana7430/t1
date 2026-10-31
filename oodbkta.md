代发 wailian999

cmd > out.log 2>&1
来源：http://my.shtwfgs.cn

[R40] 追加写日志
来源：http://tj.jianghongdianzi.cn

echo "log" >> out.log
来源：http://it.panjiajie.cn

[R41] 丢弃输出
来源：http://ot.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://fo.jianghongdianzi.cn

[R42] 输入重定向
来源：http://hz.newstarts.cn

wc -l < a.txt
来源：http://bc.nszjky.cn

[R43] 按名字查找文件
来源：http://zu.9csxet.cn

find . -name "*.log" -type f
来源：http://dt.hahajie.cn

[R44] 按修改时间查找
来源：http://di.colortex.cn

find . -mtime -7 -type f
来源：http://vk.colortex.cn

[R45] 批量删除
来源：http://aq.asd995.cn

find . -name "*.tmp" -delete
来源：http://yh.yuntaijiaju.cn

[R46] 递归替换文件内容
来源：http://in.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ev.haigaiapp.cn

[R47] sed 单行替换
来源：http://sc.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gb.jctech888.com.cn

[R48] awk 取指定列
来源：http://kw.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://ju.yuntaijiaju.cn

[R49] awk 带条件
来源：http://pe.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mg.huixinmuqiang.cn

[R50] awk 求和
来源：http://of.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://il.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://am.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cu.shtwfgs.cn

[R52] 统计行数
来源：http://kg.huixiangedu.cn

wc -l a.txt
来源：http://vv.521024.cn

[R53] 查看文件头与实时尾
来源：http://vd.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ol.9csxet.cn

[R54] 比较两个文件
来源：http://ep.newstarts.cn

diff a.txt b.txt
来源：http://ah.huixiangedu.cn

[R55] 压缩与解压
来源：http://ir.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://np.colortex.cn

[R56] 远程拷贝
来源：http://ea.muxihuayi.cn

scp file user@host:/path/
来源：http://xw.asd995.cn

[R57] 远程执行命令
来源：http://ba.hahajie.cn

ssh user@host 'uptime'
来源：http://jw.szxytkj.cn

[R58] 下载文件
来源：http://sc.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aa.chemitech.net.cn

[R59] 发 POST JSON
来源：http://ru.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uf.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://fn.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lx.shxzukj.cn

[R61] 磁盘占用
来源：http://ap.colortex.cn

df -h;  du -sh *
来源：http://dd.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://wr.lnxyls.cn

du -ah . | sort -rh | head -10
来源：http://wz.asd995.cn

[R63] 内存与进程
来源：http://wu.colortex.cn

free -h;  ps aux | grep nginx
来源：http://no.bjjhwx.cn

[R64] 结束进程
来源：http://du.nicolike.cn

kill -9 $(pgrep -f app.py)
来源：http://do.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://gw.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cn.nszjky.cn

[R66] 定时任务
来源：http://qd.asd995.cn

crontab -e;  crontab -l
来源：http://dl.521024.cn

[R67] 生成随机十六进制串
来源：http://jb.panjiajie.cn

openssl rand -hex 16
来源：http://ow.panjiajie.cn

[R68] 计算文件校验值
来源：http://vt.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jn.szxytkj.cn

[R69] 生成随机密码
来源：http://fk.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://zv.asd995.cn

[R70] 时间戳与互转
来源：http://rq.521024.cn

date +%s;  date -d @1700000000
来源：http://hu.hnjuh.cn

[R71] 日期格式化
来源：http://kv.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lm.muxihuayi.cn

[R72] 等待端口就绪
来源：http://gz.jianghongdianzi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yo.nicolike.cn

[R73] 分割大日志
来源：http://bk.hahajie.cn

split -l 1000 big.log part_
来源：http://hw.bjjhwx.cn

[R74] 批量重命名
来源：http://id.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://um.9csxet.cn

[R75] 导出环境变量
来源：http://vb.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://gp.jctech888.com.cn

[R76] 使用临时文件
来源：http://ib.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://du.szxytkj.cn

[R77] 读取用户输入
来源：http://lw.hnjuh.cn

read -rp "请输入: " ans
来源：http://hr.nszjky.cn

[R78] 交互式菜单
来源：http://bd.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gs.gzmigu.cn

[R79] 解析命令行选项
来源：http://aj.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zi.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://sf.wgjwhj.cn

time ./run.sh
来源：http://ep.bjjhwx.cn

================================================================================
来源：http://il.shxzskj.cn

S. C / C++ 专题
来源：http://ax.gzmigu.cn

================================================================================
来源：http://wf.yuexingan06.cn

[S01] C：Hello World
来源：http://bk.bookmarksfly.cn

#include <stdio.h>
来源：http://tg.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hu.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://ad.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://ad.wgjwhj.cn

[S03] C：读入整数
来源：http://jj.9csxet.cn

int x; scanf("%d", &x);
来源：http://mx.shxzskj.cn

[S04] C：字符串复制
来源：http://th.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rh.szsharing.cn

[S05] C：字符串长度
来源：http://wn.gzmigu.cn

strlen(s)
来源：http://nh.gzmigu.cn

[S06] C：字符串比较
来源：http://et.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://hg.asd995.cn

[S07] C：数组遍历求和
来源：http://xs.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://on.colortex.cn

[S08] C：动态内存分配与释放
来源：http://np.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qe.521024.cn

[S09] C：结构体定义与初始化
来源：http://ht.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ja.bjjhwx.cn

[S10] C：指针与解引用
来源：http://yl.521024.cn

int *p = &a;  *p = 5;
来源：http://sr.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://km.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://cr.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sv.lnxyls.cn

fclose(f);
来源：http://ut.bjjhwx.cn

[S12] C：写文件
来源：http://mr.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://os.panjiajie.cn

[S13] C：宏定义
来源：http://be.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dh.yuntaijiaju.cn

[S14] C：枚举
来源：http://hy.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://uk.521024.cn

[S15] C：类型转换
来源：http://xs.haigaiapp.cn

(double) a / b
来源：http://cs.muxihuayi.cn

[S16] C：位操作置位
来源：http://xy.hahajie.cn

x |= (1 << 3);
来源：http://qt.newstarts.cn

[S17] C：安全拼接字符串
来源：http://xg.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ux.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://oo.wgjwhj.cn

int main(int argc, char **argv)
来源：http://lp.panjiajie.cn

[S19] C：快速排序
来源：http://cb.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zg.bjjhwx.cn

[S20] C：二分查找
来源：http://mz.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zg.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://ad.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qj.panjiajie.cn

[S22] C：字符串转数字
来源：http://jt.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zx.gzmigu.cn

[S23] C：随机数
来源：http://yp.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pk.9csxet.cn

[S24] C：获取本地时间
来源：http://xt.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ac.wgjwhj.cn

[S25] C：内存拷贝
来源：http://gx.shxzskj.cn

memcpy(dst, src, n);
来源：http://rg.yuntaijiaju.cn

[S26] C：内存清零
来源：http://ub.colortex.cn

memset(a, 0, sizeof a);
来源：http://or.jctech888.com.cn

[S27] C：定义常量
来源：http://bt.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://dq.szsharing.cn

[S28] C：静态变量
来源：http://ul.muxihuayi.cn

static int counter = 0;
来源：http://ru.huixiangedu.cn

[S29] C：变参函数
来源：http://nx.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ny.bjjhwx.cn

[S30] C：头文件保护
来源：http://wy.yuntaijiaju.cn

#ifndef X_H
来源：http://ia.shxzskj.cn

#define X_H
来源：http://mh.bookmarksfly.cn

#endif
来源：http://ff.asd995.cn

[S31] C++：Hello World
来源：http://wv.521024.cn

#include <iostream>
来源：http://qc.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://vp.jianghongdianzi.cn

[S32] C++：字符串
来源：http://ku.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://bs.nszjky.cn

[S33] C++：vector 增删
来源：http://hb.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dp.colortex.cn

[S34] C++：遍历 vector
来源：http://oq.yuntaijiaju.cn

for (auto &x : v) { std::cout << x; }
来源：http://ao.huixinmuqiang.cn

[S35] C++：map
来源：http://uu.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bh.jctech888.com.cn

[S36] C++：unordered_map
来源：http://si.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ex.chemitech.net.cn

[S37] C++：set
来源：http://am.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zf.chemitech.net.cn

[S38] C++：排序
来源：http://xs.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://vj.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://at.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rd.521024.cn

[S40] C++：查找元素
来源：http://dn.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://se.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://cd.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lc.colortex.cn

[S42] C++：继承与虚函数
来源：http://di.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://se.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://kt.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://kx.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://wg.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://mb.colortex.cn

[S45] C++：lambda
来源：http://qt.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://al.bjjhwx.cn

[S46] C++：函数模板
来源：http://zx.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://di.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://xh.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nz.newstarts.cn

[S48] C++：逐行读文件
来源：http://mw.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kl.szsharing.cn

while (std::getline(in, line)) { }
来源：http://wk.yuntaijiaju.cn

[S49] C++：写文件
来源：http://al.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nm.newstarts.cn

[S50] C++：格式化数字
来源：http://lb.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uc.shxzskj.cn

[S51] C++：显式类型转换
来源：http://se.colortex.cn

static_cast<double>(a) / b
来源：http://oy.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://ij.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://ga.hahajie.cn

[S53] C++：移动语义
来源：http://ph.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://yl.asd995.cn

[S54] C++：异常处理
来源：http://pt.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aa.newstarts.cn

[S55] C++：结构化绑定
来源：http://iu.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kg.asd995.cn

[S56] C++：optional
来源：http://vw.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sp.hahajie.cn

[S57] C++：编译期常量
来源：http://fi.muxihuayi.cn

constexpr int N = 10;
来源：http://zy.bookmarksfly.cn

[S58] C++：命名空间
来源：http://eq.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://ss.shxzskj.cn

[S59] C++：静态断言
来源：http://ul.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bm.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://tb.9csxet.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dk.haigaiapp.cn

================================================================================
来源：http://vr.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://to.bjjhwx.cn

================================================================================
来源：http://io.asd995.cn

[T01] Kotlin：Hello World
来源：http://dt.yuexingan06.cn

println("Hello")
来源：http://yp.nszjky.cn

[T02] Kotlin：变量
来源：http://dk.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jy.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://xe.yuexingan06.cn

"值: $b"
来源：http://fs.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://uw.lnxyls.cn

val n: String? = null;  n?.length
来源：http://qf.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://di.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://os.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://rl.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://iw.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://hz.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gf.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://iu.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://mg.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://hj.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://ln.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://pe.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://se.chemitech.net.cn

[T11] Kotlin：协程
来源：http://zy.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gf.shxzukj.cn

[T12] Kotlin：解构声明
来源：http://km.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://js.shxzskj.cn

[T13] Kotlin：只读 Map
来源：http://gc.szsharing.cn

val m = mapOf("a" to 1)
来源：http://wd.yuexingan06.cn

[T14] Kotlin：循环
来源：http://xo.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://ja.szsharing.cn

[T15] Kotlin：接口
来源：http://sa.hahajie.cn

interface Shape { fun area(): Double }
来源：http://zm.yuntaijiaju.cn

[T16] Swift：Hello World
来源：http://sw.asd995.cn

print("Hello")
来源：http://so.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://us.huanxung.cn

var a = 1;  let b = 2
来源：http://vf.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://vn.yuexingan06.cn

"值: \(b)"
来源：http://fg.bookmarksfly.cn

[T19] Swift：可选绑定
来源：http://yb.huixiangedu.cn

if let n = opt { print(n) }
来源：http://zr.chemitech.net.cn

[T20] Swift：数组操作
来源：http://rf.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xq.haigaiapp.cn

[T21] Swift：遍历
来源：http://sh.shxzskj.cn

for x in a { print(x) }
来源：http://jl.szxytkj.cn

[T22] Swift：字典
来源：http://qw.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ap.jianghongdianzi.cn

[T23] Swift：函数
来源：http://gu.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ul.asd995.cn

[T24] Swift：闭包
来源：http://vm.hnjuh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ki.yuexingan06.cn

[T25] Swift：结构体
来源：http://tx.newstarts.cn

struct P { var x: Int }
来源：http://ja.9csxet.cn

[T26] Swift：类与重写
来源：http://ms.shxzukj.cn

class A: Base { override func f() {} }
来源：http://ah.panjiajie.cn

[T27] Swift：错误处理
来源：http://og.panjiajie.cn

do { try f() } catch { print(error) }
来源：http://la.shxzukj.cn

[T28] Swift：枚举
来源：http://vq.asd995.cn

enum Color { case red, green }
来源：http://zy.shtwfgs.cn

[T29] Swift：guard 提前返回
来源：http://is.szxytkj.cn

guard let x = opt else { return }
来源：http://vx.colortex.cn

[T30] Swift：协议
来源：http://fd.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://dl.muxihuayi.cn

[T31] Lua：Hello World
来源：http://ch.nszjky.cn

print("Hello")
来源：http://gd.huixiangedu.cn

[T32] Lua：局部变量
来源：http://ej.9csxet.cn

local a = 1
来源：http://xh.szsharing.cn

[T33] Lua：表（数组）
来源：http://lr.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gg.yuexingan06.cn

[T34] Lua：遍历表
来源：http://hp.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ip.shtwfgs.cn

[T35] Lua：字典表
来源：http://ec.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://uc.muxihuayi.cn

[T36] Lua：函数
来源：http://ha.hnjuh.cn

function add(a, b) return a + b end
来源：http://ik.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://go.yuexingan06.cn

"a" .. "b"
来源：http://gm.jianghongdianzi.cn

[T38] Lua：条件
来源：http://yc.huanxung.cn

if x > 0 then print("正") end
来源：http://ml.shtwfgs.cn

[T39] Lua：模式匹配
来源：http://yo.haigaiapp.cn

string.find(s, "%d+")
来源：http://ko.huixiangedu.cn

[T40] Lua：元表
来源：http://rg.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://aa.colortex.cn

[T41] Perl：Hello World
来源：http://jp.shxzskj.cn

print "Hello\n";
来源：http://uj.nszjky.cn

[T42] Perl：变量类型
来源：http://mz.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gw.shxzskj.cn


<!-- 参考信息 -->