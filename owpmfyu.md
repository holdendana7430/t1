代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xq.wgjwhj.cn

[R24] 大小写转换
来源：http://zb.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nl.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://yb.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://px.shxzskj.cn

[R26] 命令替换
来源：http://wb.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://tw.huixinmuqiang.cn

[R27] 算术展开
来源：http://ch.gzmigu.cn

echo $((1 + 2 * 3))
来源：http://yb.panjiajie.cn

[R28] 浮点运算
来源：http://el.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://na.huixiangedu.cn

[R29] 定义函数
来源：http://bm.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cg.haigaiapp.cn

[R30] 函数返回状态码
来源：http://rt.9csxet.cn

f() { return 0; }; f || echo "失败了"
来源：http://uq.521024.cn

[R31] 局部变量
来源：http://rb.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://nm.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://oc.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dz.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://lm.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ub.bjjhwx.cn

[R34] 退出时清理
来源：http://po.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cp.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://ep.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tt.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://js.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jv.bjjhwx.cn

[R37] 把输出赋给变量
来源：http://au.haigaiapp.cn

files=$(ls -1)
来源：http://ua.huanxung.cn

[R38] 管道串联
来源：http://xb.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://yy.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://pp.yuexingan06.cn

cmd > out.log 2>&1
来源：http://zn.huixinmuqiang.cn

[R40] 追加写日志
来源：http://mb.521024.cn

echo "log" >> out.log
来源：http://ls.gzmigu.cn

[R41] 丢弃输出
来源：http://jx.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://lw.wgjwhj.cn

[R42] 输入重定向
来源：http://yh.colortex.cn

wc -l < a.txt
来源：http://ma.szsharing.cn

[R43] 按名字查找文件
来源：http://mp.shxzskj.cn

find . -name "*.log" -type f
来源：http://gt.bjjhwx.cn

[R44] 按修改时间查找
来源：http://kq.yuexingan06.cn

find . -mtime -7 -type f
来源：http://eo.yuexingan06.cn

[R45] 批量删除
来源：http://sy.huanxung.cn

find . -name "*.tmp" -delete
来源：http://ul.gzmigu.cn

[R46] 递归替换文件内容
来源：http://ml.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ch.lnxyls.cn

[R47] sed 单行替换
来源：http://nt.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ug.asd995.cn

[R48] awk 取指定列
来源：http://pe.521024.cn

awk '{print $1, $3}' a.txt
来源：http://fk.nszjky.cn

[R49] awk 带条件
来源：http://kp.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wv.shtwfgs.cn

[R50] awk 求和
来源：http://ia.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://la.shtwfgs.cn

[R51] 排序去重取前几
来源：http://ba.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pm.jianghongdianzi.cn

[R52] 统计行数
来源：http://jj.bjjhwx.cn

wc -l a.txt
来源：http://fb.shtwfgs.cn

[R53] 查看文件头与实时尾
来源：http://hz.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gl.bookmarksfly.cn

[R54] 比较两个文件
来源：http://oh.huixinmuqiang.cn

diff a.txt b.txt
来源：http://en.shxzukj.cn

[R55] 压缩与解压
来源：http://oe.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qk.newstarts.cn

[R56] 远程拷贝
来源：http://go.haigaiapp.cn

scp file user@host:/path/
来源：http://ei.gzmigu.cn

[R57] 远程执行命令
来源：http://le.521024.cn

ssh user@host 'uptime'
来源：http://nr.hahajie.cn

[R58] 下载文件
来源：http://gm.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wm.hnjuh.cn

[R59] 发 POST JSON
来源：http://xk.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rn.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://is.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wp.nszjky.cn

[R61] 磁盘占用
来源：http://hy.jianghongdianzi.cn

df -h;  du -sh *
来源：http://qb.huanxung.cn

[R62] 找最占空间的文件
来源：http://oq.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://oj.panjiajie.cn

[R63] 内存与进程
来源：http://gh.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://zu.chemitech.net.cn

[R64] 结束进程
来源：http://sj.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://mo.shxzskj.cn

[R65] 查看端口占用
来源：http://pw.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eo.shtwfgs.cn

[R66] 定时任务
来源：http://ya.9csxet.cn

crontab -e;  crontab -l
来源：http://ec.haigaiapp.cn

[R67] 生成随机十六进制串
来源：http://nx.bookmarksfly.cn

openssl rand -hex 16
来源：http://vs.szxytkj.cn

[R68] 计算文件校验值
来源：http://st.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ij.hnjuh.cn

[R69] 生成随机密码
来源：http://im.colortex.cn

