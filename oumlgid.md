代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://xh.jianghongdianzi.cn

[R26] 命令替换
来源：http://pk.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://vu.521024.cn

[R27] 算术展开
来源：http://hu.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://jl.wgjwhj.cn

[R28] 浮点运算
来源：http://ul.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://nv.hnjuh.cn

[R29] 定义函数
来源：http://pr.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yi.nszjky.cn

[R30] 函数返回状态码
来源：http://uj.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://aj.panjiajie.cn

[R31] 局部变量
来源：http://ic.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://ec.wgjwhj.cn

[R32] 参数个数校验
来源：http://ku.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pi.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://fg.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ap.huixinmuqiang.cn

[R34] 退出时清理
来源：http://ba.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://iq.shxzskj.cn

[R35] 后台执行并等待
来源：http://vh.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://de.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://vu.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fu.lnxyls.cn

[R37] 把输出赋给变量
来源：http://rc.wgjwhj.cn

files=$(ls -1)
来源：http://ue.bjjhwx.cn

[R38] 管道串联
来源：http://qf.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://mk.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://et.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://hw.huixiangedu.cn

[R40] 追加写日志
来源：http://wg.521024.cn

echo "log" >> out.log
来源：http://sl.521024.cn

[R41] 丢弃输出
来源：http://lc.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://sw.nszjky.cn

[R42] 输入重定向
来源：http://ch.newstarts.cn

wc -l < a.txt
来源：http://xr.jctech888.com.cn

[R43] 按名字查找文件
来源：http://nu.nszjky.cn

find . -name "*.log" -type f
来源：http://ei.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://wi.shtwfgs.cn

find . -mtime -7 -type f
来源：http://kl.bjjhwx.cn

[R45] 批量删除
来源：http://cg.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://je.9csxet.cn

[R46] 递归替换文件内容
来源：http://mj.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fa.yuexingan06.cn

[R47] sed 单行替换
来源：http://uo.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ct.panjiajie.cn

[R48] awk 取指定列
来源：http://ex.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://ay.shtwfgs.cn

[R49] awk 带条件
来源：http://fw.lnxyls.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pi.muxihuayi.cn

[R50] awk 求和
来源：http://wx.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sr.hnjuh.cn

[R51] 排序去重取前几
来源：http://tk.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lm.shxzukj.cn

[R52] 统计行数
来源：http://jx.shtwfgs.cn

wc -l a.txt
来源：http://ej.panjiajie.cn

[R53] 查看文件头与实时尾
来源：http://pi.shxzskj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wo.bjjhwx.cn

[R54] 比较两个文件
来源：http://qp.szxytkj.cn

diff a.txt b.txt
来源：http://vq.shxzukj.cn

[R55] 压缩与解压
来源：http://mz.shxzukj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hu.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://ex.haigaiapp.cn

scp file user@host:/path/
来源：http://tu.szxytkj.cn

[R57] 远程执行命令
来源：http://pu.hahajie.cn

ssh user@host 'uptime'
来源：http://uc.yuexingan06.cn

[R58] 下载文件
来源：http://pe.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xh.wgjwhj.cn

[R59] 发 POST JSON
来源：http://tm.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://np.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://zj.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fy.521024.cn

[R61] 磁盘占用
来源：http://ka.shtwfgs.cn

df -h;  du -sh *
来源：http://vp.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://tb.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://bu.yuexingan06.cn

[R63] 内存与进程
来源：http://xn.colortex.cn

free -h;  ps aux | grep nginx
来源：http://nu.gzmigu.cn

[R64] 结束进程
来源：http://ma.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://yu.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://rf.colortex.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://df.szxytkj.cn

[R66] 定时任务
来源：http://xl.lnxyls.cn

crontab -e;  crontab -l
来源：http://vv.nicolike.cn

[R67] 生成随机十六进制串
来源：http://kp.chemitech.net.cn

openssl rand -hex 16
来源：http://ix.asd995.cn

[R68] 计算文件校验值
来源：http://ue.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://io.521024.cn

[R69] 生成随机密码
来源：http://wl.huanxung.cn

head -c 16 /dev/urandom | base64
来源：http://my.521024.cn

[R70] 时间戳与互转
来源：http://bh.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://hb.shxzskj.cn

[R71] 日期格式化
来源：http://ao.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nb.jctech888.com.cn

[R72] 等待端口就绪
来源：http://ap.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tm.jctech888.com.cn

