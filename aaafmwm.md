代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://ws.szsharing.cn

[R36] 并发执行多个任务
来源：http://bl.nszjky.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lj.szsharing.cn

[R37] 把输出赋给变量
来源：http://iw.asd995.cn

files=$(ls -1)
来源：http://us.shtwfgs.cn

[R38] 管道串联
来源：http://cy.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://kh.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://gf.9csxet.cn

cmd > out.log 2>&1
来源：http://vw.muxihuayi.cn

[R40] 追加写日志
来源：http://qn.haigaiapp.cn

echo "log" >> out.log
来源：http://jg.shxzskj.cn

[R41] 丢弃输出
来源：http://co.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://ij.jctech888.com.cn

[R42] 输入重定向
来源：http://pi.nicolike.cn

wc -l < a.txt
来源：http://ng.gzmigu.cn

[R43] 按名字查找文件
来源：http://nq.newstarts.cn

find . -name "*.log" -type f
来源：http://ea.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://if.lnxyls.cn

find . -mtime -7 -type f
来源：http://jq.gzmigu.cn

[R45] 批量删除
来源：http://fz.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://ug.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://or.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bl.asd995.cn

[R47] sed 单行替换
来源：http://gw.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nv.gzmigu.cn

[R48] awk 取指定列
来源：http://kv.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://mv.newstarts.cn

[R49] awk 带条件
来源：http://pn.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://la.huanxung.cn

[R50] awk 求和
来源：http://cr.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://iw.hahajie.cn

[R51] 排序去重取前几
来源：http://tf.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qr.bookmarksfly.cn

[R52] 统计行数
来源：http://tn.gzmigu.cn

wc -l a.txt
来源：http://fl.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://mg.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jp.muxihuayi.cn

[R54] 比较两个文件
来源：http://nz.asd995.cn

diff a.txt b.txt
来源：http://rw.shxzskj.cn

[R55] 压缩与解压
来源：http://op.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ff.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://yg.haigaiapp.cn

scp file user@host:/path/
来源：http://bg.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://md.nicolike.cn

ssh user@host 'uptime'
来源：http://sx.szxytkj.cn

[R58] 下载文件
来源：http://up.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kv.9csxet.cn

[R59] 发 POST JSON
来源：http://zz.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xv.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://vb.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kh.nszjky.cn

[R61] 磁盘占用
来源：http://il.521024.cn

df -h;  du -sh *
来源：http://da.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://ry.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://zk.shtwfgs.cn

[R63] 内存与进程
来源：http://pj.jctech888.com.cn

free -h;  ps aux | grep nginx
来源：http://uw.szsharing.cn

[R64] 结束进程
来源：http://kv.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://ba.yuexingan06.cn

[R65] 查看端口占用
来源：http://cb.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://le.jianghongdianzi.cn

[R66] 定时任务
来源：http://mg.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://yh.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://zn.nicolike.cn

openssl rand -hex 16
来源：http://xx.hnjuh.cn

[R68] 计算文件校验值
来源：http://kv.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ly.yuexingan06.cn

[R69] 生成随机密码
来源：http://dm.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://pq.panjiajie.cn

[R70] 时间戳与互转
来源：http://xo.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://ac.nszjky.cn

[R71] 日期格式化
来源：http://nu.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cn.colortex.cn

[R72] 等待端口就绪
来源：http://ua.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://el.asd995.cn

[R73] 分割大日志
来源：http://id.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://wr.huixinmuqiang.cn

[R74] 批量重命名
来源：http://lj.gzmigu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jr.shxzskj.cn

[R75] 导出环境变量
来源：http://qi.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://uy.521024.cn

[R76] 使用临时文件
来源：http://fc.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ky.newstarts.cn

[R77] 读取用户输入
来源：http://nv.huixiangedu.cn

read -rp "请输入: " ans
来源：http://rd.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://ie.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vo.shtwfgs.cn

[R79] 解析命令行选项
来源：http://qy.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yp.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://bk.hahajie.cn

time ./run.sh
来源：http://cx.shxzukj.cn

================================================================================
来源：http://uc.jianghongdianzi.cn

S. C / C++ 专题
来源：http://jp.chemitech.net.cn

================================================================================
来源：http://hx.muxihuayi.cn

[S01] C：Hello World
来源：http://ow.shxzskj.cn

