代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jj.yuexingan06.cn

[R24] 大小写转换
来源：http://ca.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ru.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://jx.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jg.nicolike.cn

[R26] 命令替换
来源：http://rr.huixiangedu.cn

now=$(date +%F); echo "$now"
来源：http://jx.nszjky.cn

[R27] 算术展开
来源：http://nq.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://px.shxzskj.cn

[R28] 浮点运算
来源：http://kq.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://wl.colortex.cn

[R29] 定义函数
来源：http://ei.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bs.huanxung.cn

[R30] 函数返回状态码
来源：http://iy.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://sr.colortex.cn

[R31] 局部变量
来源：http://bz.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://cf.haigaiapp.cn

[R32] 参数个数校验
来源：http://yg.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fj.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://mv.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gq.huixinmuqiang.cn

[R34] 退出时清理
来源：http://zy.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ta.haigaiapp.cn

[R35] 后台执行并等待
来源：http://xp.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cw.nszjky.cn

[R36] 并发执行多个任务
来源：http://ig.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ic.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://bf.huixinmuqiang.cn

files=$(ls -1)
来源：http://yc.nszjky.cn

[R38] 管道串联
来源：http://cl.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://tv.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://ad.yuexingan06.cn

cmd > out.log 2>&1
来源：http://xk.hahajie.cn

[R40] 追加写日志
来源：http://oe.szsharing.cn

echo "log" >> out.log
来源：http://se.chemitech.net.cn

[R41] 丢弃输出
来源：http://ir.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://ui.jianghongdianzi.cn

[R42] 输入重定向
来源：http://bc.szxytkj.cn

wc -l < a.txt
来源：http://nk.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://el.shtwfgs.cn

find . -name "*.log" -type f
来源：http://pu.newstarts.cn

[R44] 按修改时间查找
来源：http://kx.bjjhwx.cn

find . -mtime -7 -type f
来源：http://tq.szxytkj.cn

[R45] 批量删除
来源：http://zr.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://zt.hnjuh.cn

[R46] 递归替换文件内容
来源：http://kp.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pc.chemitech.net.cn

[R47] sed 单行替换
来源：http://zr.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hm.hahajie.cn

[R48] awk 取指定列
来源：http://ie.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://lt.shtwfgs.cn

[R49] awk 带条件
来源：http://pn.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uf.yuntaijiaju.cn

[R50] awk 求和
来源：http://mf.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yc.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://ck.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pd.huixiangedu.cn

[R52] 统计行数
来源：http://vk.nicolike.cn

wc -l a.txt
来源：http://xl.521024.cn

[R53] 查看文件头与实时尾
来源：http://ai.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fk.lnxyls.cn

[R54] 比较两个文件
来源：http://vy.yuntaijiaju.cn

diff a.txt b.txt
来源：http://li.nszjky.cn

[R55] 压缩与解压
来源：http://rc.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rj.haigaiapp.cn

[R56] 远程拷贝
来源：http://fl.szsharing.cn

scp file user@host:/path/
来源：http://jl.huanxung.cn

[R57] 远程执行命令
来源：http://jy.asd995.cn

ssh user@host 'uptime'
来源：http://xy.shxzskj.cn

[R58] 下载文件
来源：http://ft.hnjuh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jr.huixiangedu.cn

[R59] 发 POST JSON
来源：http://sr.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wr.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://qg.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kf.hnjuh.cn

[R61] 磁盘占用
来源：http://dx.yuexingan06.cn

df -h;  du -sh *
来源：http://gp.9csxet.cn

[R62] 找最占空间的文件
来源：http://hj.jctech888.com.cn

du -ah . | sort -rh | head -10
来源：http://of.9csxet.cn

[R63] 内存与进程
来源：http://pg.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://fp.shxzskj.cn

[R64] 结束进程
来源：http://dz.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://dr.huanxung.cn

[R65] 查看端口占用
来源：http://eo.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://el.huixiangedu.cn

[R66] 定时任务
来源：http://gz.panjiajie.cn

crontab -e;  crontab -l
来源：http://gs.colortex.cn

[R67] 生成随机十六进制串
来源：http://wo.huixiangedu.cn

openssl rand -hex 16
来源：http://iw.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://wa.newstarts.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tb.9csxet.cn

[R69] 生成随机密码
来源：http://ys.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://rq.szxytkj.cn

[R70] 时间戳与互转
来源：http://ri.nicolike.cn

date +%s;  date -d @1700000000
来源：http://ns.hnjuh.cn

[R71] 日期格式化
来源：http://li.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pm.521024.cn

