代发 wailian999

files=$(ls -1)
来源：http://da.jianghongdianzi.cn

[R38] 管道串联
来源：http://eq.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://dz.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://rw.colortex.cn

cmd > out.log 2>&1
来源：http://rj.shxzskj.cn

[R40] 追加写日志
来源：http://br.huixinmuqiang.cn

echo "log" >> out.log
来源：http://em.chemitech.net.cn

[R41] 丢弃输出
来源：http://er.nicolike.cn

cmd >/dev/null 2>&1
来源：http://li.huixiangedu.cn

[R42] 输入重定向
来源：http://fy.huanxung.cn

wc -l < a.txt
来源：http://zd.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://tc.nszjky.cn

find . -name "*.log" -type f
来源：http://kn.chemitech.net.cn

[R44] 按修改时间查找
来源：http://jq.szsharing.cn

find . -mtime -7 -type f
来源：http://qr.lnxyls.cn

[R45] 批量删除
来源：http://ht.jianghongdianzi.cn

find . -name "*.tmp" -delete
来源：http://mp.shxzskj.cn

[R46] 递归替换文件内容
来源：http://gb.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tx.colortex.cn

[R47] sed 单行替换
来源：http://dw.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ji.521024.cn

[R48] awk 取指定列
来源：http://ay.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://me.wgjwhj.cn

[R49] awk 带条件
来源：http://me.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vs.shxzukj.cn

[R50] awk 求和
来源：http://va.jctech888.com.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wg.jctech888.com.cn

[R51] 排序去重取前几
来源：http://oh.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qp.chemitech.net.cn

[R52] 统计行数
来源：http://re.newstarts.cn

wc -l a.txt
来源：http://no.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://yx.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gv.gzmigu.cn

[R54] 比较两个文件
来源：http://da.newstarts.cn

diff a.txt b.txt
来源：http://tj.hahajie.cn

[R55] 压缩与解压
来源：http://hu.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ib.bookmarksfly.cn

[R56] 远程拷贝
来源：http://ue.jctech888.com.cn

scp file user@host:/path/
来源：http://nm.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://vh.huanxung.cn

ssh user@host 'uptime'
来源：http://pf.nicolike.cn

[R58] 下载文件
来源：http://yq.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://af.asd995.cn

[R59] 发 POST JSON
来源：http://ox.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ic.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://ag.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ww.chemitech.net.cn

[R61] 磁盘占用
来源：http://eo.nicolike.cn

df -h;  du -sh *
来源：http://cc.szsharing.cn

[R62] 找最占空间的文件
来源：http://vv.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://og.asd995.cn

[R63] 内存与进程
来源：http://zl.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://eg.bookmarksfly.cn

[R64] 结束进程
来源：http://tj.haigaiapp.cn

kill -9 $(pgrep -f app.py)
来源：http://cw.gzmigu.cn

[R65] 查看端口占用
来源：http://py.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kv.yuexingan06.cn

[R66] 定时任务
来源：http://vc.wgjwhj.cn

crontab -e;  crontab -l
来源：http://qg.haigaiapp.cn

[R67] 生成随机十六进制串
来源：http://uu.yuntaijiaju.cn

openssl rand -hex 16
来源：http://hd.hahajie.cn

[R68] 计算文件校验值
来源：http://nt.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sm.muxihuayi.cn

[R69] 生成随机密码
来源：http://id.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://ug.huanxung.cn

[R70] 时间戳与互转
来源：http://hq.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://zs.yuexingan06.cn

[R71] 日期格式化
来源：http://tn.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xe.shxzskj.cn

[R72] 等待端口就绪
来源：http://ya.huixinmuqiang.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ea.szxytkj.cn

[R73] 分割大日志
来源：http://vs.521024.cn

split -l 1000 big.log part_
来源：http://oj.yuntaijiaju.cn

[R74] 批量重命名
来源：http://ni.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xk.521024.cn

[R75] 导出环境变量
来源：http://ub.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://ck.nszjky.cn

[R76] 使用临时文件
来源：http://jt.shxzukj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://li.9csxet.cn

[R77] 读取用户输入
来源：http://uc.jctech888.com.cn

read -rp "请输入: " ans
来源：http://kz.bookmarksfly.cn

[R78] 交互式菜单
来源：http://yo.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pr.yuexingan06.cn

[R79] 解析命令行选项
来源：http://ry.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ux.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://tz.asd995.cn

time ./run.sh
来源：http://sp.newstarts.cn

================================================================================
来源：http://gl.yuntaijiaju.cn

S. C / C++ 专题
来源：http://gh.bookmarksfly.cn

================================================================================
来源：http://zd.gzmigu.cn

