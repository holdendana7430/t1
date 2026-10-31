代发 wailian999

files=$(ls -1)
来源：http://zm.newstarts.cn

[R38] 管道串联
来源：http://su.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://bv.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://nx.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://tq.gzmigu.cn

[R40] 追加写日志
来源：http://ln.colortex.cn

echo "log" >> out.log
来源：http://df.muxihuayi.cn

[R41] 丢弃输出
来源：http://pt.nszjky.cn

cmd >/dev/null 2>&1
来源：http://jj.lnxyls.cn

[R42] 输入重定向
来源：http://ua.haigaiapp.cn

wc -l < a.txt
来源：http://tb.panjiajie.cn

[R43] 按名字查找文件
来源：http://im.colortex.cn

find . -name "*.log" -type f
来源：http://hm.haigaiapp.cn

[R44] 按修改时间查找
来源：http://mq.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://gp.huixiangedu.cn

[R45] 批量删除
来源：http://nh.huanxung.cn

find . -name "*.tmp" -delete
来源：http://sm.hnjuh.cn

[R46] 递归替换文件内容
来源：http://my.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nx.szxytkj.cn

[R47] sed 单行替换
来源：http://dq.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://je.gzmigu.cn

[R48] awk 取指定列
来源：http://rk.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://ya.wgjwhj.cn

[R49] awk 带条件
来源：http://oz.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ik.huixinmuqiang.cn

[R50] awk 求和
来源：http://hq.bookmarksfly.cn

awk '{s += $2} END {print s}' a.txt
来源：http://au.hahajie.cn

[R51] 排序去重取前几
来源：http://vd.lnxyls.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ap.521024.cn

[R52] 统计行数
来源：http://io.huixiangedu.cn

wc -l a.txt
来源：http://qm.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://yl.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vd.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://iq.gzmigu.cn

diff a.txt b.txt
来源：http://mq.gzmigu.cn

[R55] 压缩与解压
来源：http://kb.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gq.lnxyls.cn

[R56] 远程拷贝
来源：http://hh.nicolike.cn

scp file user@host:/path/
来源：http://on.szxytkj.cn

[R57] 远程执行命令
来源：http://sd.muxihuayi.cn

ssh user@host 'uptime'
来源：http://jt.521024.cn

[R58] 下载文件
来源：http://ll.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nl.gzmigu.cn

[R59] 发 POST JSON
来源：http://vy.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wq.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://me.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mf.szsharing.cn

[R61] 磁盘占用
来源：http://si.huixinmuqiang.cn

df -h;  du -sh *
来源：http://li.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://cw.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://ac.colortex.cn

[R63] 内存与进程
来源：http://du.asd995.cn

free -h;  ps aux | grep nginx
来源：http://jk.huixinmuqiang.cn

[R64] 结束进程
来源：http://oc.chemitech.net.cn

kill -9 $(pgrep -f app.py)
来源：http://kg.nszjky.cn

[R65] 查看端口占用
来源：http://de.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tu.huanxung.cn

[R66] 定时任务
来源：http://xf.panjiajie.cn

crontab -e;  crontab -l
来源：http://id.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://if.newstarts.cn

openssl rand -hex 16
来源：http://ti.gzmigu.cn

[R68] 计算文件校验值
来源：http://hz.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wa.gzmigu.cn

[R69] 生成随机密码
来源：http://bf.hahajie.cn

head -c 16 /dev/urandom | base64
来源：http://nf.muxihuayi.cn

[R70] 时间戳与互转
来源：http://jq.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://ge.huixinmuqiang.cn

[R71] 日期格式化
来源：http://rh.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vh.huixinmuqiang.cn

[R72] 等待端口就绪
来源：http://mp.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ol.hnjuh.cn

[R73] 分割大日志
来源：http://lc.wgjwhj.cn

split -l 1000 big.log part_
来源：http://gy.hahajie.cn

[R74] 批量重命名
来源：http://po.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rz.bookmarksfly.cn

[R75] 导出环境变量
来源：http://yu.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://ae.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://pj.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mc.asd995.cn

[R77] 读取用户输入
来源：http://ip.hnjuh.cn

read -rp "请输入: " ans
来源：http://fz.jctech888.com.cn

[R78] 交互式菜单
来源：http://bu.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cz.asd995.cn

[R79] 解析命令行选项
来源：http://ep.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://st.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://sm.wgjwhj.cn

time ./run.sh
来源：http://kn.shxzskj.cn

================================================================================
来源：http://ej.colortex.cn

S. C / C++ 专题
来源：http://pj.panjiajie.cn

================================================================================
来源：http://rg.bookmarksfly.cn

