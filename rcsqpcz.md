代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://dg.yuexingan06.cn

[R26] 命令替换
来源：http://nb.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://jx.hnjuh.cn

[R27] 算术展开
来源：http://au.newstarts.cn

echo $((1 + 2 * 3))
来源：http://rs.colortex.cn

[R28] 浮点运算
来源：http://au.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://gz.jctech888.com.cn

[R29] 定义函数
来源：http://je.yuexingan06.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ke.wgjwhj.cn

[R30] 函数返回状态码
来源：http://ef.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://sw.shxzskj.cn

[R31] 局部变量
来源：http://ke.521024.cn

f() { local x=1; echo "$x"; }
来源：http://uv.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://nc.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sj.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://mi.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mp.nicolike.cn

[R34] 退出时清理
来源：http://th.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vo.asd995.cn

[R35] 后台执行并等待
来源：http://wa.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://iq.521024.cn

[R36] 并发执行多个任务
来源：http://rd.shxzskj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rd.521024.cn

[R37] 把输出赋给变量
来源：http://ug.panjiajie.cn

files=$(ls -1)
来源：http://js.colortex.cn

[R38] 管道串联
来源：http://gs.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://gu.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://gf.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://so.nicolike.cn

[R40] 追加写日志
来源：http://xg.gzmigu.cn

echo "log" >> out.log
来源：http://xd.szsharing.cn

[R41] 丢弃输出
来源：http://um.nicolike.cn

cmd >/dev/null 2>&1
来源：http://fp.9csxet.cn

[R42] 输入重定向
来源：http://yo.jctech888.com.cn

wc -l < a.txt
来源：http://wr.muxihuayi.cn

[R43] 按名字查找文件
来源：http://th.asd995.cn

find . -name "*.log" -type f
来源：http://mm.jctech888.com.cn

[R44] 按修改时间查找
来源：http://do.hnjuh.cn

find . -mtime -7 -type f
来源：http://jw.asd995.cn

[R45] 批量删除
来源：http://my.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://kn.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://bm.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rm.newstarts.cn

[R47] sed 单行替换
来源：http://bs.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xy.huanxung.cn

[R48] awk 取指定列
来源：http://as.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://rp.haigaiapp.cn

[R49] awk 带条件
来源：http://bo.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kd.colortex.cn

[R50] awk 求和
来源：http://pk.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ow.bjjhwx.cn

[R51] 排序去重取前几
来源：http://pp.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sf.yuexingan06.cn

[R52] 统计行数
来源：http://dc.panjiajie.cn

wc -l a.txt
来源：http://ap.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://ah.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uh.hahajie.cn

[R54] 比较两个文件
来源：http://rj.jctech888.com.cn

diff a.txt b.txt
来源：http://hp.521024.cn

[R55] 压缩与解压
来源：http://qd.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ww.jctech888.com.cn

[R56] 远程拷贝
来源：http://rn.szxytkj.cn

scp file user@host:/path/
来源：http://ci.panjiajie.cn

[R57] 远程执行命令
来源：http://zi.asd995.cn

ssh user@host 'uptime'
来源：http://ec.huixiangedu.cn

[R58] 下载文件
来源：http://mt.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zl.shtwfgs.cn

[R59] 发 POST JSON
来源：http://cp.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yq.huixiangedu.cn

[R60] 只看 HTTP 状态码
来源：http://ol.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wl.hahajie.cn

[R61] 磁盘占用
来源：http://kz.nicolike.cn

df -h;  du -sh *
来源：http://kq.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://fq.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://ey.bjjhwx.cn

[R63] 内存与进程
来源：http://yt.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://zu.hnjuh.cn

[R64] 结束进程
来源：http://ou.lnxyls.cn

kill -9 $(pgrep -f app.py)
来源：http://an.asd995.cn

[R65] 查看端口占用
来源：http://xl.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hh.chemitech.net.cn

[R66] 定时任务
来源：http://fw.gzmigu.cn

crontab -e;  crontab -l
来源：http://do.huanxung.cn

[R67] 生成随机十六进制串
来源：http://mm.asd995.cn

openssl rand -hex 16
来源：http://qx.shxzukj.cn

[R68] 计算文件校验值
来源：http://nb.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jr.hahajie.cn

[R69] 生成随机密码
来源：http://po.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://ww.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://sh.asd995.cn

date +%s;  date -d @1700000000
来源：http://xf.shtwfgs.cn

[R71] 日期格式化
来源：http://wx.nszjky.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ka.haigaiapp.cn

