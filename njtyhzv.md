代发 wailian999

cmd >/dev/null 2>&1
来源：http://gb.yuntaijiaju.cn

[R42] 输入重定向
来源：http://pc.newstarts.cn

wc -l < a.txt
来源：http://ql.szsharing.cn

[R43] 按名字查找文件
来源：http://eo.bjjhwx.cn

find . -name "*.log" -type f
来源：http://og.shxzukj.cn

[R44] 按修改时间查找
来源：http://bi.panjiajie.cn

find . -mtime -7 -type f
来源：http://cm.huanxung.cn

[R45] 批量删除
来源：http://yt.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://ks.newstarts.cn

[R46] 递归替换文件内容
来源：http://yy.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kc.huixiangedu.cn

[R47] sed 单行替换
来源：http://pg.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nm.nszjky.cn

[R48] awk 取指定列
来源：http://fq.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://tl.asd995.cn

[R49] awk 带条件
来源：http://eh.jianghongdianzi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ak.bjjhwx.cn

[R50] awk 求和
来源：http://lo.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ct.bjjhwx.cn

[R51] 排序去重取前几
来源：http://nu.nszjky.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kz.panjiajie.cn

[R52] 统计行数
来源：http://ba.asd995.cn

wc -l a.txt
来源：http://ns.hahajie.cn

[R53] 查看文件头与实时尾
来源：http://qk.gzmigu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mj.gzmigu.cn

[R54] 比较两个文件
来源：http://mj.asd995.cn

diff a.txt b.txt
来源：http://gy.shxzukj.cn

[R55] 压缩与解压
来源：http://ib.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mc.shtwfgs.cn

[R56] 远程拷贝
来源：http://kt.lnxyls.cn

scp file user@host:/path/
来源：http://vc.colortex.cn

[R57] 远程执行命令
来源：http://ws.szxytkj.cn

ssh user@host 'uptime'
来源：http://in.huixiangedu.cn

[R58] 下载文件
来源：http://kq.huixiangedu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hr.nszjky.cn

[R59] 发 POST JSON
来源：http://af.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qn.colortex.cn

[R60] 只看 HTTP 状态码
来源：http://ct.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uz.nszjky.cn

[R61] 磁盘占用
来源：http://pm.colortex.cn

df -h;  du -sh *
来源：http://ik.szsharing.cn

[R62] 找最占空间的文件
来源：http://gc.colortex.cn

du -ah . | sort -rh | head -10
来源：http://sa.chemitech.net.cn

[R63] 内存与进程
来源：http://la.521024.cn

free -h;  ps aux | grep nginx
来源：http://vj.lnxyls.cn

[R64] 结束进程
来源：http://ud.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://vp.bookmarksfly.cn

[R65] 查看端口占用
来源：http://fw.huixinmuqiang.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kd.muxihuayi.cn

[R66] 定时任务
来源：http://hv.shxzukj.cn

crontab -e;  crontab -l
来源：http://wp.colortex.cn

[R67] 生成随机十六进制串
来源：http://qb.yuntaijiaju.cn

openssl rand -hex 16
来源：http://xx.haigaiapp.cn

[R68] 计算文件校验值
来源：http://tm.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qq.colortex.cn

[R69] 生成随机密码
来源：http://xv.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://ty.shxzukj.cn

[R70] 时间戳与互转
来源：http://pj.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://va.9csxet.cn

[R71] 日期格式化
来源：http://iw.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vg.9csxet.cn

[R72] 等待端口就绪
来源：http://pu.newstarts.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://me.bookmarksfly.cn

[R73] 分割大日志
来源：http://yx.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://gf.chemitech.net.cn

[R74] 批量重命名
来源：http://ja.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bb.bookmarksfly.cn

[R75] 导出环境变量
来源：http://bj.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://ku.jctech888.com.cn

[R76] 使用临时文件
来源：http://az.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ft.lnxyls.cn

[R77] 读取用户输入
来源：http://vj.haigaiapp.cn

read -rp "请输入: " ans
来源：http://yr.lnxyls.cn

[R78] 交互式菜单
来源：http://ms.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qj.bjjhwx.cn

[R79] 解析命令行选项
来源：http://hs.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zw.nszjky.cn

[R80] 查看脚本执行耗时
来源：http://le.muxihuayi.cn

time ./run.sh
来源：http://zd.panjiajie.cn

================================================================================
来源：http://tm.shtwfgs.cn

S. C / C++ 专题
来源：http://gy.szxytkj.cn

================================================================================
来源：http://vo.lnxyls.cn

[S01] C：Hello World
来源：http://mz.chemitech.net.cn

#include <stdio.h>
来源：http://yh.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gk.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://el.gzmigu.cn

