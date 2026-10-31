代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://ai.shxzskj.cn

[R36] 并发执行多个任务
来源：http://qa.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ds.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://sz.lnxyls.cn

files=$(ls -1)
来源：http://rx.hnjuh.cn

[R38] 管道串联
来源：http://di.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://dl.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://ot.shxzukj.cn

cmd > out.log 2>&1
来源：http://ad.yuntaijiaju.cn

[R40] 追加写日志
来源：http://dc.newstarts.cn

echo "log" >> out.log
来源：http://ew.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://wj.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://uj.huixinmuqiang.cn

[R42] 输入重定向
来源：http://ju.shxzskj.cn

wc -l < a.txt
来源：http://tw.szsharing.cn

[R43] 按名字查找文件
来源：http://pr.muxihuayi.cn

find . -name "*.log" -type f
来源：http://nf.chemitech.net.cn

[R44] 按修改时间查找
来源：http://jm.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://gh.colortex.cn

[R45] 批量删除
来源：http://lr.newstarts.cn

find . -name "*.tmp" -delete
来源：http://xx.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://jc.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dt.shtwfgs.cn

[R47] sed 单行替换
来源：http://hi.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://iw.szsharing.cn

[R48] awk 取指定列
来源：http://mf.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://jo.haigaiapp.cn

[R49] awk 带条件
来源：http://ii.chemitech.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wx.szsharing.cn

[R50] awk 求和
来源：http://kf.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kd.muxihuayi.cn

[R51] 排序去重取前几
来源：http://gv.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://de.nicolike.cn

[R52] 统计行数
来源：http://we.nszjky.cn

wc -l a.txt
来源：http://qd.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://vz.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://by.nicolike.cn

[R54] 比较两个文件
来源：http://cs.asd995.cn

diff a.txt b.txt
来源：http://nb.shtwfgs.cn

[R55] 压缩与解压
来源：http://rl.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hg.wgjwhj.cn

[R56] 远程拷贝
来源：http://nc.521024.cn

scp file user@host:/path/
来源：http://du.asd995.cn

[R57] 远程执行命令
来源：http://lz.shxzskj.cn

ssh user@host 'uptime'
来源：http://tw.asd995.cn

[R58] 下载文件
来源：http://rk.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wy.newstarts.cn

[R59] 发 POST JSON
来源：http://vf.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ij.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://nx.huanxung.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ki.shtwfgs.cn

[R61] 磁盘占用
来源：http://pi.wgjwhj.cn

df -h;  du -sh *
来源：http://tl.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://sm.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://uc.huixinmuqiang.cn

[R63] 内存与进程
来源：http://pu.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://ca.nszjky.cn

[R64] 结束进程
来源：http://mt.hnjuh.cn

kill -9 $(pgrep -f app.py)
来源：http://yu.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://yg.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wy.yuexingan06.cn

[R66] 定时任务
来源：http://ng.szxytkj.cn

crontab -e;  crontab -l
来源：http://wp.jctech888.com.cn

[R67] 生成随机十六进制串
来源：http://bs.gzmigu.cn

openssl rand -hex 16
来源：http://zm.gzmigu.cn

[R68] 计算文件校验值
来源：http://en.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ow.hnjuh.cn

[R69] 生成随机密码
来源：http://it.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://xt.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://of.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://vq.yuexingan06.cn

[R71] 日期格式化
来源：http://nb.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rv.huixiangedu.cn

[R72] 等待端口就绪
来源：http://sz.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ji.newstarts.cn

[R73] 分割大日志
来源：http://ci.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://gz.newstarts.cn

[R74] 批量重命名
来源：http://au.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://el.newstarts.cn

[R75] 导出环境变量
来源：http://ia.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://tr.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://dl.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nw.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://jk.huanxung.cn

read -rp "请输入: " ans
来源：http://wt.521024.cn

[R78] 交互式菜单
来源：http://hz.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mi.bjjhwx.cn

[R79] 解析命令行选项
来源：http://jd.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uu.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://fd.chemitech.net.cn

time ./run.sh
来源：http://xx.newstarts.cn

================================================================================
来源：http://hp.wgjwhj.cn

S. C / C++ 专题
来源：http://cs.shtwfgs.cn

================================================================================
来源：http://ff.huanxung.cn

[S01] C：Hello World
来源：http://se.lnxyls.cn

#include <stdio.h>
来源：http://gh.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sn.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://sa.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://iv.jianghongdianzi.cn

