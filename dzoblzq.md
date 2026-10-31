代发 wailian999

cmd >/dev/null 2>&1
来源：http://ms.nszjky.cn

[R42] 输入重定向
来源：http://tb.colortex.cn

wc -l < a.txt
来源：http://ii.haigaiapp.cn

[R43] 按名字查找文件
来源：http://xq.chemitech.net.cn

find . -name "*.log" -type f
来源：http://do.shtwfgs.cn

[R44] 按修改时间查找
来源：http://ip.wgjwhj.cn

find . -mtime -7 -type f
来源：http://tx.shtwfgs.cn

[R45] 批量删除
来源：http://zh.asd995.cn

find . -name "*.tmp" -delete
来源：http://tc.shxzskj.cn

[R46] 递归替换文件内容
来源：http://ma.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ve.nszjky.cn

[R47] sed 单行替换
来源：http://lk.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://im.szsharing.cn

[R48] awk 取指定列
来源：http://oj.huixiangedu.cn

awk '{print $1, $3}' a.txt
来源：http://yn.huixinmuqiang.cn

[R49] awk 带条件
来源：http://uy.huixiangedu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gl.jianghongdianzi.cn

[R50] awk 求和
来源：http://ir.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pu.hnjuh.cn

[R51] 排序去重取前几
来源：http://kc.yuexingan06.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qi.bjjhwx.cn

[R52] 统计行数
来源：http://ji.szxytkj.cn

wc -l a.txt
来源：http://pr.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://aq.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uf.huixiangedu.cn

[R54] 比较两个文件
来源：http://ey.jctech888.com.cn

diff a.txt b.txt
来源：http://le.shtwfgs.cn

[R55] 压缩与解压
来源：http://rs.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mv.wgjwhj.cn

[R56] 远程拷贝
来源：http://po.hahajie.cn

scp file user@host:/path/
来源：http://cc.yuexingan06.cn

[R57] 远程执行命令
来源：http://pq.panjiajie.cn

ssh user@host 'uptime'
来源：http://nf.chemitech.net.cn

[R58] 下载文件
来源：http://dc.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kg.yuexingan06.cn

[R59] 发 POST JSON
来源：http://kb.szxytkj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yw.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://lr.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tl.521024.cn

[R61] 磁盘占用
来源：http://pn.newstarts.cn

df -h;  du -sh *
来源：http://io.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://tt.521024.cn

du -ah . | sort -rh | head -10
来源：http://eg.gzmigu.cn

[R63] 内存与进程
来源：http://nk.panjiajie.cn

free -h;  ps aux | grep nginx
来源：http://ww.wgjwhj.cn

[R64] 结束进程
来源：http://kb.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://ui.wgjwhj.cn

[R65] 查看端口占用
来源：http://hh.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dl.newstarts.cn

[R66] 定时任务
来源：http://ov.newstarts.cn

crontab -e;  crontab -l
来源：http://uy.szsharing.cn

[R67] 生成随机十六进制串
来源：http://ik.muxihuayi.cn

openssl rand -hex 16
来源：http://fc.nszjky.cn

[R68] 计算文件校验值
来源：http://gl.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ox.shtwfgs.cn

[R69] 生成随机密码
来源：http://uy.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://zs.lnxyls.cn

[R70] 时间戳与互转
来源：http://oj.asd995.cn

date +%s;  date -d @1700000000
来源：http://qw.szsharing.cn

[R71] 日期格式化
来源：http://ju.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uz.lnxyls.cn

[R72] 等待端口就绪
来源：http://wa.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://me.colortex.cn

[R73] 分割大日志
来源：http://cn.panjiajie.cn

split -l 1000 big.log part_
来源：http://if.hahajie.cn

[R74] 批量重命名
来源：http://gm.nszjky.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ob.wgjwhj.cn

[R75] 导出环境变量
来源：http://fr.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://ly.bookmarksfly.cn

[R76] 使用临时文件
来源：http://qx.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ca.wgjwhj.cn

[R77] 读取用户输入
来源：http://ga.shxzskj.cn

read -rp "请输入: " ans
来源：http://ey.newstarts.cn

[R78] 交互式菜单
来源：http://uq.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uk.szxytkj.cn

[R79] 解析命令行选项
来源：http://bg.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kd.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://co.chemitech.net.cn

time ./run.sh
来源：http://wx.jctech888.com.cn

================================================================================
来源：http://hp.muxihuayi.cn

S. C / C++ 专题
来源：http://jn.huanxung.cn

================================================================================
来源：http://jf.haigaiapp.cn

[S01] C：Hello World
来源：http://zy.huixiangedu.cn

#include <stdio.h>
来源：http://za.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kp.9csxet.cn

