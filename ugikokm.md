代发 wailian999

echo "${#s}"
来源：http://xr.chemitech.net.cn

[R22] 截取子串
来源：http://bc.bookmarksfly.cn

echo "${s:0:5}"
来源：http://zm.nicolike.cn

[R23] 字符串替换
来源：http://qt.huixinmuqiang.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wg.asd995.cn

[R24] 大小写转换
来源：http://nr.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kv.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://nb.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://at.newstarts.cn

[R26] 命令替换
来源：http://ke.colortex.cn

now=$(date +%F); echo "$now"
来源：http://pp.chemitech.net.cn

[R27] 算术展开
来源：http://ic.hnjuh.cn

echo $((1 + 2 * 3))
来源：http://xa.szxytkj.cn

[R28] 浮点运算
来源：http://yk.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://od.muxihuayi.cn

[R29] 定义函数
来源：http://zc.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dl.hahajie.cn

[R30] 函数返回状态码
来源：http://om.bookmarksfly.cn

f() { return 0; }; f || echo "失败了"
来源：http://un.shxzukj.cn

[R31] 局部变量
来源：http://lc.haigaiapp.cn

f() { local x=1; echo "$x"; }
来源：http://uk.haigaiapp.cn

[R32] 参数个数校验
来源：http://wl.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sm.521024.cn

[R33] 捕获错误并提示行号
来源：http://gr.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sg.521024.cn

[R34] 退出时清理
来源：http://mm.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ne.panjiajie.cn

[R35] 后台执行并等待
来源：http://sk.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ta.asd995.cn

[R36] 并发执行多个任务
来源：http://we.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fx.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://oa.hnjuh.cn

files=$(ls -1)
来源：http://rd.huixiangedu.cn

[R38] 管道串联
来源：http://xg.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://an.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://rx.newstarts.cn

cmd > out.log 2>&1
来源：http://bj.lnxyls.cn

[R40] 追加写日志
来源：http://qs.hnjuh.cn

echo "log" >> out.log
来源：http://pn.bjjhwx.cn

[R41] 丢弃输出
来源：http://qz.nicolike.cn

cmd >/dev/null 2>&1
来源：http://tf.huanxung.cn

[R42] 输入重定向
来源：http://vr.hahajie.cn

wc -l < a.txt
来源：http://pk.huixiangedu.cn

[R43] 按名字查找文件
来源：http://ux.muxihuayi.cn

find . -name "*.log" -type f
来源：http://ix.shxzskj.cn

[R44] 按修改时间查找
来源：http://xq.huixinmuqiang.cn

find . -mtime -7 -type f
来源：http://bp.newstarts.cn

[R45] 批量删除
来源：http://wc.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://gy.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://os.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fv.huixiangedu.cn

[R47] sed 单行替换
来源：http://yj.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ce.lnxyls.cn

[R48] awk 取指定列
来源：http://bx.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://rr.521024.cn

[R49] awk 带条件
来源：http://uj.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qx.shxzskj.cn

[R50] awk 求和
来源：http://uj.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hi.bjjhwx.cn

[R51] 排序去重取前几
来源：http://dx.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oz.nszjky.cn

[R52] 统计行数
来源：http://am.newstarts.cn

wc -l a.txt
来源：http://ud.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://rc.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vh.nicolike.cn

[R54] 比较两个文件
来源：http://pc.szsharing.cn

diff a.txt b.txt
来源：http://bg.bookmarksfly.cn

[R55] 压缩与解压
来源：http://he.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uk.chemitech.net.cn

[R56] 远程拷贝
来源：http://be.hahajie.cn

scp file user@host:/path/
来源：http://pt.shxzskj.cn

[R57] 远程执行命令
来源：http://cl.wgjwhj.cn

ssh user@host 'uptime'
来源：http://lt.bookmarksfly.cn

[R58] 下载文件
来源：http://iy.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dx.panjiajie.cn

[R59] 发 POST JSON
来源：http://nc.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://na.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://ar.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://im.shxzskj.cn

[R61] 磁盘占用
来源：http://zo.shtwfgs.cn

df -h;  du -sh *
来源：http://ek.hnjuh.cn

[R62] 找最占空间的文件
来源：http://gi.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://ll.521024.cn

[R63] 内存与进程
来源：http://yx.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://co.huixiangedu.cn

[R64] 结束进程
来源：http://do.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://wh.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://hy.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://md.shxzskj.cn

