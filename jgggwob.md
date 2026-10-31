代发 wailian999

cmd >/dev/null 2>&1
来源：http://jq.asd995.cn

[R42] 输入重定向
来源：http://rc.nszjky.cn

wc -l < a.txt
来源：http://ml.shxzukj.cn

[R43] 按名字查找文件
来源：http://mq.chemitech.net.cn

find . -name "*.log" -type f
来源：http://te.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://bl.521024.cn

find . -mtime -7 -type f
来源：http://kx.shxzskj.cn

[R45] 批量删除
来源：http://wk.jianghongdianzi.cn

find . -name "*.tmp" -delete
来源：http://tc.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://fj.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rt.wgjwhj.cn

[R47] sed 单行替换
来源：http://ba.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qx.muxihuayi.cn

[R48] awk 取指定列
来源：http://yi.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://hs.nicolike.cn

[R49] awk 带条件
来源：http://pi.lnxyls.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mc.asd995.cn

[R50] awk 求和
来源：http://ew.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cb.hahajie.cn

[R51] 排序去重取前几
来源：http://md.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://za.haigaiapp.cn

[R52] 统计行数
来源：http://uq.haigaiapp.cn

wc -l a.txt
来源：http://ul.asd995.cn

[R53] 查看文件头与实时尾
来源：http://bm.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pz.bookmarksfly.cn

[R54] 比较两个文件
来源：http://yf.szxytkj.cn

diff a.txt b.txt
来源：http://rx.shxzskj.cn

[R55] 压缩与解压
来源：http://rq.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fz.muxihuayi.cn

[R56] 远程拷贝
来源：http://cu.yuexingan06.cn

scp file user@host:/path/
来源：http://cn.nicolike.cn

[R57] 远程执行命令
来源：http://yu.szxytkj.cn

ssh user@host 'uptime'
来源：http://sn.bjjhwx.cn

[R58] 下载文件
来源：http://it.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tt.shxzskj.cn

[R59] 发 POST JSON
来源：http://yf.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hw.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://jh.muxihuayi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hn.szxytkj.cn

[R61] 磁盘占用
来源：http://qn.9csxet.cn

df -h;  du -sh *
来源：http://su.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://oc.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://ca.wgjwhj.cn

[R63] 内存与进程
来源：http://sz.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://ky.yuntaijiaju.cn

[R64] 结束进程
来源：http://ky.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://uu.wgjwhj.cn

[R65] 查看端口占用
来源：http://ow.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ll.huixiangedu.cn

[R66] 定时任务
来源：http://ci.521024.cn

crontab -e;  crontab -l
来源：http://sl.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://ep.panjiajie.cn

openssl rand -hex 16
来源：http://il.yuexingan06.cn

[R68] 计算文件校验值
来源：http://rx.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ib.shxzskj.cn

[R69] 生成随机密码
来源：http://cl.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://qd.nicolike.cn

[R70] 时间戳与互转
来源：http://vj.nszjky.cn

date +%s;  date -d @1700000000
来源：http://fq.shtwfgs.cn

[R71] 日期格式化
来源：http://qe.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yi.lnxyls.cn

[R72] 等待端口就绪
来源：http://pk.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kd.newstarts.cn

[R73] 分割大日志
来源：http://dh.bjjhwx.cn

split -l 1000 big.log part_
来源：http://hl.asd995.cn

[R74] 批量重命名
来源：http://ur.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ts.newstarts.cn

[R75] 导出环境变量
来源：http://dt.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://rp.shxzskj.cn

[R76] 使用临时文件
来源：http://do.jianghongdianzi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qx.huixiangedu.cn

[R77] 读取用户输入
来源：http://jw.yuexingan06.cn

read -rp "请输入: " ans
来源：http://wz.bjjhwx.cn

[R78] 交互式菜单
来源：http://zi.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rq.521024.cn

[R79] 解析命令行选项
来源：http://br.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zv.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://nq.asd995.cn

time ./run.sh
来源：http://xj.yuexingan06.cn

================================================================================
来源：http://bn.gzmigu.cn

S. C / C++ 专题
来源：http://eq.wgjwhj.cn

================================================================================
来源：http://zg.hnjuh.cn

[S01] C：Hello World
来源：http://vs.jctech888.com.cn

#include <stdio.h>
来源：http://zc.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vf.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://nn.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://ro.yuexingan06.cn

[S03] C：读入整数
来源：http://od.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://wb.jctech888.com.cn

[S04] C：字符串复制
来源：http://on.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jw.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://fn.szsharing.cn

strlen(s)
来源：http://ej.yuexingan06.cn

[S06] C：字符串比较
来源：http://bu.lnxyls.cn

