代发 wailian999

files=$(ls -1)
来源：http://kd.newstarts.cn

[R38] 管道串联
来源：http://er.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://am.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://dp.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://vj.huixinmuqiang.cn

[R40] 追加写日志
来源：http://fj.panjiajie.cn

echo "log" >> out.log
来源：http://nf.muxihuayi.cn

[R41] 丢弃输出
来源：http://zz.asd995.cn

cmd >/dev/null 2>&1
来源：http://wx.huanxung.cn

[R42] 输入重定向
来源：http://sw.colortex.cn

wc -l < a.txt
来源：http://qf.gzmigu.cn

[R43] 按名字查找文件
来源：http://uf.huixiangedu.cn

find . -name "*.log" -type f
来源：http://io.9csxet.cn

[R44] 按修改时间查找
来源：http://ez.yuexingan06.cn

find . -mtime -7 -type f
来源：http://ed.szsharing.cn

[R45] 批量删除
来源：http://ia.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://cg.shxzukj.cn

[R46] 递归替换文件内容
来源：http://yj.chemitech.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mt.shxzukj.cn

[R47] sed 单行替换
来源：http://oq.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bh.huixiangedu.cn

[R48] awk 取指定列
来源：http://ij.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://ij.jianghongdianzi.cn

[R49] awk 带条件
来源：http://cg.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mh.haigaiapp.cn

[R50] awk 求和
来源：http://zu.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ud.huixiangedu.cn

[R51] 排序去重取前几
来源：http://di.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fn.shxzskj.cn

[R52] 统计行数
来源：http://ge.chemitech.net.cn

wc -l a.txt
来源：http://bn.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://mn.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kp.hahajie.cn

[R54] 比较两个文件
来源：http://ge.asd995.cn

diff a.txt b.txt
来源：http://wu.hnjuh.cn

[R55] 压缩与解压
来源：http://bj.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oo.chemitech.net.cn

[R56] 远程拷贝
来源：http://ir.shtwfgs.cn

scp file user@host:/path/
来源：http://wm.521024.cn

[R57] 远程执行命令
来源：http://mt.yuexingan06.cn

ssh user@host 'uptime'
来源：http://qv.hnjuh.cn

[R58] 下载文件
来源：http://fm.jianghongdianzi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oy.huixiangedu.cn

[R59] 发 POST JSON
来源：http://fw.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://du.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://tc.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vj.szsharing.cn

[R61] 磁盘占用
来源：http://kk.gzmigu.cn

df -h;  du -sh *
来源：http://ov.asd995.cn

[R62] 找最占空间的文件
来源：http://jc.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://wj.szsharing.cn

[R63] 内存与进程
来源：http://cq.yuntaijiaju.cn

free -h;  ps aux | grep nginx
来源：http://ut.jianghongdianzi.cn

[R64] 结束进程
来源：http://op.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://vj.jctech888.com.cn

[R65] 查看端口占用
来源：http://kx.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ca.shtwfgs.cn

[R66] 定时任务
来源：http://lg.huixiangedu.cn

crontab -e;  crontab -l
来源：http://hy.nszjky.cn

[R67] 生成随机十六进制串
来源：http://ke.huixiangedu.cn

openssl rand -hex 16
来源：http://qy.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://cn.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kd.chemitech.net.cn

[R69] 生成随机密码
来源：http://lc.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://tv.nszjky.cn

[R70] 时间戳与互转
来源：http://xy.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://kb.jianghongdianzi.cn

[R71] 日期格式化
来源：http://ef.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://at.521024.cn

[R72] 等待端口就绪
来源：http://wt.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ia.bjjhwx.cn

[R73] 分割大日志
来源：http://jf.hahajie.cn

split -l 1000 big.log part_
来源：http://ns.huixiangedu.cn

[R74] 批量重命名
来源：http://lf.nszjky.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cp.newstarts.cn

[R75] 导出环境变量
来源：http://cn.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://tp.yuexingan06.cn

[R76] 使用临时文件
来源：http://wq.szxytkj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oy.hnjuh.cn

[R77] 读取用户输入
来源：http://ii.colortex.cn

read -rp "请输入: " ans
来源：http://xm.jctech888.com.cn

[R78] 交互式菜单
来源：http://nc.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nl.asd995.cn

[R79] 解析命令行选项
来源：http://gs.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mo.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://ld.nszjky.cn

time ./run.sh
来源：http://pz.yuexingan06.cn

================================================================================
来源：http://qn.muxihuayi.cn

S. C / C++ 专题
来源：http://cp.9csxet.cn

================================================================================
来源：http://lf.asd995.cn

[S01] C：Hello World
来源：http://zk.bookmarksfly.cn

#include <stdio.h>
来源：http://de.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xp.nszjky.cn

