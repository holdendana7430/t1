代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://ag.panjiajie.cn

[R36] 并发执行多个任务
来源：http://mb.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bk.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://yf.yuexingan06.cn

files=$(ls -1)
来源：http://sm.hnjuh.cn

[R38] 管道串联
来源：http://fp.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://lp.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://iu.huixiangedu.cn

cmd > out.log 2>&1
来源：http://ut.shxzukj.cn

[R40] 追加写日志
来源：http://en.huixinmuqiang.cn

echo "log" >> out.log
来源：http://uj.hahajie.cn

[R41] 丢弃输出
来源：http://tk.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://yx.newstarts.cn

[R42] 输入重定向
来源：http://dc.nicolike.cn

wc -l < a.txt
来源：http://zk.haigaiapp.cn

[R43] 按名字查找文件
来源：http://hq.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://wa.huanxung.cn

[R44] 按修改时间查找
来源：http://nm.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://mq.szsharing.cn

[R45] 批量删除
来源：http://vf.colortex.cn

find . -name "*.tmp" -delete
来源：http://vs.nszjky.cn

[R46] 递归替换文件内容
来源：http://hb.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vf.huixiangedu.cn

[R47] sed 单行替换
来源：http://xt.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gk.panjiajie.cn

[R48] awk 取指定列
来源：http://wb.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://na.lnxyls.cn

[R49] awk 带条件
来源：http://oe.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ia.wgjwhj.cn

[R50] awk 求和
来源：http://cy.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xw.yuexingan06.cn

[R51] 排序去重取前几
来源：http://wc.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vs.wgjwhj.cn

[R52] 统计行数
来源：http://qm.haigaiapp.cn

wc -l a.txt
来源：http://cn.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://qz.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zb.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://ty.hnjuh.cn

diff a.txt b.txt
来源：http://cm.huixiangedu.cn

[R55] 压缩与解压
来源：http://la.jctech888.com.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dk.hahajie.cn

[R56] 远程拷贝
来源：http://lo.shxzukj.cn

scp file user@host:/path/
来源：http://vb.huanxung.cn

[R57] 远程执行命令
来源：http://uf.szsharing.cn

ssh user@host 'uptime'
来源：http://vj.muxihuayi.cn

[R58] 下载文件
来源：http://yc.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hn.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://oe.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rt.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://ok.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xl.shxzskj.cn

[R61] 磁盘占用
来源：http://za.panjiajie.cn

df -h;  du -sh *
来源：http://cg.muxihuayi.cn

[R62] 找最占空间的文件
来源：http://uh.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://hc.szsharing.cn

[R63] 内存与进程
来源：http://eo.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://ki.asd995.cn

[R64] 结束进程
来源：http://qf.nicolike.cn

kill -9 $(pgrep -f app.py)
来源：http://sq.bookmarksfly.cn

[R65] 查看端口占用
来源：http://cq.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ww.shxzskj.cn

[R66] 定时任务
来源：http://jt.521024.cn

crontab -e;  crontab -l
来源：http://jf.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://on.yuntaijiaju.cn

openssl rand -hex 16
来源：http://im.9csxet.cn

[R68] 计算文件校验值
来源：http://kn.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bg.bjjhwx.cn

[R69] 生成随机密码
来源：http://my.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://os.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://sd.huixiangedu.cn

date +%s;  date -d @1700000000
来源：http://fo.yuexingan06.cn

[R71] 日期格式化
来源：http://ei.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ab.huixiangedu.cn

[R72] 等待端口就绪
来源：http://vl.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sp.szsharing.cn

[R73] 分割大日志
来源：http://tl.muxihuayi.cn

split -l 1000 big.log part_
来源：http://dy.huixiangedu.cn

[R74] 批量重命名
来源：http://an.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tw.lnxyls.cn

[R75] 导出环境变量
来源：http://ba.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://kq.bjjhwx.cn

[R76] 使用临时文件
来源：http://nr.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vr.asd995.cn

[R77] 读取用户输入
来源：http://mn.lnxyls.cn

read -rp "请输入: " ans
来源：http://mm.szsharing.cn

[R78] 交互式菜单
来源：http://mg.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uf.lnxyls.cn

[R79] 解析命令行选项
来源：http://ft.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ha.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://qj.yuexingan06.cn

time ./run.sh
来源：http://eg.hahajie.cn

================================================================================
来源：http://yx.521024.cn

S. C / C++ 专题
来源：http://io.shtwfgs.cn

================================================================================
来源：http://ss.colortex.cn

[S01] C：Hello World
来源：http://xs.chemitech.net.cn