int a = 10; printf("%d\n", a);
来源：http://su.wgjwhj.cn

[S03] C：读入整数
来源：http://cc.nicolike.cn

int x; scanf("%d", &x);
来源：http://uv.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://qg.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rq.hnjuh.cn

[S05] C：字符串长度
来源：http://sh.huixinmuqiang.cn

strlen(s)
来源：http://oj.huixiangedu.cn

[S06] C：字符串比较
来源：http://if.huanxung.cn

strcmp(a, b) == 0
来源：http://mw.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://af.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kr.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://vx.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rt.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://uw.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rd.yuexingan06.cn

[S10] C：指针与解引用
来源：http://ge.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://vl.yuexingan06.cn

[S11] C：逐行读文件
来源：http://wv.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://tg.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vw.yuntaijiaju.cn

fclose(f);
来源：http://ge.colortex.cn

[S12] C：写文件
来源：http://no.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fr.jctech888.com.cn

[S13] C：宏定义
来源：http://kk.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ar.wgjwhj.cn

[S14] C：枚举
来源：http://ic.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://mj.yuexingan06.cn

[S15] C：类型转换
来源：http://ud.szxytkj.cn

(double) a / b
来源：http://qd.asd995.cn

[S16] C：位操作置位
来源：http://xz.hahajie.cn

x |= (1 << 3);
来源：http://fa.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://ot.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jf.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://jz.huanxung.cn

int main(int argc, char **argv)
来源：http://uf.shtwfgs.cn

[S19] C：快速排序
来源：http://kx.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zn.panjiajie.cn

[S20] C：二分查找
来源：http://fm.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bx.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://ra.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bp.hnjuh.cn

[S22] C：字符串转数字
来源：http://vr.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cw.hahajie.cn

[S23] C：随机数
来源：http://sz.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mt.muxihuayi.cn

[S24] C：获取本地时间
来源：http://ju.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yd.chemitech.net.cn

[S25] C：内存拷贝
来源：http://jj.szsharing.cn

memcpy(dst, src, n);
来源：http://sn.521024.cn

[S26] C：内存清零
来源：http://rz.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://ss.colortex.cn

[S27] C：定义常量
来源：http://ul.muxihuayi.cn

const double PI = 3.14159;
来源：http://wm.jianghongdianzi.cn

[S28] C：静态变量
来源：http://th.bookmarksfly.cn

static int counter = 0;
来源：http://vq.lnxyls.cn

[S29] C：变参函数
来源：http://eg.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kv.nszjky.cn

[S30] C：头文件保护
来源：http://fm.shtwfgs.cn

#ifndef X_H
来源：http://fg.9csxet.cn

#define X_H
来源：http://pe.chemitech.net.cn

#endif
来源：http://wz.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://zo.yuexingan06.cn

#include <iostream>
来源：http://sk.bookmarksfly.cn

int main() { std::cout << "Hello\n"; }
来源：http://mt.521024.cn

[S32] C++：字符串
来源：http://cf.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://jp.szsharing.cn

[S33] C++：vector 增删
来源：http://fq.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cr.colortex.cn

[S34] C++：遍历 vector
来源：http://zv.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://bq.colortex.cn

[S35] C++：map
来源：http://zp.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hq.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://hy.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gd.gzmigu.cn

[S37] C++：set
来源：http://ke.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ek.bookmarksfly.cn

[S38] C++：排序
来源：http://uk.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://yp.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://md.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sj.521024.cn

[S40] C++：查找元素
来源：http://rz.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ww.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://ad.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lv.colortex.cn

[S42] C++：继承与虚函数
来源：http://bv.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://li.haigaiapp.cn

[S43] C++：智能指针
来源：http://ak.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://yv.colortex.cn

[S44] C++：引用传参
来源：http://gc.huanxung.cn

void inc(int &x) { ++x; }
来源：http://mj.jctech888.com.cn

[S45] C++：lambda
来源：http://pi.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ff.gzmigu.cn

[S46] C++：函数模板
来源：http://gq.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yb.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://my.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nt.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://tw.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jf.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://gw.yuexingan06.cn

[S49] C++：写文件
来源：http://fx.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zw.szxytkj.cn

[S50] C++：格式化数字
来源：http://ht.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vu.nicolike.cn

[S51] C++：显式类型转换
来源：http://nw.nszjky.cn

static_cast<double>(a) / b
来源：http://jz.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://zm.colortex.cn

int size() const noexcept { return n_; }
来源：http://vn.shxzskj.cn

[S53] C++：移动语义
来源：http://tu.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://my.chemitech.net.cn

[S54] C++：异常处理
来源：http://ka.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://da.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://pt.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mx.muxihuayi.cn

[S56] C++：optional
来源：http://pb.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vl.hahajie.cn