[S02] C：变量与格式化输出
来源：http://iw.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://mu.lnxyls.cn

[S03] C：读入整数
来源：http://hb.lnxyls.cn

int x; scanf("%d", &x);
来源：http://ji.szsharing.cn

[S04] C：字符串复制
来源：http://pi.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ow.szxytkj.cn

[S05] C：字符串长度
来源：http://nv.asd995.cn

strlen(s)
来源：http://ew.nicolike.cn

[S06] C：字符串比较
来源：http://ye.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://xc.szxytkj.cn

[S07] C：数组遍历求和
来源：http://on.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gl.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://lz.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xa.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://bs.bookmarksfly.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pb.shtwfgs.cn

[S10] C：指针与解引用
来源：http://nq.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://fc.bjjhwx.cn

[S11] C：逐行读文件
来源：http://lz.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://gr.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zp.lnxyls.cn

fclose(f);
来源：http://zc.9csxet.cn

[S12] C：写文件
来源：http://oc.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://az.muxihuayi.cn

[S13] C：宏定义
来源：http://wq.newstarts.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mu.lnxyls.cn

[S14] C：枚举
来源：http://pp.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://ch.szsharing.cn

[S15] C：类型转换
来源：http://zl.szsharing.cn

(double) a / b
来源：http://gh.shxzskj.cn

[S16] C：位操作置位
来源：http://ld.chemitech.net.cn

x |= (1 << 3);
来源：http://oo.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://ov.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nd.newstarts.cn

[S18] C：命令行参数
来源：http://uy.huanxung.cn

int main(int argc, char **argv)
来源：http://zi.jianghongdianzi.cn

[S19] C：快速排序
来源：http://lo.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rz.hnjuh.cn

[S20] C：二分查找
来源：http://ve.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yf.hahajie.cn

[S21] C：字符类别判断
来源：http://ik.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bs.huanxung.cn

[S22] C：字符串转数字
来源：http://vx.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qe.9csxet.cn

[S23] C：随机数
来源：http://yi.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yg.colortex.cn

[S24] C：获取本地时间
来源：http://pq.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ko.shtwfgs.cn

[S25] C：内存拷贝
来源：http://cp.jctech888.com.cn

memcpy(dst, src, n);
来源：http://bu.shxzskj.cn

[S26] C：内存清零
来源：http://kl.szsharing.cn

memset(a, 0, sizeof a);
来源：http://la.yuntaijiaju.cn

[S27] C：定义常量
来源：http://gy.colortex.cn

const double PI = 3.14159;
来源：http://jv.huixinmuqiang.cn

[S28] C：静态变量
来源：http://gt.nszjky.cn

static int counter = 0;
来源：http://aa.newstarts.cn

[S29] C：变参函数
来源：http://pc.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bb.521024.cn

[S30] C：头文件保护
来源：http://oc.shxzskj.cn

#ifndef X_H
来源：http://ey.nicolike.cn

#define X_H
来源：http://rk.wgjwhj.cn

#endif
来源：http://tn.bookmarksfly.cn

[S31] C++：Hello World
来源：http://ve.hnjuh.cn

#include <iostream>
来源：http://mi.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://js.chemitech.net.cn

[S32] C++：字符串
来源：http://ni.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://ag.lnxyls.cn

[S33] C++：vector 增删
来源：http://lx.haigaiapp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qr.shxzukj.cn

[S34] C++：遍历 vector
来源：http://vs.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://nl.shxzskj.cn

[S35] C++：map
来源：http://fx.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dv.newstarts.cn

[S36] C++：unordered_map
来源：http://dp.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rs.newstarts.cn

[S37] C++：set
来源：http://vq.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xn.9csxet.cn

[S38] C++：排序
来源：http://pm.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://fo.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://mo.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rl.muxihuayi.cn

[S40] C++：查找元素
来源：http://jt.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sz.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://iz.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wd.9csxet.cn

[S42] C++：继承与虚函数
来源：http://pc.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://ol.szsharing.cn

[S43] C++：智能指针
来源：http://fz.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://jy.lnxyls.cn

[S44] C++：引用传参
来源：http://el.9csxet.cn

void inc(int &x) { ++x; }
来源：http://iu.chemitech.net.cn

[S45] C++：lambda
来源：http://qo.hahajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yq.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://bp.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vp.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://wm.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cq.gzmigu.cn

[S48] C++：逐行读文件
来源：http://lp.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yv.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://dc.jianghongdianzi.cn

[S49] C++：写文件
来源：http://yp.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vk.lnxyls.cn

[S50] C++：格式化数字
来源：http://ag.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bi.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://nz.lnxyls.cn

static_cast<double>(a) / b
来源：http://ym.newstarts.cn