head -c 16 /dev/urandom | base64
来源：http://gb.huixiangedu.cn

[R70] 时间戳与互转
来源：http://ol.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://bw.hnjuh.cn

[R71] 日期格式化
来源：http://bp.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hu.newstarts.cn

[R72] 等待端口就绪
来源：http://id.chemitech.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zt.jctech888.com.cn

[R73] 分割大日志
来源：http://im.shtwfgs.cn

split -l 1000 big.log part_
来源：http://yo.asd995.cn

[R74] 批量重命名
来源：http://mc.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xy.bjjhwx.cn

[R75] 导出环境变量
来源：http://fo.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://yn.haigaiapp.cn

[R76] 使用临时文件
来源：http://ll.shxzskj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dh.nicolike.cn

[R77] 读取用户输入
来源：http://vd.hnjuh.cn

read -rp "请输入: " ans
来源：http://aj.gzmigu.cn

[R78] 交互式菜单
来源：http://fi.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zv.9csxet.cn

[R79] 解析命令行选项
来源：http://tp.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zl.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://av.bjjhwx.cn

time ./run.sh
来源：http://ei.gzmigu.cn

================================================================================
来源：http://gf.szsharing.cn

S. C / C++ 专题
来源：http://xo.huanxung.cn

================================================================================
来源：http://jl.lnxyls.cn

[S01] C：Hello World
来源：http://gq.huixiangedu.cn

#include <stdio.h>
来源：http://dm.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gf.hahajie.cn

[S02] C：变量与格式化输出
来源：http://it.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://uu.9csxet.cn

[S03] C：读入整数
来源：http://vi.panjiajie.cn

int x; scanf("%d", &x);
来源：http://ld.nszjky.cn

[S04] C：字符串复制
来源：http://fj.panjiajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ty.newstarts.cn

[S05] C：字符串长度
来源：http://cn.lnxyls.cn

strlen(s)
来源：http://tn.nicolike.cn

[S06] C：字符串比较
来源：http://ot.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://ar.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://fk.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ug.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://yr.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ld.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://pw.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bd.nicolike.cn

[S10] C：指针与解引用
来源：http://nc.asd995.cn

int *p = &a;  *p = 5;
来源：http://gg.yuexingan06.cn

[S11] C：逐行读文件
来源：http://ll.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://nx.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://du.newstarts.cn

fclose(f);
来源：http://ob.huixinmuqiang.cn

[S12] C：写文件
来源：http://ds.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gu.szxytkj.cn

[S13] C：宏定义
来源：http://ve.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lk.shxzukj.cn

[S14] C：枚举
来源：http://bx.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://un.lnxyls.cn

[S15] C：类型转换
来源：http://zk.chemitech.net.cn

(double) a / b
来源：http://eh.nszjky.cn

[S16] C：位操作置位
来源：http://jm.hahajie.cn

x |= (1 << 3);
来源：http://iv.nszjky.cn

[S17] C：安全拼接字符串
来源：http://zf.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://do.gzmigu.cn

[S18] C：命令行参数
来源：http://vh.newstarts.cn

int main(int argc, char **argv)
来源：http://xn.huanxung.cn

[S19] C：快速排序
来源：http://hm.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dh.huixinmuqiang.cn

[S20] C：二分查找
来源：http://rj.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tq.newstarts.cn

[S21] C：字符类别判断
来源：http://pi.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sz.muxihuayi.cn

[S22] C：字符串转数字
来源：http://wb.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xa.bookmarksfly.cn

[S23] C：随机数
来源：http://zz.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nc.haigaiapp.cn

[S24] C：获取本地时间
来源：http://ty.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://vn.muxihuayi.cn

memcpy(dst, src, n);
来源：http://lw.gzmigu.cn

[S26] C：内存清零
来源：http://oy.521024.cn

memset(a, 0, sizeof a);
来源：http://gz.wgjwhj.cn

[S27] C：定义常量
来源：http://vi.521024.cn

const double PI = 3.14159;
来源：http://ka.chemitech.net.cn

[S28] C：静态变量
来源：http://ci.yuexingan06.cn

static int counter = 0;
来源：http://gv.nszjky.cn

[S29] C：变参函数
来源：http://vw.huanxung.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sa.panjiajie.cn

[S30] C：头文件保护
来源：http://qo.nicolike.cn

#ifndef X_H
来源：http://lv.hnjuh.cn

#define X_H
来源：http://cd.muxihuayi.cn

#endif
来源：http://pa.panjiajie.cn

[S31] C++：Hello World
来源：http://vo.huanxung.cn