#include <stdio.h>
来源：http://kb.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tx.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://th.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://gg.szxytkj.cn

[S03] C：读入整数
来源：http://hj.521024.cn

int x; scanf("%d", &x);
来源：http://ru.colortex.cn

[S04] C：字符串复制
来源：http://di.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ao.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://az.hahajie.cn

strlen(s)
来源：http://mv.521024.cn

[S06] C：字符串比较
来源：http://vt.haigaiapp.cn

strcmp(a, b) == 0
来源：http://mi.jctech888.com.cn

[S07] C：数组遍历求和
来源：http://on.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tj.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://xs.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kz.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://bp.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fv.nszjky.cn

[S10] C：指针与解引用
来源：http://on.nszjky.cn

int *p = &a;  *p = 5;
来源：http://ot.shxzukj.cn

[S11] C：逐行读文件
来源：http://yd.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://xe.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fw.hahajie.cn

fclose(f);
来源：http://dj.shtwfgs.cn

[S12] C：写文件
来源：http://ww.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pv.hahajie.cn

[S13] C：宏定义
来源：http://hb.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://iw.newstarts.cn

[S14] C：枚举
来源：http://ei.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://cp.nszjky.cn

[S15] C：类型转换
来源：http://jt.yuntaijiaju.cn

(double) a / b
来源：http://nf.nszjky.cn

[S16] C：位操作置位
来源：http://rm.yuntaijiaju.cn

x |= (1 << 3);
来源：http://qu.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://zs.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nb.muxihuayi.cn

[S18] C：命令行参数
来源：http://og.colortex.cn

int main(int argc, char **argv)
来源：http://ws.wgjwhj.cn

[S19] C：快速排序
来源：http://ap.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pv.yuexingan06.cn

[S20] C：二分查找
来源：http://vc.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zo.nszjky.cn

[S21] C：字符类别判断
来源：http://fu.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yb.9csxet.cn

[S22] C：字符串转数字
来源：http://ue.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://iv.shxzukj.cn

[S23] C：随机数
来源：http://qn.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://px.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://nn.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://im.nicolike.cn

[S25] C：内存拷贝
来源：http://yz.shxzskj.cn

memcpy(dst, src, n);
来源：http://pn.colortex.cn

[S26] C：内存清零
来源：http://be.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://cf.jctech888.com.cn

[S27] C：定义常量
来源：http://do.shtwfgs.cn

const double PI = 3.14159;
来源：http://hf.colortex.cn

[S28] C：静态变量
来源：http://rc.yuntaijiaju.cn

static int counter = 0;
来源：http://lr.shxzskj.cn

[S29] C：变参函数
来源：http://hu.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jv.newstarts.cn

[S30] C：头文件保护
来源：http://zm.panjiajie.cn

#ifndef X_H
来源：http://ur.shtwfgs.cn

#define X_H
来源：http://pt.huixiangedu.cn

#endif
来源：http://ty.bookmarksfly.cn

[S31] C++：Hello World
来源：http://ye.bjjhwx.cn

#include <iostream>
来源：http://md.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://rx.huixinmuqiang.cn

[S32] C++：字符串
来源：http://pp.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://ay.shtwfgs.cn

[S33] C++：vector 增删
来源：http://ef.jctech888.com.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sn.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://ju.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://sd.newstarts.cn

[S35] C++：map
来源：http://eu.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uu.yuexingan06.cn

[S36] C++：unordered_map
来源：http://ha.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://md.bjjhwx.cn

[S37] C++：set
来源：http://sf.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zz.haigaiapp.cn

[S38] C++：排序
来源：http://nm.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://xa.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://mn.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fv.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://of.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gm.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://eo.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jx.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://vm.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://ze.colortex.cn

[S43] C++：智能指针
来源：http://vz.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://bt.hnjuh.cn

[S44] C++：引用传参
来源：http://cg.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://mv.muxihuayi.cn

[S45] C++：lambda
来源：http://ie.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ii.521024.cn

[S46] C++：函数模板
来源：http://cn.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wa.yuexingan06.cn

[S47] C++：结构化绑定遍历
来源：http://ss.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://le.colortex.cn

[S48] C++：逐行读文件
来源：http://xk.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gx.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://dp.shxzukj.cn

[S49] C++：写文件
来源：http://xb.chemitech.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ot.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://ly.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rz.colortex.cn

[S51] C++：显式类型转换
来源：http://mq.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://ej.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://sg.nicolike.cn