[S01] C：Hello World
来源：http://yf.gzmigu.cn

#include <stdio.h>
来源：http://gk.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dr.yuntaijiaju.cn

[S02] C：变量与格式化输出
来源：http://dd.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://by.huixiangedu.cn

[S03] C：读入整数
来源：http://al.huanxung.cn

int x; scanf("%d", &x);
来源：http://fg.hnjuh.cn

[S04] C：字符串复制
来源：http://wk.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uf.newstarts.cn

[S05] C：字符串长度
来源：http://ad.asd995.cn

strlen(s)
来源：http://xl.szsharing.cn

[S06] C：字符串比较
来源：http://ir.nicolike.cn

strcmp(a, b) == 0
来源：http://up.szsharing.cn

[S07] C：数组遍历求和
来源：http://oo.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ww.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://ne.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://el.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://ic.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ji.szsharing.cn

[S10] C：指针与解引用
来源：http://kj.nicolike.cn

int *p = &a;  *p = 5;
来源：http://jm.shxzukj.cn

[S11] C：逐行读文件
来源：http://fj.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://cv.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lt.jianghongdianzi.cn

fclose(f);
来源：http://wx.muxihuayi.cn

[S12] C：写文件
来源：http://wi.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://si.szxytkj.cn

[S13] C：宏定义
来源：http://me.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bt.521024.cn

[S14] C：枚举
来源：http://ob.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://zj.yuexingan06.cn

[S15] C：类型转换
来源：http://nu.hahajie.cn

(double) a / b
来源：http://jj.hnjuh.cn

[S16] C：位操作置位
来源：http://uv.yuntaijiaju.cn

x |= (1 << 3);
来源：http://vy.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://wq.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vr.szxytkj.cn

[S18] C：命令行参数
来源：http://dc.nicolike.cn

int main(int argc, char **argv)
来源：http://dq.bookmarksfly.cn

[S19] C：快速排序
来源：http://on.9csxet.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gx.shtwfgs.cn

[S20] C：二分查找
来源：http://cj.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hj.hahajie.cn

[S21] C：字符类别判断
来源：http://ma.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cl.szsharing.cn

[S22] C：字符串转数字
来源：http://na.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jp.bjjhwx.cn

[S23] C：随机数
来源：http://nt.bookmarksfly.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ku.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://qs.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lr.chemitech.net.cn

[S25] C：内存拷贝
来源：http://ab.hahajie.cn

memcpy(dst, src, n);
来源：http://wg.haigaiapp.cn

[S26] C：内存清零
来源：http://kb.hahajie.cn

memset(a, 0, sizeof a);
来源：http://ef.szxytkj.cn

[S27] C：定义常量
来源：http://ci.hahajie.cn

const double PI = 3.14159;
来源：http://zc.521024.cn

[S28] C：静态变量
来源：http://bn.shxzskj.cn

static int counter = 0;
来源：http://dl.gzmigu.cn

[S29] C：变参函数
来源：http://iw.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bg.shxzskj.cn

[S30] C：头文件保护
来源：http://pj.yuexingan06.cn

#ifndef X_H
来源：http://rv.asd995.cn

#define X_H
来源：http://co.521024.cn

#endif
来源：http://lx.huixiangedu.cn

[S31] C++：Hello World
来源：http://zq.szxytkj.cn

#include <iostream>
来源：http://aw.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://ag.nicolike.cn

[S32] C++：字符串
来源：http://bi.521024.cn

std::string s = "hi";  s += "!";
来源：http://im.asd995.cn

[S33] C++：vector 增删
来源：http://tj.wgjwhj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cr.9csxet.cn

[S34] C++：遍历 vector
来源：http://au.asd995.cn

for (auto &x : v) { std::cout << x; }
来源：http://pp.lnxyls.cn

[S35] C++：map
来源：http://pc.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pp.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://mk.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qf.panjiajie.cn

[S37] C++：set
来源：http://hz.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nt.hnjuh.cn

[S38] C++：排序
来源：http://vf.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://jm.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://ro.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iu.shxzskj.cn

[S40] C++：查找元素
来源：http://dz.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://za.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://ro.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jh.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://im.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://tc.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://ku.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://xz.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://df.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://sd.jctech888.com.cn

[S45] C++：lambda
来源：http://sh.hahajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jl.wgjwhj.cn

[S46] C++：函数模板
来源：http://qv.shxzukj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ll.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://jz.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cc.521024.cn

[S48] C++：逐行读文件
来源：http://wa.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://un.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://lw.wgjwhj.cn

[S49] C++：写文件
来源：http://je.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lc.lnxyls.cn

[S50] C++：格式化数字
来源：http://vx.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mw.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://yf.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://js.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://sy.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://xl.bookmarksfly.cn

