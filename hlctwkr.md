代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://yv.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://lt.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.muxihuayi.cn

[R37] 把输出赋给变量
来源：http://yy.shxzskj.cn

files=$(ls -1)
来源：http://ws.shxzukj.cn

[R38] 管道串联
来源：http://hp.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://aq.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://qh.9csxet.cn

cmd > out.log 2>&1
来源：http://jy.newstarts.cn

[R40] 追加写日志
来源：http://gh.bookmarksfly.cn

echo "log" >> out.log
来源：http://na.colortex.cn

[R41] 丢弃输出
来源：http://dw.nszjky.cn

cmd >/dev/null 2>&1
来源：http://hn.521024.cn

[R42] 输入重定向
来源：http://ts.colortex.cn

wc -l < a.txt
来源：http://cr.nszjky.cn

[R43] 按名字查找文件
来源：http://ei.chemitech.net.cn

find . -name "*.log" -type f
来源：http://ln.hnjuh.cn

[R44] 按修改时间查找
来源：http://aj.panjiajie.cn

find . -mtime -7 -type f
来源：http://hn.shtwfgs.cn

[R45] 批量删除
来源：http://zz.szsharing.cn

find . -name "*.tmp" -delete
来源：http://nr.shxzukj.cn

[R46] 递归替换文件内容
来源：http://qi.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bk.shxzukj.cn

[R47] sed 单行替换
来源：http://ze.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sw.bookmarksfly.cn

[R48] awk 取指定列
来源：http://hu.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://ux.asd995.cn

[R49] awk 带条件
来源：http://nr.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sv.hahajie.cn

[R50] awk 求和
来源：http://yq.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tv.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://la.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tn.jianghongdianzi.cn

[R52] 统计行数
来源：http://qa.gzmigu.cn

wc -l a.txt
来源：http://qk.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://fn.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wg.panjiajie.cn

[R54] 比较两个文件
来源：http://ib.bjjhwx.cn

diff a.txt b.txt
来源：http://ku.huanxung.cn

[R55] 压缩与解压
来源：http://dt.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jx.szsharing.cn

[R56] 远程拷贝
来源：http://rh.yuntaijiaju.cn

scp file user@host:/path/
来源：http://mj.9csxet.cn

[R57] 远程执行命令
来源：http://uf.521024.cn

ssh user@host 'uptime'
来源：http://qg.szsharing.cn

[R58] 下载文件
来源：http://pp.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://va.nszjky.cn

[R59] 发 POST JSON
来源：http://oo.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mm.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://sf.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lx.hnjuh.cn

[R61] 磁盘占用
来源：http://ub.jianghongdianzi.cn

df -h;  du -sh *
来源：http://xx.shxzukj.cn

[R62] 找最占空间的文件
来源：http://au.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://ns.nszjky.cn

[R63] 内存与进程
来源：http://fp.jctech888.com.cn

free -h;  ps aux | grep nginx
来源：http://nq.panjiajie.cn

[R64] 结束进程
来源：http://dv.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://ta.hnjuh.cn

[R65] 查看端口占用
来源：http://dr.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vo.nicolike.cn

[R66] 定时任务
来源：http://ji.huixiangedu.cn

crontab -e;  crontab -l
来源：http://md.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://qp.newstarts.cn

openssl rand -hex 16
来源：http://ge.shxzskj.cn

[R68] 计算文件校验值
来源：http://eu.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cg.haigaiapp.cn

[R69] 生成随机密码
来源：http://nh.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://gw.szsharing.cn

[R70] 时间戳与互转
来源：http://xw.huixiangedu.cn

date +%s;  date -d @1700000000
来源：http://zr.hahajie.cn

[R71] 日期格式化
来源：http://xm.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gy.shxzskj.cn

[R72] 等待端口就绪
来源：http://nj.newstarts.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wq.bookmarksfly.cn

[R73] 分割大日志
来源：http://li.shxzskj.cn

split -l 1000 big.log part_
来源：http://vq.521024.cn

[R74] 批量重命名
来源：http://kz.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qb.muxihuayi.cn

[R75] 导出环境变量
来源：http://dk.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://zv.9csxet.cn

[R76] 使用临时文件
来源：http://je.szxytkj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bi.521024.cn

[R77] 读取用户输入
来源：http://jg.bjjhwx.cn

read -rp "请输入: " ans
来源：http://bx.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://ok.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://al.bookmarksfly.cn

[R79] 解析命令行选项
来源：http://mb.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://la.asd995.cn

[R80] 查看脚本执行耗时
来源：http://id.gzmigu.cn

time ./run.sh
来源：http://em.jianghongdianzi.cn

================================================================================
来源：http://fg.muxihuayi.cn

