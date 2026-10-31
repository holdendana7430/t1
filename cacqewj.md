代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rk.hahajie.cn

[R34] 退出时清理
来源：http://bs.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lo.bjjhwx.cn

[R35] 后台执行并等待
来源：http://sa.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wa.szxytkj.cn

[R36] 并发执行多个任务
来源：http://xg.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://es.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://fd.jctech888.com.cn

files=$(ls -1)
来源：http://wl.muxihuayi.cn

[R38] 管道串联
来源：http://am.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://me.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://pn.nicolike.cn

cmd > out.log 2>&1
来源：http://ar.bookmarksfly.cn

[R40] 追加写日志
来源：http://tp.gzmigu.cn

echo "log" >> out.log
来源：http://ps.hnjuh.cn

[R41] 丢弃输出
来源：http://wy.asd995.cn

cmd >/dev/null 2>&1
来源：http://iv.colortex.cn

[R42] 输入重定向
来源：http://xc.yuexingan06.cn

wc -l < a.txt
来源：http://vv.chemitech.net.cn

[R43] 按名字查找文件
来源：http://ib.asd995.cn

find . -name "*.log" -type f
来源：http://vp.panjiajie.cn

[R44] 按修改时间查找
来源：http://ln.chemitech.net.cn

find . -mtime -7 -type f
来源：http://pj.asd995.cn

[R45] 批量删除
来源：http://zm.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://zf.colortex.cn

[R46] 递归替换文件内容
来源：http://uz.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ck.chemitech.net.cn

[R47] sed 单行替换
来源：http://wt.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qw.shxzskj.cn

[R48] awk 取指定列
来源：http://nx.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://ht.wgjwhj.cn

[R49] awk 带条件
来源：http://xp.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://or.huixiangedu.cn

[R50] awk 求和
来源：http://xa.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uc.haigaiapp.cn

[R51] 排序去重取前几
来源：http://kx.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sn.muxihuayi.cn

[R52] 统计行数
来源：http://yj.shtwfgs.cn

wc -l a.txt
来源：http://ev.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://ju.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lc.bjjhwx.cn

[R54] 比较两个文件
来源：http://fw.szxytkj.cn

diff a.txt b.txt
来源：http://cx.haigaiapp.cn

[R55] 压缩与解压
来源：http://yw.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dp.szxytkj.cn

[R56] 远程拷贝
来源：http://bq.hahajie.cn

scp file user@host:/path/
来源：http://zw.gzmigu.cn

[R57] 远程执行命令
来源：http://du.521024.cn

ssh user@host 'uptime'
来源：http://mn.bookmarksfly.cn

[R58] 下载文件
来源：http://hl.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vh.nicolike.cn

[R59] 发 POST JSON
来源：http://aj.yuexingan06.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://th.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://js.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ra.lnxyls.cn

[R61] 磁盘占用
来源：http://qo.hnjuh.cn

df -h;  du -sh *
来源：http://ih.huanxung.cn

[R62] 找最占空间的文件
来源：http://jj.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://cc.wgjwhj.cn

[R63] 内存与进程
来源：http://xk.jctech888.com.cn

free -h;  ps aux | grep nginx
来源：http://ml.newstarts.cn

[R64] 结束进程
来源：http://pm.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://tp.wgjwhj.cn

[R65] 查看端口占用
来源：http://se.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rc.shtwfgs.cn

[R66] 定时任务
来源：http://nh.yuexingan06.cn

crontab -e;  crontab -l
来源：http://ci.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://zf.jctech888.com.cn

openssl rand -hex 16
来源：http://jv.bjjhwx.cn

[R68] 计算文件校验值
来源：http://ji.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ue.muxihuayi.cn

[R69] 生成随机密码
来源：http://jw.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://rv.shxzskj.cn

[R70] 时间戳与互转
来源：http://iz.newstarts.cn

date +%s;  date -d @1700000000
来源：http://uw.jctech888.com.cn

[R71] 日期格式化
来源：http://bw.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://be.chemitech.net.cn

[R72] 等待端口就绪
来源：http://dl.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://df.hahajie.cn

[R73] 分割大日志
来源：http://hb.wgjwhj.cn

split -l 1000 big.log part_
来源：http://fh.szsharing.cn

[R74] 批量重命名
来源：http://bp.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pz.shxzukj.cn

[R75] 导出环境变量
来源：http://mw.bjjhwx.cn

export PATH="$HOME/bin:$PATH"
来源：http://bg.muxihuayi.cn

[R76] 使用临时文件
来源：http://wx.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nh.jctech888.com.cn

[R77] 读取用户输入
来源：http://wg.huanxung.cn