strcmp(a, b) == 0
来源：http://lp.jctech888.com.cn

[S07] C：数组遍历求和
来源：http://gq.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yg.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://dk.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jv.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://am.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ma.huixiangedu.cn

[S10] C：指针与解引用
来源：http://dy.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://ec.wgjwhj.cn

[S11] C：逐行读文件
来源：http://it.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://dk.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ck.nszjky.cn

fclose(f);
来源：http://qn.yuntaijiaju.cn

[S12] C：写文件
来源：http://bj.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mf.colortex.cn

[S13] C：宏定义
来源：http://fd.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fl.gzmigu.cn

[S14] C：枚举
来源：http://mn.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://ld.colortex.cn

[S15] C：类型转换
来源：http://qv.yuntaijiaju.cn

(double) a / b
来源：http://el.haigaiapp.cn

[S16] C：位操作置位
来源：http://jd.huixinmuqiang.cn

x |= (1 << 3);
来源：http://ln.asd995.cn

[S17] C：安全拼接字符串
来源：http://kf.huixiangedu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://us.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://ho.bjjhwx.cn

int main(int argc, char **argv)
来源：http://el.szxytkj.cn

[S19] C：快速排序
来源：http://sz.521024.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jr.bjjhwx.cn

[S20] C：二分查找
来源：http://em.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hi.panjiajie.cn

[S21] C：字符类别判断
来源：http://cc.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ld.jctech888.com.cn

[S22] C：字符串转数字
来源：http://kw.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ej.9csxet.cn

[S23] C：随机数
来源：http://vu.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yh.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://ng.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ma.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://ej.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://ov.asd995.cn

[S26] C：内存清零
来源：http://zm.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://rp.colortex.cn

[S27] C：定义常量
来源：http://hu.yuexingan06.cn

const double PI = 3.14159;
来源：http://gi.haigaiapp.cn

[S28] C：静态变量
来源：http://xd.hnjuh.cn

static int counter = 0;
来源：http://kp.gzmigu.cn

[S29] C：变参函数
来源：http://bk.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ih.bjjhwx.cn

[S30] C：头文件保护
来源：http://ad.gzmigu.cn

#ifndef X_H
来源：http://kb.wgjwhj.cn

#define X_H
来源：http://at.colortex.cn

#endif
来源：http://hv.asd995.cn

[S31] C++：Hello World
来源：http://ql.asd995.cn

#include <iostream>
来源：http://sn.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://cf.9csxet.cn

[S32] C++：字符串
来源：http://yj.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://mp.521024.cn

[S33] C++：vector 增删
来源：http://md.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tm.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://ur.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://wz.yuntaijiaju.cn

[S35] C++：map
来源：http://xv.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oz.gzmigu.cn

[S36] C++：unordered_map
来源：http://ht.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sk.gzmigu.cn

[S37] C++：set
来源：http://ui.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ri.huixiangedu.cn

[S38] C++：排序
来源：http://eh.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://en.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://cf.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://om.yuexingan06.cn

[S40] C++：查找元素
来源：http://ps.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ai.szxytkj.cn

[S41] C++：类与构造函数
来源：http://zz.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://in.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://cd.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://qa.newstarts.cn

[S43] C++：智能指针
来源：http://kl.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://fo.hnjuh.cn

[S44] C++：引用传参
来源：http://xd.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://lw.521024.cn

[S45] C++：lambda
来源：http://yf.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ua.shtwfgs.cn

[S46] C++：函数模板
来源：http://qw.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gx.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://ia.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ci.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://al.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://em.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://ef.haigaiapp.cn

[S49] C++：写文件
来源：http://bq.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nq.haigaiapp.cn

[S50] C++：格式化数字
来源：http://ix.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zs.nszjky.cn

[S51] C++：显式类型转换
来源：http://rh.9csxet.cn

static_cast<double>(a) / b
来源：http://yk.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://vc.szsharing.cn

int size() const noexcept { return n_; }
来源：http://hn.szsharing.cn

[S53] C++：移动语义
来源：http://tq.colortex.cn

std::vector<int> w = std::move(v);
来源：http://uc.asd995.cn

[S54] C++：异常处理
来源：http://tg.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qv.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://fo.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ug.jctech888.com.cn

[S56] C++：optional
来源：http://xv.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qs.9csxet.cn

[S57] C++：编译期常量
来源：http://vp.yuexingan06.cn

constexpr int N = 10;
来源：http://jk.bjjhwx.cn

[S58] C++：命名空间
来源：http://mg.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://hg.hahajie.cn

[S59] C++：静态断言
来源：http://kk.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jn.colortex.cn