#include <iostream>
来源：http://cx.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://vk.wgjwhj.cn

[S32] C++：字符串
来源：http://pe.colortex.cn

std::string s = "hi";  s += "!";
来源：http://mi.asd995.cn

[S33] C++：vector 增删
来源：http://nu.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sm.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://ij.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://vt.hahajie.cn

[S35] C++：map
来源：http://wn.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fm.521024.cn

[S36] C++：unordered_map
来源：http://eb.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jx.gzmigu.cn

[S37] C++：set
来源：http://eo.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xn.jianghongdianzi.cn

[S38] C++：排序
来源：http://td.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://jk.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://er.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lz.panjiajie.cn

[S40] C++：查找元素
来源：http://xv.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ct.lnxyls.cn

[S41] C++：类与构造函数
来源：http://ae.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wq.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://zr.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://zz.panjiajie.cn

[S43] C++：智能指针
来源：http://vp.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://jp.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://zf.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://je.9csxet.cn

[S45] C++：lambda
来源：http://lw.colortex.cn

auto add = [](int a, int b) { return a + b; };
来源：http://im.shtwfgs.cn

[S46] C++：函数模板
来源：http://bp.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ev.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://am.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://et.colortex.cn

[S48] C++：逐行读文件
来源：http://gv.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wb.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://if.521024.cn

[S49] C++：写文件
来源：http://jx.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ox.yuexingan06.cn

[S50] C++：格式化数字
来源：http://ay.shxzukj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pd.shxzukj.cn

[S51] C++：显式类型转换
来源：http://ee.yuexingan06.cn

static_cast<double>(a) / b
来源：http://dc.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://zy.9csxet.cn

int size() const noexcept { return n_; }
来源：http://pi.asd995.cn

[S53] C++：移动语义
来源：http://um.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://ak.bjjhwx.cn

[S54] C++：异常处理
来源：http://xg.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ye.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://iy.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tw.szsharing.cn

[S56] C++：optional
来源：http://kt.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://za.wgjwhj.cn

[S57] C++：编译期常量
来源：http://sp.yuexingan06.cn

constexpr int N = 10;
来源：http://mj.nszjky.cn

[S58] C++：命名空间
来源：http://dw.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://gb.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://vm.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qm.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://sf.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yp.jctech888.com.cn

================================================================================
来源：http://aw.haigaiapp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vl.szsharing.cn

================================================================================
来源：http://fq.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://bb.yuexingan06.cn

println("Hello")
来源：http://al.nszjky.cn

[T02] Kotlin：变量
来源：http://qm.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ky.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://zy.asd995.cn

"值: $b"
来源：http://kv.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://gu.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://xs.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://tk.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tt.9csxet.cn

[T06] Kotlin：集合映射
来源：http://wa.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xj.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://qo.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mc.hnjuh.cn

[T08] Kotlin：数据类
来源：http://de.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://yy.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://mu.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://yp.asd995.cn

[T10] Kotlin：默认参数
来源：http://hc.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://us.gzmigu.cn

[T11] Kotlin：协程
来源：http://eh.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://no.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://qg.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://vg.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://qf.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://wu.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://ag.nicolike.cn

for (i in 1..10) println(i)
来源：http://fa.nszjky.cn

[T15] Kotlin：接口
来源：http://wm.asd995.cn

interface Shape { fun area(): Double }
来源：http://qa.newstarts.cn

[T16] Swift：Hello World
来源：http://mj.9csxet.cn

print("Hello")
来源：http://qh.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://wz.yuexingan06.cn

var a = 1;  let b = 2
来源：http://ey.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://jw.bjjhwx.cn

"值: \(b)"
来源：http://zs.panjiajie.cn

[T19] Swift：可选绑定
来源：http://xf.bjjhwx.cn

if let n = opt { print(n) }
来源：http://xt.nszjky.cn

[T20] Swift：数组操作
来源：http://fl.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nu.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://mz.newstarts.cn

for x in a { print(x) }
来源：http://zg.wgjwhj.cn

[T22] Swift：字典
来源：http://ns.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zh.hnjuh.cn

[T23] Swift：函数
来源：http://zf.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mn.chemitech.net.cn

[T24] Swift：闭包
来源：http://fb.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gz.newstarts.cn

[T25] Swift：结构体
来源：http://rv.asd995.cn

struct P { var x: Int }
来源：http://sg.shtwfgs.cn

[T26] Swift：类与重写
来源：http://qj.szsharing.cn

class A: Base { override func f() {} }
来源：http://yi.yuntaijiaju.cn


<!-- 参考信息 -->