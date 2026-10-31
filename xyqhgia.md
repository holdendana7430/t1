代发 wailian999

files=$(ls -1)
来源：http://qe.yuexingan06.cn

[R38] 管道串联
来源：http://jl.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://ab.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://yc.hnjuh.cn

cmd > out.log 2>&1
来源：http://oo.hahajie.cn

[R40] 追加写日志
来源：http://hz.muxihuayi.cn

echo "log" >> out.log
来源：http://ez.huanxung.cn

[R41] 丢弃输出
来源：http://gj.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://hb.shtwfgs.cn

[R42] 输入重定向
来源：http://zi.panjiajie.cn

wc -l < a.txt
来源：http://an.newstarts.cn

[R43] 按名字查找文件
来源：http://ck.9csxet.cn

find . -name "*.log" -type f
来源：http://of.9csxet.cn

[R44] 按修改时间查找
来源：http://ce.gzmigu.cn

find . -mtime -7 -type f
来源：http://gb.hnjuh.cn

[R45] 批量删除
来源：http://yx.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://tg.asd995.cn

[R46] 递归替换文件内容
来源：http://da.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ie.jctech888.com.cn

[R47] sed 单行替换
来源：http://qt.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dg.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://rz.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://kt.nszjky.cn

[R49] awk 带条件
来源：http://ma.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tf.lnxyls.cn

[R50] awk 求和
来源：http://zl.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ua.asd995.cn

[R51] 排序去重取前几
来源：http://zy.huixiangedu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lt.jctech888.com.cn

[R52] 统计行数
来源：http://qm.9csxet.cn

wc -l a.txt
来源：http://kc.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://nc.lnxyls.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ck.521024.cn

[R54] 比较两个文件
来源：http://lb.hahajie.cn

diff a.txt b.txt
来源：http://sf.chemitech.net.cn

[R55] 压缩与解压
来源：http://ji.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uu.wgjwhj.cn

[R56] 远程拷贝
来源：http://jf.colortex.cn

scp file user@host:/path/
来源：http://xl.asd995.cn

[R57] 远程执行命令
来源：http://hx.szxytkj.cn

ssh user@host 'uptime'
来源：http://uc.jctech888.com.cn

[R58] 下载文件
来源：http://yw.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xp.shxzukj.cn

[R59] 发 POST JSON
来源：http://bu.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://el.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://ll.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yr.9csxet.cn

[R61] 磁盘占用
来源：http://lc.panjiajie.cn

df -h;  du -sh *
来源：http://mf.panjiajie.cn

[R62] 找最占空间的文件
来源：http://mi.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://pq.jctech888.com.cn

[R63] 内存与进程
来源：http://vk.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://dd.colortex.cn

[R64] 结束进程
来源：http://yw.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://mr.shxzukj.cn

[R65] 查看端口占用
来源：http://mo.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ze.huixinmuqiang.cn

[R66] 定时任务
来源：http://km.9csxet.cn

crontab -e;  crontab -l
来源：http://di.asd995.cn

[R67] 生成随机十六进制串
来源：http://wu.bookmarksfly.cn

openssl rand -hex 16
来源：http://rx.chemitech.net.cn

[R68] 计算文件校验值
来源：http://co.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hp.521024.cn

[R69] 生成随机密码
来源：http://fp.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://nf.asd995.cn

[R70] 时间戳与互转
来源：http://eu.9csxet.cn

date +%s;  date -d @1700000000
来源：http://qt.haigaiapp.cn

[R71] 日期格式化
来源：http://av.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ql.chemitech.net.cn

[R72] 等待端口就绪
来源：http://nm.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ug.nszjky.cn

[R73] 分割大日志
来源：http://bs.colortex.cn

split -l 1000 big.log part_
来源：http://hw.9csxet.cn

[R74] 批量重命名
来源：http://ul.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wc.panjiajie.cn

[R75] 导出环境变量
来源：http://oe.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://uu.colortex.cn

[R76] 使用临时文件
来源：http://ju.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mw.hnjuh.cn

[R77] 读取用户输入
来源：http://ib.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://aw.521024.cn

[R78] 交互式菜单
来源：http://ny.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dm.jianghongdianzi.cn

[R79] 解析命令行选项
来源：http://kc.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ew.colortex.cn

[R80] 查看脚本执行耗时
来源：http://lw.wgjwhj.cn

time ./run.sh
来源：http://en.9csxet.cn

================================================================================
来源：http://bb.nicolike.cn

S. C / C++ 专题
来源：http://ea.jianghongdianzi.cn