[S01] C：Hello World
来源：http://ks.haigaiapp.cn

#include <stdio.h>
来源：http://yt.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://av.521024.cn

[S02] C：变量与格式化输出
来源：http://ah.521024.cn

int a = 10; printf("%d\n", a);
来源：http://wg.panjiajie.cn

[S03] C：读入整数
来源：http://ak.hahajie.cn

int x; scanf("%d", &x);
来源：http://gg.huixiangedu.cn

[S04] C：字符串复制
来源：http://xn.huixinmuqiang.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hc.szxytkj.cn

[S05] C：字符串长度
来源：http://fh.colortex.cn

strlen(s)
来源：http://ig.lnxyls.cn

[S06] C：字符串比较
来源：http://il.colortex.cn

strcmp(a, b) == 0
来源：http://jo.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://zp.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jp.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://ty.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mj.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://kb.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ks.nicolike.cn

[S10] C：指针与解引用
来源：http://nf.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://lt.muxihuayi.cn

[S11] C：逐行读文件
来源：http://ek.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://ri.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qy.huanxung.cn

fclose(f);
来源：http://gp.chemitech.net.cn

[S12] C：写文件
来源：http://zf.lnxyls.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cn.hnjuh.cn

[S13] C：宏定义
来源：http://jq.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://js.bjjhwx.cn

[S14] C：枚举
来源：http://ff.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://tk.shtwfgs.cn

[S15] C：类型转换
来源：http://mn.bookmarksfly.cn

(double) a / b
来源：http://si.szxytkj.cn

[S16] C：位操作置位
来源：http://mo.wgjwhj.cn

x |= (1 << 3);
来源：http://pc.nicolike.cn

[S17] C：安全拼接字符串
来源：http://nc.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mt.9csxet.cn

[S18] C：命令行参数
来源：http://el.bjjhwx.cn

int main(int argc, char **argv)
来源：http://qm.panjiajie.cn

[S19] C：快速排序
来源：http://tu.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rw.chemitech.net.cn

[S20] C：二分查找
来源：http://ee.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ga.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://aj.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yk.muxihuayi.cn

[S22] C：字符串转数字
来源：http://jy.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qj.hahajie.cn

[S23] C：随机数
来源：http://xk.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lj.hnjuh.cn

[S24] C：获取本地时间
来源：http://dz.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ly.shtwfgs.cn

[S25] C：内存拷贝
来源：http://cs.wgjwhj.cn

memcpy(dst, src, n);
来源：http://lm.jctech888.com.cn

[S26] C：内存清零
来源：http://ry.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://kk.shxzskj.cn

[S27] C：定义常量
来源：http://cl.huanxung.cn

const double PI = 3.14159;
来源：http://wr.yuntaijiaju.cn

[S28] C：静态变量
来源：http://yd.hahajie.cn

static int counter = 0;
来源：http://pg.haigaiapp.cn

[S29] C：变参函数
来源：http://po.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cu.wgjwhj.cn

[S30] C：头文件保护
来源：http://zp.jianghongdianzi.cn

#ifndef X_H
来源：http://dy.shtwfgs.cn

#define X_H
来源：http://ld.nicolike.cn

#endif
来源：http://nw.panjiajie.cn

[S31] C++：Hello World
来源：http://lu.521024.cn

#include <iostream>
来源：http://hf.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://yn.jctech888.com.cn

[S32] C++：字符串
来源：http://bh.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://xa.jctech888.com.cn

[S33] C++：vector 增删
来源：http://uf.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lg.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://dt.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://dd.shxzskj.cn

[S35] C++：map
来源：http://ev.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ka.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://ej.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hi.huanxung.cn

[S37] C++：set
来源：http://ng.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ff.muxihuayi.cn

[S38] C++：排序
来源：http://rr.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://ih.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://sg.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mk.huixiangedu.cn

[S40] C++：查找元素
来源：http://he.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cd.gzmigu.cn

[S41] C++：类与构造函数
来源：http://mx.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ig.newstarts.cn

[S42] C++：继承与虚函数
来源：http://lw.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://yh.colortex.cn

[S43] C++：智能指针
来源：http://rn.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://cr.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://sf.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://db.bjjhwx.cn

[S45] C++：lambda
来源：http://bm.szxytkj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uw.lnxyls.cn

[S46] C++：函数模板
来源：http://tx.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uh.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://vd.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qj.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://qc.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mz.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://nl.huixinmuqiang.cn

[S49] C++：写文件
来源：http://qa.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://we.szxytkj.cn

[S50] C++：格式化数字
来源：http://sj.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://px.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://kt.yuexingan06.cn