[R73] 分割大日志
来源：http://iu.chemitech.net.cn

split -l 1000 big.log part_
来源：http://jh.shxzukj.cn

[R74] 批量重命名
来源：http://xe.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://re.nicolike.cn

[R75] 导出环境变量
来源：http://ii.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://oh.nicolike.cn

[R76] 使用临时文件
来源：http://ri.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oy.panjiajie.cn

[R77] 读取用户输入
来源：http://hv.asd995.cn

read -rp "请输入: " ans
来源：http://af.panjiajie.cn

[R78] 交互式菜单
来源：http://jr.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uk.nszjky.cn

[R79] 解析命令行选项
来源：http://ko.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hs.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://ju.huixiangedu.cn

time ./run.sh
来源：http://ym.hnjuh.cn

================================================================================
来源：http://ym.panjiajie.cn

S. C / C++ 专题
来源：http://ss.huixiangedu.cn

================================================================================
来源：http://kp.asd995.cn

[S01] C：Hello World
来源：http://fl.colortex.cn

#include <stdio.h>
来源：http://gd.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pp.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://lh.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://hv.huixinmuqiang.cn

[S03] C：读入整数
来源：http://cg.szxytkj.cn

int x; scanf("%d", &x);
来源：http://sp.gzmigu.cn

[S04] C：字符串复制
来源：http://wa.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://li.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://cs.shxzskj.cn

strlen(s)
来源：http://wl.shtwfgs.cn

[S06] C：字符串比较
来源：http://mc.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://kl.szxytkj.cn

[S07] C：数组遍历求和
来源：http://dj.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kb.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://tz.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ty.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://ud.hnjuh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ie.jctech888.com.cn

[S10] C：指针与解引用
来源：http://vr.colortex.cn

int *p = &a;  *p = 5;
来源：http://fn.panjiajie.cn

[S11] C：逐行读文件
来源：http://xj.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://ll.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uv.asd995.cn

fclose(f);
来源：http://ka.szxytkj.cn

[S12] C：写文件
来源：http://nl.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ft.haigaiapp.cn

[S13] C：宏定义
来源：http://dq.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uu.colortex.cn

[S14] C：枚举
来源：http://qo.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://pu.521024.cn

[S15] C：类型转换
来源：http://de.shxzskj.cn

(double) a / b
来源：http://qa.yuexingan06.cn

[S16] C：位操作置位
来源：http://qm.muxihuayi.cn

x |= (1 << 3);
来源：http://dq.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://my.huixiangedu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gs.szsharing.cn

[S18] C：命令行参数
来源：http://zu.nicolike.cn

int main(int argc, char **argv)
来源：http://aa.jianghongdianzi.cn

[S19] C：快速排序
来源：http://vn.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vz.shxzskj.cn

[S20] C：二分查找
来源：http://cz.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rz.shxzskj.cn

[S21] C：字符类别判断
来源：http://qi.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vj.asd995.cn

[S22] C：字符串转数字
来源：http://qt.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cl.hnjuh.cn

[S23] C：随机数
来源：http://qa.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bb.hnjuh.cn

[S24] C：获取本地时间
来源：http://pc.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lg.nszjky.cn

[S25] C：内存拷贝
来源：http://yd.huanxung.cn

memcpy(dst, src, n);
来源：http://aw.shxzskj.cn

[S26] C：内存清零
来源：http://bp.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://ti.chemitech.net.cn

[S27] C：定义常量
来源：http://fo.newstarts.cn

const double PI = 3.14159;
来源：http://is.huixinmuqiang.cn

[S28] C：静态变量
来源：http://iv.szsharing.cn

static int counter = 0;
来源：http://sx.muxihuayi.cn

[S29] C：变参函数
来源：http://lj.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uc.szxytkj.cn

[S30] C：头文件保护
来源：http://dh.bookmarksfly.cn

#ifndef X_H
来源：http://ut.asd995.cn

#define X_H
来源：http://qw.huanxung.cn

#endif
来源：http://om.bjjhwx.cn

[S31] C++：Hello World
来源：http://oy.szxytkj.cn

#include <iostream>
来源：http://ve.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://xo.wgjwhj.cn

[S32] C++：字符串
来源：http://xf.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://cs.wgjwhj.cn

[S33] C++：vector 增删
来源：http://uj.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ao.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://ng.asd995.cn

for (auto &x : v) { std::cout << x; }
来源：http://zm.chemitech.net.cn