[S03] C：读入整数
来源：http://sv.9csxet.cn

int x; scanf("%d", &x);
来源：http://vu.muxihuayi.cn

[S04] C：字符串复制
来源：http://jz.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ss.521024.cn

[S05] C：字符串长度
来源：http://xg.nicolike.cn

strlen(s)
来源：http://zz.asd995.cn

[S06] C：字符串比较
来源：http://wn.colortex.cn

strcmp(a, b) == 0
来源：http://gs.huanxung.cn

[S07] C：数组遍历求和
来源：http://uo.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ap.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://qw.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ym.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://vb.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ik.huixiangedu.cn

[S10] C：指针与解引用
来源：http://km.9csxet.cn

int *p = &a;  *p = 5;
来源：http://yn.nicolike.cn

[S11] C：逐行读文件
来源：http://qx.haigaiapp.cn

FILE *f = fopen("a.txt", "r");
来源：http://ll.hnjuh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vt.yuntaijiaju.cn

fclose(f);
来源：http://rd.yuntaijiaju.cn

[S12] C：写文件
来源：http://yh.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yy.shxzskj.cn

[S13] C：宏定义
来源：http://ce.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ic.huixinmuqiang.cn

[S14] C：枚举
来源：http://yk.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://cq.szxytkj.cn

[S15] C：类型转换
来源：http://qb.jianghongdianzi.cn

(double) a / b
来源：http://hu.haigaiapp.cn

[S16] C：位操作置位
来源：http://no.szsharing.cn

x |= (1 << 3);
来源：http://if.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://fi.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ep.colortex.cn

[S18] C：命令行参数
来源：http://co.huixinmuqiang.cn

int main(int argc, char **argv)
来源：http://ax.newstarts.cn

[S19] C：快速排序
来源：http://bx.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gi.newstarts.cn

[S20] C：二分查找
来源：http://fy.hahajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qa.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://ux.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gg.shxzskj.cn

[S22] C：字符串转数字
来源：http://xu.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kd.szsharing.cn

[S23] C：随机数
来源：http://jr.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vz.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://dq.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gd.lnxyls.cn

[S25] C：内存拷贝
来源：http://pc.gzmigu.cn

memcpy(dst, src, n);
来源：http://yr.shxzukj.cn

[S26] C：内存清零
来源：http://yp.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://jx.wgjwhj.cn

[S27] C：定义常量
来源：http://qp.szsharing.cn

const double PI = 3.14159;
来源：http://vt.wgjwhj.cn

[S28] C：静态变量
来源：http://fx.yuexingan06.cn

static int counter = 0;
来源：http://mb.jianghongdianzi.cn

[S29] C：变参函数
来源：http://du.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rq.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://ps.hnjuh.cn

#ifndef X_H
来源：http://xa.huixinmuqiang.cn

#define X_H
来源：http://cj.yuexingan06.cn

#endif
来源：http://oy.yuexingan06.cn

[S31] C++：Hello World
来源：http://zy.wgjwhj.cn

#include <iostream>
来源：http://sk.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://kd.9csxet.cn

[S32] C++：字符串
来源：http://ft.huixinmuqiang.cn

std::string s = "hi";  s += "!";
来源：http://jm.muxihuayi.cn

[S33] C++：vector 增删
来源：http://yh.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tr.szxytkj.cn

[S34] C++：遍历 vector
来源：http://re.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://kh.asd995.cn

[S35] C++：map
来源：http://mc.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://db.shxzukj.cn

[S36] C++：unordered_map
来源：http://jk.9csxet.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rx.bjjhwx.cn

[S37] C++：set
来源：http://oa.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://by.shtwfgs.cn

[S38] C++：排序
来源：http://ty.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://vq.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://wf.huixinmuqiang.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iz.haigaiapp.cn

[S40] C++：查找元素
来源：http://rj.jianghongdianzi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xt.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://iy.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vu.521024.cn

[S42] C++：继承与虚函数
来源：http://is.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://sf.asd995.cn

[S43] C++：智能指针
来源：http://rw.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://ku.nszjky.cn

[S44] C++：引用传参
来源：http://tn.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://xq.lnxyls.cn

[S45] C++：lambda
来源：http://mb.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ms.chemitech.net.cn

[S46] C++：函数模板
来源：http://um.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wh.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://tt.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://es.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://gp.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jl.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://hj.colortex.cn