int size() const noexcept { return n_; }
来源：http://wm.haigaiapp.cn

[S53] C++：移动语义
来源：http://pt.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://gm.gzmigu.cn

[S54] C++：异常处理
来源：http://ps.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ow.bookmarksfly.cn

[S55] C++：结构化绑定
来源：http://oo.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gc.huanxung.cn

[S56] C++：optional
来源：http://mp.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jb.lnxyls.cn

[S57] C++：编译期常量
来源：http://ac.521024.cn

constexpr int N = 10;
来源：http://na.colortex.cn

[S58] C++：命名空间
来源：http://ai.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://qm.gzmigu.cn

[S59] C++：静态断言
来源：http://wz.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uf.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://tg.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oi.jianghongdianzi.cn

================================================================================
来源：http://pj.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hf.lnxyls.cn

================================================================================
来源：http://pe.asd995.cn

[T01] Kotlin：Hello World
来源：http://yw.jctech888.com.cn

println("Hello")
来源：http://ha.szxytkj.cn

[T02] Kotlin：变量
来源：http://ey.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gs.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://bx.jctech888.com.cn

"值: $b"
来源：http://ki.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://uq.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://my.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://xu.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vj.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://sq.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://or.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://fn.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://la.shxzskj.cn

[T08] Kotlin：数据类
来源：http://hg.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://av.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://xp.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://mc.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://ia.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gm.lnxyls.cn

[T11] Kotlin：协程
来源：http://yd.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tt.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://tb.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://kq.shxzskj.cn

[T13] Kotlin：只读 Map
来源：http://un.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://mk.nicolike.cn

[T14] Kotlin：循环
来源：http://iz.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://hz.huanxung.cn

[T15] Kotlin：接口
来源：http://as.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://ej.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://en.shxzskj.cn

print("Hello")
来源：http://bs.asd995.cn

[T17] Swift：变量与常量
来源：http://gg.shtwfgs.cn

var a = 1;  let b = 2
来源：http://hm.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://ip.bjjhwx.cn

"值: \(b)"
来源：http://jm.nszjky.cn

[T19] Swift：可选绑定
来源：http://jp.lnxyls.cn

if let n = opt { print(n) }
来源：http://op.muxihuayi.cn

[T20] Swift：数组操作
来源：http://wg.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gv.szxytkj.cn

[T21] Swift：遍历
来源：http://fn.shtwfgs.cn

for x in a { print(x) }
来源：http://tp.muxihuayi.cn

[T22] Swift：字典
来源：http://oe.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hz.nszjky.cn

[T23] Swift：函数
来源：http://fs.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lo.szxytkj.cn

[T24] Swift：闭包
来源：http://zb.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fq.muxihuayi.cn

[T25] Swift：结构体
来源：http://db.nszjky.cn

struct P { var x: Int }
来源：http://ap.521024.cn

[T26] Swift：类与重写
来源：http://ov.shxzskj.cn

class A: Base { override func f() {} }
来源：http://rs.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://cj.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://os.wgjwhj.cn

[T28] Swift：枚举
来源：http://ed.huanxung.cn

enum Color { case red, green }
来源：http://ig.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://pf.haigaiapp.cn

guard let x = opt else { return }
来源：http://ew.hnjuh.cn

[T30] Swift：协议
来源：http://qn.yuexingan06.cn

protocol Shape { func area() -> Double }
来源：http://iz.panjiajie.cn

[T31] Lua：Hello World
来源：http://ts.bjjhwx.cn

print("Hello")
来源：http://dr.colortex.cn

[T32] Lua：局部变量
来源：http://si.colortex.cn

local a = 1
来源：http://dj.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://fp.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ah.huixiangedu.cn

[T34] Lua：遍历表
来源：http://ff.521024.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ns.asd995.cn

[T35] Lua：字典表
来源：http://tn.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://xl.haigaiapp.cn

[T36] Lua：函数
来源：http://pd.huixiangedu.cn

function add(a, b) return a + b end
来源：http://ul.colortex.cn

[T37] Lua：字符串拼接
来源：http://kg.521024.cn

"a" .. "b"
来源：http://ys.huixiangedu.cn

[T38] Lua：条件
来源：http://ph.bjjhwx.cn

if x > 0 then print("正") end
来源：http://ng.gzmigu.cn


<!-- 参考信息 -->