[R66] 定时任务
来源：http://bo.szsharing.cn

crontab -e;  crontab -l
来源：http://yh.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://dd.asd995.cn

openssl rand -hex 16
来源：http://ts.jctech888.com.cn

[R68] 计算文件校验值
来源：http://ig.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://us.muxihuayi.cn

[R69] 生成随机密码
来源：http://pa.521024.cn

head -c 16 /dev/urandom | base64
来源：http://fi.chemitech.net.cn

[R70] 时间戳与互转
来源：http://hl.hahajie.cn

date +%s;  date -d @1700000000
来源：http://lr.hahajie.cn

[R71] 日期格式化
来源：http://cj.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rp.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://eq.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nu.huixinmuqiang.cn

[R73] 分割大日志
来源：http://ev.9csxet.cn

split -l 1000 big.log part_
来源：http://gg.panjiajie.cn

[R74] 批量重命名
来源：http://zf.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dj.chemitech.net.cn

[R75] 导出环境变量
来源：http://in.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://dv.bookmarksfly.cn

[R76] 使用临时文件
来源：http://gc.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dx.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://sg.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://wh.gzmigu.cn

[R78] 交互式菜单
来源：http://lr.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://un.hahajie.cn

[R79] 解析命令行选项
来源：http://fi.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wm.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://ky.huixinmuqiang.cn

time ./run.sh
来源：http://nw.muxihuayi.cn

================================================================================
来源：http://vn.newstarts.cn

S. C / C++ 专题
来源：http://kj.hahajie.cn

================================================================================
来源：http://eg.panjiajie.cn

[S01] C：Hello World
来源：http://zs.szsharing.cn

#include <stdio.h>
来源：http://ks.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mp.521024.cn

[S02] C：变量与格式化输出
来源：http://hh.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://ls.chemitech.net.cn

[S03] C：读入整数
来源：http://uh.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://wo.newstarts.cn

[S04] C：字符串复制
来源：http://ru.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pq.shxzukj.cn

[S05] C：字符串长度
来源：http://jo.huanxung.cn

strlen(s)
来源：http://nl.huixiangedu.cn

[S06] C：字符串比较
来源：http://zq.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://go.gzmigu.cn

[S07] C：数组遍历求和
来源：http://jl.521024.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lc.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://fu.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bj.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://nj.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ue.shxzukj.cn

[S10] C：指针与解引用
来源：http://tu.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://zq.521024.cn

[S11] C：逐行读文件
来源：http://nx.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://fl.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nh.yuntaijiaju.cn

fclose(f);
来源：http://vq.szxytkj.cn

[S12] C：写文件
来源：http://nz.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fg.jctech888.com.cn

[S13] C：宏定义
来源：http://il.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lf.yuntaijiaju.cn

[S14] C：枚举
来源：http://be.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://uv.9csxet.cn

[S15] C：类型转换
来源：http://lk.shxzukj.cn

(double) a / b
来源：http://lu.szxytkj.cn

[S16] C：位操作置位
来源：http://yu.asd995.cn

x |= (1 << 3);
来源：http://xz.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://py.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eq.huanxung.cn

[S18] C：命令行参数
来源：http://gj.szxytkj.cn

int main(int argc, char **argv)
来源：http://re.szsharing.cn

[S19] C：快速排序
来源：http://cm.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ed.jianghongdianzi.cn

[S20] C：二分查找
来源：http://yu.521024.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jk.huanxung.cn

[S21] C：字符类别判断
来源：http://qp.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iv.shxzukj.cn

[S22] C：字符串转数字
来源：http://ny.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xi.hnjuh.cn

[S23] C：随机数
来源：http://gf.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ls.shxzskj.cn

[S24] C：获取本地时间
来源：http://pf.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mm.huanxung.cn

[S25] C：内存拷贝
来源：http://ig.wgjwhj.cn

memcpy(dst, src, n);
来源：http://qs.szxytkj.cn

[S26] C：内存清零
来源：http://aj.hahajie.cn

memset(a, 0, sizeof a);
来源：http://la.jianghongdianzi.cn

[S27] C：定义常量
来源：http://xf.asd995.cn

const double PI = 3.14159;
来源：http://qf.bjjhwx.cn

[S28] C：静态变量
来源：http://gc.wgjwhj.cn

static int counter = 0;
来源：http://vs.9csxet.cn

[S29] C：变参函数
来源：http://qt.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dn.wgjwhj.cn

