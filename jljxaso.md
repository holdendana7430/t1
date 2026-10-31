代发 wailian999

cmd > out.log 2>&1
来源：http://ov.nicolike.cn

[R40] 追加写日志
来源：http://rq.huixiangedu.cn

echo "log" >> out.log
来源：http://qu.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://iw.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://bt.asd995.cn

[R42] 输入重定向
来源：http://gi.haigaiapp.cn

wc -l < a.txt
来源：http://dw.muxihuayi.cn

[R43] 按名字查找文件
来源：http://iy.nszjky.cn

find . -name "*.log" -type f
来源：http://ih.colortex.cn

[R44] 按修改时间查找
来源：http://ko.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://ek.yuexingan06.cn

[R45] 批量删除
来源：http://rh.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://xu.lnxyls.cn

[R46] 递归替换文件内容
来源：http://ge.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sp.lnxyls.cn

[R47] sed 单行替换
来源：http://lo.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qe.bjjhwx.cn

[R48] awk 取指定列
来源：http://kl.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://xa.shxzukj.cn

[R49] awk 带条件
来源：http://dq.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xs.gzmigu.cn

[R50] awk 求和
来源：http://sq.bjjhwx.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tm.haigaiapp.cn

[R51] 排序去重取前几
来源：http://wh.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://eb.shtwfgs.cn

[R52] 统计行数
来源：http://bc.yuexingan06.cn

wc -l a.txt
来源：http://ne.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://ex.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tj.newstarts.cn

[R54] 比较两个文件
来源：http://gq.wgjwhj.cn

diff a.txt b.txt
来源：http://yk.shxzukj.cn

[R55] 压缩与解压
来源：http://qu.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ea.lnxyls.cn

[R56] 远程拷贝
来源：http://bc.huanxung.cn

scp file user@host:/path/
来源：http://nx.newstarts.cn

[R57] 远程执行命令
来源：http://df.colortex.cn

ssh user@host 'uptime'
来源：http://fh.colortex.cn

[R58] 下载文件
来源：http://oy.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xj.huixiangedu.cn

[R59] 发 POST JSON
来源：http://zb.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://re.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://uu.muxihuayi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ey.szxytkj.cn

[R61] 磁盘占用
来源：http://ln.nszjky.cn

df -h;  du -sh *
来源：http://zc.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://tr.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://xu.521024.cn

[R63] 内存与进程
来源：http://jr.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://vu.9csxet.cn

[R64] 结束进程
来源：http://kp.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://og.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://ju.jctech888.com.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bc.huixinmuqiang.cn

[R66] 定时任务
来源：http://gj.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://cv.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://xj.newstarts.cn

openssl rand -hex 16
来源：http://wy.asd995.cn

[R68] 计算文件校验值
来源：http://ro.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mk.huixiangedu.cn

[R69] 生成随机密码
来源：http://rw.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://bp.asd995.cn

[R70] 时间戳与互转
来源：http://bb.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://dj.wgjwhj.cn

[R71] 日期格式化
来源：http://ou.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pl.muxihuayi.cn

[R72] 等待端口就绪
来源：http://iw.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ab.szsharing.cn

[R73] 分割大日志
来源：http://ow.panjiajie.cn

split -l 1000 big.log part_
来源：http://jh.szsharing.cn

[R74] 批量重命名
来源：http://lk.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ov.huixiangedu.cn

[R75] 导出环境变量
来源：http://rt.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://ez.wgjwhj.cn

[R76] 使用临时文件
来源：http://pk.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kh.szxytkj.cn

[R77] 读取用户输入
来源：http://jq.chemitech.net.cn

read -rp "请输入: " ans
来源：http://wq.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://fn.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oz.shtwfgs.cn

[R79] 解析命令行选项
来源：http://yj.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://af.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://yi.nicolike.cn

time ./run.sh
来源：http://qv.panjiajie.cn

================================================================================
来源：http://ly.szxytkj.cn

S. C / C++ 专题
来源：http://xm.chemitech.net.cn

================================================================================
来源：http://zi.bjjhwx.cn

[S01] C：Hello World
来源：http://yu.huixinmuqiang.cn

#include <stdio.h>
来源：http://dd.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bd.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://uu.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://ky.chemitech.net.cn

[S03] C：读入整数
来源：http://fw.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://wt.shxzskj.cn