[R72] 等待端口就绪
来源：http://gr.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pd.newstarts.cn

[R73] 分割大日志
来源：http://ds.jctech888.com.cn

split -l 1000 big.log part_
来源：http://cz.nicolike.cn

[R74] 批量重命名
来源：http://um.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fn.nicolike.cn

[R75] 导出环境变量
来源：http://pl.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://aq.szsharing.cn

[R76] 使用临时文件
来源：http://xn.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zn.nszjky.cn

[R77] 读取用户输入
来源：http://dn.muxihuayi.cn

read -rp "请输入: " ans
来源：http://lk.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://ok.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gk.panjiajie.cn

[R79] 解析命令行选项
来源：http://nv.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sq.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://zy.szsharing.cn

time ./run.sh
来源：http://sd.shxzukj.cn

================================================================================
来源：http://ge.nszjky.cn

S. C / C++ 专题
来源：http://sf.muxihuayi.cn

================================================================================
来源：http://dg.nicolike.cn

[S01] C：Hello World
来源：http://ue.huanxung.cn

#include <stdio.h>
来源：http://oc.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pz.nicolike.cn

[S02] C：变量与格式化输出
来源：http://ds.panjiajie.cn

int a = 10; printf("%d\n", a);
来源：http://sj.gzmigu.cn

[S03] C：读入整数
来源：http://ck.asd995.cn

int x; scanf("%d", &x);
来源：http://dg.gzmigu.cn

[S04] C：字符串复制
来源：http://km.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hb.wgjwhj.cn

[S05] C：字符串长度
来源：http://vc.szsharing.cn

strlen(s)
来源：http://zs.bookmarksfly.cn

[S06] C：字符串比较
来源：http://if.jctech888.com.cn

strcmp(a, b) == 0
来源：http://vc.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://sg.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hn.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://iq.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zp.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://on.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ei.asd995.cn

[S10] C：指针与解引用
来源：http://vp.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://ln.chemitech.net.cn

[S11] C：逐行读文件
来源：http://yb.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://or.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gu.panjiajie.cn

fclose(f);
来源：http://eb.szxytkj.cn

[S12] C：写文件
来源：http://ql.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xb.hnjuh.cn

[S13] C：宏定义
来源：http://gk.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vj.bookmarksfly.cn

[S14] C：枚举
来源：http://xr.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://hw.asd995.cn

[S15] C：类型转换
来源：http://hm.yuntaijiaju.cn

(double) a / b
来源：http://jl.muxihuayi.cn

[S16] C：位操作置位
来源：http://fx.gzmigu.cn

x |= (1 << 3);
来源：http://mt.nicolike.cn

[S17] C：安全拼接字符串
来源：http://aj.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cn.shtwfgs.cn

[S18] C：命令行参数
来源：http://jm.shxzskj.cn

int main(int argc, char **argv)
来源：http://ru.hahajie.cn

[S19] C：快速排序
来源：http://ve.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zp.chemitech.net.cn

[S20] C：二分查找
来源：http://gp.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wo.wgjwhj.cn

[S21] C：字符类别判断
来源：http://nh.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rr.colortex.cn

[S22] C：字符串转数字
来源：http://me.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dp.haigaiapp.cn

[S23] C：随机数
来源：http://hz.bookmarksfly.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ao.shxzskj.cn

[S24] C：获取本地时间
来源：http://oi.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ns.shxzskj.cn

[S25] C：内存拷贝
来源：http://fg.haigaiapp.cn

memcpy(dst, src, n);
来源：http://ic.wgjwhj.cn

[S26] C：内存清零
来源：http://hp.newstarts.cn

memset(a, 0, sizeof a);
来源：http://wm.nicolike.cn

[S27] C：定义常量
来源：http://dd.haigaiapp.cn

const double PI = 3.14159;
来源：http://wa.chemitech.net.cn

[S28] C：静态变量
来源：http://yz.hnjuh.cn

static int counter = 0;
来源：http://dl.huixinmuqiang.cn

[S29] C：变参函数
来源：http://un.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ub.shxzskj.cn

[S30] C：头文件保护
来源：http://it.nszjky.cn

#ifndef X_H
来源：http://jj.521024.cn

#define X_H
来源：http://er.bookmarksfly.cn

#endif
来源：http://rm.chemitech.net.cn

[S31] C++：Hello World
来源：http://eo.muxihuayi.cn

#include <iostream>
来源：http://wl.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://vl.shtwfgs.cn

[S32] C++：字符串
来源：http://to.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://mu.wgjwhj.cn

