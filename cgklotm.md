代发 wailian999

files=$(ls -1)
来源：http://ki.nicolike.cn

[R38] 管道串联
来源：http://ml.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://hx.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://kc.colortex.cn

cmd > out.log 2>&1
来源：http://cn.yuntaijiaju.cn

[R40] 追加写日志
来源：http://ko.szxytkj.cn

echo "log" >> out.log
来源：http://ex.colortex.cn

[R41] 丢弃输出
来源：http://dh.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://eg.jianghongdianzi.cn

[R42] 输入重定向
来源：http://vh.521024.cn

wc -l < a.txt
来源：http://zg.nszjky.cn

[R43] 按名字查找文件
来源：http://yr.huixiangedu.cn

find . -name "*.log" -type f
来源：http://xw.hnjuh.cn

[R44] 按修改时间查找
来源：http://wp.panjiajie.cn

find . -mtime -7 -type f
来源：http://ra.muxihuayi.cn

[R45] 批量删除
来源：http://ux.jianghongdianzi.cn

find . -name "*.tmp" -delete
来源：http://vc.521024.cn

[R46] 递归替换文件内容
来源：http://eu.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hi.nszjky.cn

[R47] sed 单行替换
来源：http://es.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mm.nicolike.cn

[R48] awk 取指定列
来源：http://co.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://lp.huixiangedu.cn

[R49] awk 带条件
来源：http://aq.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tw.chemitech.net.cn

[R50] awk 求和
来源：http://zx.bookmarksfly.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yz.jctech888.com.cn

[R51] 排序去重取前几
来源：http://to.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jv.jianghongdianzi.cn

[R52] 统计行数
来源：http://rv.shxzukj.cn

wc -l a.txt
来源：http://ko.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://io.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uq.szsharing.cn

[R54] 比较两个文件
来源：http://jz.haigaiapp.cn

diff a.txt b.txt
来源：http://kd.nszjky.cn

[R55] 压缩与解压
来源：http://mc.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ub.newstarts.cn

[R56] 远程拷贝
来源：http://da.shtwfgs.cn

scp file user@host:/path/
来源：http://tj.hnjuh.cn

[R57] 远程执行命令
来源：http://vm.bjjhwx.cn

ssh user@host 'uptime'
来源：http://tr.jianghongdianzi.cn

[R58] 下载文件
来源：http://bk.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ia.nszjky.cn

[R59] 发 POST JSON
来源：http://bu.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jn.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://zr.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fb.colortex.cn

[R61] 磁盘占用
来源：http://rp.bjjhwx.cn

df -h;  du -sh *
来源：http://aa.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://xm.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://zg.yuntaijiaju.cn

[R63] 内存与进程
来源：http://uz.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://qs.panjiajie.cn

[R64] 结束进程
来源：http://ci.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://yi.jctech888.com.cn

[R65] 查看端口占用
来源：http://le.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ch.nszjky.cn

[R66] 定时任务
来源：http://ty.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://if.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://qg.shxzukj.cn

openssl rand -hex 16
来源：http://zr.muxihuayi.cn

[R68] 计算文件校验值
来源：http://nv.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xn.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://eo.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://tv.huanxung.cn

[R70] 时间戳与互转
来源：http://mn.521024.cn

date +%s;  date -d @1700000000
来源：http://ae.huixiangedu.cn

[R71] 日期格式化
来源：http://el.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://oe.colortex.cn

[R72] 等待端口就绪
来源：http://hf.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ud.521024.cn

[R73] 分割大日志
来源：http://vv.shxzskj.cn

split -l 1000 big.log part_
来源：http://xy.szsharing.cn

[R74] 批量重命名
来源：http://aw.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kp.chemitech.net.cn

[R75] 导出环境变量
来源：http://ok.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://uy.gzmigu.cn

[R76] 使用临时文件
来源：http://zl.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gm.bookmarksfly.cn

[R77] 读取用户输入
来源：http://wy.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://es.gzmigu.cn

[R78] 交互式菜单
来源：http://ei.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sq.haigaiapp.cn

[R79] 解析命令行选项
来源：http://vj.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://en.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://kb.huixiangedu.cn

time ./run.sh
来源：http://fk.huanxung.cn

================================================================================
来源：http://xa.jianghongdianzi.cn

S. C / C++ 专题
来源：http://ja.huanxung.cn

================================================================================
来源：http://mg.panjiajie.cn

[S01] C：Hello World
来源：http://iy.shxzukj.cn

#include <stdio.h>
来源：http://ao.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dz.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://oz.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://oy.chemitech.net.cn

[S03] C：读入整数
来源：http://mc.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://yd.panjiajie.cn