#include <stdio.h>
来源：http://hq.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://eq.asd995.cn

[S02] C：变量与格式化输出
来源：http://ma.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://ni.asd995.cn

[S03] C：读入整数
来源：http://it.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://fj.yuexingan06.cn

[S04] C：字符串复制
来源：http://lt.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dg.szsharing.cn

[S05] C：字符串长度
来源：http://xr.nszjky.cn

strlen(s)
来源：http://ja.wgjwhj.cn

[S06] C：字符串比较
来源：http://nn.szxytkj.cn

strcmp(a, b) == 0
来源：http://go.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://ui.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ex.9csxet.cn

[S08] C：动态内存分配与释放
来源：http://lm.chemitech.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cb.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://gf.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vp.haigaiapp.cn

[S10] C：指针与解引用
来源：http://xs.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://fq.newstarts.cn

[S11] C：逐行读文件
来源：http://sy.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://nd.nicolike.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qe.muxihuayi.cn

fclose(f);
来源：http://bl.521024.cn

[S12] C：写文件
来源：http://nc.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ms.9csxet.cn

[S13] C：宏定义
来源：http://bc.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hk.haigaiapp.cn

[S14] C：枚举
来源：http://rn.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://io.chemitech.net.cn

[S15] C：类型转换
来源：http://un.yuntaijiaju.cn

(double) a / b
来源：http://uj.asd995.cn

[S16] C：位操作置位
来源：http://ve.wgjwhj.cn

x |= (1 << 3);
来源：http://pg.nicolike.cn

[S17] C：安全拼接字符串
来源：http://az.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://my.9csxet.cn

[S18] C：命令行参数
来源：http://vc.shtwfgs.cn

int main(int argc, char **argv)
来源：http://fw.gzmigu.cn

[S19] C：快速排序
来源：http://ot.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ae.yuntaijiaju.cn

[S20] C：二分查找
来源：http://pz.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cg.hahajie.cn

[S21] C：字符类别判断
来源：http://rc.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jh.jctech888.com.cn

[S22] C：字符串转数字
来源：http://hb.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qu.shxzukj.cn

[S23] C：随机数
来源：http://fs.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mp.shxzskj.cn

[S24] C：获取本地时间
来源：http://ws.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ex.wgjwhj.cn

[S25] C：内存拷贝
来源：http://xh.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://mr.szxytkj.cn

[S26] C：内存清零
来源：http://uk.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://cy.shxzskj.cn

[S27] C：定义常量
来源：http://pc.jianghongdianzi.cn

const double PI = 3.14159;
来源：http://fz.hahajie.cn

[S28] C：静态变量
来源：http://nw.muxihuayi.cn

static int counter = 0;
来源：http://el.asd995.cn

[S29] C：变参函数
来源：http://qj.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zf.9csxet.cn

[S30] C：头文件保护
来源：http://le.bookmarksfly.cn

#ifndef X_H
来源：http://nm.newstarts.cn

#define X_H
来源：http://uq.muxihuayi.cn

#endif
来源：http://hy.asd995.cn

[S31] C++：Hello World
来源：http://gj.shxzskj.cn

#include <iostream>
来源：http://se.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://hv.newstarts.cn

[S32] C++：字符串
来源：http://kb.521024.cn

std::string s = "hi";  s += "!";
来源：http://fd.gzmigu.cn

[S33] C++：vector 增删
来源：http://gn.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ej.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://ni.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://mo.9csxet.cn

[S35] C++：map
来源：http://te.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://va.szsharing.cn

[S36] C++：unordered_map
来源：http://ly.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nq.haigaiapp.cn

[S37] C++：set
来源：http://zx.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fy.shxzukj.cn

[S38] C++：排序
来源：http://vx.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://qc.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://hj.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kb.wgjwhj.cn

[S40] C++：查找元素
来源：http://uk.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cp.hahajie.cn

[S41] C++：类与构造函数
来源：http://if.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lw.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://fr.521024.cn

class B : public Base { public: void f() override {} };
来源：http://ze.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://ty.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://lw.chemitech.net.cn

[S44] C++：引用传参
来源：http://aa.lnxyls.cn

void inc(int &x) { ++x; }
来源：http://ki.nicolike.cn

[S45] C++：lambda
来源：http://is.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cs.chemitech.net.cn

[S46] C++：函数模板
来源：http://ux.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rp.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://gj.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nu.szxytkj.cn

[S48] C++：逐行读文件
来源：http://fm.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ym.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://ic.szsharing.cn

[S49] C++：写文件
来源：http://qp.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nc.szsharing.cn