[S04] C：字符串复制
来源：http://gp.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cu.newstarts.cn

[S05] C：字符串长度
来源：http://ra.hahajie.cn

strlen(s)
来源：http://it.huanxung.cn

[S06] C：字符串比较
来源：http://cm.muxihuayi.cn

strcmp(a, b) == 0
来源：http://bf.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://rd.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ld.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://xn.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ic.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://nt.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vh.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://kf.9csxet.cn

int *p = &a;  *p = 5;
来源：http://si.shxzukj.cn

[S11] C：逐行读文件
来源：http://cs.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://jp.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gv.wgjwhj.cn

fclose(f);
来源：http://yf.jianghongdianzi.cn

[S12] C：写文件
来源：http://eq.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gf.9csxet.cn

[S13] C：宏定义
来源：http://eg.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nd.bjjhwx.cn

[S14] C：枚举
来源：http://wg.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://js.yuexingan06.cn

[S15] C：类型转换
来源：http://ln.jctech888.com.cn

(double) a / b
来源：http://ff.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://ya.szsharing.cn

x |= (1 << 3);
来源：http://ae.colortex.cn

[S17] C：安全拼接字符串
来源：http://ap.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://li.wgjwhj.cn

[S18] C：命令行参数
来源：http://mb.szsharing.cn

int main(int argc, char **argv)
来源：http://eb.jianghongdianzi.cn

[S19] C：快速排序
来源：http://qp.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ph.hnjuh.cn

[S20] C：二分查找
来源：http://xs.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vg.9csxet.cn

[S21] C：字符类别判断
来源：http://sm.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://td.gzmigu.cn

[S22] C：字符串转数字
来源：http://cj.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fn.shtwfgs.cn

[S23] C：随机数
来源：http://fl.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xn.jctech888.com.cn

[S24] C：获取本地时间
来源：http://oy.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hs.chemitech.net.cn

[S25] C：内存拷贝
来源：http://jc.huixiangedu.cn

memcpy(dst, src, n);
来源：http://li.yuexingan06.cn

[S26] C：内存清零
来源：http://km.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://oy.yuexingan06.cn

[S27] C：定义常量
来源：http://dw.nszjky.cn

const double PI = 3.14159;
来源：http://sk.asd995.cn

[S28] C：静态变量
来源：http://ru.shxzskj.cn

static int counter = 0;
来源：http://fn.shxzukj.cn

[S29] C：变参函数
来源：http://if.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ta.haigaiapp.cn

[S30] C：头文件保护
来源：http://ul.bjjhwx.cn

#ifndef X_H
来源：http://ld.szsharing.cn

#define X_H
来源：http://od.szxytkj.cn

#endif
来源：http://xi.panjiajie.cn

[S31] C++：Hello World
来源：http://nz.yuntaijiaju.cn

#include <iostream>
来源：http://tr.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://wr.jctech888.com.cn

[S32] C++：字符串
来源：http://oy.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://nh.haigaiapp.cn

[S33] C++：vector 增删
来源：http://fn.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://br.shxzskj.cn

[S34] C++：遍历 vector
来源：http://vo.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://ay.huanxung.cn

[S35] C++：map
来源：http://uy.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ba.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://di.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ou.shxzskj.cn

[S37] C++：set
来源：http://qt.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://md.newstarts.cn

[S38] C++：排序
来源：http://xi.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://ph.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://ym.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gh.wgjwhj.cn

[S40] C++：查找元素
来源：http://zo.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bu.521024.cn

[S41] C++：类与构造函数
来源：http://ii.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mh.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://xn.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://re.shtwfgs.cn

[S43] C++：智能指针
来源：http://dc.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://ez.asd995.cn

[S44] C++：引用传参
来源：http://ix.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://cr.panjiajie.cn

[S45] C++：lambda
来源：http://gu.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ra.huixiangedu.cn

[S46] C++：函数模板
来源：http://vl.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hg.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://oo.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://he.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://xi.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mu.jctech888.com.cn

while (std::getline(in, line)) { }
来源：http://aa.muxihuayi.cn

[S49] C++：写文件
来源：http://mf.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sg.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://rx.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lp.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://ca.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://bv.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://zr.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://kh.shxzskj.cn

[S53] C++：移动语义
来源：http://qp.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://je.nicolike.cn

[S54] C++：异常处理
来源：http://oc.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bp.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://hu.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zm.shxzukj.cn

