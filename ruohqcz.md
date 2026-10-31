代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://dr.colortex.cn

[R36] 并发执行多个任务
来源：http://ie.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uk.jianghongdianzi.cn

[R37] 把输出赋给变量
来源：http://od.huanxung.cn

files=$(ls -1)
来源：http://tw.shxzukj.cn

[R38] 管道串联
来源：http://aw.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://zr.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://oz.muxihuayi.cn

cmd > out.log 2>&1
来源：http://kw.shxzukj.cn

[R40] 追加写日志
来源：http://cb.lnxyls.cn

echo "log" >> out.log
来源：http://bf.newstarts.cn

[R41] 丢弃输出
来源：http://iw.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://mb.chemitech.net.cn

[R42] 输入重定向
来源：http://pn.hahajie.cn

wc -l < a.txt
来源：http://mc.haigaiapp.cn

[R43] 按名字查找文件
来源：http://lh.shxzukj.cn

find . -name "*.log" -type f
来源：http://ph.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://kx.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://cj.bookmarksfly.cn

[R45] 批量删除
来源：http://kk.asd995.cn

find . -name "*.tmp" -delete
来源：http://vm.newstarts.cn

[R46] 递归替换文件内容
来源：http://pz.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gq.huixiangedu.cn

[R47] sed 单行替换
来源：http://lf.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qi.colortex.cn

[R48] awk 取指定列
来源：http://hu.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://jj.jctech888.com.cn

[R49] awk 带条件
来源：http://dm.jianghongdianzi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yq.chemitech.net.cn

[R50] awk 求和
来源：http://py.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pv.haigaiapp.cn

[R51] 排序去重取前几
来源：http://us.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hx.hnjuh.cn

[R52] 统计行数
来源：http://ka.bjjhwx.cn

wc -l a.txt
来源：http://qg.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://yt.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ma.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://mx.huixiangedu.cn

diff a.txt b.txt
来源：http://jt.bookmarksfly.cn

[R55] 压缩与解压
来源：http://ef.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ys.haigaiapp.cn

[R56] 远程拷贝
来源：http://qy.huixinmuqiang.cn

scp file user@host:/path/
来源：http://gf.wgjwhj.cn

[R57] 远程执行命令
来源：http://gm.huanxung.cn

ssh user@host 'uptime'
来源：http://ep.lnxyls.cn

[R58] 下载文件
来源：http://yz.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xi.shxzskj.cn

[R59] 发 POST JSON
来源：http://sm.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ye.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://qq.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mc.chemitech.net.cn

[R61] 磁盘占用
来源：http://en.huanxung.cn

df -h;  du -sh *
来源：http://ny.huixinmuqiang.cn

[R62] 找最占空间的文件
来源：http://fi.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://bu.shxzskj.cn

[R63] 内存与进程
来源：http://gr.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://jd.hahajie.cn

[R64] 结束进程
来源：http://pp.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://hh.muxihuayi.cn

[R65] 查看端口占用
来源：http://zu.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ap.nicolike.cn

[R66] 定时任务
来源：http://sp.hnjuh.cn

crontab -e;  crontab -l
来源：http://ru.hahajie.cn

[R67] 生成随机十六进制串
来源：http://jc.asd995.cn

openssl rand -hex 16
来源：http://aw.szsharing.cn

[R68] 计算文件校验值
来源：http://lg.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nr.panjiajie.cn

[R69] 生成随机密码
来源：http://ok.jctech888.com.cn

head -c 16 /dev/urandom | base64
来源：http://hg.hahajie.cn

[R70] 时间戳与互转
来源：http://ul.newstarts.cn

date +%s;  date -d @1700000000
来源：http://xi.521024.cn

[R71] 日期格式化
来源：http://ic.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://so.szsharing.cn

[R72] 等待端口就绪
来源：http://ow.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uu.haigaiapp.cn

[R73] 分割大日志
来源：http://nq.shxzskj.cn

split -l 1000 big.log part_
来源：http://xx.chemitech.net.cn

[R74] 批量重命名
来源：http://zz.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hi.muxihuayi.cn

[R75] 导出环境变量
来源：http://hx.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://fx.bookmarksfly.cn

[R76] 使用临时文件
来源：http://tf.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gn.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://mw.nicolike.cn

read -rp "请输入: " ans
来源：http://lz.lnxyls.cn

[R78] 交互式菜单
来源：http://yb.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zv.gzmigu.cn

[R79] 解析命令行选项
来源：http://tc.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fs.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://lg.huixiangedu.cn

time ./run.sh
来源：http://am.szsharing.cn

