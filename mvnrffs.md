代发 wailian999

echo $((1 + 2 * 3))
来源：http://mt.colortex.cn

[R28] 浮点运算
来源：http://dv.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://ii.muxihuayi.cn

[R29] 定义函数
来源：http://iy.newstarts.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qf.szxytkj.cn

[R30] 函数返回状态码
来源：http://zg.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://rx.9csxet.cn

[R31] 局部变量
来源：http://sd.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://jj.shxzukj.cn

[R32] 参数个数校验
来源：http://ck.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ev.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://um.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ex.shtwfgs.cn

[R34] 退出时清理
来源：http://xq.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xo.haigaiapp.cn

[R35] 后台执行并等待
来源：http://ia.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yp.9csxet.cn

[R36] 并发执行多个任务
来源：http://vo.shxzskj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vb.huanxung.cn

[R37] 把输出赋给变量
来源：http://rt.colortex.cn

files=$(ls -1)
来源：http://cp.nszjky.cn

[R38] 管道串联
来源：http://sv.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://md.asd995.cn

[R39] 重定向标准输出与错误
来源：http://ud.shxzukj.cn

cmd > out.log 2>&1
来源：http://js.bjjhwx.cn

[R40] 追加写日志
来源：http://og.jctech888.com.cn

echo "log" >> out.log
来源：http://zu.asd995.cn

[R41] 丢弃输出
来源：http://bl.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://cf.521024.cn

[R42] 输入重定向
来源：http://ne.shxzukj.cn

wc -l < a.txt
来源：http://tg.muxihuayi.cn

[R43] 按名字查找文件
来源：http://cf.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://ue.yuexingan06.cn

[R44] 按修改时间查找
来源：http://xt.gzmigu.cn

find . -mtime -7 -type f
来源：http://hh.yuntaijiaju.cn

[R45] 批量删除
来源：http://rq.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://gk.gzmigu.cn

[R46] 递归替换文件内容
来源：http://jc.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zs.gzmigu.cn

[R47] sed 单行替换
来源：http://ns.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kx.haigaiapp.cn

[R48] awk 取指定列
来源：http://hf.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://gg.szxytkj.cn

[R49] awk 带条件
来源：http://ek.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wq.bjjhwx.cn

[R50] awk 求和
来源：http://pk.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pk.wgjwhj.cn

[R51] 排序去重取前几
来源：http://pr.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pr.shxzskj.cn

[R52] 统计行数
来源：http://wh.huixinmuqiang.cn

wc -l a.txt
来源：http://he.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://lc.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mv.lnxyls.cn

[R54] 比较两个文件
来源：http://dl.521024.cn

diff a.txt b.txt
来源：http://we.szxytkj.cn

[R55] 压缩与解压
来源：http://ms.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tm.asd995.cn

[R56] 远程拷贝
来源：http://xm.wgjwhj.cn

scp file user@host:/path/
来源：http://hw.521024.cn

[R57] 远程执行命令
来源：http://az.panjiajie.cn

ssh user@host 'uptime'
来源：http://al.szxytkj.cn

[R58] 下载文件
来源：http://wx.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hj.521024.cn

[R59] 发 POST JSON
来源：http://sp.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bg.colortex.cn

[R60] 只看 HTTP 状态码
来源：http://dd.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mz.jctech888.com.cn

[R61] 磁盘占用
来源：http://ua.shxzukj.cn

df -h;  du -sh *
来源：http://ad.huixinmuqiang.cn

[R62] 找最占空间的文件
来源：http://bs.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://co.shtwfgs.cn

[R63] 内存与进程
来源：http://wg.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://xt.asd995.cn

[R64] 结束进程
来源：http://sf.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://nu.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://eh.shtwfgs.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://as.panjiajie.cn

[R66] 定时任务
来源：http://kw.hahajie.cn

crontab -e;  crontab -l
来源：http://fi.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://er.haigaiapp.cn

openssl rand -hex 16
来源：http://ua.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://cb.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kd.panjiajie.cn

[R69] 生成随机密码
来源：http://rg.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://pb.muxihuayi.cn

[R70] 时间戳与互转
来源：http://cw.szsharing.cn

date +%s;  date -d @1700000000
来源：http://pk.newstarts.cn

[R71] 日期格式化
来源：http://vq.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gl.9csxet.cn

[R72] 等待端口就绪
来源：http://ab.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ij.newstarts.cn

[R73] 分割大日志
来源：http://od.shxzukj.cn

split -l 1000 big.log part_
来源：http://wm.huanxung.cn

[R74] 批量重命名
来源：http://io.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gt.colortex.cn