[R72] 等待端口就绪
来源：http://ao.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kc.9csxet.cn

[R73] 分割大日志
来源：http://aa.shxzukj.cn

split -l 1000 big.log part_
来源：http://bj.szxytkj.cn

[R74] 批量重命名
来源：http://pa.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ci.colortex.cn

[R75] 导出环境变量
来源：http://tm.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://ij.bookmarksfly.cn

[R76] 使用临时文件
来源：http://ma.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yw.bookmarksfly.cn

[R77] 读取用户输入
来源：http://cp.newstarts.cn

read -rp "请输入: " ans
来源：http://td.panjiajie.cn

[R78] 交互式菜单
来源：http://lw.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mn.szxytkj.cn

[R79] 解析命令行选项
来源：http://rr.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rt.wgjwhj.cn

[R80] 查看脚本执行耗时
来源：http://dp.szsharing.cn

time ./run.sh
来源：http://zg.9csxet.cn

================================================================================
来源：http://sv.9csxet.cn

S. C / C++ 专题
来源：http://wy.asd995.cn

================================================================================
来源：http://jj.huanxung.cn

[S01] C：Hello World
来源：http://ex.hnjuh.cn

#include <stdio.h>
来源：http://ad.jianghongdianzi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bv.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://ek.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://vd.shxzukj.cn

[S03] C：读入整数
来源：http://og.asd995.cn

int x; scanf("%d", &x);
来源：http://dv.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://jo.panjiajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ng.szxytkj.cn

[S05] C：字符串长度
来源：http://nl.szsharing.cn

strlen(s)
来源：http://hu.muxihuayi.cn

[S06] C：字符串比较
来源：http://lu.nszjky.cn

strcmp(a, b) == 0
来源：http://xe.hnjuh.cn

[S07] C：数组遍历求和
来源：http://tb.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ci.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://li.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tf.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://at.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vq.bjjhwx.cn

[S10] C：指针与解引用
来源：http://ps.newstarts.cn

int *p = &a;  *p = 5;
来源：http://nw.colortex.cn

[S11] C：逐行读文件
来源：http://qz.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://yd.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yg.nszjky.cn

fclose(f);
来源：http://mm.wgjwhj.cn

[S12] C：写文件
来源：http://ta.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://du.9csxet.cn

[S13] C：宏定义
来源：http://vb.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xr.9csxet.cn

[S14] C：枚举
来源：http://wd.huanxung.cn

enum Color { RED, GREEN, BLUE };
来源：http://er.chemitech.net.cn

[S15] C：类型转换
来源：http://rc.newstarts.cn

(double) a / b
来源：http://bq.asd995.cn

[S16] C：位操作置位
来源：http://bz.hahajie.cn

x |= (1 << 3);
来源：http://yk.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://di.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://im.hnjuh.cn

[S18] C：命令行参数
来源：http://vk.gzmigu.cn

int main(int argc, char **argv)
来源：http://qj.haigaiapp.cn

[S19] C：快速排序
来源：http://ja.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tb.bjjhwx.cn

[S20] C：二分查找
来源：http://rf.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pf.nicolike.cn

[S21] C：字符类别判断
来源：http://gl.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gf.huanxung.cn

[S22] C：字符串转数字
来源：http://ta.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://go.9csxet.cn

[S23] C：随机数
来源：http://ch.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zm.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://rt.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xs.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://mi.wgjwhj.cn

memcpy(dst, src, n);
来源：http://la.chemitech.net.cn

[S26] C：内存清零
来源：http://wn.nszjky.cn

memset(a, 0, sizeof a);
来源：http://pa.9csxet.cn

[S27] C：定义常量
来源：http://xg.gzmigu.cn

const double PI = 3.14159;
来源：http://qq.asd995.cn

[S28] C：静态变量
来源：http://ia.shxzskj.cn

static int counter = 0;
来源：http://lf.gzmigu.cn

[S29] C：变参函数
来源：http://br.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ur.panjiajie.cn

[S30] C：头文件保护
来源：http://db.newstarts.cn

#ifndef X_H
来源：http://js.muxihuayi.cn

#define X_H
来源：http://nd.nicolike.cn

#endif
来源：http://xr.wgjwhj.cn

[S31] C++：Hello World
来源：http://lo.asd995.cn

#include <iostream>
来源：http://go.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://vb.szsharing.cn

[S32] C++：字符串
来源：http://cy.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://ws.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://gm.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vs.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://hl.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://vj.colortex.cn

[S35] C++：map
来源：http://bu.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bs.yuexingan06.cn