[S56] C++：optional
来源：http://rl.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ek.hnjuh.cn

[S57] C++：编译期常量
来源：http://fc.jianghongdianzi.cn

constexpr int N = 10;
来源：http://ka.huanxung.cn

[S58] C++：命名空间
来源：http://vm.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://rd.wgjwhj.cn

[S59] C++：静态断言
来源：http://ft.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sm.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://dr.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://be.muxihuayi.cn

================================================================================
来源：http://gy.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mh.nicolike.cn

================================================================================
来源：http://dz.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://fp.hnjuh.cn

println("Hello")
来源：http://ru.szsharing.cn

[T02] Kotlin：变量
来源：http://ch.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sy.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://fd.shtwfgs.cn

"值: $b"
来源：http://rc.nicolike.cn

[T04] Kotlin：空安全
来源：http://yo.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://oz.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://xv.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://au.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://wt.gzmigu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cw.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://rp.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://he.hnjuh.cn

[T08] Kotlin：数据类
来源：http://zn.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://ab.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://tb.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://qs.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://dl.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ua.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://mt.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uu.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://tm.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://uo.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://fv.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://vi.nicolike.cn

[T14] Kotlin：循环
来源：http://hw.hahajie.cn

for (i in 1..10) println(i)
来源：http://ia.521024.cn

[T15] Kotlin：接口
来源：http://pk.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://ch.hnjuh.cn

[T16] Swift：Hello World
来源：http://pn.asd995.cn

print("Hello")
来源：http://nz.nicolike.cn

[T17] Swift：变量与常量
来源：http://ze.nszjky.cn

var a = 1;  let b = 2
来源：http://my.bookmarksfly.cn

[T18] Swift：字符串插值
来源：http://ys.yuexingan06.cn

"值: \(b)"
来源：http://kb.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://ac.lnxyls.cn

if let n = opt { print(n) }
来源：http://cu.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://ja.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zw.nicolike.cn

[T21] Swift：遍历
来源：http://au.jctech888.com.cn

for x in a { print(x) }
来源：http://eh.newstarts.cn

[T22] Swift：字典
来源：http://id.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xj.bjjhwx.cn

[T23] Swift：函数
来源：http://us.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dq.hahajie.cn

[T24] Swift：闭包
来源：http://rj.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rt.lnxyls.cn

[T25] Swift：结构体
来源：http://xn.gzmigu.cn

struct P { var x: Int }
来源：http://ce.gzmigu.cn

[T26] Swift：类与重写
来源：http://ic.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://cv.huanxung.cn

[T27] Swift：错误处理
来源：http://cn.521024.cn

do { try f() } catch { print(error) }
来源：http://cb.szxytkj.cn

[T28] Swift：枚举
来源：http://jy.asd995.cn

enum Color { case red, green }
来源：http://vr.colortex.cn

[T29] Swift：guard 提前返回
来源：http://vc.lnxyls.cn

guard let x = opt else { return }
来源：http://pc.newstarts.cn

[T30] Swift：协议
来源：http://pa.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://da.wgjwhj.cn

[T31] Lua：Hello World
来源：http://go.shtwfgs.cn

print("Hello")
来源：http://wi.colortex.cn

[T32] Lua：局部变量
来源：http://yx.bjjhwx.cn

local a = 1
来源：http://vz.nicolike.cn

[T33] Lua：表（数组）
来源：http://wv.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sx.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://ho.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hu.huixiangedu.cn

[T35] Lua：字典表
来源：http://lq.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://ks.asd995.cn

[T36] Lua：函数
来源：http://zh.hnjuh.cn

function add(a, b) return a + b end
来源：http://fh.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://ds.hahajie.cn

"a" .. "b"
来源：http://eb.szsharing.cn

[T38] Lua：条件
来源：http://or.colortex.cn

if x > 0 then print("正") end
来源：http://xm.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://ww.wgjwhj.cn

string.find(s, "%d+")
来源：http://ic.szxytkj.cn

[T40] Lua：元表
来源：http://pz.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://jy.huanxung.cn

[T41] Perl：Hello World
来源：http://js.bjjhwx.cn

print "Hello\n";
来源：http://bz.hahajie.cn

[T42] Perl：变量类型
来源：http://aq.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bs.huixiangedu.cn


<!-- 参考信息 -->