[S02] C：变量与格式化输出
来源：http://ht.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://cw.haigaiapp.cn

[S03] C：读入整数
来源：http://sk.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://ns.newstarts.cn

[S04] C：字符串复制
来源：http://ft.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lz.huanxung.cn

[S05] C：字符串长度
来源：http://rl.nicolike.cn

strlen(s)
来源：http://ie.shxzukj.cn

[S06] C：字符串比较
来源：http://hz.szsharing.cn

strcmp(a, b) == 0
来源：http://nr.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://gz.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jc.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://do.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ql.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://dc.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eu.jctech888.com.cn

[S10] C：指针与解引用
来源：http://ug.colortex.cn

int *p = &a;  *p = 5;
来源：http://kp.wgjwhj.cn

[S11] C：逐行读文件
来源：http://re.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://fl.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qx.shtwfgs.cn

fclose(f);
来源：http://gt.521024.cn

[S12] C：写文件
来源：http://pa.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ht.szxytkj.cn

[S13] C：宏定义
来源：http://kc.nicolike.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fw.gzmigu.cn

[S14] C：枚举
来源：http://hl.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://bo.panjiajie.cn

[S15] C：类型转换
来源：http://vv.gzmigu.cn

(double) a / b
来源：http://pz.shxzskj.cn

[S16] C：位操作置位
来源：http://oi.lnxyls.cn

x |= (1 << 3);
来源：http://lk.colortex.cn

[S17] C：安全拼接字符串
来源：http://nb.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jl.9csxet.cn

[S18] C：命令行参数
来源：http://iw.asd995.cn

int main(int argc, char **argv)
来源：http://rh.gzmigu.cn

[S19] C：快速排序
来源：http://cd.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gs.chemitech.net.cn

[S20] C：二分查找
来源：http://rw.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://na.bookmarksfly.cn

[S21] C：字符类别判断
来源：http://zr.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cg.haigaiapp.cn

[S22] C：字符串转数字
来源：http://dy.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://df.huixinmuqiang.cn

[S23] C：随机数
来源：http://rp.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gf.nicolike.cn

[S24] C：获取本地时间
来源：http://uf.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lt.yuexingan06.cn

[S25] C：内存拷贝
来源：http://ib.muxihuayi.cn

memcpy(dst, src, n);
来源：http://yo.jianghongdianzi.cn

[S26] C：内存清零
来源：http://ne.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://tr.shxzukj.cn

[S27] C：定义常量
来源：http://ut.yuexingan06.cn

const double PI = 3.14159;
来源：http://mt.hnjuh.cn

[S28] C：静态变量
来源：http://zw.bookmarksfly.cn

static int counter = 0;
来源：http://yv.shtwfgs.cn

[S29] C：变参函数
来源：http://gx.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cn.colortex.cn

[S30] C：头文件保护
来源：http://gt.huanxung.cn

#ifndef X_H
来源：http://lz.bookmarksfly.cn

#define X_H
来源：http://vf.hahajie.cn

#endif
来源：http://ih.szsharing.cn

[S31] C++：Hello World
来源：http://xa.hahajie.cn

#include <iostream>
来源：http://io.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://xb.nszjky.cn

[S32] C++：字符串
来源：http://ng.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://ya.muxihuayi.cn

[S33] C++：vector 增删
来源：http://vt.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ec.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://mu.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://ud.panjiajie.cn

[S35] C++：map
来源：http://ry.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ut.jctech888.com.cn

[S36] C++：unordered_map
来源：http://hp.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ea.nicolike.cn

[S37] C++：set
来源：http://qa.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ow.newstarts.cn

[S38] C++：排序
来源：http://zh.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://qi.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://mz.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hp.shtwfgs.cn

[S40] C++：查找元素
来源：http://sv.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nb.nszjky.cn

[S41] C++：类与构造函数
来源：http://li.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kh.newstarts.cn

[S42] C++：继承与虚函数
来源：http://sj.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://sm.hnjuh.cn

[S43] C++：智能指针
来源：http://ob.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://ex.bookmarksfly.cn

[S44] C++：引用传参
来源：http://zm.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://dp.hahajie.cn

[S45] C++：lambda
来源：http://yx.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sp.panjiajie.cn

[S46] C++：函数模板
来源：http://sk.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ed.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://ai.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ov.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://qh.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xh.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://kb.muxihuayi.cn

[S49] C++：写文件
来源：http://pp.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://na.wgjwhj.cn

[S50] C++：格式化数字
来源：http://ba.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fh.colortex.cn

[S51] C++：显式类型转换
来源：http://hg.gzmigu.cn

static_cast<double>(a) / b
来源：http://fl.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://wv.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://ah.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://mt.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://yh.nicolike.cn

[S54] C++：异常处理
来源：http://ed.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bo.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://ww.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bp.bjjhwx.cn