[S04] C：字符串复制
来源：http://lo.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hc.colortex.cn

[S05] C：字符串长度
来源：http://ls.yuexingan06.cn

strlen(s)
来源：http://rk.colortex.cn

[S06] C：字符串比较
来源：http://kl.huanxung.cn

strcmp(a, b) == 0
来源：http://wb.hnjuh.cn

[S07] C：数组遍历求和
来源：http://kd.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://js.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://ov.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zj.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://fp.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ok.chemitech.net.cn

[S10] C：指针与解引用
来源：http://wd.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://dw.haigaiapp.cn

[S11] C：逐行读文件
来源：http://yt.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://mr.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kd.gzmigu.cn

fclose(f);
来源：http://ob.yuntaijiaju.cn

[S12] C：写文件
来源：http://zo.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sb.9csxet.cn

[S13] C：宏定义
来源：http://ah.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bc.asd995.cn

[S14] C：枚举
来源：http://pw.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://ux.colortex.cn

[S15] C：类型转换
来源：http://as.huanxung.cn

(double) a / b
来源：http://ym.hnjuh.cn

[S16] C：位操作置位
来源：http://rc.jctech888.com.cn

x |= (1 << 3);
来源：http://dm.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://oa.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gw.wgjwhj.cn

[S18] C：命令行参数
来源：http://kb.hahajie.cn

int main(int argc, char **argv)
来源：http://xu.newstarts.cn

[S19] C：快速排序
来源：http://uw.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qh.wgjwhj.cn

[S20] C：二分查找
来源：http://hy.521024.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sx.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://ra.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cz.9csxet.cn

[S22] C：字符串转数字
来源：http://pr.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zq.bjjhwx.cn

[S23] C：随机数
来源：http://nt.huixinmuqiang.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://in.huanxung.cn

[S24] C：获取本地时间
来源：http://pl.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tu.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://ku.wgjwhj.cn

memcpy(dst, src, n);
来源：http://pm.jctech888.com.cn

[S26] C：内存清零
来源：http://jx.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://zu.newstarts.cn

[S27] C：定义常量
来源：http://aa.chemitech.net.cn

const double PI = 3.14159;
来源：http://ob.szxytkj.cn

[S28] C：静态变量
来源：http://bn.szsharing.cn

static int counter = 0;
来源：http://xw.nszjky.cn

[S29] C：变参函数
来源：http://zj.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rk.huanxung.cn

[S30] C：头文件保护
来源：http://gf.521024.cn

#ifndef X_H
来源：http://fu.jianghongdianzi.cn

#define X_H
来源：http://wc.shtwfgs.cn

#endif
来源：http://hg.jctech888.com.cn

[S31] C++：Hello World
来源：http://rn.lnxyls.cn

#include <iostream>
来源：http://oc.yuexingan06.cn

int main() { std::cout << "Hello\n"; }
来源：http://fm.hnjuh.cn

[S32] C++：字符串
来源：http://es.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://dr.panjiajie.cn

[S33] C++：vector 增删
来源：http://ef.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://de.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://ta.yuntaijiaju.cn

for (auto &x : v) { std::cout << x; }
来源：http://nr.yuexingan06.cn

[S35] C++：map
来源：http://ll.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lv.nszjky.cn

[S36] C++：unordered_map
来源：http://lf.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ku.hahajie.cn

[S37] C++：set
来源：http://fv.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gt.huixinmuqiang.cn

[S38] C++：排序
来源：http://uj.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://de.gzmigu.cn

[S39] C++：自定义比较器排序
来源：http://el.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ao.jctech888.com.cn

[S40] C++：查找元素
来源：http://ou.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://is.newstarts.cn

[S41] C++：类与构造函数
来源：http://ix.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dl.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://pu.521024.cn

class B : public Base { public: void f() override {} };
来源：http://cv.lnxyls.cn

[S43] C++：智能指针
来源：http://mx.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://cc.hahajie.cn

[S44] C++：引用传参
来源：http://zz.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://xg.lnxyls.cn

[S45] C++：lambda
来源：http://ew.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rh.huanxung.cn

[S46] C++：函数模板
来源：http://qi.asd995.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ds.521024.cn

[S47] C++：结构化绑定遍历
来源：http://jt.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tf.nszjky.cn

[S48] C++：逐行读文件
来源：http://yi.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wk.asd995.cn

while (std::getline(in, line)) { }
来源：http://ej.asd995.cn

[S49] C++：写文件
来源：http://ds.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zn.jctech888.com.cn

[S50] C++：格式化数字
来源：http://ii.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jt.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://gh.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://by.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://we.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://gw.hnjuh.cn

[S53] C++：移动语义
来源：http://bi.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://mf.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://jq.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ok.asd995.cn

