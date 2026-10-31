代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://tp.wgjwhj.cn

[R26] 命令替换
来源：http://tp.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://pm.bjjhwx.cn

[R27] 算术展开
来源：http://se.hnjuh.cn

echo $((1 + 2 * 3))
来源：http://fc.jianghongdianzi.cn

[R28] 浮点运算
来源：http://bx.newstarts.cn

echo "scale=2; 10/3" | bc
来源：http://ti.huixinmuqiang.cn

[R29] 定义函数
来源：http://kc.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://go.newstarts.cn

[R30] 函数返回状态码
来源：http://pv.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://xo.yuexingan06.cn

[R31] 局部变量
来源：http://od.shxzukj.cn

f() { local x=1; echo "$x"; }
来源：http://nn.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://rx.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://df.bjjhwx.cn

[R33] 捕获错误并提示行号
来源：http://tc.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xu.9csxet.cn

[R34] 退出时清理
来源：http://kc.chemitech.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://an.huixiangedu.cn

[R35] 后台执行并等待
来源：http://hz.gzmigu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nn.asd995.cn

[R36] 并发执行多个任务
来源：http://iq.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iw.lnxyls.cn

[R37] 把输出赋给变量
来源：http://yh.nszjky.cn

files=$(ls -1)
来源：http://od.yuexingan06.cn

[R38] 管道串联
来源：http://af.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://nz.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://lq.hnjuh.cn

cmd > out.log 2>&1
来源：http://fu.nicolike.cn

[R40] 追加写日志
来源：http://no.asd995.cn

echo "log" >> out.log
来源：http://ev.9csxet.cn

[R41] 丢弃输出
来源：http://am.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://vs.bookmarksfly.cn

[R42] 输入重定向
来源：http://pl.huixiangedu.cn

wc -l < a.txt
来源：http://fv.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://kz.wgjwhj.cn

find . -name "*.log" -type f
来源：http://oz.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://vo.hnjuh.cn

find . -mtime -7 -type f
来源：http://ql.chemitech.net.cn

[R45] 批量删除
来源：http://uk.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://us.shxzukj.cn

[R46] 递归替换文件内容
来源：http://zf.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uo.wgjwhj.cn

[R47] sed 单行替换
来源：http://zu.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://uk.hahajie.cn

[R48] awk 取指定列
来源：http://yi.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://wk.shxzskj.cn

[R49] awk 带条件
来源：http://rz.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zq.huixiangedu.cn

[R50] awk 求和
来源：http://pk.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yh.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://qr.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hp.gzmigu.cn

[R52] 统计行数
来源：http://vl.9csxet.cn

wc -l a.txt
来源：http://lw.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://ka.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tp.chemitech.net.cn

[R54] 比较两个文件
来源：http://ch.newstarts.cn

diff a.txt b.txt
来源：http://lr.bjjhwx.cn

[R55] 压缩与解压
来源：http://qs.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ct.wgjwhj.cn

[R56] 远程拷贝
来源：http://sk.bookmarksfly.cn

scp file user@host:/path/
来源：http://bl.huixiangedu.cn

[R57] 远程执行命令
来源：http://nm.szxytkj.cn

ssh user@host 'uptime'
来源：http://lk.lnxyls.cn

[R58] 下载文件
来源：http://wd.colortex.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hc.colortex.cn

[R59] 发 POST JSON
来源：http://fc.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xq.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://zj.yuntaijiaju.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rc.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://ja.colortex.cn

df -h;  du -sh *
来源：http://sj.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://yt.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://fs.panjiajie.cn

[R63] 内存与进程
来源：http://ec.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://el.jianghongdianzi.cn

[R64] 结束进程
来源：http://fr.chemitech.net.cn

kill -9 $(pgrep -f app.py)
来源：http://ji.jctech888.com.cn

[R65] 查看端口占用
来源：http://qy.szxytkj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gn.colortex.cn

[R66] 定时任务
来源：http://rq.wgjwhj.cn

crontab -e;  crontab -l
来源：http://qq.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://xc.hahajie.cn

openssl rand -hex 16
来源：http://wi.panjiajie.cn

[R68] 计算文件校验值
来源：http://ud.newstarts.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xx.yuexingan06.cn

[R69] 生成随机密码
来源：http://hy.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://cf.shtwfgs.cn

[R70] 时间戳与互转
来源：http://tx.jianghongdianzi.cn

date +%s;  date -d @1700000000
来源：http://wq.jianghongdianzi.cn

[R71] 日期格式化
来源：http://je.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jb.huixiangedu.cn

