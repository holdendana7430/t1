代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qe.521024.cn

[R30] 函数返回状态码
来源：http://hf.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://yb.gzmigu.cn

[R31] 局部变量
来源：http://xv.huanxung.cn

f() { local x=1; echo "$x"; }
来源：http://ax.szsharing.cn

[R32] 参数个数校验
来源：http://ux.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mg.asd995.cn

[R33] 捕获错误并提示行号
来源：http://th.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ll.9csxet.cn

[R34] 退出时清理
来源：http://tn.bjjhwx.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ez.shtwfgs.cn

[R35] 后台执行并等待
来源：http://et.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xn.jianghongdianzi.cn

[R36] 并发执行多个任务
来源：http://hj.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hd.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://ds.szxytkj.cn

files=$(ls -1)
来源：http://ow.9csxet.cn

[R38] 管道串联
来源：http://iy.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://py.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://vr.shxzukj.cn

cmd > out.log 2>&1
来源：http://ks.yuntaijiaju.cn

[R40] 追加写日志
来源：http://em.yuexingan06.cn

echo "log" >> out.log
来源：http://yr.shtwfgs.cn

[R41] 丢弃输出
来源：http://qd.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://qg.bookmarksfly.cn

[R42] 输入重定向
来源：http://nv.muxihuayi.cn

wc -l < a.txt
来源：http://tv.shxzukj.cn

[R43] 按名字查找文件
来源：http://oa.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://ve.asd995.cn

[R44] 按修改时间查找
来源：http://zu.nicolike.cn

find . -mtime -7 -type f
来源：http://qh.asd995.cn

[R45] 批量删除
来源：http://qc.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://qu.shxzskj.cn

[R46] 递归替换文件内容
来源：http://lv.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vp.huanxung.cn

[R47] sed 单行替换
来源：http://fw.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://er.jctech888.com.cn

[R48] awk 取指定列
来源：http://no.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://oi.lnxyls.cn

[R49] awk 带条件
来源：http://hw.wgjwhj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://le.521024.cn

[R50] awk 求和
来源：http://mj.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jo.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://mp.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ky.wgjwhj.cn

[R52] 统计行数
来源：http://gi.huixiangedu.cn

wc -l a.txt
来源：http://cg.huanxung.cn

[R53] 查看文件头与实时尾
来源：http://gb.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kp.9csxet.cn

[R54] 比较两个文件
来源：http://lj.nicolike.cn

diff a.txt b.txt
来源：http://cs.bookmarksfly.cn

[R55] 压缩与解压
来源：http://ky.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tz.chemitech.net.cn

[R56] 远程拷贝
来源：http://uo.jctech888.com.cn

scp file user@host:/path/
来源：http://ch.huixinmuqiang.cn

[R57] 远程执行命令
来源：http://xw.lnxyls.cn

ssh user@host 'uptime'
来源：http://lw.asd995.cn

[R58] 下载文件
来源：http://zr.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sy.haigaiapp.cn

[R59] 发 POST JSON
来源：http://fv.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uc.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://pl.yuntaijiaju.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fm.newstarts.cn

[R61] 磁盘占用
来源：http://pf.bookmarksfly.cn

df -h;  du -sh *
来源：http://fs.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://su.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://gr.huixinmuqiang.cn

[R63] 内存与进程
来源：http://bg.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://kl.nszjky.cn

[R64] 结束进程
来源：http://kc.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://xx.huixiangedu.cn

[R65] 查看端口占用
来源：http://wa.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zc.nicolike.cn

[R66] 定时任务
来源：http://ev.shxzukj.cn

crontab -e;  crontab -l
来源：http://gs.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://zx.bookmarksfly.cn

openssl rand -hex 16
来源：http://kl.gzmigu.cn

[R68] 计算文件校验值
来源：http://gb.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ta.panjiajie.cn

[R69] 生成随机密码
来源：http://yg.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://vv.szsharing.cn

[R70] 时间戳与互转
来源：http://sl.521024.cn

date +%s;  date -d @1700000000
来源：http://mc.gzmigu.cn

[R71] 日期格式化
来源：http://hm.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://de.colortex.cn

[R72] 等待端口就绪
来源：http://hl.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dz.shxzskj.cn

[R73] 分割大日志
来源：http://dg.chemitech.net.cn

split -l 1000 big.log part_
来源：http://ns.panjiajie.cn

[R74] 批量重命名
来源：http://om.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fx.jctech888.com.cn

[R75] 导出环境变量
来源：http://ww.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://sx.newstarts.cn

