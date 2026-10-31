代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://um.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://nq.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nw.nicolike.cn

[R37] 把输出赋给变量
来源：http://gq.huixinmuqiang.cn

files=$(ls -1)
来源：http://sd.hahajie.cn

[R38] 管道串联
来源：http://vo.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://pb.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://zh.gzmigu.cn

cmd > out.log 2>&1
来源：http://wv.hnjuh.cn

[R40] 追加写日志
来源：http://xw.9csxet.cn

echo "log" >> out.log
来源：http://ok.shxzskj.cn

[R41] 丢弃输出
来源：http://cc.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://rl.hahajie.cn

[R42] 输入重定向
来源：http://tq.huanxung.cn

wc -l < a.txt
来源：http://bm.jctech888.com.cn

[R43] 按名字查找文件
来源：http://sc.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://sr.haigaiapp.cn

[R44] 按修改时间查找
来源：http://nt.yuexingan06.cn

find . -mtime -7 -type f
来源：http://aq.wgjwhj.cn

[R45] 批量删除
来源：http://eq.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://di.szxytkj.cn

[R46] 递归替换文件内容
来源：http://zf.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fj.newstarts.cn

[R47] sed 单行替换
来源：http://la.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rw.colortex.cn

[R48] awk 取指定列
来源：http://pp.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://ie.jctech888.com.cn

[R49] awk 带条件
来源：http://dg.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fh.chemitech.net.cn

[R50] awk 求和
来源：http://no.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lv.lnxyls.cn

[R51] 排序去重取前几
来源：http://ao.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cx.jianghongdianzi.cn

[R52] 统计行数
来源：http://wm.szxytkj.cn

wc -l a.txt
来源：http://ld.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://iw.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://th.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://aq.chemitech.net.cn

diff a.txt b.txt
来源：http://iq.bjjhwx.cn

[R55] 压缩与解压
来源：http://om.jctech888.com.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gt.shxzukj.cn

[R56] 远程拷贝
来源：http://uv.yuntaijiaju.cn

scp file user@host:/path/
来源：http://wh.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://pz.gzmigu.cn

ssh user@host 'uptime'
来源：http://or.newstarts.cn

[R58] 下载文件
来源：http://ev.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cb.hnjuh.cn

[R59] 发 POST JSON
来源：http://ud.jianghongdianzi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nm.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://bm.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rw.asd995.cn

[R61] 磁盘占用
来源：http://id.yuexingan06.cn

df -h;  du -sh *
来源：http://br.gzmigu.cn

[R62] 找最占空间的文件
来源：http://qe.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://vu.szxytkj.cn

[R63] 内存与进程
来源：http://gc.wgjwhj.cn

free -h;  ps aux | grep nginx
来源：http://zr.colortex.cn

[R64] 结束进程
来源：http://cx.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://tw.muxihuayi.cn

[R65] 查看端口占用
来源：http://kh.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wc.bookmarksfly.cn

[R66] 定时任务
来源：http://yf.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://wp.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://qe.lnxyls.cn

openssl rand -hex 16
来源：http://cw.hahajie.cn

[R68] 计算文件校验值
来源：http://bx.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ff.gzmigu.cn

[R69] 生成随机密码
来源：http://uz.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://ss.nicolike.cn

[R70] 时间戳与互转
来源：http://lx.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://qz.nszjky.cn

[R71] 日期格式化
来源：http://iw.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ly.wgjwhj.cn

[R72] 等待端口就绪
来源：http://oz.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hv.huixinmuqiang.cn

[R73] 分割大日志
来源：http://ea.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://hd.colortex.cn

[R74] 批量重命名
来源：http://ch.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qq.9csxet.cn

[R75] 导出环境变量
来源：http://kx.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://if.gzmigu.cn

[R76] 使用临时文件
来源：http://ds.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ok.huixiangedu.cn

[R77] 读取用户输入
来源：http://cr.huixiangedu.cn

read -rp "请输入: " ans
来源：http://dg.9csxet.cn

[R78] 交互式菜单
来源：http://si.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bx.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://wr.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://us.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://ma.bookmarksfly.cn

time ./run.sh
来源：http://gd.chemitech.net.cn

================================================================================
来源：http://bb.521024.cn

S. C / C++ 专题
来源：http://vq.yuntaijiaju.cn

================================================================================
来源：http://pc.jianghongdianzi.cn

[S01] C：Hello World
来源：http://he.panjiajie.cn

#include <stdio.h>
来源：http://rw.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wo.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://ma.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://eo.huanxung.cn

[S03] C：读入整数
来源：http://wz.newstarts.cn

int x; scanf("%d", &x);
来源：http://tj.szsharing.cn