[R72] 等待端口就绪
来源：http://fs.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mw.shxzukj.cn

[R73] 分割大日志
来源：http://ns.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://gx.szxytkj.cn

[R74] 批量重命名
来源：http://ek.jianghongdianzi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://we.lnxyls.cn

[R75] 导出环境变量
来源：http://of.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://jf.wgjwhj.cn

[R76] 使用临时文件
来源：http://wg.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jp.asd995.cn

[R77] 读取用户输入
来源：http://rg.wgjwhj.cn

read -rp "请输入: " ans
来源：http://vj.9csxet.cn

[R78] 交互式菜单
来源：http://kp.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ow.521024.cn

[R79] 解析命令行选项
来源：http://ci.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sy.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://cp.521024.cn

time ./run.sh
来源：http://yt.hnjuh.cn

================================================================================
来源：http://hc.jctech888.com.cn

S. C / C++ 专题
来源：http://ln.asd995.cn

================================================================================
来源：http://rn.szxytkj.cn

[S01] C：Hello World
来源：http://bw.colortex.cn

#include <stdio.h>
来源：http://qb.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vc.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://fn.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://tz.yuexingan06.cn

[S03] C：读入整数
来源：http://zq.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://ya.lnxyls.cn

[S04] C：字符串复制
来源：http://hh.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bl.bjjhwx.cn

[S05] C：字符串长度
来源：http://ft.shtwfgs.cn

strlen(s)
来源：http://oh.shxzukj.cn

[S06] C：字符串比较
来源：http://wt.panjiajie.cn

strcmp(a, b) == 0
来源：http://ec.shxzukj.cn

[S07] C：数组遍历求和
来源：http://zb.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qt.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://xi.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xk.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://pj.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uf.panjiajie.cn

[S10] C：指针与解引用
来源：http://st.szsharing.cn

int *p = &a;  *p = 5;
来源：http://ui.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://ip.muxihuayi.cn

FILE *f = fopen("a.txt", "r");
来源：http://gl.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hi.lnxyls.cn

fclose(f);
来源：http://mp.huixiangedu.cn

[S12] C：写文件
来源：http://pi.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ed.bjjhwx.cn

[S13] C：宏定义
来源：http://tc.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lg.chemitech.net.cn

[S14] C：枚举
来源：http://zb.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://yq.szsharing.cn

[S15] C：类型转换
来源：http://jk.hnjuh.cn

(double) a / b
来源：http://vf.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://gi.yuexingan06.cn

x |= (1 << 3);
来源：http://yy.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://tw.lnxyls.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xe.nicolike.cn

[S18] C：命令行参数
来源：http://nt.jctech888.com.cn

int main(int argc, char **argv)
来源：http://gw.521024.cn

[S19] C：快速排序
来源：http://sf.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ci.panjiajie.cn

[S20] C：二分查找
来源：http://zi.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cx.newstarts.cn

[S21] C：字符类别判断
来源：http://xf.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sg.szsharing.cn

[S22] C：字符串转数字
来源：http://fu.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://we.9csxet.cn

[S23] C：随机数
来源：http://ow.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qx.shxzskj.cn

[S24] C：获取本地时间
来源：http://yg.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ws.wgjwhj.cn

[S25] C：内存拷贝
来源：http://il.nicolike.cn

memcpy(dst, src, n);
来源：http://sk.jianghongdianzi.cn

[S26] C：内存清零
来源：http://qb.9csxet.cn

memset(a, 0, sizeof a);
来源：http://ir.chemitech.net.cn

[S27] C：定义常量
来源：http://dd.yuexingan06.cn

const double PI = 3.14159;
来源：http://bx.yuexingan06.cn

[S28] C：静态变量
来源：http://yl.jctech888.com.cn

static int counter = 0;
来源：http://yj.521024.cn

[S29] C：变参函数
来源：http://ak.huixinmuqiang.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hc.yuexingan06.cn

[S30] C：头文件保护
来源：http://tv.lnxyls.cn

#ifndef X_H
来源：http://ye.panjiajie.cn

#define X_H
来源：http://uc.9csxet.cn

#endif
来源：http://af.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://kt.chemitech.net.cn

#include <iostream>
来源：http://ps.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://wm.asd995.cn

[S32] C++：字符串
来源：http://uy.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://ri.yuexingan06.cn

[S33] C++：vector 增删
来源：http://cx.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://du.panjiajie.cn

[S34] C++：遍历 vector
来源：http://ik.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://vi.yuexingan06.cn

[S35] C++：map
来源：http://fx.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dq.nszjky.cn

[S36] C++：unordered_map
来源：http://th.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mc.asd995.cn

