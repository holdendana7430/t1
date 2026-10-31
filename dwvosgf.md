代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://je.newstarts.cn

[R30] 函数返回状态码
来源：http://ps.nicolike.cn

f() { return 0; }; f || echo "失败了"
来源：http://lp.wgjwhj.cn

[R31] 局部变量
来源：http://jp.nszjky.cn

f() { local x=1; echo "$x"; }
来源：http://fv.jctech888.com.cn

[R32] 参数个数校验
来源：http://sr.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uz.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://hf.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://if.521024.cn

[R34] 退出时清理
来源：http://az.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ou.jctech888.com.cn

[R35] 后台执行并等待
来源：http://cv.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qn.szsharing.cn

[R36] 并发执行多个任务
来源：http://cs.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sh.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://cn.yuntaijiaju.cn

files=$(ls -1)
来源：http://vm.shxzukj.cn

[R38] 管道串联
来源：http://pm.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://pl.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://cl.shxzskj.cn

cmd > out.log 2>&1
来源：http://jf.shxzukj.cn

[R40] 追加写日志
来源：http://di.haigaiapp.cn

echo "log" >> out.log
来源：http://ov.huanxung.cn

[R41] 丢弃输出
来源：http://th.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://gi.bookmarksfly.cn

[R42] 输入重定向
来源：http://ey.yuexingan06.cn

wc -l < a.txt
来源：http://mm.shxzukj.cn

[R43] 按名字查找文件
来源：http://af.asd995.cn

find . -name "*.log" -type f
来源：http://vk.asd995.cn

[R44] 按修改时间查找
来源：http://ad.lnxyls.cn

find . -mtime -7 -type f
来源：http://bl.huanxung.cn

[R45] 批量删除
来源：http://cp.huanxung.cn

find . -name "*.tmp" -delete
来源：http://zz.yuexingan06.cn

[R46] 递归替换文件内容
来源：http://oe.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rb.lnxyls.cn

[R47] sed 单行替换
来源：http://zc.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ws.huixiangedu.cn

[R48] awk 取指定列
来源：http://ds.hahajie.cn

awk '{print $1, $3}' a.txt
来源：http://px.huixiangedu.cn

[R49] awk 带条件
来源：http://tw.muxihuayi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iw.lnxyls.cn

[R50] awk 求和
来源：http://ys.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qi.szsharing.cn

[R51] 排序去重取前几
来源：http://bm.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gy.huixinmuqiang.cn

[R52] 统计行数
来源：http://km.nszjky.cn

wc -l a.txt
来源：http://kr.nszjky.cn

[R53] 查看文件头与实时尾
来源：http://xy.shxzskj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ca.bjjhwx.cn

[R54] 比较两个文件
来源：http://cs.hahajie.cn

diff a.txt b.txt
来源：http://tx.nszjky.cn

[R55] 压缩与解压
来源：http://ar.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dc.9csxet.cn

[R56] 远程拷贝
来源：http://nl.chemitech.net.cn

scp file user@host:/path/
来源：http://je.521024.cn

[R57] 远程执行命令
来源：http://cg.shtwfgs.cn

ssh user@host 'uptime'
来源：http://jo.huanxung.cn

[R58] 下载文件
来源：http://fj.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://so.colortex.cn

[R59] 发 POST JSON
来源：http://qe.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lj.521024.cn

[R60] 只看 HTTP 状态码
来源：http://oc.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uh.szsharing.cn

[R61] 磁盘占用
来源：http://sf.wgjwhj.cn

df -h;  du -sh *
来源：http://sl.hahajie.cn

[R62] 找最占空间的文件
来源：http://xi.lnxyls.cn

du -ah . | sort -rh | head -10
来源：http://ph.bjjhwx.cn

[R63] 内存与进程
来源：http://yf.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://gq.hahajie.cn

[R64] 结束进程
来源：http://mw.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://pc.nszjky.cn

[R65] 查看端口占用
来源：http://up.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cd.bookmarksfly.cn

[R66] 定时任务
来源：http://fo.shxzskj.cn

crontab -e;  crontab -l
来源：http://jd.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://ts.wgjwhj.cn

openssl rand -hex 16
来源：http://vp.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://ic.huixiangedu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jd.colortex.cn

[R69] 生成随机密码
来源：http://kh.9csxet.cn

head -c 16 /dev/urandom | base64
来源：http://iz.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://vf.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://ls.yuntaijiaju.cn

[R71] 日期格式化
来源：http://nl.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bm.huanxung.cn

[R72] 等待端口就绪
来源：http://lw.huixinmuqiang.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pf.lnxyls.cn