[R76] 使用临时文件
来源：http://wf.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mt.9csxet.cn

[R77] 读取用户输入
来源：http://fm.shxzskj.cn

read -rp "请输入: " ans
来源：http://jo.hahajie.cn

[R78] 交互式菜单
来源：http://us.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xa.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://el.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://px.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://hk.gzmigu.cn

time ./run.sh
来源：http://sw.nszjky.cn

================================================================================
来源：http://th.haigaiapp.cn

S. C / C++ 专题
来源：http://in.haigaiapp.cn

================================================================================
来源：http://je.hnjuh.cn

[S01] C：Hello World
来源：http://js.yuexingan06.cn

#include <stdio.h>
来源：http://xm.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zh.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://fn.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://qd.nicolike.cn

[S03] C：读入整数
来源：http://my.jianghongdianzi.cn

int x; scanf("%d", &x);
来源：http://nn.wgjwhj.cn

[S04] C：字符串复制
来源：http://su.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jh.jianghongdianzi.cn

[S05] C：字符串长度
来源：http://xs.huixinmuqiang.cn

strlen(s)
来源：http://bu.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://cv.haigaiapp.cn

strcmp(a, b) == 0
来源：http://kq.bookmarksfly.cn

[S07] C：数组遍历求和
来源：http://se.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vq.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://ka.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mi.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://fi.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ou.jctech888.com.cn

[S10] C：指针与解引用
来源：http://pn.hahajie.cn

int *p = &a;  *p = 5;
来源：http://lg.asd995.cn

[S11] C：逐行读文件
来源：http://jc.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://mn.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cx.jctech888.com.cn

fclose(f);
来源：http://mz.chemitech.net.cn

[S12] C：写文件
来源：http://xt.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hy.huanxung.cn

[S13] C：宏定义
来源：http://sy.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fc.szsharing.cn

[S14] C：枚举
来源：http://jj.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://sl.yuexingan06.cn

[S15] C：类型转换
来源：http://mw.newstarts.cn

(double) a / b
来源：http://mf.shtwfgs.cn

[S16] C：位操作置位
来源：http://cb.chemitech.net.cn

x |= (1 << 3);
来源：http://rl.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://gx.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zr.muxihuayi.cn

[S18] C：命令行参数
来源：http://hy.521024.cn

int main(int argc, char **argv)
来源：http://kv.asd995.cn

[S19] C：快速排序
来源：http://cm.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rq.muxihuayi.cn

[S20] C：二分查找
来源：http://re.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://aj.521024.cn

[S21] C：字符类别判断
来源：http://li.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pl.huixiangedu.cn

[S22] C：字符串转数字
来源：http://nf.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mq.nszjky.cn

[S23] C：随机数
来源：http://rs.bookmarksfly.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xd.nicolike.cn

[S24] C：获取本地时间
来源：http://mk.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ox.521024.cn

[S25] C：内存拷贝
来源：http://xg.shxzukj.cn

memcpy(dst, src, n);
来源：http://lj.muxihuayi.cn

[S26] C：内存清零
来源：http://cr.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://zo.jctech888.com.cn

[S27] C：定义常量
来源：http://mx.szxytkj.cn

const double PI = 3.14159;
来源：http://uc.chemitech.net.cn

[S28] C：静态变量
来源：http://kv.gzmigu.cn

static int counter = 0;
来源：http://ml.9csxet.cn

[S29] C：变参函数
来源：http://ym.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sp.bjjhwx.cn

[S30] C：头文件保护
来源：http://gf.asd995.cn

#ifndef X_H
来源：http://ky.nszjky.cn

#define X_H
来源：http://vw.hnjuh.cn

#endif
来源：http://py.colortex.cn

[S31] C++：Hello World
来源：http://uo.haigaiapp.cn

#include <iostream>
来源：http://do.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://uh.shxzskj.cn

[S32] C++：字符串
来源：http://bw.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://vy.wgjwhj.cn

[S33] C++：vector 增删
来源：http://ib.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://im.colortex.cn

[S34] C++：遍历 vector
来源：http://vn.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://rc.huanxung.cn

[S35] C++：map
来源：http://aw.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xz.shxzukj.cn

[S36] C++：unordered_map
来源：http://pw.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qu.yuntaijiaju.cn

[S37] C++：set
来源：http://nr.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yv.jctech888.com.cn

[S38] C++：排序
来源：http://st.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://uc.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://qd.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jg.nicolike.cn

[S40] C++：查找元素
来源：http://gy.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vp.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://kz.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://np.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://zv.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://ec.newstarts.cn

