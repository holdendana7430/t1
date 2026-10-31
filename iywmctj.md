代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://qi.huanxung.cn

[R36] 并发执行多个任务
来源：http://mo.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fg.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://hn.wgjwhj.cn

files=$(ls -1)
来源：http://yv.bookmarksfly.cn

[R38] 管道串联
来源：http://kd.szxytkj.cn

cat a.txt | grep -i error | wc -l
来源：http://bs.colortex.cn

[R39] 重定向标准输出与错误
来源：http://xd.shtwfgs.cn

cmd > out.log 2>&1
来源：http://bb.asd995.cn

[R40] 追加写日志
来源：http://nm.szxytkj.cn

echo "log" >> out.log
来源：http://me.wgjwhj.cn

[R41] 丢弃输出
来源：http://ba.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://iu.huixiangedu.cn

[R42] 输入重定向
来源：http://jp.yuntaijiaju.cn

wc -l < a.txt
来源：http://sg.huanxung.cn

[R43] 按名字查找文件
来源：http://jl.huixiangedu.cn

find . -name "*.log" -type f
来源：http://kc.huixiangedu.cn

[R44] 按修改时间查找
来源：http://xj.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://nv.yuexingan06.cn

[R45] 批量删除
来源：http://jo.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://xy.lnxyls.cn

[R46] 递归替换文件内容
来源：http://ie.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rr.asd995.cn

[R47] sed 单行替换
来源：http://mn.bookmarksfly.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ve.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://yq.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://qu.9csxet.cn

[R49] awk 带条件
来源：http://hb.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zt.haigaiapp.cn

[R50] awk 求和
来源：http://ya.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://av.nszjky.cn

[R51] 排序去重取前几
来源：http://uf.hnjuh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gd.shxzskj.cn

[R52] 统计行数
来源：http://kp.shtwfgs.cn

wc -l a.txt
来源：http://jq.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://yi.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rw.lnxyls.cn

[R54] 比较两个文件
来源：http://uw.muxihuayi.cn

diff a.txt b.txt
来源：http://ec.panjiajie.cn

[R55] 压缩与解压
来源：http://ev.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mk.gzmigu.cn

[R56] 远程拷贝
来源：http://mp.hnjuh.cn

scp file user@host:/path/
来源：http://ui.gzmigu.cn

[R57] 远程执行命令
来源：http://tw.newstarts.cn

ssh user@host 'uptime'
来源：http://zt.yuntaijiaju.cn

[R58] 下载文件
来源：http://es.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eq.panjiajie.cn

[R59] 发 POST JSON
来源：http://mp.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://di.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://kj.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ce.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://oa.hahajie.cn

df -h;  du -sh *
来源：http://qe.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://ul.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://hn.hnjuh.cn

[R63] 内存与进程
来源：http://oe.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://xy.gzmigu.cn

[R64] 结束进程
来源：http://sv.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://cu.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://nk.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ym.huanxung.cn

[R66] 定时任务
来源：http://kn.jctech888.com.cn

crontab -e;  crontab -l
来源：http://hp.szsharing.cn

[R67] 生成随机十六进制串
来源：http://hl.haigaiapp.cn

openssl rand -hex 16
来源：http://to.gzmigu.cn

[R68] 计算文件校验值
来源：http://we.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cu.nicolike.cn

[R69] 生成随机密码
来源：http://cj.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://dk.colortex.cn

[R70] 时间戳与互转
来源：http://yj.newstarts.cn

date +%s;  date -d @1700000000
来源：http://ep.huixinmuqiang.cn

[R71] 日期格式化
来源：http://ar.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.newstarts.cn

[R72] 等待端口就绪
来源：http://va.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zn.shxzskj.cn

[R73] 分割大日志
来源：http://gh.bjjhwx.cn

split -l 1000 big.log part_
来源：http://ce.colortex.cn

[R74] 批量重命名
来源：http://gn.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tl.chemitech.net.cn

[R75] 导出环境变量
来源：http://zg.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://dy.shxzskj.cn

[R76] 使用临时文件
来源：http://kp.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vm.shxzukj.cn

[R77] 读取用户输入
来源：http://yi.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://df.haigaiapp.cn

[R78] 交互式菜单
来源：http://sr.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qh.shxzskj.cn

[R79] 解析命令行选项
来源：http://nx.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gn.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://qr.yuntaijiaju.cn

time ./run.sh
来源：http://ji.521024.cn

================================================================================
来源：http://pc.chemitech.net.cn

S. C / C++ 专题
来源：http://pm.9csxet.cn

================================================================================
来源：http://dn.hnjuh.cn

[S01] C：Hello World
来源：http://ty.nszjky.cn

#include <stdio.h>
来源：http://go.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sl.nszjky.cn