[S36] C++：unordered_map
来源：http://tj.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bz.jctech888.com.cn

[S37] C++：set
来源：http://rg.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qz.szsharing.cn

[S38] C++：排序
来源：http://fm.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://qi.521024.cn

[S39] C++：自定义比较器排序
来源：http://fz.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hj.jctech888.com.cn

[S40] C++：查找元素
来源：http://gw.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://md.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://tt.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gv.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://cn.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://kj.nicolike.cn

[S43] C++：智能指针
来源：http://hn.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://tv.muxihuayi.cn

[S44] C++：引用传参
来源：http://ix.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://ib.yuexingan06.cn

[S45] C++：lambda
来源：http://bv.hahajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bm.huixiangedu.cn

[S46] C++：函数模板
来源：http://bb.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wh.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://ga.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kx.panjiajie.cn

[S48] C++：逐行读文件
来源：http://la.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fy.hahajie.cn

while (std::getline(in, line)) { }
来源：http://kk.huixiangedu.cn

[S49] C++：写文件
来源：http://lc.huixinmuqiang.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cu.jctech888.com.cn

[S50] C++：格式化数字
来源：http://zf.shtwfgs.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eq.shxzskj.cn

[S51] C++：显式类型转换
来源：http://tg.newstarts.cn

static_cast<double>(a) / b
来源：http://hb.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://iw.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://yv.shxzukj.cn

[S53] C++：移动语义
来源：http://sj.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://ne.bookmarksfly.cn

[S54] C++：异常处理
来源：http://kz.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zm.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://oc.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ee.huixiangedu.cn

[S56] C++：optional
来源：http://qd.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://js.szsharing.cn

[S57] C++：编译期常量
来源：http://mq.huixiangedu.cn

constexpr int N = 10;
来源：http://fb.nicolike.cn

[S58] C++：命名空间
来源：http://tj.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://nz.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://sh.huixiangedu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uz.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://hh.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eg.szsharing.cn

================================================================================
来源：http://lg.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ae.jctech888.com.cn

================================================================================
来源：http://hf.huanxung.cn

[T01] Kotlin：Hello World
来源：http://xq.huixinmuqiang.cn

println("Hello")
来源：http://yw.muxihuayi.cn

[T02] Kotlin：变量
来源：http://pd.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://un.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://el.jctech888.com.cn

"值: $b"
来源：http://kr.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://qy.huanxung.cn

val n: String? = null;  n?.length
来源：http://vp.9csxet.cn

[T05] Kotlin：when 表达式
来源：http://ad.wgjwhj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tl.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://oc.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sl.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://om.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qc.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://jy.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://dl.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://xn.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://ps.521024.cn

[T10] Kotlin：默认参数
来源：http://ye.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lp.asd995.cn

[T11] Kotlin：协程
来源：http://ys.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://du.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://bg.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://lx.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://jz.huanxung.cn

val m = mapOf("a" to 1)
来源：http://bh.panjiajie.cn

[T14] Kotlin：循环
来源：http://ie.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://vb.hnjuh.cn

[T15] Kotlin：接口
来源：http://ov.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://lv.lnxyls.cn

[T16] Swift：Hello World
来源：http://yl.haigaiapp.cn

print("Hello")
来源：http://xz.huanxung.cn

[T17] Swift：变量与常量
来源：http://aa.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://rj.hnjuh.cn

[T18] Swift：字符串插值
来源：http://zk.newstarts.cn

"值: \(b)"
来源：http://qp.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://bx.gzmigu.cn

if let n = opt { print(n) }
来源：http://lg.huixiangedu.cn

[T20] Swift：数组操作
来源：http://kg.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ia.panjiajie.cn

[T21] Swift：遍历
来源：http://wu.huixiangedu.cn

for x in a { print(x) }
来源：http://wl.yuexingan06.cn

[T22] Swift：字典
来源：http://tp.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sz.chemitech.net.cn

[T23] Swift：函数
来源：http://bd.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://me.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://kr.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ms.colortex.cn

[T25] Swift：结构体
来源：http://dq.panjiajie.cn

struct P { var x: Int }
来源：http://tt.panjiajie.cn

[T26] Swift：类与重写
来源：http://mv.newstarts.cn

class A: Base { override func f() {} }
来源：http://sd.521024.cn

[T27] Swift：错误处理
来源：http://mf.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://yf.gzmigu.cn

[T28] Swift：枚举
来源：http://oo.bjjhwx.cn

enum Color { case red, green }
来源：http://gm.shxzukj.cn


<!-- 参考信息 -->