[S33] C++：vector 增删
来源：http://ee.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ck.muxihuayi.cn

[S34] C++：遍历 vector
来源：http://zl.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://qb.wgjwhj.cn

[S35] C++：map
来源：http://pb.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pl.shxzukj.cn

[S36] C++：unordered_map
来源：http://qs.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hr.asd995.cn

[S37] C++：set
来源：http://wk.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ou.lnxyls.cn

[S38] C++：排序
来源：http://kz.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://gt.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://hr.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yv.jianghongdianzi.cn

[S40] C++：查找元素
来源：http://kh.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ir.colortex.cn

[S41] C++：类与构造函数
来源：http://vp.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kv.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://zb.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://ou.bjjhwx.cn

[S43] C++：智能指针
来源：http://eo.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://yu.muxihuayi.cn

[S44] C++：引用传参
来源：http://fi.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://mj.yuexingan06.cn

[S45] C++：lambda
来源：http://yx.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ai.hahajie.cn

[S46] C++：函数模板
来源：http://xn.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ck.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://jo.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gr.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://ud.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hq.colortex.cn

while (std::getline(in, line)) { }
来源：http://rm.nszjky.cn

[S49] C++：写文件
来源：http://ck.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ri.gzmigu.cn

[S50] C++：格式化数字
来源：http://ji.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ec.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://tn.gzmigu.cn

static_cast<double>(a) / b
来源：http://ta.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://is.szsharing.cn

int size() const noexcept { return n_; }
来源：http://rd.haigaiapp.cn

[S53] C++：移动语义
来源：http://ln.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://ws.colortex.cn

[S54] C++：异常处理
来源：http://ve.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pb.yuexingan06.cn

[S55] C++：结构化绑定
来源：http://uk.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://st.newstarts.cn

[S56] C++：optional
来源：http://zq.9csxet.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wq.nicolike.cn

[S57] C++：编译期常量
来源：http://sx.huixinmuqiang.cn

constexpr int N = 10;
来源：http://rs.nicolike.cn

[S58] C++：命名空间
来源：http://vj.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://ix.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://my.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nd.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://rd.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ba.yuexingan06.cn

================================================================================
来源：http://ww.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mg.nszjky.cn

================================================================================
来源：http://ca.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://xz.newstarts.cn

println("Hello")
来源：http://wu.lnxyls.cn

[T02] Kotlin：变量
来源：http://hx.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dm.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://el.huixinmuqiang.cn

"值: $b"
来源：http://ce.szxytkj.cn

[T04] Kotlin：空安全
来源：http://yw.521024.cn

val n: String? = null;  n?.length
来源：http://yk.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://wl.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dz.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://xr.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vv.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://sa.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uj.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://wl.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://ib.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://gq.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://si.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://dx.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ie.haigaiapp.cn

[T11] Kotlin：协程
来源：http://uc.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mi.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://pk.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://zv.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://tn.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://mi.bjjhwx.cn

[T14] Kotlin：循环
来源：http://bt.shxzskj.cn

for (i in 1..10) println(i)
来源：http://rb.bjjhwx.cn

[T15] Kotlin：接口
来源：http://yn.9csxet.cn

interface Shape { fun area(): Double }
来源：http://si.huanxung.cn

[T16] Swift：Hello World
来源：http://lj.shxzskj.cn

print("Hello")
来源：http://kp.521024.cn

[T17] Swift：变量与常量
来源：http://qf.hahajie.cn

var a = 1;  let b = 2
来源：http://mv.panjiajie.cn

[T18] Swift：字符串插值
来源：http://um.yuexingan06.cn

"值: \(b)"
来源：http://sv.nicolike.cn

[T19] Swift：可选绑定
来源：http://gl.gzmigu.cn

if let n = opt { print(n) }
来源：http://gf.nszjky.cn

[T20] Swift：数组操作
来源：http://co.yuntaijiaju.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nv.asd995.cn

[T21] Swift：遍历
来源：http://tr.muxihuayi.cn

for x in a { print(x) }
来源：http://et.shxzukj.cn

[T22] Swift：字典
来源：http://xn.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fp.hnjuh.cn

[T23] Swift：函数
来源：http://fk.wgjwhj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pm.wgjwhj.cn

[T24] Swift：闭包
来源：http://hm.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xe.521024.cn

[T25] Swift：结构体
来源：http://cy.9csxet.cn

struct P { var x: Int }
来源：http://sz.nicolike.cn

[T26] Swift：类与重写
来源：http://tl.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://av.shtwfgs.cn


<!-- 参考信息 -->