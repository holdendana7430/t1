代发 wailian999

echo $((1 + 2 * 3))
来源：http://ja.huanxung.cn

[R28] 浮点运算
来源：http://pk.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://yl.huanxung.cn

[R29] 定义函数
来源：http://tz.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rm.szxytkj.cn

[R30] 函数返回状态码
来源：http://ob.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://as.shxzskj.cn

[R31] 局部变量
来源：http://na.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://zv.asd995.cn

[R32] 参数个数校验
来源：http://sy.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fw.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://yv.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kg.bookmarksfly.cn

[R34] 退出时清理
来源：http://bm.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rc.newstarts.cn

[R35] 后台执行并等待
来源：http://lw.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oe.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://hq.wgjwhj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bv.newstarts.cn

[R37] 把输出赋给变量
来源：http://vi.shtwfgs.cn

files=$(ls -1)
来源：http://qa.hahajie.cn

[R38] 管道串联
来源：http://vh.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://gc.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://dt.haigaiapp.cn

cmd > out.log 2>&1
来源：http://yl.bookmarksfly.cn

[R40] 追加写日志
来源：http://gk.521024.cn

echo "log" >> out.log
来源：http://zs.nicolike.cn

[R41] 丢弃输出
来源：http://co.hahajie.cn

cmd >/dev/null 2>&1
来源：http://td.chemitech.net.cn

[R42] 输入重定向
来源：http://ep.nszjky.cn

wc -l < a.txt
来源：http://tc.chemitech.net.cn

[R43] 按名字查找文件
来源：http://cd.shxzskj.cn

find . -name "*.log" -type f
来源：http://yu.yuexingan06.cn

[R44] 按修改时间查找
来源：http://hh.yuexingan06.cn

find . -mtime -7 -type f
来源：http://ji.shxzskj.cn

[R45] 批量删除
来源：http://hd.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://lb.gzmigu.cn

[R46] 递归替换文件内容
来源：http://qy.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eu.panjiajie.cn

[R47] sed 单行替换
来源：http://ya.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://px.szxytkj.cn

[R48] awk 取指定列
来源：http://qn.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://qh.yuntaijiaju.cn

[R49] awk 带条件
来源：http://aa.asd995.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rt.hahajie.cn

[R50] awk 求和
来源：http://qy.colortex.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kh.shxzskj.cn

[R51] 排序去重取前几
来源：http://hx.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pa.wgjwhj.cn

[R52] 统计行数
来源：http://mb.bookmarksfly.cn

wc -l a.txt
来源：http://is.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://gl.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jb.nszjky.cn

[R54] 比较两个文件
来源：http://cm.yuntaijiaju.cn

diff a.txt b.txt
来源：http://rw.wgjwhj.cn

[R55] 压缩与解压
来源：http://ss.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rg.huixiangedu.cn

[R56] 远程拷贝
来源：http://ki.bjjhwx.cn

scp file user@host:/path/
来源：http://eh.asd995.cn

[R57] 远程执行命令
来源：http://lx.9csxet.cn

ssh user@host 'uptime'
来源：http://zk.asd995.cn

[R58] 下载文件
来源：http://tp.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://td.shtwfgs.cn

[R59] 发 POST JSON
来源：http://wl.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gc.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://zc.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sx.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://im.wgjwhj.cn

df -h;  du -sh *
来源：http://lh.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://vr.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://py.521024.cn

[R63] 内存与进程
来源：http://il.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://dc.jianghongdianzi.cn

[R64] 结束进程
来源：http://wv.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://ft.szxytkj.cn

[R65] 查看端口占用
来源：http://vm.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yj.colortex.cn

[R66] 定时任务
来源：http://mv.shxzskj.cn

crontab -e;  crontab -l
来源：http://dj.nicolike.cn

[R67] 生成随机十六进制串
来源：http://cd.huixinmuqiang.cn

openssl rand -hex 16
来源：http://hh.shtwfgs.cn

[R68] 计算文件校验值
来源：http://os.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sn.jctech888.com.cn

[R69] 生成随机密码
来源：http://iv.521024.cn

head -c 16 /dev/urandom | base64
来源：http://yq.gzmigu.cn

[R70] 时间戳与互转
来源：http://fq.9csxet.cn

date +%s;  date -d @1700000000
来源：http://bz.shtwfgs.cn

[R71] 日期格式化
来源：http://mt.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rw.lnxyls.cn

[R72] 等待端口就绪
来源：http://ke.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rq.shxzskj.cn

[R73] 分割大日志
来源：http://fr.521024.cn

split -l 1000 big.log part_
来源：http://pt.huixinmuqiang.cn

[R74] 批量重命名
来源：http://xt.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gr.9csxet.cn

[R75] 导出环境变量
来源：http://fy.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://sz.szxytkj.cn