[S35] C++：map
来源：http://co.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qw.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://fl.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mw.hahajie.cn

[S37] C++：set
来源：http://gm.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mx.shxzukj.cn

[S38] C++：排序
来源：http://ss.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://di.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://rv.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nz.chemitech.net.cn

[S40] C++：查找元素
来源：http://it.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://di.newstarts.cn

[S41] C++：类与构造函数
来源：http://zd.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://en.huanxung.cn

[S42] C++：继承与虚函数
来源：http://au.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://yq.lnxyls.cn

[S43] C++：智能指针
来源：http://ji.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://dv.521024.cn

[S44] C++：引用传参
来源：http://td.szsharing.cn

void inc(int &x) { ++x; }
来源：http://gt.szxytkj.cn

[S45] C++：lambda
来源：http://wn.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ek.huanxung.cn

[S46] C++：函数模板
来源：http://sm.shxzukj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://os.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://zk.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qx.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://od.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vv.asd995.cn

while (std::getline(in, line)) { }
来源：http://vr.9csxet.cn

[S49] C++：写文件
来源：http://qp.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jd.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://jh.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://le.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://aw.shtwfgs.cn

static_cast<double>(a) / b
来源：http://uw.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://sa.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://hf.huixiangedu.cn

[S53] C++：移动语义
来源：http://xe.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://nq.szxytkj.cn

[S54] C++：异常处理
来源：http://wh.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ni.hnjuh.cn

[S55] C++：结构化绑定
来源：http://uw.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kx.nszjky.cn

[S56] C++：optional
来源：http://ap.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wj.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://hy.yuexingan06.cn

constexpr int N = 10;
来源：http://on.9csxet.cn

[S58] C++：命名空间
来源：http://tp.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://sl.bjjhwx.cn

[S59] C++：静态断言
来源：http://vf.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yl.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://my.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lg.szxytkj.cn

================================================================================
来源：http://kw.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wg.yuntaijiaju.cn

================================================================================
来源：http://tr.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://vz.wgjwhj.cn

println("Hello")
来源：http://be.muxihuayi.cn

[T02] Kotlin：变量
来源：http://hb.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tj.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://id.haigaiapp.cn

"值: $b"
来源：http://of.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://bt.szsharing.cn

val n: String? = null;  n?.length
来源：http://of.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://wx.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cc.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://sn.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sj.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://uu.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gg.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://wo.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://tl.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://li.colortex.cn

fun String.exclaim() = this + "!"
来源：http://hc.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://tt.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ep.wgjwhj.cn

[T11] Kotlin：协程
来源：http://kr.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cj.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://hd.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://ks.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://jd.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://pe.521024.cn

[T14] Kotlin：循环
来源：http://ul.gzmigu.cn

for (i in 1..10) println(i)
来源：http://ig.yuexingan06.cn

[T15] Kotlin：接口
来源：http://sh.colortex.cn

interface Shape { fun area(): Double }
来源：http://td.shtwfgs.cn

[T16] Swift：Hello World
来源：http://lh.hahajie.cn

print("Hello")
来源：http://ji.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://xc.hnjuh.cn

var a = 1;  let b = 2
来源：http://mz.9csxet.cn

[T18] Swift：字符串插值
来源：http://tf.yuexingan06.cn

"值: \(b)"
来源：http://tt.colortex.cn

[T19] Swift：可选绑定
来源：http://on.yuexingan06.cn

if let n = opt { print(n) }
来源：http://rw.hnjuh.cn

[T20] Swift：数组操作
来源：http://ub.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fb.gzmigu.cn

[T21] Swift：遍历
来源：http://hr.bjjhwx.cn

for x in a { print(x) }
来源：http://xi.wgjwhj.cn

[T22] Swift：字典
来源：http://yo.huixinmuqiang.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bt.jianghongdianzi.cn

[T23] Swift：函数
来源：http://ky.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xn.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://bn.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sd.nicolike.cn

[T25] Swift：结构体
来源：http://eb.shxzukj.cn

struct P { var x: Int }
来源：http://tr.shtwfgs.cn

[T26] Swift：类与重写
来源：http://wf.szxytkj.cn

class A: Base { override func f() {} }
来源：http://nf.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://ct.521024.cn

do { try f() } catch { print(error) }
来源：http://ls.huanxung.cn

[T28] Swift：枚举
来源：http://hg.yuexingan06.cn

enum Color { case red, green }
来源：http://xs.shxzskj.cn


<!-- 参考信息 -->