static_cast<double>(a) / b
来源：http://la.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://hb.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://pi.bookmarksfly.cn

[S53] C++：移动语义
来源：http://qv.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://bt.wgjwhj.cn

[S54] C++：异常处理
来源：http://ev.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vz.shxzskj.cn

[S55] C++：结构化绑定
来源：http://ip.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hl.nszjky.cn

[S56] C++：optional
来源：http://oz.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iu.bjjhwx.cn

[S57] C++：编译期常量
来源：http://my.newstarts.cn

constexpr int N = 10;
来源：http://eg.shtwfgs.cn

[S58] C++：命名空间
来源：http://dm.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://zu.shtwfgs.cn

[S59] C++：静态断言
来源：http://gs.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://km.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://ae.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yz.huanxung.cn

================================================================================
来源：http://fj.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uc.wgjwhj.cn

================================================================================
来源：http://vj.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://pw.yuntaijiaju.cn

println("Hello")
来源：http://br.szsharing.cn

[T02] Kotlin：变量
来源：http://em.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://va.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://zt.9csxet.cn

"值: $b"
来源：http://hl.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://gt.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://fa.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://bv.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uy.lnxyls.cn

[T06] Kotlin：集合映射
来源：http://wn.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oj.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://vz.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zj.newstarts.cn

[T08] Kotlin：数据类
来源：http://yo.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://wg.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://xd.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://kz.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://tj.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://re.haigaiapp.cn

[T11] Kotlin：协程
来源：http://du.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ub.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://uq.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://og.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://np.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://kd.hnjuh.cn

[T14] Kotlin：循环
来源：http://fq.521024.cn

for (i in 1..10) println(i)
来源：http://ia.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://er.huixinmuqiang.cn

interface Shape { fun area(): Double }
来源：http://kd.panjiajie.cn

[T16] Swift：Hello World
来源：http://ff.colortex.cn

print("Hello")
来源：http://mk.jctech888.com.cn

[T17] Swift：变量与常量
来源：http://yz.chemitech.net.cn

var a = 1;  let b = 2
来源：http://qy.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://sc.nicolike.cn

"值: \(b)"
来源：http://ae.nszjky.cn

[T19] Swift：可选绑定
来源：http://hg.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://pl.szsharing.cn

[T20] Swift：数组操作
来源：http://ju.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sv.wgjwhj.cn

[T21] Swift：遍历
来源：http://zs.9csxet.cn

for x in a { print(x) }
来源：http://at.colortex.cn

[T22] Swift：字典
来源：http://oj.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://px.hahajie.cn

[T23] Swift：函数
来源：http://hc.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yt.huanxung.cn

[T24] Swift：闭包
来源：http://kq.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://no.szsharing.cn

[T25] Swift：结构体
来源：http://ns.yuexingan06.cn

struct P { var x: Int }
来源：http://zm.lnxyls.cn

[T26] Swift：类与重写
来源：http://dj.hahajie.cn

class A: Base { override func f() {} }
来源：http://is.hnjuh.cn

[T27] Swift：错误处理
来源：http://hn.asd995.cn

do { try f() } catch { print(error) }
来源：http://og.jctech888.com.cn

[T28] Swift：枚举
来源：http://pv.huanxung.cn

enum Color { case red, green }
来源：http://wz.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://cb.haigaiapp.cn

guard let x = opt else { return }
来源：http://tg.haigaiapp.cn

[T30] Swift：协议
来源：http://ax.521024.cn

protocol Shape { func area() -> Double }
来源：http://il.hnjuh.cn

[T31] Lua：Hello World
来源：http://fy.wgjwhj.cn

print("Hello")
来源：http://ho.hnjuh.cn

[T32] Lua：局部变量
来源：http://ls.colortex.cn

local a = 1
来源：http://sj.nszjky.cn

[T33] Lua：表（数组）
来源：http://jb.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fw.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://gq.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nw.muxihuayi.cn

[T35] Lua：字典表
来源：http://bn.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://fp.wgjwhj.cn

[T36] Lua：函数
来源：http://yb.nicolike.cn

function add(a, b) return a + b end
来源：http://qz.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://wc.9csxet.cn

"a" .. "b"
来源：http://ys.gzmigu.cn

[T38] Lua：条件
来源：http://wr.521024.cn

if x > 0 then print("正") end
来源：http://hl.szxytkj.cn

[T39] Lua：模式匹配
来源：http://rz.jianghongdianzi.cn

string.find(s, "%d+")
来源：http://an.newstarts.cn

[T40] Lua：元表
来源：http://yh.colortex.cn

setmetatable({}, { __index = base })
来源：http://am.wgjwhj.cn


<!-- 参考信息 -->