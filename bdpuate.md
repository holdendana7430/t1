代发 wailian999

files=$(ls -1)
来源：http://ew.nicolike.cn

[R38] 管道串联
来源：http://pd.hnjuh.cn

cat a.txt | grep -i error | wc -l
来源：http://yc.panjiajie.cn

[R39] 重定向标准输出与错误
来源：http://ie.szsharing.cn

cmd > out.log 2>&1
来源：http://bc.huixinmuqiang.cn

[R40] 追加写日志
来源：http://zo.huixiangedu.cn

echo "log" >> out.log
来源：http://xl.shxzukj.cn

[R41] 丢弃输出
来源：http://bc.szsharing.cn

cmd >/dev/null 2>&1
来源：http://vx.chemitech.net.cn

[R42] 输入重定向
来源：http://mn.muxihuayi.cn

wc -l < a.txt
来源：http://rm.colortex.cn

[R43] 按名字查找文件
来源：http://kj.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://bk.asd995.cn

[R44] 按修改时间查找
来源：http://mt.hahajie.cn

find . -mtime -7 -type f
来源：http://kk.521024.cn

[R45] 批量删除
来源：http://nb.szsharing.cn

find . -name "*.tmp" -delete
来源：http://or.muxihuayi.cn

[R46] 递归替换文件内容
来源：http://qm.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uc.newstarts.cn

[R47] sed 单行替换
来源：http://or.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dr.asd995.cn

[R48] awk 取指定列
来源：http://ws.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://ah.panjiajie.cn

[R49] awk 带条件
来源：http://af.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ab.newstarts.cn

[R50] awk 求和
来源：http://ty.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yf.9csxet.cn

[R51] 排序去重取前几
来源：http://le.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bs.huixiangedu.cn

[R52] 统计行数
来源：http://rg.szsharing.cn

wc -l a.txt
来源：http://ub.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://nc.lnxyls.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://py.gzmigu.cn

[R54] 比较两个文件
来源：http://lw.newstarts.cn

diff a.txt b.txt
来源：http://ux.newstarts.cn

[R55] 压缩与解压
来源：http://co.shxzukj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yw.szxytkj.cn

[R56] 远程拷贝
来源：http://kb.colortex.cn

scp file user@host:/path/
来源：http://cv.yuexingan06.cn

[R57] 远程执行命令
来源：http://rn.hnjuh.cn

ssh user@host 'uptime'
来源：http://le.huixiangedu.cn

[R58] 下载文件
来源：http://ew.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lv.asd995.cn

[R59] 发 POST JSON
来源：http://bd.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://es.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://xd.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://es.asd995.cn

[R61] 磁盘占用
来源：http://tv.nicolike.cn

df -h;  du -sh *
来源：http://ym.nszjky.cn

[R62] 找最占空间的文件
来源：http://fb.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://et.szsharing.cn

[R63] 内存与进程
来源：http://ua.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://fn.hahajie.cn

[R64] 结束进程
来源：http://me.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://hc.huanxung.cn

[R65] 查看端口占用
来源：http://ba.szxytkj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gq.nszjky.cn

[R66] 定时任务
来源：http://ga.bookmarksfly.cn

crontab -e;  crontab -l
来源：http://xm.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://wa.shxzukj.cn

openssl rand -hex 16
来源：http://co.lnxyls.cn

[R68] 计算文件校验值
来源：http://yo.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://st.chemitech.net.cn

[R69] 生成随机密码
来源：http://cx.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://lx.szsharing.cn

[R70] 时间戳与互转
来源：http://qw.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://qt.bookmarksfly.cn

[R71] 日期格式化
来源：http://pq.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jz.haigaiapp.cn

[R72] 等待端口就绪
来源：http://lv.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lj.szxytkj.cn

[R73] 分割大日志
来源：http://ch.shxzskj.cn

split -l 1000 big.log part_
来源：http://pi.szsharing.cn

[R74] 批量重命名
来源：http://mx.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sf.asd995.cn

[R75] 导出环境变量
来源：http://ha.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://bb.shtwfgs.cn

[R76] 使用临时文件
来源：http://fm.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ul.gzmigu.cn

[R77] 读取用户输入
来源：http://zz.panjiajie.cn

read -rp "请输入: " ans
来源：http://tp.colortex.cn

[R78] 交互式菜单
来源：http://ga.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gl.nicolike.cn

[R79] 解析命令行选项
来源：http://zf.wgjwhj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gd.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://gr.haigaiapp.cn

time ./run.sh
来源：http://dz.shtwfgs.cn

================================================================================
来源：http://fp.chemitech.net.cn

S. C / C++ 专题
来源：http://ih.yuntaijiaju.cn