[S57] C++：编译期常量
来源：http://ev.shxzukj.cn

constexpr int N = 10;
来源：http://em.newstarts.cn

[S58] C++：命名空间
来源：http://on.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://hd.shxzskj.cn

[S59] C++：静态断言
来源：http://rq.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lk.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://pm.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eu.gzmigu.cn

================================================================================
来源：http://td.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bz.hahajie.cn

================================================================================
来源：http://yg.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://xt.yuexingan06.cn

println("Hello")
来源：http://lw.wgjwhj.cn

[T02] Kotlin：变量
来源：http://cw.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rx.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://nf.huixinmuqiang.cn

"值: $b"
来源：http://ya.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://hd.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://ma.521024.cn

[T05] Kotlin：when 表达式
来源：http://hd.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://su.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://mo.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pc.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://kl.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rt.nicolike.cn

[T08] Kotlin：数据类
来源：http://qs.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://rl.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://nm.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://sz.asd995.cn

[T10] Kotlin：默认参数
来源：http://em.bjjhwx.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mp.bjjhwx.cn

[T11] Kotlin：协程
来源：http://pm.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://no.shxzukj.cn

[T12] Kotlin：解构声明
来源：http://jc.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://rr.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://zi.hahajie.cn

val m = mapOf("a" to 1)
来源：http://tb.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://iq.nicolike.cn

for (i in 1..10) println(i)
来源：http://rt.panjiajie.cn

[T15] Kotlin：接口
来源：http://xw.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://uz.nicolike.cn

[T16] Swift：Hello World
来源：http://oc.colortex.cn

print("Hello")
来源：http://iw.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://lk.wgjwhj.cn

var a = 1;  let b = 2
来源：http://li.lnxyls.cn

[T18] Swift：字符串插值
来源：http://ne.huixinmuqiang.cn

"值: \(b)"
来源：http://fe.szsharing.cn

[T19] Swift：可选绑定
来源：http://ui.huanxung.cn

if let n = opt { print(n) }
来源：http://pw.hahajie.cn

[T20] Swift：数组操作
来源：http://ug.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uc.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://nv.chemitech.net.cn

for x in a { print(x) }
来源：http://ej.shxzskj.cn

[T22] Swift：字典
来源：http://vn.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xm.wgjwhj.cn

[T23] Swift：函数
来源：http://xp.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mk.wgjwhj.cn

[T24] Swift：闭包
来源：http://hg.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://eo.szxytkj.cn

[T25] Swift：结构体
来源：http://xn.lnxyls.cn

struct P { var x: Int }
来源：http://gz.newstarts.cn

[T26] Swift：类与重写
来源：http://tf.lnxyls.cn

class A: Base { override func f() {} }
来源：http://ro.haigaiapp.cn

[T27] Swift：错误处理
来源：http://dw.521024.cn

do { try f() } catch { print(error) }
来源：http://lo.shtwfgs.cn

[T28] Swift：枚举
来源：http://kc.shtwfgs.cn

enum Color { case red, green }
来源：http://fc.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://wx.521024.cn

guard let x = opt else { return }
来源：http://ff.wgjwhj.cn

[T30] Swift：协议
来源：http://bo.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://ew.muxihuayi.cn

[T31] Lua：Hello World
来源：http://fb.colortex.cn

print("Hello")
来源：http://xh.newstarts.cn

[T32] Lua：局部变量
来源：http://du.haigaiapp.cn

local a = 1
来源：http://ae.szxytkj.cn

[T33] Lua：表（数组）
来源：http://mp.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uq.newstarts.cn

[T34] Lua：遍历表
来源：http://au.newstarts.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wg.hnjuh.cn

[T35] Lua：字典表
来源：http://sr.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://qq.jianghongdianzi.cn

[T36] Lua：函数
来源：http://zg.asd995.cn

function add(a, b) return a + b end
来源：http://wg.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://mm.huixinmuqiang.cn

"a" .. "b"
来源：http://gu.asd995.cn

[T38] Lua：条件
来源：http://vd.huixiangedu.cn

if x > 0 then print("正") end
来源：http://ff.newstarts.cn

[T39] Lua：模式匹配
来源：http://ms.shxzukj.cn

string.find(s, "%d+")
来源：http://kg.newstarts.cn

[T40] Lua：元表
来源：http://au.szsharing.cn

setmetatable({}, { __index = base })
来源：http://vg.szsharing.cn

[T41] Perl：Hello World
来源：http://iw.newstarts.cn

print "Hello\n";
来源：http://lc.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://hl.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://db.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://nn.nszjky.cn

"值: $a"
来源：http://qq.muxihuayi.cn

[T44] Perl：条件
来源：http://se.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://vw.nicolike.cn


<!-- 参考信息 -->