[S04] C：字符串复制
来源：http://lv.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ed.nszjky.cn

[S05] C：字符串长度
来源：http://yr.huixinmuqiang.cn

strlen(s)
来源：http://nk.gzmigu.cn

[S06] C：字符串比较
来源：http://ez.yuexingan06.cn

strcmp(a, b) == 0
来源：http://lw.hnjuh.cn

[S07] C：数组遍历求和
来源：http://yi.jianghongdianzi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bx.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://md.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wd.asd995.cn

[S09] C：结构体定义与初始化
来源：http://kz.hnjuh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ay.shxzukj.cn

[S10] C：指针与解引用
来源：http://md.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://hv.nicolike.cn

[S11] C：逐行读文件
来源：http://ek.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://on.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ve.szxytkj.cn

fclose(f);
来源：http://rp.huixinmuqiang.cn

[S12] C：写文件
来源：http://xa.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xf.newstarts.cn

[S13] C：宏定义
来源：http://bn.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ga.huixinmuqiang.cn

[S14] C：枚举
来源：http://dv.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://dn.521024.cn

[S15] C：类型转换
来源：http://ad.bookmarksfly.cn

(double) a / b
来源：http://qz.chemitech.net.cn

[S16] C：位操作置位
来源：http://eu.lnxyls.cn

x |= (1 << 3);
来源：http://ik.huanxung.cn

[S17] C：安全拼接字符串
来源：http://an.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jy.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://zu.yuexingan06.cn

int main(int argc, char **argv)
来源：http://qk.lnxyls.cn

[S19] C：快速排序
来源：http://gu.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sj.hnjuh.cn

[S20] C：二分查找
来源：http://he.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ie.huixiangedu.cn

[S21] C：字符类别判断
来源：http://pr.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kb.521024.cn

[S22] C：字符串转数字
来源：http://mw.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://da.panjiajie.cn

[S23] C：随机数
来源：http://rk.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wx.shxzukj.cn

[S24] C：获取本地时间
来源：http://cf.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vh.chemitech.net.cn

[S25] C：内存拷贝
来源：http://ou.shxzukj.cn

memcpy(dst, src, n);
来源：http://tp.asd995.cn

[S26] C：内存清零
来源：http://ks.colortex.cn

memset(a, 0, sizeof a);
来源：http://bt.nszjky.cn

[S27] C：定义常量
来源：http://zp.colortex.cn

const double PI = 3.14159;
来源：http://fg.szsharing.cn

[S28] C：静态变量
来源：http://iq.nszjky.cn

static int counter = 0;
来源：http://di.gzmigu.cn

[S29] C：变参函数
来源：http://xp.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pc.szsharing.cn

[S30] C：头文件保护
来源：http://bs.hnjuh.cn

#ifndef X_H
来源：http://hw.bjjhwx.cn

#define X_H
来源：http://ga.asd995.cn

#endif
来源：http://up.nszjky.cn

[S31] C++：Hello World
来源：http://bl.hahajie.cn

#include <iostream>
来源：http://fg.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://ry.hahajie.cn

[S32] C++：字符串
来源：http://gr.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://rs.chemitech.net.cn

[S33] C++：vector 增删
来源：http://hq.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kk.lnxyls.cn

[S34] C++：遍历 vector
来源：http://zi.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://qb.chemitech.net.cn

[S35] C++：map
来源：http://ds.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ed.yuexingan06.cn

[S36] C++：unordered_map
来源：http://hi.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qv.shxzskj.cn

[S37] C++：set
来源：http://ev.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xq.shxzukj.cn

[S38] C++：排序
来源：http://jp.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://gr.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://zu.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wu.colortex.cn

[S40] C++：查找元素
来源：http://mo.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rq.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://kl.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://is.szsharing.cn

[S42] C++：继承与虚函数
来源：http://vr.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://rl.9csxet.cn

[S43] C++：智能指针
来源：http://gf.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://os.jctech888.com.cn

[S44] C++：引用传参
来源：http://mw.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://ig.muxihuayi.cn

[S45] C++：lambda
来源：http://pa.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://se.chemitech.net.cn

[S46] C++：函数模板
来源：http://rc.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vw.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://ov.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ca.shxzukj.cn

[S48] C++：逐行读文件
来源：http://gx.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qd.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://ky.wgjwhj.cn

[S49] C++：写文件
来源：http://fo.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qz.shxzskj.cn

[S50] C++：格式化数字
来源：http://wh.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lo.nicolike.cn

[S51] C++：显式类型转换
来源：http://vs.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://gt.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://qq.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://je.hahajie.cn