[S02] C：变量与格式化输出
来源：http://wt.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://fh.521024.cn

[S03] C：读入整数
来源：http://qm.panjiajie.cn

int x; scanf("%d", &x);
来源：http://xs.huanxung.cn

[S04] C：字符串复制
来源：http://kn.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://iv.szxytkj.cn

[S05] C：字符串长度
来源：http://wj.shtwfgs.cn

strlen(s)
来源：http://ds.shxzskj.cn

[S06] C：字符串比较
来源：http://ra.shtwfgs.cn

strcmp(a, b) == 0
来源：http://yu.jctech888.com.cn

[S07] C：数组遍历求和
来源：http://qu.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qo.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://xc.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://my.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://nr.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://co.panjiajie.cn

[S10] C：指针与解引用
来源：http://ob.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://sm.huanxung.cn

[S11] C：逐行读文件
来源：http://nz.lnxyls.cn

FILE *f = fopen("a.txt", "r");
来源：http://ew.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://oc.wgjwhj.cn

fclose(f);
来源：http://kh.szxytkj.cn

[S12] C：写文件
来源：http://sg.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wp.panjiajie.cn

[S13] C：宏定义
来源：http://mx.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nq.shxzskj.cn

[S14] C：枚举
来源：http://tj.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://hu.wgjwhj.cn

[S15] C：类型转换
来源：http://rj.huixinmuqiang.cn

(double) a / b
来源：http://yh.huanxung.cn

[S16] C：位操作置位
来源：http://aw.bjjhwx.cn

x |= (1 << 3);
来源：http://jm.hahajie.cn

[S17] C：安全拼接字符串
来源：http://uv.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vf.haigaiapp.cn

[S18] C：命令行参数
来源：http://ka.521024.cn

int main(int argc, char **argv)
来源：http://pf.huanxung.cn

[S19] C：快速排序
来源：http://od.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dl.haigaiapp.cn

[S20] C：二分查找
来源：http://ni.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lr.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://ez.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xv.shxzskj.cn

[S22] C：字符串转数字
来源：http://nk.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nn.huixinmuqiang.cn

[S23] C：随机数
来源：http://ar.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zn.yuexingan06.cn

[S24] C：获取本地时间
来源：http://wd.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gp.shxzukj.cn

[S25] C：内存拷贝
来源：http://se.shxzskj.cn

memcpy(dst, src, n);
来源：http://uo.nszjky.cn

[S26] C：内存清零
来源：http://vq.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://qi.panjiajie.cn

[S27] C：定义常量
来源：http://of.hnjuh.cn

const double PI = 3.14159;
来源：http://fg.lnxyls.cn

[S28] C：静态变量
来源：http://oz.yuexingan06.cn

static int counter = 0;
来源：http://zi.huixiangedu.cn

[S29] C：变参函数
来源：http://ya.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bb.yuexingan06.cn

[S30] C：头文件保护
来源：http://ox.nicolike.cn

#ifndef X_H
来源：http://eb.shxzukj.cn

#define X_H
来源：http://ew.panjiajie.cn

#endif
来源：http://ya.shxzskj.cn

[S31] C++：Hello World
来源：http://ss.huixiangedu.cn

#include <iostream>
来源：http://sl.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://kh.shxzskj.cn

[S32] C++：字符串
来源：http://sc.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://sj.asd995.cn

[S33] C++：vector 增删
来源：http://vn.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nz.hnjuh.cn

[S34] C++：遍历 vector
来源：http://km.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://cd.haigaiapp.cn

[S35] C++：map
来源：http://xb.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xx.newstarts.cn

[S36] C++：unordered_map
来源：http://zt.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dv.szsharing.cn

[S37] C++：set
来源：http://fj.521024.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fs.hahajie.cn

[S38] C++：排序
来源：http://jn.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://rl.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://pk.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ri.asd995.cn

[S40] C++：查找元素
来源：http://hz.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lj.hnjuh.cn

[S41] C++：类与构造函数
来源：http://bl.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rf.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://ur.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://fc.hnjuh.cn

[S43] C++：智能指针
来源：http://ly.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://uw.521024.cn

[S44] C++：引用传参
来源：http://mh.nszjky.cn

void inc(int &x) { ++x; }
来源：http://nf.hnjuh.cn

[S45] C++：lambda
来源：http://uh.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yl.521024.cn

[S46] C++：函数模板
来源：http://ji.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://es.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://ci.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yp.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://wg.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xw.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://ac.wgjwhj.cn

[S49] C++：写文件
来源：http://pe.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sw.shxzskj.cn

[S50] C++：格式化数字
来源：http://bj.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zu.nicolike.cn

[S51] C++：显式类型转换
来源：http://ui.521024.cn