S. C / C++ 专题
来源：http://ph.jctech888.com.cn

================================================================================
来源：http://by.nicolike.cn

[S01] C：Hello World
来源：http://aw.huixiangedu.cn

#include <stdio.h>
来源：http://kk.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mx.nszjky.cn

[S02] C：变量与格式化输出
来源：http://pk.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://no.hahajie.cn

[S03] C：读入整数
来源：http://gw.haigaiapp.cn

int x; scanf("%d", &x);
来源：http://yy.gzmigu.cn

[S04] C：字符串复制
来源：http://ux.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tr.asd995.cn

[S05] C：字符串长度
来源：http://cl.colortex.cn

strlen(s)
来源：http://ps.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://ta.gzmigu.cn

strcmp(a, b) == 0
来源：http://wx.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://fq.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jk.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://ip.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xs.521024.cn

[S09] C：结构体定义与初始化
来源：http://iv.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xj.jctech888.com.cn

[S10] C：指针与解引用
来源：http://fm.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://bb.wgjwhj.cn

[S11] C：逐行读文件
来源：http://uz.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://to.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zc.szsharing.cn

fclose(f);
来源：http://ec.wgjwhj.cn

[S12] C：写文件
来源：http://ld.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ah.hahajie.cn

[S13] C：宏定义
来源：http://hz.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tf.9csxet.cn

[S14] C：枚举
来源：http://cl.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://ba.bookmarksfly.cn

[S15] C：类型转换
来源：http://cu.szsharing.cn

(double) a / b
来源：http://hk.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://zh.huixinmuqiang.cn

x |= (1 << 3);
来源：http://rn.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://xt.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ak.521024.cn

[S18] C：命令行参数
来源：http://uw.9csxet.cn

int main(int argc, char **argv)
来源：http://ds.muxihuayi.cn

[S19] C：快速排序
来源：http://ib.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xk.bookmarksfly.cn

[S20] C：二分查找
来源：http://ee.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zn.szxytkj.cn

[S21] C：字符类别判断
来源：http://sm.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mc.shxzukj.cn

[S22] C：字符串转数字
来源：http://fv.nszjky.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cd.yuexingan06.cn

[S23] C：随机数
来源：http://bz.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kq.huixiangedu.cn

[S24] C：获取本地时间
来源：http://ve.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bn.nicolike.cn

[S25] C：内存拷贝
来源：http://bu.yuexingan06.cn

memcpy(dst, src, n);
来源：http://as.huixiangedu.cn

[S26] C：内存清零
来源：http://cx.9csxet.cn

memset(a, 0, sizeof a);
来源：http://yk.jctech888.com.cn

[S27] C：定义常量
来源：http://re.huixiangedu.cn

const double PI = 3.14159;
来源：http://sx.nszjky.cn

[S28] C：静态变量
来源：http://hs.bookmarksfly.cn

static int counter = 0;
来源：http://zt.hahajie.cn

[S29] C：变参函数
来源：http://jy.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xk.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://dx.muxihuayi.cn

#ifndef X_H
来源：http://dt.haigaiapp.cn

#define X_H
来源：http://bl.jctech888.com.cn

#endif
来源：http://bf.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://jn.yuexingan06.cn

#include <iostream>
来源：http://ms.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://as.szsharing.cn

[S32] C++：字符串
来源：http://gn.colortex.cn

std::string s = "hi";  s += "!";
来源：http://ce.newstarts.cn

[S33] C++：vector 增删
来源：http://qh.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rs.shxzukj.cn

[S34] C++：遍历 vector
来源：http://tw.asd995.cn

for (auto &x : v) { std::cout << x; }
来源：http://ko.521024.cn

[S35] C++：map
来源：http://od.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wf.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://jx.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://by.muxihuayi.cn

[S37] C++：set
来源：http://kr.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://un.shxzskj.cn

[S38] C++：排序
来源：http://fz.shxzukj.cn

std::sort(v.begin(), v.end());
来源：http://hz.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://rp.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kf.jctech888.com.cn

[S40] C++：查找元素
来源：http://yq.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nr.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://il.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mp.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://gt.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://sg.9csxet.cn

[S43] C++：智能指针
来源：http://tz.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://ho.wgjwhj.cn

[S44] C++：引用传参
来源：http://hg.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://xl.chemitech.net.cn

[S45] C++：lambda
来源：http://yg.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oq.asd995.cn

[S46] C++：函数模板
来源：http://ar.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nv.521024.cn

[S47] C++：结构化绑定遍历
来源：http://fn.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://st.9csxet.cn

[S48] C++：逐行读文件
来源：http://zr.haigaiapp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ns.nicolike.cn

while (std::getline(in, line)) { }
来源：http://ga.shtwfgs.cn