[S53] C++：移动语义
来源：http://hm.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://dh.hahajie.cn

[S54] C++：异常处理
来源：http://fp.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jw.bookmarksfly.cn

[S55] C++：结构化绑定
来源：http://an.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bj.newstarts.cn

[S56] C++：optional
来源：http://md.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fg.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://ms.hnjuh.cn

constexpr int N = 10;
来源：http://on.haigaiapp.cn

[S58] C++：命名空间
来源：http://bc.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://en.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://hs.yuntaijiaju.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rx.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://ze.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wz.asd995.cn

================================================================================
来源：http://hq.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vx.shxzskj.cn

================================================================================
来源：http://tp.huanxung.cn

[T01] Kotlin：Hello World
来源：http://vs.hahajie.cn

println("Hello")
来源：http://ab.shtwfgs.cn

[T02] Kotlin：变量
来源：http://hg.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ia.colortex.cn

[T03] Kotlin：字符串模板
来源：http://nf.hnjuh.cn

"值: $b"
来源：http://bc.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://ce.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://jv.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://aj.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ji.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://sr.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rk.nicolike.cn

[T07] Kotlin：集合过滤
来源：http://ho.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://oy.shxzskj.cn

[T08] Kotlin：数据类
来源：http://pj.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://gb.lnxyls.cn

[T09] Kotlin：扩展函数
来源：http://ay.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://oy.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://bk.bjjhwx.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zg.bjjhwx.cn

[T11] Kotlin：协程
来源：http://xp.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bz.szsharing.cn

[T12] Kotlin：解构声明
来源：http://cu.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://xq.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://sx.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://fj.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://nz.gzmigu.cn

for (i in 1..10) println(i)
来源：http://ax.szsharing.cn

[T15] Kotlin：接口
来源：http://am.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://vg.9csxet.cn

[T16] Swift：Hello World
来源：http://ge.panjiajie.cn

print("Hello")
来源：http://tk.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://qj.wgjwhj.cn

var a = 1;  let b = 2
来源：http://qv.szxytkj.cn

[T18] Swift：字符串插值
来源：http://tc.newstarts.cn

"值: \(b)"
来源：http://vo.nicolike.cn

[T19] Swift：可选绑定
来源：http://il.shxzukj.cn

if let n = opt { print(n) }
来源：http://cl.huixiangedu.cn

[T20] Swift：数组操作
来源：http://es.yuntaijiaju.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yt.gzmigu.cn

[T21] Swift：遍历
来源：http://jk.gzmigu.cn

for x in a { print(x) }
来源：http://xm.hnjuh.cn

[T22] Swift：字典
来源：http://fw.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ef.haigaiapp.cn

[T23] Swift：函数
来源：http://zd.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://et.9csxet.cn

[T24] Swift：闭包
来源：http://wj.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wt.hahajie.cn

[T25] Swift：结构体
来源：http://nd.huanxung.cn

struct P { var x: Int }
来源：http://um.colortex.cn

[T26] Swift：类与重写
来源：http://kz.szsharing.cn

class A: Base { override func f() {} }
来源：http://zt.szxytkj.cn

[T27] Swift：错误处理
来源：http://sj.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://in.szxytkj.cn

[T28] Swift：枚举
来源：http://zh.shtwfgs.cn

enum Color { case red, green }
来源：http://ok.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://tw.muxihuayi.cn

guard let x = opt else { return }
来源：http://uv.chemitech.net.cn

[T30] Swift：协议
来源：http://fd.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://fx.bookmarksfly.cn

[T31] Lua：Hello World
来源：http://li.szsharing.cn

print("Hello")
来源：http://qx.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://pz.panjiajie.cn

local a = 1
来源：http://nz.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://ca.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yf.shxzukj.cn

[T34] Lua：遍历表
来源：http://fi.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://id.asd995.cn

[T35] Lua：字典表
来源：http://jw.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://ex.9csxet.cn

[T36] Lua：函数
来源：http://ht.szxytkj.cn

function add(a, b) return a + b end
来源：http://sp.szsharing.cn

[T37] Lua：字符串拼接
来源：http://by.chemitech.net.cn

"a" .. "b"
来源：http://du.huixinmuqiang.cn

[T38] Lua：条件
来源：http://wm.szxytkj.cn

if x > 0 then print("正") end
来源：http://rn.shtwfgs.cn

[T39] Lua：模式匹配
来源：http://vo.panjiajie.cn

string.find(s, "%d+")
来源：http://cw.yuntaijiaju.cn

[T40] Lua：元表
来源：http://nz.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://va.newstarts.cn


<!-- 参考信息 -->