[S49] C++：写文件
来源：http://zp.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bj.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://um.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ij.colortex.cn

[S51] C++：显式类型转换
来源：http://ax.huanxung.cn

static_cast<double>(a) / b
来源：http://lz.521024.cn

[S52] C++：const 与 noexcept
来源：http://ke.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://hu.haigaiapp.cn

[S53] C++：移动语义
来源：http://lj.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://kd.hahajie.cn

[S54] C++：异常处理
来源：http://vx.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sg.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://ol.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jb.wgjwhj.cn

[S56] C++：optional
来源：http://hg.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://er.huixiangedu.cn

[S57] C++：编译期常量
来源：http://au.haigaiapp.cn

constexpr int N = 10;
来源：http://tn.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://nn.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://au.shtwfgs.cn

[S59] C++：静态断言
来源：http://qs.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kp.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://xv.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gp.asd995.cn

================================================================================
来源：http://uh.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tn.chemitech.net.cn

================================================================================
来源：http://jz.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://wy.521024.cn

println("Hello")
来源：http://az.shxzukj.cn

[T02] Kotlin：变量
来源：http://gs.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qo.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://tg.hahajie.cn

"值: $b"
来源：http://kj.lnxyls.cn

[T04] Kotlin：空安全
来源：http://qk.shxzskj.cn

val n: String? = null;  n?.length
来源：http://gn.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://uo.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oo.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://ck.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://aj.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://ii.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vy.gzmigu.cn

[T08] Kotlin：数据类
来源：http://oi.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://xl.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://kr.hahajie.cn

fun String.exclaim() = this + "!"
来源：http://nc.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://vj.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rd.asd995.cn

[T11] Kotlin：协程
来源：http://cj.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mm.asd995.cn

[T12] Kotlin：解构声明
来源：http://eh.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://pu.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://lu.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://on.gzmigu.cn

[T14] Kotlin：循环
来源：http://rq.huanxung.cn

for (i in 1..10) println(i)
来源：http://mh.yuexingan06.cn

[T15] Kotlin：接口
来源：http://is.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://gl.szsharing.cn

[T16] Swift：Hello World
来源：http://th.yuexingan06.cn

print("Hello")
来源：http://af.bookmarksfly.cn

[T17] Swift：变量与常量
来源：http://pw.jctech888.com.cn

var a = 1;  let b = 2
来源：http://te.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://ou.9csxet.cn

"值: \(b)"
来源：http://ib.nicolike.cn

[T19] Swift：可选绑定
来源：http://kq.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://hq.haigaiapp.cn

[T20] Swift：数组操作
来源：http://yx.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://km.yuexingan06.cn

[T21] Swift：遍历
来源：http://zp.jianghongdianzi.cn

for x in a { print(x) }
来源：http://am.newstarts.cn

[T22] Swift：字典
来源：http://pl.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fh.nicolike.cn

[T23] Swift：函数
来源：http://bc.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ab.nszjky.cn

[T24] Swift：闭包
来源：http://gz.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ft.shxzukj.cn

[T25] Swift：结构体
来源：http://ko.jianghongdianzi.cn

struct P { var x: Int }
来源：http://ce.shxzskj.cn

[T26] Swift：类与重写
来源：http://zw.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://rs.521024.cn

[T27] Swift：错误处理
来源：http://bo.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://su.shxzskj.cn

[T28] Swift：枚举
来源：http://lr.bookmarksfly.cn

enum Color { case red, green }
来源：http://zp.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://uh.bjjhwx.cn

guard let x = opt else { return }
来源：http://md.szsharing.cn

[T30] Swift：协议
来源：http://ay.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://rp.9csxet.cn

[T31] Lua：Hello World
来源：http://vk.asd995.cn

print("Hello")
来源：http://ps.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://dr.521024.cn

local a = 1
来源：http://bz.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://so.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://om.shxzukj.cn

[T34] Lua：遍历表
来源：http://so.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zq.szxytkj.cn

[T35] Lua：字典表
来源：http://ul.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://jz.chemitech.net.cn

[T36] Lua：函数
来源：http://oo.muxihuayi.cn

function add(a, b) return a + b end
来源：http://bd.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://mq.bjjhwx.cn

"a" .. "b"
来源：http://ew.muxihuayi.cn

[T38] Lua：条件
来源：http://nu.szxytkj.cn

if x > 0 then print("正") end
来源：http://lj.szsharing.cn


<!-- 参考信息 -->