[S37] C++：set
来源：http://yy.jctech888.com.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ez.haigaiapp.cn

[S38] C++：排序
来源：http://gi.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://br.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://dj.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oo.panjiajie.cn

[S40] C++：查找元素
来源：http://yk.nicolike.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bb.521024.cn

[S41] C++：类与构造函数
来源：http://zm.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yv.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://dz.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://zk.colortex.cn

[S43] C++：智能指针
来源：http://dn.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://ve.gzmigu.cn

[S44] C++：引用传参
来源：http://kw.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://xg.nicolike.cn

[S45] C++：lambda
来源：http://ry.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ax.yuexingan06.cn

[S46] C++：函数模板
来源：http://dl.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ny.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://bv.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rz.newstarts.cn

[S48] C++：逐行读文件
来源：http://rz.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zd.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://fj.colortex.cn

[S49] C++：写文件
来源：http://hz.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vw.hahajie.cn

[S50] C++：格式化数字
来源：http://ed.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gz.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://vz.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://xf.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://iy.newstarts.cn

int size() const noexcept { return n_; }
来源：http://ry.lnxyls.cn

[S53] C++：移动语义
来源：http://sl.asd995.cn

std::vector<int> w = std::move(v);
来源：http://wu.gzmigu.cn

[S54] C++：异常处理
来源：http://zb.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ve.lnxyls.cn

[S55] C++：结构化绑定
来源：http://pr.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kq.jctech888.com.cn

[S56] C++：optional
来源：http://yx.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hy.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://fz.bookmarksfly.cn

constexpr int N = 10;
来源：http://hk.521024.cn

[S58] C++：命名空间
来源：http://mw.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://pk.haigaiapp.cn

[S59] C++：静态断言
来源：http://rw.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ex.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://of.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mi.colortex.cn

================================================================================
来源：http://bb.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lc.shxzskj.cn

================================================================================
来源：http://vd.asd995.cn

[T01] Kotlin：Hello World
来源：http://xs.jctech888.com.cn

println("Hello")
来源：http://yf.9csxet.cn

[T02] Kotlin：变量
来源：http://fe.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nx.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://gl.nszjky.cn

"值: $b"
来源：http://bu.gzmigu.cn

[T04] Kotlin：空安全
来源：http://rb.gzmigu.cn

val n: String? = null;  n?.length
来源：http://uy.521024.cn

[T05] Kotlin：when 表达式
来源：http://wk.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ja.huanxung.cn

[T06] Kotlin：集合映射
来源：http://yl.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lw.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://ad.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wf.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://qz.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://qb.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://zh.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://wm.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://cx.bookmarksfly.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pp.szsharing.cn

[T11] Kotlin：协程
来源：http://zb.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xe.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://zw.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://hc.521024.cn

[T13] Kotlin：只读 Map
来源：http://mb.szsharing.cn

val m = mapOf("a" to 1)
来源：http://qo.521024.cn

[T14] Kotlin：循环
来源：http://gg.colortex.cn

for (i in 1..10) println(i)
来源：http://gl.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://wz.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://kg.nicolike.cn

[T16] Swift：Hello World
来源：http://cb.yuntaijiaju.cn

print("Hello")
来源：http://ke.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://wh.panjiajie.cn

var a = 1;  let b = 2
来源：http://ix.9csxet.cn

[T18] Swift：字符串插值
来源：http://uz.bookmarksfly.cn

"值: \(b)"
来源：http://wn.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://kb.hnjuh.cn

if let n = opt { print(n) }
来源：http://xc.nicolike.cn

[T20] Swift：数组操作
来源：http://zr.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kv.szxytkj.cn

[T21] Swift：遍历
来源：http://il.newstarts.cn

for x in a { print(x) }
来源：http://ow.9csxet.cn

[T22] Swift：字典
来源：http://ug.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://af.panjiajie.cn

[T23] Swift：函数
来源：http://wr.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rw.szxytkj.cn

[T24] Swift：闭包
来源：http://vv.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zd.muxihuayi.cn

[T25] Swift：结构体
来源：http://yv.asd995.cn

struct P { var x: Int }
来源：http://sc.colortex.cn

[T26] Swift：类与重写
来源：http://jv.9csxet.cn

class A: Base { override func f() {} }
来源：http://jm.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://lv.nicolike.cn

do { try f() } catch { print(error) }
来源：http://tw.521024.cn

[T28] Swift：枚举
来源：http://hv.wgjwhj.cn

enum Color { case red, green }
来源：http://xt.hnjuh.cn


<!-- 参考信息 -->