================================================================================
来源：http://vx.yuexingan06.cn

[S01] C：Hello World
来源：http://kx.shxzukj.cn

#include <stdio.h>
来源：http://db.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ke.asd995.cn

[S02] C：变量与格式化输出
来源：http://pe.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://wb.huixiangedu.cn

[S03] C：读入整数
来源：http://jl.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://jf.shtwfgs.cn

[S04] C：字符串复制
来源：http://sb.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tl.huixiangedu.cn

[S05] C：字符串长度
来源：http://zi.nicolike.cn

strlen(s)
来源：http://fc.yuexingan06.cn

[S06] C：字符串比较
来源：http://xt.yuexingan06.cn

strcmp(a, b) == 0
来源：http://ln.hnjuh.cn

[S07] C：数组遍历求和
来源：http://nq.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wa.asd995.cn

[S08] C：动态内存分配与释放
来源：http://fu.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dn.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://ws.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qg.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://ek.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://qn.yuexingan06.cn

[S11] C：逐行读文件
来源：http://xe.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://bn.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xu.shxzukj.cn

fclose(f);
来源：http://gp.nicolike.cn

[S12] C：写文件
来源：http://ly.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xy.huanxung.cn

[S13] C：宏定义
来源：http://jr.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ld.bjjhwx.cn

[S14] C：枚举
来源：http://ue.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://zp.9csxet.cn

[S15] C：类型转换
来源：http://fh.nicolike.cn

(double) a / b
来源：http://xm.szsharing.cn

[S16] C：位操作置位
来源：http://fp.jianghongdianzi.cn

x |= (1 << 3);
来源：http://vv.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://dz.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://po.nszjky.cn

[S18] C：命令行参数
来源：http://qg.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://wy.yuexingan06.cn

[S19] C：快速排序
来源：http://sl.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qh.bookmarksfly.cn

[S20] C：二分查找
来源：http://zr.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ga.9csxet.cn

[S21] C：字符类别判断
来源：http://nu.wgjwhj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iu.wgjwhj.cn

[S22] C：字符串转数字
来源：http://ac.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://un.jianghongdianzi.cn

[S23] C：随机数
来源：http://jp.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bq.huanxung.cn

[S24] C：获取本地时间
来源：http://qr.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xp.shxzskj.cn

[S25] C：内存拷贝
来源：http://gi.szsharing.cn

memcpy(dst, src, n);
来源：http://yc.asd995.cn

[S26] C：内存清零
来源：http://va.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://ga.jianghongdianzi.cn

[S27] C：定义常量
来源：http://bd.nszjky.cn

const double PI = 3.14159;
来源：http://dc.huixinmuqiang.cn

[S28] C：静态变量
来源：http://ie.9csxet.cn

static int counter = 0;
来源：http://pv.szsharing.cn

[S29] C：变参函数
来源：http://wl.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hu.jctech888.com.cn

[S30] C：头文件保护
来源：http://tx.huixinmuqiang.cn

#ifndef X_H
来源：http://vv.yuexingan06.cn

#define X_H
来源：http://kb.lnxyls.cn

#endif
来源：http://aj.nicolike.cn

[S31] C++：Hello World
来源：http://be.yuntaijiaju.cn

#include <iostream>
来源：http://gp.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://iy.huixinmuqiang.cn

[S32] C++：字符串
来源：http://ow.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://dd.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://nk.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fn.newstarts.cn

[S34] C++：遍历 vector
来源：http://ah.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://qe.yuntaijiaju.cn

[S35] C++：map
来源：http://zt.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ii.panjiajie.cn

[S36] C++：unordered_map
来源：http://lf.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zr.szsharing.cn

[S37] C++：set
来源：http://qs.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wv.muxihuayi.cn

[S38] C++：排序
来源：http://nv.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://oc.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://nu.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sa.nszjky.cn

[S40] C++：查找元素
来源：http://mb.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qs.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://ap.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bn.9csxet.cn

[S42] C++：继承与虚函数
来源：http://wg.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://vi.huanxung.cn

[S43] C++：智能指针
来源：http://lh.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://sv.huixiangedu.cn

[S44] C++：引用传参
来源：http://cl.nszjky.cn

void inc(int &x) { ++x; }
来源：http://pu.muxihuayi.cn

[S45] C++：lambda
来源：http://hm.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nb.lnxyls.cn

[S46] C++：函数模板
来源：http://po.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uo.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://bk.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nj.shxzukj.cn

[S48] C++：逐行读文件
来源：http://yg.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nx.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://nt.gzmigu.cn