[R73] 分割大日志
来源：http://sh.newstarts.cn

split -l 1000 big.log part_
来源：http://ci.jianghongdianzi.cn

[R74] 批量重命名
来源：http://ed.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vg.jctech888.com.cn

[R75] 导出环境变量
来源：http://gm.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://hk.shxzskj.cn

[R76] 使用临时文件
来源：http://yj.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mh.asd995.cn

[R77] 读取用户输入
来源：http://ch.shxzukj.cn

read -rp "请输入: " ans
来源：http://kh.9csxet.cn

[R78] 交互式菜单
来源：http://sx.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rm.shtwfgs.cn

[R79] 解析命令行选项
来源：http://ez.yuexingan06.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xq.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://yg.haigaiapp.cn

time ./run.sh
来源：http://hq.huanxung.cn

================================================================================
来源：http://oy.9csxet.cn

S. C / C++ 专题
来源：http://yd.shxzukj.cn

================================================================================
来源：http://oa.hahajie.cn

[S01] C：Hello World
来源：http://tt.gzmigu.cn

#include <stdio.h>
来源：http://re.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://je.nszjky.cn

[S02] C：变量与格式化输出
来源：http://yf.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://yu.haigaiapp.cn

[S03] C：读入整数
来源：http://iz.colortex.cn

int x; scanf("%d", &x);
来源：http://pj.huanxung.cn

[S04] C：字符串复制
来源：http://ki.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mc.521024.cn

[S05] C：字符串长度
来源：http://pe.jianghongdianzi.cn

strlen(s)
来源：http://ar.hahajie.cn

[S06] C：字符串比较
来源：http://ag.hahajie.cn

strcmp(a, b) == 0
来源：http://rf.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://cx.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nj.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://gf.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://re.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://zd.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yx.huixiangedu.cn

[S10] C：指针与解引用
来源：http://sb.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://is.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://fn.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://pj.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qp.shtwfgs.cn

fclose(f);
来源：http://th.521024.cn

[S12] C：写文件
来源：http://pb.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fg.nszjky.cn

[S13] C：宏定义
来源：http://ak.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fc.huanxung.cn

[S14] C：枚举
来源：http://kh.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://gt.9csxet.cn

[S15] C：类型转换
来源：http://xt.szsharing.cn

(double) a / b
来源：http://bx.nicolike.cn

[S16] C：位操作置位
来源：http://jl.shtwfgs.cn

x |= (1 << 3);
来源：http://wq.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://yj.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xd.bookmarksfly.cn

[S18] C：命令行参数
来源：http://na.gzmigu.cn

int main(int argc, char **argv)
来源：http://vj.yuntaijiaju.cn

[S19] C：快速排序
来源：http://aa.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://en.yuntaijiaju.cn

[S20] C：二分查找
来源：http://cm.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kv.bjjhwx.cn

[S21] C：字符类别判断
来源：http://oi.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bf.newstarts.cn

[S22] C：字符串转数字
来源：http://dn.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dj.colortex.cn

[S23] C：随机数
来源：http://px.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://it.bjjhwx.cn

[S24] C：获取本地时间
来源：http://pd.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ed.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://gd.wgjwhj.cn

memcpy(dst, src, n);
来源：http://gi.colortex.cn

[S26] C：内存清零
来源：http://eu.521024.cn

memset(a, 0, sizeof a);
来源：http://be.jctech888.com.cn

[S27] C：定义常量
来源：http://vx.bookmarksfly.cn

const double PI = 3.14159;
来源：http://bl.colortex.cn

[S28] C：静态变量
来源：http://ni.shtwfgs.cn

static int counter = 0;
来源：http://wc.shxzukj.cn

[S29] C：变参函数
来源：http://ei.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cv.shtwfgs.cn

[S30] C：头文件保护
来源：http://ry.hahajie.cn

#ifndef X_H
来源：http://hl.chemitech.net.cn

#define X_H
来源：http://ue.lnxyls.cn

#endif
来源：http://ow.gzmigu.cn

[S31] C++：Hello World
来源：http://hp.hnjuh.cn

#include <iostream>
来源：http://en.huixiangedu.cn

int main() { std::cout << "Hello\n"; }
来源：http://rd.szxytkj.cn

[S32] C++：字符串
来源：http://nv.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://qo.bjjhwx.cn

[S33] C++：vector 增删
来源：http://ox.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mp.nicolike.cn

[S34] C++：遍历 vector
来源：http://ya.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://of.szxytkj.cn

[S35] C++：map
来源：http://uz.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dq.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://du.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qv.szxytkj.cn