================================================================================
来源：http://an.jianghongdianzi.cn

S. C / C++ 专题
来源：http://mc.huixiangedu.cn

================================================================================
来源：http://ln.jctech888.com.cn

[S01] C：Hello World
来源：http://ss.huixinmuqiang.cn

#include <stdio.h>
来源：http://gc.huixiangedu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qx.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://ac.gzmigu.cn

int a = 10; printf("%d\n", a);
来源：http://sr.jctech888.com.cn

[S03] C：读入整数
来源：http://og.huanxung.cn

int x; scanf("%d", &x);
来源：http://my.shtwfgs.cn

[S04] C：字符串复制
来源：http://uj.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sl.shxzskj.cn

[S05] C：字符串长度
来源：http://ns.shxzukj.cn

strlen(s)
来源：http://gz.nszjky.cn

[S06] C：字符串比较
来源：http://pz.newstarts.cn

strcmp(a, b) == 0
来源：http://ah.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://cx.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jm.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://zl.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://it.panjiajie.cn

[S09] C：结构体定义与初始化
来源：http://hc.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yk.shxzskj.cn

[S10] C：指针与解引用
来源：http://mo.huanxung.cn

int *p = &a;  *p = 5;
来源：http://dd.chemitech.net.cn

[S11] C：逐行读文件
来源：http://xt.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://ju.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://iw.haigaiapp.cn

fclose(f);
来源：http://xf.szxytkj.cn

[S12] C：写文件
来源：http://ib.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cm.hahajie.cn

[S13] C：宏定义
来源：http://pn.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://be.wgjwhj.cn

[S14] C：枚举
来源：http://xg.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://vx.huixiangedu.cn

[S15] C：类型转换
来源：http://ro.panjiajie.cn

(double) a / b
来源：http://an.yuexingan06.cn

[S16] C：位操作置位
来源：http://zc.yuntaijiaju.cn

x |= (1 << 3);
来源：http://al.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://zx.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://np.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://eg.szsharing.cn

int main(int argc, char **argv)
来源：http://pu.muxihuayi.cn

[S19] C：快速排序
来源：http://oi.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tc.nszjky.cn

[S20] C：二分查找
来源：http://dc.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qr.asd995.cn

[S21] C：字符类别判断
来源：http://zn.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yo.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://vz.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oo.chemitech.net.cn

[S23] C：随机数
来源：http://lz.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sv.chemitech.net.cn

[S24] C：获取本地时间
来源：http://yn.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sh.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://qz.asd995.cn

memcpy(dst, src, n);
来源：http://uf.shxzskj.cn

[S26] C：内存清零
来源：http://xt.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://gs.huixiangedu.cn

[S27] C：定义常量
来源：http://cb.9csxet.cn

const double PI = 3.14159;
来源：http://nw.muxihuayi.cn

[S28] C：静态变量
来源：http://ls.jctech888.com.cn

static int counter = 0;
来源：http://hy.lnxyls.cn

[S29] C：变参函数
来源：http://qs.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ir.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://ov.lnxyls.cn

#ifndef X_H
来源：http://ui.huixiangedu.cn

#define X_H
来源：http://zq.chemitech.net.cn

#endif
来源：http://gz.hnjuh.cn

[S31] C++：Hello World
来源：http://ey.haigaiapp.cn

#include <iostream>
来源：http://lz.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://tt.huanxung.cn

[S32] C++：字符串
来源：http://wh.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://dm.lnxyls.cn

[S33] C++：vector 增删
来源：http://as.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lo.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://nt.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://pr.huixinmuqiang.cn

[S35] C++：map
来源：http://vy.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yv.chemitech.net.cn

[S36] C++：unordered_map
来源：http://op.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qj.shxzukj.cn

[S37] C++：set
来源：http://oz.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bi.muxihuayi.cn

[S38] C++：排序
来源：http://nx.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://jy.gzmigu.cn

[S39] C++：自定义比较器排序
来源：http://tn.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gr.gzmigu.cn

[S40] C++：查找元素
来源：http://uz.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uz.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://jd.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yo.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://xv.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://fk.shxzukj.cn

[S43] C++：智能指针
来源：http://mh.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://tv.huixiangedu.cn

[S44] C++：引用传参
来源：http://ii.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://yn.huixiangedu.cn

[S45] C++：lambda
来源：http://ws.hahajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nb.nszjky.cn

[S46] C++：函数模板
来源：http://gj.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fd.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://gj.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qo.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://ei.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://te.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://px.nszjky.cn