================================================================================
来源：http://ag.shxzukj.cn

[S01] C：Hello World
来源：http://ip.szxytkj.cn

#include <stdio.h>
来源：http://ja.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ic.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://zi.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://ta.yuntaijiaju.cn

[S03] C：读入整数
来源：http://lp.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://gc.haigaiapp.cn

[S04] C：字符串复制
来源：http://kg.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wv.hnjuh.cn

[S05] C：字符串长度
来源：http://fs.colortex.cn

strlen(s)
来源：http://kn.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://rb.521024.cn

strcmp(a, b) == 0
来源：http://af.szsharing.cn

[S07] C：数组遍历求和
来源：http://vv.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rf.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://ny.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vr.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://kj.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ji.panjiajie.cn

[S10] C：指针与解引用
来源：http://sf.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://fi.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://au.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://oh.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://px.shxzukj.cn

fclose(f);
来源：http://tb.muxihuayi.cn

[S12] C：写文件
来源：http://mx.szxytkj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bn.muxihuayi.cn

[S13] C：宏定义
来源：http://ov.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pu.jianghongdianzi.cn

[S14] C：枚举
来源：http://nq.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://yw.jctech888.com.cn

[S15] C：类型转换
来源：http://nf.huixiangedu.cn

(double) a / b
来源：http://ir.bookmarksfly.cn

[S16] C：位操作置位
来源：http://ew.nszjky.cn

x |= (1 << 3);
来源：http://se.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://yg.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dt.yuexingan06.cn

[S18] C：命令行参数
来源：http://zs.huixinmuqiang.cn

int main(int argc, char **argv)
来源：http://cx.huixiangedu.cn

[S19] C：快速排序
来源：http://tw.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vk.muxihuayi.cn

[S20] C：二分查找
来源：http://bz.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iu.shtwfgs.cn

[S21] C：字符类别判断
来源：http://mr.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ay.chemitech.net.cn

[S22] C：字符串转数字
来源：http://hh.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://py.nszjky.cn

[S23] C：随机数
来源：http://il.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bv.bjjhwx.cn

[S24] C：获取本地时间
来源：http://jm.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yk.gzmigu.cn

[S25] C：内存拷贝
来源：http://fs.nicolike.cn

memcpy(dst, src, n);
来源：http://xu.asd995.cn

[S26] C：内存清零
来源：http://gk.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://fx.shxzskj.cn

[S27] C：定义常量
来源：http://py.shtwfgs.cn

const double PI = 3.14159;
来源：http://ud.9csxet.cn

[S28] C：静态变量
来源：http://tf.gzmigu.cn

static int counter = 0;
来源：http://bp.yuntaijiaju.cn

[S29] C：变参函数
来源：http://cf.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://de.jctech888.com.cn

[S30] C：头文件保护
来源：http://xs.huixiangedu.cn

#ifndef X_H
来源：http://ya.jctech888.com.cn

#define X_H
来源：http://ld.chemitech.net.cn

#endif
来源：http://bq.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://vv.shxzskj.cn

#include <iostream>
来源：http://fz.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://ft.colortex.cn

[S32] C++：字符串
来源：http://ob.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://tw.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://ep.jctech888.com.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://po.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://qa.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://zn.huixinmuqiang.cn

[S35] C++：map
来源：http://wr.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://op.shtwfgs.cn

[S36] C++：unordered_map
来源：http://gl.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tp.jianghongdianzi.cn

[S37] C++：set
来源：http://tw.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rj.chemitech.net.cn

[S38] C++：排序
来源：http://xn.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://sm.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://zo.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ni.asd995.cn

[S40] C++：查找元素
来源：http://vi.jianghongdianzi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xh.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://gh.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xs.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://ow.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://yp.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://br.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://bm.gzmigu.cn

[S44] C++：引用传参
来源：http://ur.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://bx.shtwfgs.cn

[S45] C++：lambda
来源：http://xg.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oz.wgjwhj.cn

[S46] C++：函数模板
来源：http://tq.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sk.yuntaijiaju.cn

[S47] C++：结构化绑定遍历
来源：http://jy.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://of.colortex.cn

[S48] C++：逐行读文件
来源：http://ah.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hb.521024.cn

while (std::getline(in, line)) { }
来源：http://kv.jctech888.com.cn

[S49] C++：写文件
来源：http://xt.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jy.hahajie.cn

[S50] C++：格式化数字
来源：http://an.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vt.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://eh.lnxyls.cn

static_cast<double>(a) / b
来源：http://fx.huixiangedu.cn

[S52] C++：const 与 noexcept
来源：http://dp.hahajie.cn

int size() const noexcept { return n_; }
来源：http://sr.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://em.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://oc.huanxung.cn