[S37] C++：set
来源：http://fq.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ld.chemitech.net.cn

[S38] C++：排序
来源：http://tt.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://qf.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://sr.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://av.521024.cn

[S40] C++：查找元素
来源：http://sz.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ir.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://st.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bf.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://lu.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://ek.gzmigu.cn

[S43] C++：智能指针
来源：http://ig.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://hr.szsharing.cn

[S44] C++：引用传参
来源：http://is.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://zm.shxzukj.cn

[S45] C++：lambda
来源：http://iu.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ts.colortex.cn

[S46] C++：函数模板
来源：http://rr.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hr.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://bw.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ry.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://ym.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zu.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://ll.nicolike.cn

[S49] C++：写文件
来源：http://ld.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mo.shtwfgs.cn

[S50] C++：格式化数字
来源：http://gj.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zz.9csxet.cn

[S51] C++：显式类型转换
来源：http://id.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://fi.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://xp.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://rc.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://fc.panjiajie.cn

std::vector<int> w = std::move(v);
来源：http://uh.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://xk.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ih.huanxung.cn

[S55] C++：结构化绑定
来源：http://ft.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bl.huanxung.cn

[S56] C++：optional
来源：http://gv.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cz.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://wy.newstarts.cn

constexpr int N = 10;
来源：http://sn.chemitech.net.cn

[S58] C++：命名空间
来源：http://nw.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://wh.wgjwhj.cn

[S59] C++：静态断言
来源：http://gw.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yk.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://ej.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ul.gzmigu.cn

================================================================================
来源：http://og.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://af.muxihuayi.cn

================================================================================
来源：http://kk.newstarts.cn

[T01] Kotlin：Hello World
来源：http://ii.hahajie.cn

println("Hello")
来源：http://zd.asd995.cn

[T02] Kotlin：变量
来源：http://np.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wb.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://zw.wgjwhj.cn

"值: $b"
来源：http://dt.colortex.cn

[T04] Kotlin：空安全
来源：http://cb.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://we.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://ep.panjiajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://md.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://ec.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cg.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://xn.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yr.asd995.cn

[T08] Kotlin：数据类
来源：http://hh.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://kj.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://zm.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://eq.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://kc.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://eo.bjjhwx.cn

[T11] Kotlin：协程
来源：http://qg.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://el.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://xe.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://px.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://iy.lnxyls.cn

val m = mapOf("a" to 1)
来源：http://na.szxytkj.cn

[T14] Kotlin：循环
来源：http://db.jctech888.com.cn

for (i in 1..10) println(i)
来源：http://wx.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://ro.szsharing.cn

interface Shape { fun area(): Double }
来源：http://fi.huanxung.cn

[T16] Swift：Hello World
来源：http://wn.9csxet.cn

print("Hello")
来源：http://uw.yuntaijiaju.cn

[T17] Swift：变量与常量
来源：http://lp.wgjwhj.cn

var a = 1;  let b = 2
来源：http://jo.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://qn.newstarts.cn

"值: \(b)"
来源：http://lv.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://vf.521024.cn

if let n = opt { print(n) }
来源：http://jf.shxzukj.cn

[T20] Swift：数组操作
来源：http://gs.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tt.shxzukj.cn

[T21] Swift：遍历
来源：http://fz.bookmarksfly.cn

for x in a { print(x) }
来源：http://dl.colortex.cn

[T22] Swift：字典
来源：http://as.asd995.cn

var d = ["a": 1];  d["b"] = 2
来源：http://at.shxzukj.cn

[T23] Swift：函数
来源：http://kq.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ox.chemitech.net.cn

[T24] Swift：闭包
来源：http://mq.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tm.panjiajie.cn

[T25] Swift：结构体
来源：http://sm.shxzukj.cn

struct P { var x: Int }
来源：http://kq.panjiajie.cn

[T26] Swift：类与重写
来源：http://kl.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://xv.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://cb.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://dz.wgjwhj.cn

[T28] Swift：枚举
来源：http://gr.huixiangedu.cn

enum Color { case red, green }
来源：http://yw.colortex.cn

[T29] Swift：guard 提前返回
来源：http://wc.bjjhwx.cn

guard let x = opt else { return }
来源：http://ap.haigaiapp.cn

[T30] Swift：协议
来源：http://cs.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://sh.chemitech.net.cn

[T31] Lua：Hello World
来源：http://gb.9csxet.cn

print("Hello")
来源：http://iv.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://ki.hnjuh.cn

local a = 1
来源：http://cb.asd995.cn


<!-- 参考信息 -->