[S55] C++：结构化绑定
来源：http://jv.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ya.gzmigu.cn

[S56] C++：optional
来源：http://vq.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://it.szxytkj.cn

[S57] C++：编译期常量
来源：http://kg.szsharing.cn

constexpr int N = 10;
来源：http://ac.shxzukj.cn

[S58] C++：命名空间
来源：http://dy.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://ms.nicolike.cn

[S59] C++：静态断言
来源：http://fz.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dx.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://fc.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yg.lnxyls.cn

================================================================================
来源：http://be.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://di.yuntaijiaju.cn

================================================================================
来源：http://bw.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://fz.haigaiapp.cn

println("Hello")
来源：http://sj.asd995.cn

[T02] Kotlin：变量
来源：http://ff.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kh.colortex.cn

[T03] Kotlin：字符串模板
来源：http://dl.bookmarksfly.cn

"值: $b"
来源：http://gz.gzmigu.cn

[T04] Kotlin：空安全
来源：http://ot.nicolike.cn

val n: String? = null;  n?.length
来源：http://cu.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://kz.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rb.9csxet.cn

[T06] Kotlin：集合映射
来源：http://dm.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yq.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://el.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ot.shxzskj.cn

[T08] Kotlin：数据类
来源：http://pj.asd995.cn

data class User(val name: String, val age: Int)
来源：http://sh.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://py.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://ry.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://jl.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://aw.hnjuh.cn

[T11] Kotlin：协程
来源：http://ak.bookmarksfly.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qr.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://hf.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://av.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://xv.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://tx.hnjuh.cn

[T14] Kotlin：循环
来源：http://sy.nicolike.cn

for (i in 1..10) println(i)
来源：http://uv.wgjwhj.cn

[T15] Kotlin：接口
来源：http://zt.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://hc.shxzukj.cn

[T16] Swift：Hello World
来源：http://ri.shxzskj.cn

print("Hello")
来源：http://oe.hnjuh.cn

[T17] Swift：变量与常量
来源：http://cq.shxzukj.cn

var a = 1;  let b = 2
来源：http://wr.huanxung.cn

[T18] Swift：字符串插值
来源：http://xh.521024.cn

"值: \(b)"
来源：http://bt.szsharing.cn

[T19] Swift：可选绑定
来源：http://fr.nicolike.cn

if let n = opt { print(n) }
来源：http://qc.szxytkj.cn

[T20] Swift：数组操作
来源：http://hm.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://km.hahajie.cn

[T21] Swift：遍历
来源：http://ah.gzmigu.cn

for x in a { print(x) }
来源：http://wy.shxzskj.cn

[T22] Swift：字典
来源：http://mf.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pp.asd995.cn

[T23] Swift：函数
来源：http://el.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fz.szsharing.cn

[T24] Swift：闭包
来源：http://lf.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jg.panjiajie.cn

[T25] Swift：结构体
来源：http://pw.9csxet.cn

struct P { var x: Int }
来源：http://am.lnxyls.cn

[T26] Swift：类与重写
来源：http://qy.521024.cn

class A: Base { override func f() {} }
来源：http://fo.muxihuayi.cn

[T27] Swift：错误处理
来源：http://qj.muxihuayi.cn

do { try f() } catch { print(error) }
来源：http://vw.chemitech.net.cn

[T28] Swift：枚举
来源：http://xx.shxzukj.cn

enum Color { case red, green }
来源：http://xs.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://zq.huanxung.cn

guard let x = opt else { return }
来源：http://mr.colortex.cn

[T30] Swift：协议
来源：http://lv.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://sf.shxzskj.cn

[T31] Lua：Hello World
来源：http://eq.asd995.cn

print("Hello")
来源：http://qv.panjiajie.cn

[T32] Lua：局部变量
来源：http://de.hnjuh.cn

local a = 1
来源：http://wj.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://mg.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cs.huanxung.cn

[T34] Lua：遍历表
来源：http://gg.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ik.newstarts.cn

[T35] Lua：字典表
来源：http://le.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://px.huanxung.cn

[T36] Lua：函数
来源：http://iz.shxzukj.cn

function add(a, b) return a + b end
来源：http://lj.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://nc.colortex.cn

"a" .. "b"
来源：http://vt.nszjky.cn

[T38] Lua：条件
来源：http://sh.shtwfgs.cn

if x > 0 then print("正") end
来源：http://dg.lnxyls.cn

[T39] Lua：模式匹配
来源：http://ab.521024.cn

string.find(s, "%d+")
来源：http://gd.bjjhwx.cn

[T40] Lua：元表
来源：http://jh.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://hh.asd995.cn


<!-- 参考信息 -->