[R75] 导出环境变量
来源：http://fd.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://ug.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://of.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mx.huixiangedu.cn

[R77] 读取用户输入
来源：http://qi.huanxung.cn

read -rp "请输入: " ans
来源：http://zs.521024.cn

[R78] 交互式菜单
来源：http://pw.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xx.yuexingan06.cn

[R79] 解析命令行选项
来源：http://lk.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xh.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://cg.szsharing.cn

time ./run.sh
来源：http://ts.wgjwhj.cn

================================================================================
来源：http://to.shxzukj.cn

S. C / C++ 专题
来源：http://yo.huixinmuqiang.cn

================================================================================
来源：http://lx.hnjuh.cn

[S01] C：Hello World
来源：http://kg.muxihuayi.cn

#include <stdio.h>
来源：http://kh.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ye.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://fm.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://gg.shxzskj.cn

[S03] C：读入整数
来源：http://uq.shxzukj.cn

int x; scanf("%d", &x);
来源：http://me.huixiangedu.cn

[S04] C：字符串复制
来源：http://gm.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tt.shtwfgs.cn

[S05] C：字符串长度
来源：http://gs.nszjky.cn

strlen(s)
来源：http://xa.yuexingan06.cn

[S06] C：字符串比较
来源：http://yl.newstarts.cn

strcmp(a, b) == 0
来源：http://sm.nicolike.cn

[S07] C：数组遍历求和
来源：http://nz.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rw.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://nt.jctech888.com.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nk.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://yo.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ut.shxzukj.cn

[S10] C：指针与解引用
来源：http://dw.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://vg.huanxung.cn

[S11] C：逐行读文件
来源：http://qd.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://su.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lg.hnjuh.cn

fclose(f);
来源：http://oi.shtwfgs.cn

[S12] C：写文件
来源：http://la.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pf.shxzukj.cn

[S13] C：宏定义
来源：http://on.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qg.nicolike.cn

[S14] C：枚举
来源：http://kp.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://vc.szsharing.cn

[S15] C：类型转换
来源：http://yy.huixinmuqiang.cn

(double) a / b
来源：http://us.wgjwhj.cn

[S16] C：位操作置位
来源：http://rs.9csxet.cn

x |= (1 << 3);
来源：http://nj.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://pu.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rc.shxzskj.cn

[S18] C：命令行参数
来源：http://pc.jctech888.com.cn

int main(int argc, char **argv)
来源：http://vz.hnjuh.cn

[S19] C：快速排序
来源：http://ja.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dn.bookmarksfly.cn

[S20] C：二分查找
来源：http://lm.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qe.huanxung.cn

[S21] C：字符类别判断
来源：http://jw.wgjwhj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xu.muxihuayi.cn

[S22] C：字符串转数字
来源：http://ge.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vq.muxihuayi.cn

[S23] C：随机数
来源：http://kc.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dj.newstarts.cn

[S24] C：获取本地时间
来源：http://dm.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uz.muxihuayi.cn

[S25] C：内存拷贝
来源：http://pk.hahajie.cn

memcpy(dst, src, n);
来源：http://mc.huixinmuqiang.cn

[S26] C：内存清零
来源：http://rr.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://yr.huixiangedu.cn

[S27] C：定义常量
来源：http://iy.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://ui.shxzskj.cn

[S28] C：静态变量
来源：http://af.szsharing.cn

static int counter = 0;
来源：http://zj.521024.cn

[S29] C：变参函数
来源：http://mk.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ao.muxihuayi.cn

[S30] C：头文件保护
来源：http://bg.shxzskj.cn

#ifndef X_H
来源：http://cq.shtwfgs.cn

#define X_H
来源：http://wr.jctech888.com.cn

#endif
来源：http://fi.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://js.shtwfgs.cn

#include <iostream>
来源：http://iv.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://yd.yuexingan06.cn

[S32] C++：字符串
来源：http://nz.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://kt.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://wd.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ih.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://xp.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://am.shxzskj.cn

[S35] C++：map
来源：http://iu.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ot.shxzskj.cn

[S36] C++：unordered_map
来源：http://pf.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ri.hnjuh.cn

[S37] C++：set
来源：http://ww.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sg.asd995.cn

[S38] C++：排序
来源：http://fu.521024.cn

std::sort(v.begin(), v.end());
来源：http://eb.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://xy.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hb.hahajie.cn

[S40] C++：查找元素
来源：http://tm.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rx.asd995.cn

[S41] C++：类与构造函数
来源：http://ir.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mb.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://mu.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://ul.szsharing.cn

[S43] C++：智能指针
来源：http://fp.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://vs.szxytkj.cn