[S49] C++：写文件
来源：http://cx.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yc.nszjky.cn

[S50] C++：格式化数字
来源：http://bh.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pk.lnxyls.cn

[S51] C++：显式类型转换
来源：http://id.haigaiapp.cn

static_cast<double>(a) / b
来源：http://dz.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://jp.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://hy.lnxyls.cn

[S53] C++：移动语义
来源：http://lp.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://aq.szsharing.cn

[S54] C++：异常处理
来源：http://bo.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://re.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://st.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://it.9csxet.cn

[S56] C++：optional
来源：http://ox.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kr.bjjhwx.cn

[S57] C++：编译期常量
来源：http://sj.yuntaijiaju.cn

constexpr int N = 10;
来源：http://va.wgjwhj.cn

[S58] C++：命名空间
来源：http://sk.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://bf.nszjky.cn

[S59] C++：静态断言
来源：http://oj.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ur.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://qj.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gn.szsharing.cn

================================================================================
来源：http://im.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yc.szxytkj.cn

================================================================================
来源：http://el.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://ug.nicolike.cn

println("Hello")
来源：http://hm.hnjuh.cn

[T02] Kotlin：变量
来源：http://ck.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ut.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://lw.panjiajie.cn

"值: $b"
来源：http://uf.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://za.newstarts.cn

val n: String? = null;  n?.length
来源：http://wt.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://cu.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ye.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://kg.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cm.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://ye.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sx.nszjky.cn

[T08] Kotlin：数据类
来源：http://px.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://rc.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://jm.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://qo.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://mb.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ci.szxytkj.cn

[T11] Kotlin：协程
来源：http://kv.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xd.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://lt.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://nz.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://jd.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://rf.shxzukj.cn

[T14] Kotlin：循环
来源：http://de.nicolike.cn

for (i in 1..10) println(i)
来源：http://nw.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://ft.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://oi.yuntaijiaju.cn

[T16] Swift：Hello World
来源：http://fg.panjiajie.cn

print("Hello")
来源：http://ho.nszjky.cn

[T17] Swift：变量与常量
来源：http://mo.shxzskj.cn

var a = 1;  let b = 2
来源：http://fj.nicolike.cn

[T18] Swift：字符串插值
来源：http://ra.bjjhwx.cn

"值: \(b)"
来源：http://tb.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://ih.nszjky.cn

if let n = opt { print(n) }
来源：http://fv.9csxet.cn

[T20] Swift：数组操作
来源：http://gz.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sd.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://xp.panjiajie.cn

for x in a { print(x) }
来源：http://al.gzmigu.cn

[T22] Swift：字典
来源：http://at.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gf.haigaiapp.cn

[T23] Swift：函数
来源：http://ni.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jc.lnxyls.cn

[T24] Swift：闭包
来源：http://pj.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zz.chemitech.net.cn

[T25] Swift：结构体
来源：http://ui.nicolike.cn

struct P { var x: Int }
来源：http://hc.panjiajie.cn

[T26] Swift：类与重写
来源：http://oh.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://qd.huixiangedu.cn

[T27] Swift：错误处理
来源：http://zz.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://xt.colortex.cn

[T28] Swift：枚举
来源：http://hm.newstarts.cn

enum Color { case red, green }
来源：http://rw.hahajie.cn

[T29] Swift：guard 提前返回
来源：http://do.jctech888.com.cn

guard let x = opt else { return }
来源：http://ld.bjjhwx.cn

[T30] Swift：协议
来源：http://ko.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://gt.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://bf.bookmarksfly.cn

print("Hello")
来源：http://uk.nszjky.cn

[T32] Lua：局部变量
来源：http://hi.521024.cn

local a = 1
来源：http://kq.szsharing.cn

[T33] Lua：表（数组）
来源：http://jf.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nx.shxzskj.cn

[T34] Lua：遍历表
来源：http://ke.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ma.gzmigu.cn

[T35] Lua：字典表
来源：http://mo.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://en.9csxet.cn

[T36] Lua：函数
来源：http://gg.szxytkj.cn

function add(a, b) return a + b end
来源：http://fh.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://af.szsharing.cn

"a" .. "b"
来源：http://gk.newstarts.cn

[T38] Lua：条件
来源：http://kq.521024.cn

if x > 0 then print("正") end
来源：http://ks.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://ki.jianghongdianzi.cn

string.find(s, "%d+")
来源：http://ox.shxzukj.cn

[T40] Lua：元表
来源：http://rg.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://xi.nicolike.cn


<!-- 参考信息 -->