static_cast<double>(a) / b
来源：http://ma.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://xv.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://zu.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://il.panjiajie.cn

std::vector<int> w = std::move(v);
来源：http://cx.muxihuayi.cn

[S54] C++：异常处理
来源：http://az.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eh.szsharing.cn

[S55] C++：结构化绑定
来源：http://sc.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pf.hnjuh.cn

[S56] C++：optional
来源：http://yp.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://so.shxzukj.cn

[S57] C++：编译期常量
来源：http://op.yuexingan06.cn

constexpr int N = 10;
来源：http://yt.muxihuayi.cn

[S58] C++：命名空间
来源：http://va.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://gx.newstarts.cn

[S59] C++：静态断言
来源：http://av.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://re.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://qh.jianghongdianzi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://he.haigaiapp.cn

================================================================================
来源：http://kk.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oa.wgjwhj.cn

================================================================================
来源：http://hl.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://kn.haigaiapp.cn

println("Hello")
来源：http://eh.521024.cn

[T02] Kotlin：变量
来源：http://cq.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eh.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://cn.bjjhwx.cn

"值: $b"
来源：http://nl.shxzukj.cn

[T04] Kotlin：空安全
来源：http://kt.hnjuh.cn

val n: String? = null;  n?.length
来源：http://jo.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://nx.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vp.colortex.cn

[T06] Kotlin：集合映射
来源：http://ad.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://me.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://vb.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gg.9csxet.cn

[T08] Kotlin：数据类
来源：http://qj.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://xr.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://iw.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://rg.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://cu.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pi.bjjhwx.cn

[T11] Kotlin：协程
来源：http://iz.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cb.huanxung.cn

[T12] Kotlin：解构声明
来源：http://gy.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://ns.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://wl.hahajie.cn

val m = mapOf("a" to 1)
来源：http://gr.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://gp.yuntaijiaju.cn

for (i in 1..10) println(i)
来源：http://gb.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://hf.huixinmuqiang.cn

interface Shape { fun area(): Double }
来源：http://sw.shxzskj.cn

[T16] Swift：Hello World
来源：http://fe.colortex.cn

print("Hello")
来源：http://oy.9csxet.cn

[T17] Swift：变量与常量
来源：http://ws.hnjuh.cn

var a = 1;  let b = 2
来源：http://si.szsharing.cn

[T18] Swift：字符串插值
来源：http://sw.jctech888.com.cn

"值: \(b)"
来源：http://sb.9csxet.cn

[T19] Swift：可选绑定
来源：http://yk.yuexingan06.cn

if let n = opt { print(n) }
来源：http://qt.521024.cn

[T20] Swift：数组操作
来源：http://dz.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lv.szsharing.cn

[T21] Swift：遍历
来源：http://lz.wgjwhj.cn

for x in a { print(x) }
来源：http://vs.wgjwhj.cn

[T22] Swift：字典
来源：http://og.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zr.9csxet.cn

[T23] Swift：函数
来源：http://bb.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://iz.jctech888.com.cn

[T24] Swift：闭包
来源：http://qp.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ii.muxihuayi.cn

[T25] Swift：结构体
来源：http://ck.hahajie.cn

struct P { var x: Int }
来源：http://cb.huixiangedu.cn

[T26] Swift：类与重写
来源：http://yc.gzmigu.cn

class A: Base { override func f() {} }
来源：http://dl.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://jo.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://hl.nszjky.cn

[T28] Swift：枚举
来源：http://ct.lnxyls.cn

enum Color { case red, green }
来源：http://xy.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://ca.nicolike.cn

guard let x = opt else { return }
来源：http://el.szxytkj.cn

[T30] Swift：协议
来源：http://zy.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://db.shtwfgs.cn

[T31] Lua：Hello World
来源：http://fv.newstarts.cn

print("Hello")
来源：http://fy.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://ne.chemitech.net.cn

local a = 1
来源：http://pa.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://ff.wgjwhj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ek.gzmigu.cn

[T34] Lua：遍历表
来源：http://ek.newstarts.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cl.newstarts.cn

[T35] Lua：字典表
来源：http://hp.nszjky.cn

local d = { a = 1 };  d.b = 2
来源：http://ym.gzmigu.cn

[T36] Lua：函数
来源：http://gd.wgjwhj.cn

function add(a, b) return a + b end
来源：http://od.shxzukj.cn

[T37] Lua：字符串拼接
来源：http://pj.huixinmuqiang.cn

"a" .. "b"
来源：http://xr.asd995.cn

[T38] Lua：条件
来源：http://sj.muxihuayi.cn

if x > 0 then print("正") end
来源：http://ly.521024.cn


<!-- 参考信息 -->