[S49] C++：写文件
来源：http://dq.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bk.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://rm.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://au.nszjky.cn

[S51] C++：显式类型转换
来源：http://zn.gzmigu.cn

static_cast<double>(a) / b
来源：http://ro.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://at.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://ko.haigaiapp.cn

[S53] C++：移动语义
来源：http://ho.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://da.nszjky.cn

[S54] C++：异常处理
来源：http://hl.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yo.shxzskj.cn

[S55] C++：结构化绑定
来源：http://cj.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qr.9csxet.cn

[S56] C++：optional
来源：http://pu.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kx.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://tl.chemitech.net.cn

constexpr int N = 10;
来源：http://po.wgjwhj.cn

[S58] C++：命名空间
来源：http://tl.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://wk.szsharing.cn

[S59] C++：静态断言
来源：http://nb.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yz.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://yu.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hf.yuexingan06.cn

================================================================================
来源：http://zn.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://in.shxzskj.cn

================================================================================
来源：http://bt.asd995.cn

[T01] Kotlin：Hello World
来源：http://vd.521024.cn

println("Hello")
来源：http://kx.asd995.cn

[T02] Kotlin：变量
来源：http://dh.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vt.colortex.cn

[T03] Kotlin：字符串模板
来源：http://ii.wgjwhj.cn

"值: $b"
来源：http://ga.newstarts.cn

[T04] Kotlin：空安全
来源：http://tt.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://sm.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://ct.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ah.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://za.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yq.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://qm.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kx.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://tc.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://fj.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://so.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://nv.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://gf.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://js.shxzskj.cn

[T11] Kotlin：协程
来源：http://nm.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pf.hahajie.cn

[T12] Kotlin：解构声明
来源：http://ih.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://vx.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://mz.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://nl.9csxet.cn

[T14] Kotlin：循环
来源：http://wv.szsharing.cn

for (i in 1..10) println(i)
来源：http://zu.haigaiapp.cn

[T15] Kotlin：接口
来源：http://zt.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://uj.huanxung.cn

[T16] Swift：Hello World
来源：http://ou.jianghongdianzi.cn

print("Hello")
来源：http://dh.panjiajie.cn

[T17] Swift：变量与常量
来源：http://rl.szxytkj.cn

var a = 1;  let b = 2
来源：http://hj.wgjwhj.cn

[T18] Swift：字符串插值
来源：http://pt.chemitech.net.cn

"值: \(b)"
来源：http://sh.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://vg.521024.cn

if let n = opt { print(n) }
来源：http://ee.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://iz.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yx.colortex.cn

[T21] Swift：遍历
来源：http://ku.asd995.cn

for x in a { print(x) }
来源：http://vm.shtwfgs.cn

[T22] Swift：字典
来源：http://gr.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sh.yuexingan06.cn

[T23] Swift：函数
来源：http://pw.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ik.newstarts.cn

[T24] Swift：闭包
来源：http://gh.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://un.bjjhwx.cn

[T25] Swift：结构体
来源：http://ri.yuntaijiaju.cn

struct P { var x: Int }
来源：http://pc.521024.cn

[T26] Swift：类与重写
来源：http://eu.colortex.cn

class A: Base { override func f() {} }
来源：http://cl.haigaiapp.cn

[T27] Swift：错误处理
来源：http://ja.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://cr.yuexingan06.cn

[T28] Swift：枚举
来源：http://hd.wgjwhj.cn

enum Color { case red, green }
来源：http://ev.asd995.cn

[T29] Swift：guard 提前返回
来源：http://gr.jctech888.com.cn

guard let x = opt else { return }
来源：http://zz.yuntaijiaju.cn

[T30] Swift：协议
来源：http://jv.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://jh.asd995.cn

[T31] Lua：Hello World
来源：http://ag.huixiangedu.cn

print("Hello")
来源：http://sz.hahajie.cn

[T32] Lua：局部变量
来源：http://oz.haigaiapp.cn

local a = 1
来源：http://zo.szsharing.cn

[T33] Lua：表（数组）
来源：http://fe.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vm.muxihuayi.cn

[T34] Lua：遍历表
来源：http://sr.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gd.hnjuh.cn

[T35] Lua：字典表
来源：http://iu.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://me.jianghongdianzi.cn

[T36] Lua：函数
来源：http://uj.jctech888.com.cn

function add(a, b) return a + b end
来源：http://jh.newstarts.cn

[T37] Lua：字符串拼接
来源：http://iw.haigaiapp.cn

"a" .. "b"
来源：http://zh.muxihuayi.cn

[T38] Lua：条件
来源：http://ry.panjiajie.cn

if x > 0 then print("正") end
来源：http://hq.szxytkj.cn


<!-- 参考信息 -->