[S53] C++：移动语义
来源：http://mj.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://qg.9csxet.cn

[S54] C++：异常处理
来源：http://wc.yuntaijiaju.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hk.szxytkj.cn

[S55] C++：结构化绑定
来源：http://xy.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wg.521024.cn

[S56] C++：optional
来源：http://fi.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yl.gzmigu.cn

[S57] C++：编译期常量
来源：http://mt.yuntaijiaju.cn

constexpr int N = 10;
来源：http://zt.lnxyls.cn

[S58] C++：命名空间
来源：http://vp.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://xk.9csxet.cn

[S59] C++：静态断言
来源：http://aq.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ok.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://xi.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lp.jctech888.com.cn

================================================================================
来源：http://vp.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uv.shxzskj.cn

================================================================================
来源：http://hj.colortex.cn

[T01] Kotlin：Hello World
来源：http://hl.jctech888.com.cn

println("Hello")
来源：http://gj.shtwfgs.cn

[T02] Kotlin：变量
来源：http://mv.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ad.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://bo.bjjhwx.cn

"值: $b"
来源：http://ye.hnjuh.cn

[T04] Kotlin：空安全
来源：http://ve.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://xk.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://ci.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ms.colortex.cn

[T06] Kotlin：集合映射
来源：http://th.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ac.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://he.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hr.huanxung.cn

[T08] Kotlin：数据类
来源：http://bf.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://rr.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://he.colortex.cn

fun String.exclaim() = this + "!"
来源：http://yc.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://qp.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ca.bjjhwx.cn

[T11] Kotlin：协程
来源：http://hr.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lw.nicolike.cn

[T12] Kotlin：解构声明
来源：http://xh.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://ar.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://dz.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://ql.nicolike.cn

[T14] Kotlin：循环
来源：http://bg.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://id.asd995.cn

[T15] Kotlin：接口
来源：http://qy.yuexingan06.cn

interface Shape { fun area(): Double }
来源：http://mv.gzmigu.cn

[T16] Swift：Hello World
来源：http://gi.bookmarksfly.cn

print("Hello")
来源：http://qe.shxzukj.cn

[T17] Swift：变量与常量
来源：http://ha.nicolike.cn

var a = 1;  let b = 2
来源：http://fe.hahajie.cn

[T18] Swift：字符串插值
来源：http://mn.nszjky.cn

"值: \(b)"
来源：http://dk.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://lx.szsharing.cn

if let n = opt { print(n) }
来源：http://tl.gzmigu.cn

[T20] Swift：数组操作
来源：http://kq.nicolike.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zc.lnxyls.cn

[T21] Swift：遍历
来源：http://qs.jianghongdianzi.cn

for x in a { print(x) }
来源：http://hk.muxihuayi.cn

[T22] Swift：字典
来源：http://rb.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kd.szsharing.cn

[T23] Swift：函数
来源：http://ty.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yb.szsharing.cn

[T24] Swift：闭包
来源：http://ji.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nh.szsharing.cn

[T25] Swift：结构体
来源：http://ua.9csxet.cn

struct P { var x: Int }
来源：http://go.huanxung.cn

[T26] Swift：类与重写
来源：http://ug.panjiajie.cn

class A: Base { override func f() {} }
来源：http://jc.szsharing.cn

[T27] Swift：错误处理
来源：http://hy.muxihuayi.cn

do { try f() } catch { print(error) }
来源：http://dg.9csxet.cn

[T28] Swift：枚举
来源：http://td.newstarts.cn

enum Color { case red, green }
来源：http://xd.colortex.cn

[T29] Swift：guard 提前返回
来源：http://xw.shtwfgs.cn

guard let x = opt else { return }
来源：http://vu.521024.cn

[T30] Swift：协议
来源：http://dt.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://dg.newstarts.cn

[T31] Lua：Hello World
来源：http://wx.bookmarksfly.cn

print("Hello")
来源：http://vv.nszjky.cn

[T32] Lua：局部变量
来源：http://ux.jianghongdianzi.cn

local a = 1
来源：http://mw.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://ao.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qs.szsharing.cn

[T34] Lua：遍历表
来源：http://fe.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tc.9csxet.cn

[T35] Lua：字典表
来源：http://kt.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://kr.newstarts.cn

[T36] Lua：函数
来源：http://rc.nicolike.cn

function add(a, b) return a + b end
来源：http://rf.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://nf.shxzskj.cn

"a" .. "b"
来源：http://eo.bookmarksfly.cn

[T38] Lua：条件
来源：http://qv.shxzukj.cn

if x > 0 then print("正") end
来源：http://kc.nicolike.cn


<!-- 参考信息 -->