[S60] C++：遍历并删除元素
来源：http://fe.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://or.huixinmuqiang.cn

================================================================================
来源：http://kn.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wx.bookmarksfly.cn

================================================================================
来源：http://ce.521024.cn

[T01] Kotlin：Hello World
来源：http://ke.gzmigu.cn

println("Hello")
来源：http://ac.asd995.cn

[T02] Kotlin：变量
来源：http://sc.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cr.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://fv.newstarts.cn

"值: $b"
来源：http://ky.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://zo.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://uw.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://lz.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fl.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://vj.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ii.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://eu.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ry.nszjky.cn

[T08] Kotlin：数据类
来源：http://hq.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://sf.colortex.cn

[T09] Kotlin：扩展函数
来源：http://us.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://si.nicolike.cn

[T10] Kotlin：默认参数
来源：http://wa.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://me.wgjwhj.cn

[T11] Kotlin：协程
来源：http://ae.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mr.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://zs.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://rt.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://oq.hahajie.cn

val m = mapOf("a" to 1)
来源：http://zw.muxihuayi.cn

[T14] Kotlin：循环
来源：http://re.huanxung.cn

for (i in 1..10) println(i)
来源：http://xb.szxytkj.cn

[T15] Kotlin：接口
来源：http://up.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://nv.nszjky.cn

[T16] Swift：Hello World
来源：http://lf.lnxyls.cn

print("Hello")
来源：http://ig.9csxet.cn

[T17] Swift：变量与常量
来源：http://jl.bjjhwx.cn

var a = 1;  let b = 2
来源：http://xk.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://na.huixinmuqiang.cn

"值: \(b)"
来源：http://ns.9csxet.cn

[T19] Swift：可选绑定
来源：http://cr.szsharing.cn

if let n = opt { print(n) }
来源：http://gg.muxihuayi.cn

[T20] Swift：数组操作
来源：http://dv.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rj.521024.cn

[T21] Swift：遍历
来源：http://gz.bjjhwx.cn

for x in a { print(x) }
来源：http://ez.wgjwhj.cn

[T22] Swift：字典
来源：http://kl.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sq.huanxung.cn

[T23] Swift：函数
来源：http://rk.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://eq.521024.cn

[T24] Swift：闭包
来源：http://es.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kt.shxzskj.cn

[T25] Swift：结构体
来源：http://tq.huanxung.cn

struct P { var x: Int }
来源：http://uy.chemitech.net.cn

[T26] Swift：类与重写
来源：http://yz.gzmigu.cn

class A: Base { override func f() {} }
来源：http://br.lnxyls.cn

[T27] Swift：错误处理
来源：http://sh.521024.cn

do { try f() } catch { print(error) }
来源：http://gi.muxihuayi.cn

[T28] Swift：枚举
来源：http://sg.shxzskj.cn

enum Color { case red, green }
来源：http://vd.asd995.cn

[T29] Swift：guard 提前返回
来源：http://xb.bookmarksfly.cn

guard let x = opt else { return }
来源：http://tv.szxytkj.cn

[T30] Swift：协议
来源：http://ww.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://yu.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://tm.yuexingan06.cn

print("Hello")
来源：http://nk.szsharing.cn

[T32] Lua：局部变量
来源：http://yf.yuntaijiaju.cn

local a = 1
来源：http://ep.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://cw.chemitech.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ez.szxytkj.cn

[T34] Lua：遍历表
来源：http://ww.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pm.nicolike.cn

[T35] Lua：字典表
来源：http://jg.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://ib.jctech888.com.cn

[T36] Lua：函数
来源：http://ai.shxzskj.cn

function add(a, b) return a + b end
来源：http://re.muxihuayi.cn

[T37] Lua：字符串拼接
来源：http://bp.panjiajie.cn

"a" .. "b"
来源：http://ei.shxzskj.cn

[T38] Lua：条件
来源：http://pj.newstarts.cn

if x > 0 then print("正") end
来源：http://wi.shxzukj.cn

[T39] Lua：模式匹配
来源：http://id.colortex.cn

string.find(s, "%d+")
来源：http://wd.shtwfgs.cn

[T40] Lua：元表
来源：http://bb.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://lu.wgjwhj.cn

[T41] Perl：Hello World
来源：http://df.lnxyls.cn

print "Hello\n";
来源：http://fy.asd995.cn

[T42] Perl：变量类型
来源：http://kx.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jo.hnjuh.cn

[T43] Perl：字符串插值
来源：http://mv.huixiangedu.cn

"值: $a"
来源：http://ro.asd995.cn

[T44] Perl：条件
来源：http://ew.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://nr.shtwfgs.cn


<!-- 参考信息 -->