read -rp "请输入: " ans
来源：http://py.521024.cn

[R78] 交互式菜单
来源：http://lq.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sf.huanxung.cn

[R79] 解析命令行选项
来源：http://gd.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bh.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://xu.szxytkj.cn

time ./run.sh
来源：http://uf.9csxet.cn

================================================================================
来源：http://si.gzmigu.cn

S. C / C++ 专题
来源：http://ub.haigaiapp.cn

================================================================================
来源：http://uj.colortex.cn

[S01] C：Hello World
来源：http://ye.nszjky.cn

#include <stdio.h>
来源：http://xv.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zq.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://nz.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://qm.chemitech.net.cn

[S03] C：读入整数
来源：http://ph.lnxyls.cn

int x; scanf("%d", &x);
来源：http://mg.shxzskj.cn

[S04] C：字符串复制
来源：http://xs.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lz.szxytkj.cn

[S05] C：字符串长度
来源：http://xe.nszjky.cn

strlen(s)
来源：http://sw.chemitech.net.cn

[S06] C：字符串比较
来源：http://zv.wgjwhj.cn

strcmp(a, b) == 0
来源：http://ik.asd995.cn

[S07] C：数组遍历求和
来源：http://ya.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uv.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://ab.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dn.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://vr.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ps.bjjhwx.cn

[S10] C：指针与解引用
来源：http://nb.nszjky.cn

int *p = &a;  *p = 5;
来源：http://vk.gzmigu.cn

[S11] C：逐行读文件
来源：http://nx.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://ld.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vm.asd995.cn

fclose(f);
来源：http://pk.haigaiapp.cn

[S12] C：写文件
来源：http://qs.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lx.521024.cn

[S13] C：宏定义
来源：http://kh.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dz.lnxyls.cn

[S14] C：枚举
来源：http://go.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://ex.gzmigu.cn

[S15] C：类型转换
来源：http://ec.muxihuayi.cn

(double) a / b
来源：http://ui.szxytkj.cn

[S16] C：位操作置位
来源：http://xo.chemitech.net.cn

x |= (1 << 3);
来源：http://fa.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://le.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pn.jctech888.com.cn

[S18] C：命令行参数
来源：http://pu.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://oo.colortex.cn

[S19] C：快速排序
来源：http://zf.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sk.yuntaijiaju.cn

[S20] C：二分查找
来源：http://zu.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ny.hnjuh.cn

[S21] C：字符类别判断
来源：http://km.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rc.huanxung.cn

[S22] C：字符串转数字
来源：http://hl.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dr.bookmarksfly.cn

[S23] C：随机数
来源：http://zb.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tz.hnjuh.cn

[S24] C：获取本地时间
来源：http://bi.yuexingan06.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jg.gzmigu.cn

[S25] C：内存拷贝
来源：http://ty.shxzukj.cn

memcpy(dst, src, n);
来源：http://kh.nszjky.cn

[S26] C：内存清零
来源：http://zj.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://ny.hahajie.cn

[S27] C：定义常量
来源：http://mn.lnxyls.cn

const double PI = 3.14159;
来源：http://wv.panjiajie.cn

[S28] C：静态变量
来源：http://xc.jctech888.com.cn

static int counter = 0;
来源：http://mq.nszjky.cn

[S29] C：变参函数
来源：http://ht.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oh.nicolike.cn

[S30] C：头文件保护
来源：http://tj.nszjky.cn

#ifndef X_H
来源：http://ss.muxihuayi.cn

#define X_H
来源：http://le.yuntaijiaju.cn

#endif
来源：http://tp.jctech888.com.cn

[S31] C++：Hello World
来源：http://bk.nszjky.cn

#include <iostream>
来源：http://po.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://eu.lnxyls.cn

[S32] C++：字符串
来源：http://ot.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://xb.panjiajie.cn

[S33] C++：vector 增删
来源：http://rn.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cg.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://iy.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://sg.chemitech.net.cn

[S35] C++：map
来源：http://me.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ny.521024.cn

[S36] C++：unordered_map
来源：http://fl.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zx.szsharing.cn

[S37] C++：set
来源：http://ri.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fk.newstarts.cn

[S38] C++：排序
来源：http://gq.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://mz.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://em.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kw.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://mw.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ct.colortex.cn

[S41] C++：类与构造函数
来源：http://nw.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yl.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://or.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://hz.shxzskj.cn

[S43] C++：智能指针
来源：http://ed.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://mv.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://ye.newstarts.cn

void inc(int &x) { ++x; }
来源：http://ow.colortex.cn

[S45] C++：lambda
来源：http://un.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ig.lnxyls.cn

[S46] C++：函数模板
来源：http://qu.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mh.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://ml.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pf.nszjky.cn