[S56] C++：optional
来源：http://kb.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://op.hnjuh.cn

[S57] C++：编译期常量
来源：http://oi.muxihuayi.cn

constexpr int N = 10;
来源：http://al.gzmigu.cn

[S58] C++：命名空间
来源：http://fk.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://jl.huanxung.cn

[S59] C++：静态断言
来源：http://ur.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kc.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://jf.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dt.muxihuayi.cn

================================================================================
来源：http://wc.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ya.szxytkj.cn

================================================================================
来源：http://qz.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://tr.bjjhwx.cn

println("Hello")
来源：http://aa.muxihuayi.cn

[T02] Kotlin：变量
来源：http://mw.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vi.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://ht.jianghongdianzi.cn

"值: $b"
来源：http://ju.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://cg.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://ca.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://xf.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uo.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://vb.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jw.colortex.cn

[T07] Kotlin：集合过滤
来源：http://wb.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ch.nszjky.cn

[T08] Kotlin：数据类
来源：http://tg.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://uq.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://jv.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://ci.huanxung.cn

[T10] Kotlin：默认参数
来源：http://ay.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kf.szsharing.cn

[T11] Kotlin：协程
来源：http://rv.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://go.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://ej.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://zh.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://ma.lnxyls.cn

val m = mapOf("a" to 1)
来源：http://mp.521024.cn

[T14] Kotlin：循环
来源：http://fk.colortex.cn

for (i in 1..10) println(i)
来源：http://ky.huixiangedu.cn

[T15] Kotlin：接口
来源：http://sr.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://xc.hnjuh.cn

[T16] Swift：Hello World
来源：http://nr.shxzukj.cn

print("Hello")
来源：http://gw.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://pi.shxzskj.cn

var a = 1;  let b = 2
来源：http://ep.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://pj.shxzskj.cn

"值: \(b)"
来源：http://of.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://bj.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://tp.szxytkj.cn

[T20] Swift：数组操作
来源：http://ga.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://iy.shtwfgs.cn

[T21] Swift：遍历
来源：http://sx.newstarts.cn

for x in a { print(x) }
来源：http://te.9csxet.cn

[T22] Swift：字典
来源：http://bq.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sw.521024.cn

[T23] Swift：函数
来源：http://yk.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cb.shtwfgs.cn

[T24] Swift：闭包
来源：http://fl.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mn.wgjwhj.cn

[T25] Swift：结构体
来源：http://tu.jianghongdianzi.cn

struct P { var x: Int }
来源：http://wn.hahajie.cn

[T26] Swift：类与重写
来源：http://hj.shxzukj.cn

class A: Base { override func f() {} }
来源：http://yu.newstarts.cn

[T27] Swift：错误处理
来源：http://mx.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://pi.newstarts.cn

[T28] Swift：枚举
来源：http://hr.haigaiapp.cn

enum Color { case red, green }
来源：http://ob.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://wg.yuexingan06.cn

guard let x = opt else { return }
来源：http://tv.521024.cn

[T30] Swift：协议
来源：http://km.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://gh.szxytkj.cn

[T31] Lua：Hello World
来源：http://bd.bookmarksfly.cn

print("Hello")
来源：http://dk.shtwfgs.cn

[T32] Lua：局部变量
来源：http://hh.szxytkj.cn

local a = 1
来源：http://ds.newstarts.cn

[T33] Lua：表（数组）
来源：http://jn.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://iu.nicolike.cn

[T34] Lua：遍历表
来源：http://le.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://oy.nicolike.cn

[T35] Lua：字典表
来源：http://sm.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://bl.szsharing.cn

[T36] Lua：函数
来源：http://mb.shtwfgs.cn

function add(a, b) return a + b end
来源：http://ym.9csxet.cn

[T37] Lua：字符串拼接
来源：http://bb.gzmigu.cn

"a" .. "b"
来源：http://kj.panjiajie.cn

[T38] Lua：条件
来源：http://sx.shxzskj.cn

if x > 0 then print("正") end
来源：http://lh.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://xe.chemitech.net.cn

string.find(s, "%d+")
来源：http://ok.haigaiapp.cn

[T40] Lua：元表
来源：http://pu.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://pg.szsharing.cn

[T41] Perl：Hello World
来源：http://qw.haigaiapp.cn

print "Hello\n";
来源：http://gr.lnxyls.cn

[T42] Perl：变量类型
来源：http://dh.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vl.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://qn.yuntaijiaju.cn

"值: $a"
来源：http://dj.huixinmuqiang.cn

[T44] Perl：条件
来源：http://cj.asd995.cn

if ($a > 0) { print "正"; }
来源：http://zq.bookmarksfly.cn


<!-- 参考信息 -->