[S43] C++：智能指针
来源：http://xd.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://bt.newstarts.cn

[S44] C++：引用传参
来源：http://dy.521024.cn

void inc(int &x) { ++x; }
来源：http://sb.newstarts.cn

[S45] C++：lambda
来源：http://hl.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xl.nszjky.cn

[S46] C++：函数模板
来源：http://gr.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fs.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://ub.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ri.panjiajie.cn

[S48] C++：逐行读文件
来源：http://iv.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rh.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://ku.panjiajie.cn

[S49] C++：写文件
来源：http://fm.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hi.panjiajie.cn

[S50] C++：格式化数字
来源：http://oo.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mk.szsharing.cn

[S51] C++：显式类型转换
来源：http://or.hahajie.cn

static_cast<double>(a) / b
来源：http://lj.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://lg.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://gn.asd995.cn

[S53] C++：移动语义
来源：http://ra.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://nl.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://qs.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rp.huanxung.cn

[S55] C++：结构化绑定
来源：http://as.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zx.jctech888.com.cn

[S56] C++：optional
来源：http://bl.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kv.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://lz.chemitech.net.cn

constexpr int N = 10;
来源：http://ua.hnjuh.cn

[S58] C++：命名空间
来源：http://uz.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://gi.shtwfgs.cn

[S59] C++：静态断言
来源：http://sk.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tp.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://gc.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jq.chemitech.net.cn

================================================================================
来源：http://qz.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tx.9csxet.cn

================================================================================
来源：http://mt.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://kd.huixinmuqiang.cn

println("Hello")
来源：http://dv.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://sf.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hs.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://oy.lnxyls.cn

"值: $b"
来源：http://uq.szxytkj.cn

[T04] Kotlin：空安全
来源：http://in.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://hs.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://ua.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kz.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://jq.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://en.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://qf.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lv.chemitech.net.cn

[T08] Kotlin：数据类
来源：http://rd.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://cs.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://rg.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://jn.nicolike.cn

[T10] Kotlin：默认参数
来源：http://lf.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ci.szxytkj.cn

[T11] Kotlin：协程
来源：http://me.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gf.asd995.cn

[T12] Kotlin：解构声明
来源：http://bh.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://or.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://jv.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://ez.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://od.9csxet.cn

for (i in 1..10) println(i)
来源：http://fk.newstarts.cn

[T15] Kotlin：接口
来源：http://im.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://zy.szsharing.cn

[T16] Swift：Hello World
来源：http://le.huanxung.cn

print("Hello")
来源：http://do.jctech888.com.cn

[T17] Swift：变量与常量
来源：http://nk.muxihuayi.cn

var a = 1;  let b = 2
来源：http://sx.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://bs.wgjwhj.cn

"值: \(b)"
来源：http://je.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://qo.nicolike.cn

if let n = opt { print(n) }
来源：http://mt.panjiajie.cn

[T20] Swift：数组操作
来源：http://pa.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nf.hahajie.cn

[T21] Swift：遍历
来源：http://ec.bookmarksfly.cn

for x in a { print(x) }
来源：http://cf.muxihuayi.cn

[T22] Swift：字典
来源：http://ed.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nh.muxihuayi.cn

[T23] Swift：函数
来源：http://ag.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gl.jctech888.com.cn

[T24] Swift：闭包
来源：http://lk.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nc.hahajie.cn

[T25] Swift：结构体
来源：http://nc.colortex.cn

struct P { var x: Int }
来源：http://ft.newstarts.cn

[T26] Swift：类与重写
来源：http://mm.hnjuh.cn

class A: Base { override func f() {} }
来源：http://rg.muxihuayi.cn

[T27] Swift：错误处理
来源：http://ih.nicolike.cn

do { try f() } catch { print(error) }
来源：http://xs.colortex.cn

[T28] Swift：枚举
来源：http://wt.haigaiapp.cn

enum Color { case red, green }
来源：http://uu.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://de.nicolike.cn

guard let x = opt else { return }
来源：http://vr.hnjuh.cn

[T30] Swift：协议
来源：http://fd.asd995.cn

protocol Shape { func area() -> Double }
来源：http://rr.szsharing.cn

[T31] Lua：Hello World
来源：http://mz.haigaiapp.cn

print("Hello")
来源：http://gw.huanxung.cn

[T32] Lua：局部变量
来源：http://ld.hnjuh.cn

local a = 1
来源：http://kb.shxzukj.cn


<!-- 参考信息 -->