[S52] C++：const 与 noexcept
来源：http://zw.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://ot.9csxet.cn

[S53] C++：移动语义
来源：http://up.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://jv.hnjuh.cn

[S54] C++：异常处理
来源：http://ms.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kt.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://ft.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://co.colortex.cn

[S56] C++：optional
来源：http://pw.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gb.huixiangedu.cn

[S57] C++：编译期常量
来源：http://ya.lnxyls.cn

constexpr int N = 10;
来源：http://nw.shxzukj.cn

[S58] C++：命名空间
来源：http://ad.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://hx.521024.cn

[S59] C++：静态断言
来源：http://jw.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fp.colortex.cn

[S60] C++：遍历并删除元素
来源：http://nf.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jt.panjiajie.cn

================================================================================
来源：http://vh.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jh.521024.cn

================================================================================
来源：http://hu.hahajie.cn

[T01] Kotlin：Hello World
来源：http://zk.9csxet.cn

println("Hello")
来源：http://bn.shtwfgs.cn

[T02] Kotlin：变量
来源：http://kk.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qc.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://ld.jctech888.com.cn

"值: $b"
来源：http://pi.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://nl.asd995.cn

val n: String? = null;  n?.length
来源：http://zx.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://uo.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oz.shtwfgs.cn

[T06] Kotlin：集合映射
来源：http://hg.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ot.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://am.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dm.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://dt.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://pn.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://er.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://mu.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://ss.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hq.szsharing.cn

[T11] Kotlin：协程
来源：http://nd.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dr.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://uk.chemitech.net.cn

val (a, b) = Pair(1, 2)
来源：http://ej.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://ok.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://le.panjiajie.cn

[T14] Kotlin：循环
来源：http://zy.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://ik.panjiajie.cn

[T15] Kotlin：接口
来源：http://jj.colortex.cn

interface Shape { fun area(): Double }
来源：http://ap.nicolike.cn

[T16] Swift：Hello World
来源：http://gi.nicolike.cn

print("Hello")
来源：http://ys.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://tk.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://yj.lnxyls.cn

[T18] Swift：字符串插值
来源：http://of.jctech888.com.cn

"值: \(b)"
来源：http://ci.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://cm.muxihuayi.cn

if let n = opt { print(n) }
来源：http://gb.shxzukj.cn

[T20] Swift：数组操作
来源：http://se.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kp.lnxyls.cn

[T21] Swift：遍历
来源：http://is.chemitech.net.cn

for x in a { print(x) }
来源：http://iy.9csxet.cn

[T22] Swift：字典
来源：http://kh.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qt.hahajie.cn

[T23] Swift：函数
来源：http://dl.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://av.shxzukj.cn

[T24] Swift：闭包
来源：http://wv.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bs.nicolike.cn

[T25] Swift：结构体
来源：http://ti.bookmarksfly.cn

struct P { var x: Int }
来源：http://hg.chemitech.net.cn

[T26] Swift：类与重写
来源：http://ce.nicolike.cn

class A: Base { override func f() {} }
来源：http://fx.huanxung.cn

[T27] Swift：错误处理
来源：http://or.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://yt.newstarts.cn

[T28] Swift：枚举
来源：http://sq.yuexingan06.cn

enum Color { case red, green }
来源：http://gh.hahajie.cn

[T29] Swift：guard 提前返回
来源：http://gu.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://kc.gzmigu.cn

[T30] Swift：协议
来源：http://fo.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://wc.haigaiapp.cn

[T31] Lua：Hello World
来源：http://yo.lnxyls.cn

print("Hello")
来源：http://li.muxihuayi.cn

[T32] Lua：局部变量
来源：http://fm.panjiajie.cn

local a = 1
来源：http://zs.huanxung.cn

[T33] Lua：表（数组）
来源：http://zg.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gt.lnxyls.cn

[T34] Lua：遍历表
来源：http://xi.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wn.haigaiapp.cn

[T35] Lua：字典表
来源：http://zl.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://jv.jianghongdianzi.cn

[T36] Lua：函数
来源：http://jc.shxzukj.cn

function add(a, b) return a + b end
来源：http://mr.nszjky.cn

[T37] Lua：字符串拼接
来源：http://nr.muxihuayi.cn

"a" .. "b"
来源：http://gt.hahajie.cn

[T38] Lua：条件
来源：http://os.asd995.cn

if x > 0 then print("正") end
来源：http://vr.shxzskj.cn

[T39] Lua：模式匹配
来源：http://xd.jctech888.com.cn

string.find(s, "%d+")
来源：http://la.panjiajie.cn

[T40] Lua：元表
来源：http://rh.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://tq.haigaiapp.cn


<!-- 参考信息 -->