[R76] 使用临时文件
来源：http://an.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dg.panjiajie.cn

[R77] 读取用户输入
来源：http://zd.huanxung.cn

read -rp "请输入: " ans
来源：http://lh.szxytkj.cn

[R78] 交互式菜单
来源：http://rt.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oq.huixiangedu.cn

[R79] 解析命令行选项
来源：http://yh.yuexingan06.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://of.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://ie.wgjwhj.cn

time ./run.sh
来源：http://rg.shxzskj.cn

================================================================================
来源：http://jv.lnxyls.cn

S. C / C++ 专题
来源：http://dp.newstarts.cn

================================================================================
来源：http://yn.gzmigu.cn

[S01] C：Hello World
来源：http://vv.huixinmuqiang.cn

#include <stdio.h>
来源：http://nz.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hj.gzmigu.cn

[S02] C：变量与格式化输出
来源：http://nm.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://wd.colortex.cn

[S03] C：读入整数
来源：http://gm.shxzskj.cn

int x; scanf("%d", &x);
来源：http://mc.hnjuh.cn

[S04] C：字符串复制
来源：http://qo.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zi.shxzukj.cn

[S05] C：字符串长度
来源：http://kr.huixinmuqiang.cn

strlen(s)
来源：http://gq.shxzukj.cn

[S06] C：字符串比较
来源：http://et.yuexingan06.cn

strcmp(a, b) == 0
来源：http://od.hnjuh.cn

[S07] C：数组遍历求和
来源：http://li.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ha.521024.cn

[S08] C：动态内存分配与释放
来源：http://tu.jctech888.com.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vq.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://zr.lnxyls.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qj.wgjwhj.cn

[S10] C：指针与解引用
来源：http://qn.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://hs.shxzskj.cn

[S11] C：逐行读文件
来源：http://ev.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://hv.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uv.huixiangedu.cn

fclose(f);
来源：http://xt.bjjhwx.cn

[S12] C：写文件
来源：http://xr.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ra.muxihuayi.cn

[S13] C：宏定义
来源：http://sl.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wd.huixinmuqiang.cn

[S14] C：枚举
来源：http://ye.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://tz.bjjhwx.cn

[S15] C：类型转换
来源：http://lk.chemitech.net.cn

(double) a / b
来源：http://rv.szsharing.cn

[S16] C：位操作置位
来源：http://ub.huixinmuqiang.cn

x |= (1 << 3);
来源：http://qa.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://rc.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cd.9csxet.cn

[S18] C：命令行参数
来源：http://ar.bookmarksfly.cn

int main(int argc, char **argv)
来源：http://vv.shtwfgs.cn

[S19] C：快速排序
来源：http://ug.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hi.jctech888.com.cn

[S20] C：二分查找
来源：http://pd.9csxet.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rx.bjjhwx.cn

[S21] C：字符类别判断
来源：http://nj.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wq.newstarts.cn

[S22] C：字符串转数字
来源：http://mi.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ma.huixinmuqiang.cn

[S23] C：随机数
来源：http://ao.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://he.nszjky.cn

[S24] C：获取本地时间
来源：http://lg.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pa.bjjhwx.cn

[S25] C：内存拷贝
来源：http://bl.colortex.cn

memcpy(dst, src, n);
来源：http://ud.nicolike.cn

[S26] C：内存清零
来源：http://mi.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://ev.jctech888.com.cn

[S27] C：定义常量
来源：http://oq.hnjuh.cn

const double PI = 3.14159;
来源：http://hq.muxihuayi.cn

[S28] C：静态变量
来源：http://gy.jianghongdianzi.cn

static int counter = 0;
来源：http://rn.colortex.cn

[S29] C：变参函数
来源：http://vh.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nd.shtwfgs.cn

[S30] C：头文件保护
来源：http://lm.huixiangedu.cn

#ifndef X_H
来源：http://ad.newstarts.cn

#define X_H
来源：http://kd.nicolike.cn

#endif
来源：http://rb.hnjuh.cn

[S31] C++：Hello World
来源：http://kz.huanxung.cn

#include <iostream>
来源：http://az.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://pr.chemitech.net.cn

[S32] C++：字符串
来源：http://fa.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://ds.wgjwhj.cn

[S33] C++：vector 增删
来源：http://qa.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uu.asd995.cn

[S34] C++：遍历 vector
来源：http://jb.szsharing.cn

for (auto &x : v) { std::cout << x; }
来源：http://iw.bjjhwx.cn

[S35] C++：map
来源：http://gc.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ex.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://up.gzmigu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lw.bjjhwx.cn

[S37] C++：set
来源：http://rw.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jc.szxytkj.cn

[S38] C++：排序
来源：http://gl.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://qg.521024.cn