[S48] C++：逐行读文件
来源：http://vw.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qj.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://uo.hnjuh.cn

[S49] C++：写文件
来源：http://nq.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dj.chemitech.net.cn

[S50] C++：格式化数字
来源：http://ub.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vz.bookmarksfly.cn

[S51] C++：显式类型转换
来源：http://ma.huixiangedu.cn

static_cast<double>(a) / b
来源：http://ju.huixinmuqiang.cn

[S52] C++：const 与 noexcept
来源：http://sp.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://wi.huanxung.cn

[S53] C++：移动语义
来源：http://td.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://jk.bjjhwx.cn

[S54] C++：异常处理
来源：http://to.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hy.bookmarksfly.cn

[S55] C++：结构化绑定
来源：http://ca.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xx.huixinmuqiang.cn

[S56] C++：optional
来源：http://ig.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kc.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://fd.gzmigu.cn

constexpr int N = 10;
来源：http://rs.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://xr.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://vw.nicolike.cn

[S59] C++：静态断言
来源：http://sh.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pw.bjjhwx.cn

[S60] C++：遍历并删除元素
来源：http://xg.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jf.asd995.cn

================================================================================
来源：http://qm.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mv.shtwfgs.cn

================================================================================
来源：http://bb.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://ya.panjiajie.cn

println("Hello")
来源：http://am.szsharing.cn

[T02] Kotlin：变量
来源：http://qq.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rp.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://eq.asd995.cn

"值: $b"
来源：http://hm.nszjky.cn

[T04] Kotlin：空安全
来源：http://xj.521024.cn

val n: String? = null;  n?.length
来源：http://dl.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://tn.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ps.9csxet.cn

[T06] Kotlin：集合映射
来源：http://cm.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://li.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://um.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kf.hnjuh.cn

[T08] Kotlin：数据类
来源：http://mo.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://ve.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://qm.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://is.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://vy.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sj.haigaiapp.cn

[T11] Kotlin：协程
来源：http://yr.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kw.muxihuayi.cn

[T12] Kotlin：解构声明
来源：http://dd.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://st.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://pm.9csxet.cn

val m = mapOf("a" to 1)
来源：http://ac.9csxet.cn

[T14] Kotlin：循环
来源：http://ml.gzmigu.cn

for (i in 1..10) println(i)
来源：http://yq.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://ig.newstarts.cn

interface Shape { fun area(): Double }
来源：http://ww.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://ya.szsharing.cn

print("Hello")
来源：http://os.shxzskj.cn

[T17] Swift：变量与常量
来源：http://vg.huanxung.cn

var a = 1;  let b = 2
来源：http://km.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://ab.hnjuh.cn

"值: \(b)"
来源：http://mo.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://xe.nicolike.cn

if let n = opt { print(n) }
来源：http://pc.shtwfgs.cn

[T20] Swift：数组操作
来源：http://gr.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vv.hnjuh.cn

[T21] Swift：遍历
来源：http://tp.jctech888.com.cn

for x in a { print(x) }
来源：http://dg.hnjuh.cn

[T22] Swift：字典
来源：http://ls.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zj.wgjwhj.cn

[T23] Swift：函数
来源：http://zg.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qx.yuexingan06.cn

[T24] Swift：闭包
来源：http://km.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://im.shxzukj.cn

[T25] Swift：结构体
来源：http://yo.9csxet.cn

struct P { var x: Int }
来源：http://hl.chemitech.net.cn

[T26] Swift：类与重写
来源：http://fc.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://ba.huanxung.cn

[T27] Swift：错误处理
来源：http://ia.colortex.cn

do { try f() } catch { print(error) }
来源：http://wx.szsharing.cn

[T28] Swift：枚举
来源：http://hk.bookmarksfly.cn

enum Color { case red, green }
来源：http://kn.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://fp.bookmarksfly.cn

guard let x = opt else { return }
来源：http://mf.huanxung.cn

[T30] Swift：协议
来源：http://fh.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://pg.nszjky.cn

[T31] Lua：Hello World
来源：http://pi.nszjky.cn

print("Hello")
来源：http://pi.haigaiapp.cn

[T32] Lua：局部变量
来源：http://ax.jctech888.com.cn

local a = 1
来源：http://fh.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://id.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jv.haigaiapp.cn

[T34] Lua：遍历表
来源：http://qj.bjjhwx.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://si.huanxung.cn

[T35] Lua：字典表
来源：http://xh.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://mn.lnxyls.cn

[T36] Lua：函数
来源：http://xu.bjjhwx.cn

function add(a, b) return a + b end
来源：http://jm.shxzskj.cn


<!-- 参考信息 -->