[S30] C：头文件保护
来源：http://aj.nszjky.cn

#ifndef X_H
来源：http://ta.yuntaijiaju.cn

#define X_H
来源：http://li.lnxyls.cn

#endif
来源：http://gu.521024.cn

[S31] C++：Hello World
来源：http://hc.asd995.cn

#include <iostream>
来源：http://bp.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://nt.hahajie.cn

[S32] C++：字符串
来源：http://wh.colortex.cn

std::string s = "hi";  s += "!";
来源：http://xz.hahajie.cn

[S33] C++：vector 增删
来源：http://mf.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pe.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://ap.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://eg.panjiajie.cn

[S35] C++：map
来源：http://cj.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ic.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://mc.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kn.huanxung.cn

[S37] C++：set
来源：http://ly.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nx.9csxet.cn

[S38] C++：排序
来源：http://nv.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://zz.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://mm.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dj.colortex.cn

[S40] C++：查找元素
来源：http://dt.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cz.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://oy.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dm.colortex.cn

[S42] C++：继承与虚函数
来源：http://up.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://si.szxytkj.cn

[S43] C++：智能指针
来源：http://se.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://pc.colortex.cn

[S44] C++：引用传参
来源：http://kr.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://ur.jctech888.com.cn

[S45] C++：lambda
来源：http://pk.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vm.hahajie.cn

[S46] C++：函数模板
来源：http://cc.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ul.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://uj.huixiangedu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xt.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://wc.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wn.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://ta.chemitech.net.cn

[S49] C++：写文件
来源：http://fl.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qi.huanxung.cn

[S50] C++：格式化数字
来源：http://ml.huixinmuqiang.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ae.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://go.chemitech.net.cn

static_cast<double>(a) / b
来源：http://aj.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://qo.hahajie.cn

int size() const noexcept { return n_; }
来源：http://hw.muxihuayi.cn

[S53] C++：移动语义
来源：http://dn.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://da.yuexingan06.cn

[S54] C++：异常处理
来源：http://as.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://on.lnxyls.cn

[S55] C++：结构化绑定
来源：http://dx.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kt.huixinmuqiang.cn

[S56] C++：optional
来源：http://ad.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ws.colortex.cn

[S57] C++：编译期常量
来源：http://pt.chemitech.net.cn

constexpr int N = 10;
来源：http://zp.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://cv.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://qt.hnjuh.cn

[S59] C++：静态断言
来源：http://cg.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qr.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://ux.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ra.wgjwhj.cn

================================================================================
来源：http://cr.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uh.huixinmuqiang.cn

================================================================================
来源：http://bt.bjjhwx.cn

[T01] Kotlin：Hello World
来源：http://as.panjiajie.cn

println("Hello")
来源：http://no.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://oh.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://aa.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://aj.yuexingan06.cn

"值: $b"
来源：http://lu.9csxet.cn

[T04] Kotlin：空安全
来源：http://ya.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://gg.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://od.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aq.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://wb.gzmigu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hw.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://oe.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vy.lnxyls.cn

[T08] Kotlin：数据类
来源：http://kd.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://hq.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://hi.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://ih.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://bk.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gl.haigaiapp.cn

[T11] Kotlin：协程
来源：http://sw.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rl.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://ub.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://xw.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://wu.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://wz.jctech888.com.cn

[T14] Kotlin：循环
来源：http://bt.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://dm.hnjuh.cn

[T15] Kotlin：接口
来源：http://um.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://th.nszjky.cn

[T16] Swift：Hello World
来源：http://xm.huixinmuqiang.cn

print("Hello")
来源：http://nd.jctech888.com.cn

[T17] Swift：变量与常量
来源：http://br.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://nx.521024.cn

[T18] Swift：字符串插值
来源：http://an.jianghongdianzi.cn

"值: \(b)"
来源：http://oy.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://jt.shxzukj.cn

if let n = opt { print(n) }
来源：http://fu.huanxung.cn

[T20] Swift：数组操作
来源：http://bw.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dt.nszjky.cn

[T21] Swift：遍历
来源：http://rk.shxzukj.cn

for x in a { print(x) }
来源：http://de.9csxet.cn

[T22] Swift：字典
来源：http://cz.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://va.lnxyls.cn

[T23] Swift：函数
来源：http://so.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qg.wgjwhj.cn

[T24] Swift：闭包
来源：http://jm.hnjuh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yl.yuntaijiaju.cn


<!-- 参考信息 -->