[S39] C++：自定义比较器排序
来源：http://is.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eq.szsharing.cn

[S40] C++：查找元素
来源：http://fy.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hs.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://sm.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wd.szsharing.cn

[S42] C++：继承与虚函数
来源：http://qq.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://km.yuexingan06.cn

[S43] C++：智能指针
来源：http://ni.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://is.bjjhwx.cn

[S44] C++：引用传参
来源：http://sd.yuntaijiaju.cn

void inc(int &x) { ++x; }
来源：http://rf.chemitech.net.cn

[S45] C++：lambda
来源：http://bs.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nv.newstarts.cn

[S46] C++：函数模板
来源：http://im.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lw.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://ab.huixiangedu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kt.hahajie.cn

[S48] C++：逐行读文件
来源：http://dp.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sz.nszjky.cn

while (std::getline(in, line)) { }
来源：http://xp.jctech888.com.cn

[S49] C++：写文件
来源：http://eo.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gl.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://qu.huanxung.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uk.panjiajie.cn

[S51] C++：显式类型转换
来源：http://fy.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://st.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://dz.newstarts.cn

int size() const noexcept { return n_; }
来源：http://ya.jctech888.com.cn

[S53] C++：移动语义
来源：http://bj.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://aa.bjjhwx.cn

[S54] C++：异常处理
来源：http://xv.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qp.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://dq.muxihuayi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wl.newstarts.cn

[S56] C++：optional
来源：http://qx.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xx.hnjuh.cn

[S57] C++：编译期常量
来源：http://ws.jianghongdianzi.cn

constexpr int N = 10;
来源：http://cf.szsharing.cn

[S58] C++：命名空间
来源：http://gq.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://kn.hnjuh.cn

[S59] C++：静态断言
来源：http://sj.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vx.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://lv.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pu.bjjhwx.cn

================================================================================
来源：http://nd.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kc.shxzukj.cn

================================================================================
来源：http://he.9csxet.cn

[T01] Kotlin：Hello World
来源：http://wd.chemitech.net.cn

println("Hello")
来源：http://yp.newstarts.cn

[T02] Kotlin：变量
来源：http://mc.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vp.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://km.gzmigu.cn

"值: $b"
来源：http://pq.huanxung.cn

[T04] Kotlin：空安全
来源：http://cg.gzmigu.cn

val n: String? = null;  n?.length
来源：http://uw.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://ld.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kh.nicolike.cn

[T06] Kotlin：集合映射
来源：http://zg.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://uu.colortex.cn

[T07] Kotlin：集合过滤
来源：http://hx.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yt.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://cc.colortex.cn

data class User(val name: String, val age: Int)
来源：http://vo.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://qa.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://vj.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://mu.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kw.bjjhwx.cn

[T11] Kotlin：协程
来源：http://uv.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fb.huanxung.cn

[T12] Kotlin：解构声明
来源：http://vt.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://sp.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://fj.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://bu.hnjuh.cn

[T14] Kotlin：循环
来源：http://ty.huixiangedu.cn

for (i in 1..10) println(i)
来源：http://pp.chemitech.net.cn

[T15] Kotlin：接口
来源：http://mi.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://ll.gzmigu.cn

[T16] Swift：Hello World
来源：http://ud.huanxung.cn

print("Hello")
来源：http://am.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://aa.szsharing.cn

var a = 1;  let b = 2
来源：http://ny.nicolike.cn

[T18] Swift：字符串插值
来源：http://ja.yuntaijiaju.cn

"值: \(b)"
来源：http://fu.yuntaijiaju.cn

[T19] Swift：可选绑定
来源：http://li.jctech888.com.cn

if let n = opt { print(n) }
来源：http://rw.bjjhwx.cn

[T20] Swift：数组操作
来源：http://nf.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ia.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://vk.shxzskj.cn

for x in a { print(x) }
来源：http://at.9csxet.cn

[T22] Swift：字典
来源：http://ko.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xf.yuntaijiaju.cn

[T23] Swift：函数
来源：http://zs.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kv.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://ei.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rg.jctech888.com.cn

[T25] Swift：结构体
来源：http://eb.bjjhwx.cn

struct P { var x: Int }
来源：http://xd.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://fe.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://op.panjiajie.cn

[T27] Swift：错误处理
来源：http://oh.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://qf.muxihuayi.cn

[T28] Swift：枚举
来源：http://cd.jianghongdianzi.cn

enum Color { case red, green }
来源：http://eq.nicolike.cn

[T29] Swift：guard 提前返回
来源：http://hy.bjjhwx.cn

guard let x = opt else { return }
来源：http://mr.shxzukj.cn

[T30] Swift：协议
来源：http://ev.colortex.cn

protocol Shape { func area() -> Double }
来源：http://ce.shxzukj.cn


<!-- 参考信息 -->