[S44] C++：引用传参
来源：http://ip.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://lg.jianghongdianzi.cn

[S45] C++：lambda
来源：http://qo.colortex.cn

auto add = [](int a, int b) { return a + b; };
来源：http://um.nszjky.cn

[S46] C++：函数模板
来源：http://yn.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://od.wgjwhj.cn

[S47] C++：结构化绑定遍历
来源：http://qx.huixiangedu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dx.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://on.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tl.huanxung.cn

while (std::getline(in, line)) { }
来源：http://bs.shxzskj.cn

[S49] C++：写文件
来源：http://an.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xa.nicolike.cn

[S50] C++：格式化数字
来源：http://dk.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xe.hnjuh.cn

[S51] C++：显式类型转换
来源：http://kb.shxzskj.cn

static_cast<double>(a) / b
来源：http://bc.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://qs.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://ip.newstarts.cn

[S53] C++：移动语义
来源：http://hx.521024.cn

std::vector<int> w = std::move(v);
来源：http://pp.lnxyls.cn

[S54] C++：异常处理
来源：http://yk.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mw.nszjky.cn

[S55] C++：结构化绑定
来源：http://nm.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wu.huanxung.cn

[S56] C++：optional
来源：http://jg.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gd.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://qo.huixiangedu.cn

constexpr int N = 10;
来源：http://do.hahajie.cn

[S58] C++：命名空间
来源：http://yu.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://pz.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://ku.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ek.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://uu.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zi.nszjky.cn

================================================================================
来源：http://og.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wb.shtwfgs.cn

================================================================================
来源：http://vp.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://lq.huixiangedu.cn

println("Hello")
来源：http://vg.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://oi.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uv.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://kh.jctech888.com.cn

"值: $b"
来源：http://ae.gzmigu.cn

[T04] Kotlin：空安全
来源：http://hg.szxytkj.cn

val n: String? = null;  n?.length
来源：http://hi.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://sp.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xg.9csxet.cn

[T06] Kotlin：集合映射
来源：http://tn.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dn.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://dn.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kc.asd995.cn

[T08] Kotlin：数据类
来源：http://ob.colortex.cn

data class User(val name: String, val age: Int)
来源：http://du.colortex.cn

[T09] Kotlin：扩展函数
来源：http://bd.colortex.cn

fun String.exclaim() = this + "!"
来源：http://th.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://bs.bjjhwx.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gk.colortex.cn

[T11] Kotlin：协程
来源：http://rf.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://un.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://lj.haigaiapp.cn

val (a, b) = Pair(1, 2)
来源：http://wn.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://ek.hahajie.cn

val m = mapOf("a" to 1)
来源：http://en.lnxyls.cn

[T14] Kotlin：循环
来源：http://hh.lnxyls.cn

for (i in 1..10) println(i)
来源：http://dr.huanxung.cn

[T15] Kotlin：接口
来源：http://vg.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://ge.muxihuayi.cn

[T16] Swift：Hello World
来源：http://iu.shtwfgs.cn

print("Hello")
来源：http://hp.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://ly.jctech888.com.cn

var a = 1;  let b = 2
来源：http://hj.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://ll.nicolike.cn

"值: \(b)"
来源：http://gn.bookmarksfly.cn

[T19] Swift：可选绑定
来源：http://xb.hahajie.cn

if let n = opt { print(n) }
来源：http://ix.bookmarksfly.cn

[T20] Swift：数组操作
来源：http://iy.yuntaijiaju.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gd.asd995.cn

[T21] Swift：遍历
来源：http://gj.haigaiapp.cn

for x in a { print(x) }
来源：http://de.yuntaijiaju.cn

[T22] Swift：字典
来源：http://bu.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lp.nicolike.cn

[T23] Swift：函数
来源：http://ev.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xx.shxzukj.cn

[T24] Swift：闭包
来源：http://ch.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nd.nszjky.cn

[T25] Swift：结构体
来源：http://fn.shxzskj.cn

struct P { var x: Int }
来源：http://yl.shxzukj.cn

[T26] Swift：类与重写
来源：http://rs.hahajie.cn

class A: Base { override func f() {} }
来源：http://fg.shtwfgs.cn

[T27] Swift：错误处理
来源：http://we.muxihuayi.cn

do { try f() } catch { print(error) }
来源：http://fe.yuexingan06.cn

[T28] Swift：枚举
来源：http://do.szxytkj.cn

enum Color { case red, green }
来源：http://nr.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://tu.panjiajie.cn

guard let x = opt else { return }
来源：http://ij.lnxyls.cn

[T30] Swift：协议
来源：http://zb.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://vo.hahajie.cn


<!-- 参考信息 -->