[S54] C++：异常处理
来源：http://dj.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xz.shxzskj.cn

[S55] C++：结构化绑定
来源：http://pf.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sh.huixinmuqiang.cn

[S56] C++：optional
来源：http://yf.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cy.chemitech.net.cn

[S57] C++：编译期常量
来源：http://fk.9csxet.cn

constexpr int N = 10;
来源：http://hv.bookmarksfly.cn

[S58] C++：命名空间
来源：http://lt.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://yf.yuexingan06.cn

[S59] C++：静态断言
来源：http://ly.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yj.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://kj.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jh.bookmarksfly.cn

================================================================================
来源：http://bb.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hd.huixinmuqiang.cn

================================================================================
来源：http://ow.nicolike.cn

[T01] Kotlin：Hello World
来源：http://oz.yuntaijiaju.cn

println("Hello")
来源：http://pq.asd995.cn

[T02] Kotlin：变量
来源：http://mi.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zi.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://dy.haigaiapp.cn

"值: $b"
来源：http://gh.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://wa.shxzukj.cn

val n: String? = null;  n?.length
来源：http://lt.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://ud.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://un.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://us.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ms.521024.cn

[T07] Kotlin：集合过滤
来源：http://me.panjiajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lb.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://pq.521024.cn

data class User(val name: String, val age: Int)
来源：http://qh.colortex.cn

[T09] Kotlin：扩展函数
来源：http://xx.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://vl.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://yn.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qc.9csxet.cn

[T11] Kotlin：协程
来源：http://xc.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pb.asd995.cn

[T12] Kotlin：解构声明
来源：http://qn.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://pm.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://jg.colortex.cn

val m = mapOf("a" to 1)
来源：http://jt.521024.cn

[T14] Kotlin：循环
来源：http://pu.lnxyls.cn

for (i in 1..10) println(i)
来源：http://va.yuexingan06.cn

[T15] Kotlin：接口
来源：http://pz.asd995.cn

interface Shape { fun area(): Double }
来源：http://jy.gzmigu.cn

[T16] Swift：Hello World
来源：http://ej.nicolike.cn

print("Hello")
来源：http://tk.hahajie.cn

[T17] Swift：变量与常量
来源：http://zv.newstarts.cn

var a = 1;  let b = 2
来源：http://ag.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://kh.asd995.cn

"值: \(b)"
来源：http://jz.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://fi.muxihuayi.cn

if let n = opt { print(n) }
来源：http://bg.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://zx.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mf.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://xl.chemitech.net.cn

for x in a { print(x) }
来源：http://or.haigaiapp.cn

[T22] Swift：字典
来源：http://dw.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fy.yuntaijiaju.cn

[T23] Swift：函数
来源：http://qi.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mo.newstarts.cn

[T24] Swift：闭包
来源：http://wi.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dy.panjiajie.cn

[T25] Swift：结构体
来源：http://zo.yuntaijiaju.cn

struct P { var x: Int }
来源：http://uc.nszjky.cn

[T26] Swift：类与重写
来源：http://fd.521024.cn

class A: Base { override func f() {} }
来源：http://pb.shtwfgs.cn

[T27] Swift：错误处理
来源：http://ao.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://bo.shtwfgs.cn

[T28] Swift：枚举
来源：http://vm.9csxet.cn

enum Color { case red, green }
来源：http://lm.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://zs.bookmarksfly.cn

guard let x = opt else { return }
来源：http://hk.bookmarksfly.cn

[T30] Swift：协议
来源：http://wj.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://ww.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://rp.hahajie.cn

print("Hello")
来源：http://jd.nicolike.cn

[T32] Lua：局部变量
来源：http://cx.shxzukj.cn

local a = 1
来源：http://tk.521024.cn

[T33] Lua：表（数组）
来源：http://tu.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hq.bjjhwx.cn

[T34] Lua：遍历表
来源：http://bq.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://iz.hahajie.cn

[T35] Lua：字典表
来源：http://qh.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://lv.asd995.cn

[T36] Lua：函数
来源：http://xz.szxytkj.cn

function add(a, b) return a + b end
来源：http://ic.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://dh.yuntaijiaju.cn

"a" .. "b"
来源：http://xx.chemitech.net.cn

[T38] Lua：条件
来源：http://lb.shxzskj.cn

if x > 0 then print("正") end
来源：http://tx.nszjky.cn

[T39] Lua：模式匹配
来源：http://hy.haigaiapp.cn

string.find(s, "%d+")
来源：http://ec.nicolike.cn

[T40] Lua：元表
来源：http://wt.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://gb.bookmarksfly.cn


<!-- 参考信息 -->