[S49] C++：写文件
来源：http://er.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ga.chemitech.net.cn

[S50] C++：格式化数字
来源：http://hv.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ia.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://vi.szxytkj.cn

static_cast<double>(a) / b
来源：http://yp.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://yj.colortex.cn

int size() const noexcept { return n_; }
来源：http://sm.shxzskj.cn

[S53] C++：移动语义
来源：http://zp.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://gg.wgjwhj.cn

[S54] C++：异常处理
来源：http://ig.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rp.lnxyls.cn

[S55] C++：结构化绑定
来源：http://ff.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yp.bookmarksfly.cn

[S56] C++：optional
来源：http://ms.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ag.hnjuh.cn

[S57] C++：编译期常量
来源：http://uz.colortex.cn

constexpr int N = 10;
来源：http://bq.gzmigu.cn

[S58] C++：命名空间
来源：http://oh.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://rn.chemitech.net.cn

[S59] C++：静态断言
来源：http://ed.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mo.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://zd.9csxet.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oy.muxihuayi.cn

================================================================================
来源：http://ro.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jc.shtwfgs.cn

================================================================================
来源：http://lh.asd995.cn

[T01] Kotlin：Hello World
来源：http://wi.haigaiapp.cn

println("Hello")
来源：http://rw.colortex.cn

[T02] Kotlin：变量
来源：http://mv.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nf.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://zy.shxzukj.cn

"值: $b"
来源：http://ki.shxzskj.cn

[T04] Kotlin：空安全
来源：http://yc.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://bk.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://qf.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jw.nicolike.cn

[T06] Kotlin：集合映射
来源：http://ih.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pq.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://co.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xr.colortex.cn

[T08] Kotlin：数据类
来源：http://to.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://sh.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://cl.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://ou.asd995.cn

[T10] Kotlin：默认参数
来源：http://jy.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://im.jctech888.com.cn

[T11] Kotlin：协程
来源：http://wi.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cr.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://ra.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://yu.521024.cn

[T13] Kotlin：只读 Map
来源：http://jv.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://em.bjjhwx.cn

[T14] Kotlin：循环
来源：http://xx.szxytkj.cn

for (i in 1..10) println(i)
来源：http://ub.panjiajie.cn

[T15] Kotlin：接口
来源：http://lf.bjjhwx.cn

interface Shape { fun area(): Double }
来源：http://pj.hahajie.cn

[T16] Swift：Hello World
来源：http://hx.haigaiapp.cn

print("Hello")
来源：http://yz.521024.cn

[T17] Swift：变量与常量
来源：http://xi.chemitech.net.cn

var a = 1;  let b = 2
来源：http://kg.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://bn.yuntaijiaju.cn

"值: \(b)"
来源：http://yk.panjiajie.cn

[T19] Swift：可选绑定
来源：http://mm.colortex.cn

if let n = opt { print(n) }
来源：http://wy.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://cl.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://so.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://ve.chemitech.net.cn

for x in a { print(x) }
来源：http://hc.szsharing.cn

[T22] Swift：字典
来源：http://ts.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sv.bookmarksfly.cn

[T23] Swift：函数
来源：http://es.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ti.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://vx.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zk.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://xf.hnjuh.cn

struct P { var x: Int }
来源：http://gj.nszjky.cn

[T26] Swift：类与重写
来源：http://ve.szsharing.cn

class A: Base { override func f() {} }
来源：http://sr.shtwfgs.cn

[T27] Swift：错误处理
来源：http://wr.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://yj.jctech888.com.cn

[T28] Swift：枚举
来源：http://vt.huixinmuqiang.cn

enum Color { case red, green }
来源：http://dx.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://tt.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://fc.muxihuayi.cn

[T30] Swift：协议
来源：http://fn.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://im.szsharing.cn

[T31] Lua：Hello World
来源：http://sc.newstarts.cn

print("Hello")
来源：http://wu.bjjhwx.cn

[T32] Lua：局部变量
来源：http://xn.nszjky.cn

local a = 1
来源：http://aa.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://pm.chemitech.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ak.nszjky.cn

[T34] Lua：遍历表
来源：http://uf.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://st.colortex.cn

[T35] Lua：字典表
来源：http://jr.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://sr.yuntaijiaju.cn

[T36] Lua：函数
来源：http://dx.huixiangedu.cn

function add(a, b) return a + b end
来源：http://go.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://jv.asd995.cn

"a" .. "b"
来源：http://ty.yuexingan06.cn

[T38] Lua：条件
来源：http://ff.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://bs.yuntaijiaju.cn


<!-- 参考信息 -->