[S50] C++：格式化数字
来源：http://pm.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lt.shxzukj.cn

[S51] C++：显式类型转换
来源：http://kw.hahajie.cn

static_cast<double>(a) / b
来源：http://tm.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://yl.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://bs.jctech888.com.cn

[S53] C++：移动语义
来源：http://ok.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://ji.hnjuh.cn

[S54] C++：异常处理
来源：http://ti.chemitech.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bq.szxytkj.cn

[S55] C++：结构化绑定
来源：http://ll.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kn.huixiangedu.cn

[S56] C++：optional
来源：http://wj.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://si.huixinmuqiang.cn

[S57] C++：编译期常量
来源：http://zu.panjiajie.cn

constexpr int N = 10;
来源：http://pg.szxytkj.cn

[S58] C++：命名空间
来源：http://is.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://vj.hahajie.cn

[S59] C++：静态断言
来源：http://mc.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rz.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://wm.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rr.jianghongdianzi.cn

================================================================================
来源：http://bn.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gz.huixinmuqiang.cn

================================================================================
来源：http://tl.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://ua.haigaiapp.cn

println("Hello")
来源：http://pd.shtwfgs.cn

[T02] Kotlin：变量
来源：http://gz.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ma.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://ag.yuntaijiaju.cn

"值: $b"
来源：http://rw.huanxung.cn

[T04] Kotlin：空安全
来源：http://uf.colortex.cn

val n: String? = null;  n?.length
来源：http://bq.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://em.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xe.nszjky.cn

[T06] Kotlin：集合映射
来源：http://xd.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://uh.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://ku.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ud.hahajie.cn

[T08] Kotlin：数据类
来源：http://ou.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://xz.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://hf.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://qs.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://ft.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://op.wgjwhj.cn

[T11] Kotlin：协程
来源：http://wo.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ay.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://iq.gzmigu.cn

val (a, b) = Pair(1, 2)
来源：http://wa.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://iv.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://gw.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://rl.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://uu.shtwfgs.cn

[T15] Kotlin：接口
来源：http://ta.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://xw.nicolike.cn

[T16] Swift：Hello World
来源：http://bj.szsharing.cn

print("Hello")
来源：http://ty.gzmigu.cn

[T17] Swift：变量与常量
来源：http://bs.nszjky.cn

var a = 1;  let b = 2
来源：http://iy.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://gg.nszjky.cn

"值: \(b)"
来源：http://oi.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://fe.nszjky.cn

if let n = opt { print(n) }
来源：http://by.huixiangedu.cn

[T20] Swift：数组操作
来源：http://rb.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yh.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://xs.jctech888.com.cn

for x in a { print(x) }
来源：http://yi.hnjuh.cn

[T22] Swift：字典
来源：http://aw.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ci.nszjky.cn

[T23] Swift：函数
来源：http://on.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wp.shxzskj.cn

[T24] Swift：闭包
来源：http://ch.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uy.szsharing.cn

[T25] Swift：结构体
来源：http://vy.gzmigu.cn

struct P { var x: Int }
来源：http://bx.szxytkj.cn

[T26] Swift：类与重写
来源：http://wk.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://li.newstarts.cn

[T27] Swift：错误处理
来源：http://qo.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://fi.chemitech.net.cn

[T28] Swift：枚举
来源：http://wi.huixinmuqiang.cn

enum Color { case red, green }
来源：http://yl.hahajie.cn

[T29] Swift：guard 提前返回
来源：http://oh.chemitech.net.cn

guard let x = opt else { return }
来源：http://hz.shtwfgs.cn

[T30] Swift：协议
来源：http://nb.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://zd.shxzukj.cn

[T31] Lua：Hello World
来源：http://yd.wgjwhj.cn

print("Hello")
来源：http://mq.lnxyls.cn

[T32] Lua：局部变量
来源：http://di.bjjhwx.cn

local a = 1
来源：http://ft.hahajie.cn

[T33] Lua：表（数组）
来源：http://jt.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cr.nicolike.cn

[T34] Lua：遍历表
来源：http://ws.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://we.panjiajie.cn

[T35] Lua：字典表
来源：http://ar.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://rv.huanxung.cn

[T36] Lua：函数
来源：http://ih.lnxyls.cn

function add(a, b) return a + b end
来源：http://tm.nszjky.cn

[T37] Lua：字符串拼接
来源：http://tf.huixiangedu.cn

"a" .. "b"
来源：http://uc.colortex.cn

[T38] Lua：条件
来源：http://xs.shxzskj.cn

if x > 0 then print("正") end
来源：http://ws.hahajie.cn


<!-- 参考信息 -->