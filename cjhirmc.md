代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ze.nszjky.cn

[R24] 大小写转换
来源：http://cp.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lg.panjiajie.cn

[R25] 去后缀 / 去前缀
来源：http://zl.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ka.huixiangedu.cn

[R26] 命令替换
来源：http://yt.yuntaijiaju.cn

now=$(date +%F); echo "$now"
来源：http://zn.szxytkj.cn

[R27] 算术展开
来源：http://ke.szsharing.cn

echo $((1 + 2 * 3))
来源：http://ub.panjiajie.cn

[R28] 浮点运算
来源：http://xo.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://ev.szxytkj.cn

[R29] 定义函数
来源：http://lq.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iz.chemitech.net.cn

[R30] 函数返回状态码
来源：http://af.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://vl.hnjuh.cn

[R31] 局部变量
来源：http://ac.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://fu.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://ls.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zv.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://mk.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pu.huanxung.cn

[R34] 退出时清理
来源：http://yu.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rt.nszjky.cn

[R35] 后台执行并等待
来源：http://ul.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qi.hnjuh.cn

[R36] 并发执行多个任务
来源：http://xn.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xd.newstarts.cn

[R37] 把输出赋给变量
来源：http://ud.yuntaijiaju.cn

files=$(ls -1)
来源：http://qm.haigaiapp.cn

[R38] 管道串联
来源：http://pm.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://dl.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://bh.huanxung.cn

cmd > out.log 2>&1
来源：http://uw.szxytkj.cn

[R40] 追加写日志
来源：http://oh.szsharing.cn

echo "log" >> out.log
来源：http://ne.shtwfgs.cn

[R41] 丢弃输出
来源：http://ah.asd995.cn

cmd >/dev/null 2>&1
来源：http://to.muxihuayi.cn

[R42] 输入重定向
来源：http://ni.jianghongdianzi.cn

wc -l < a.txt
来源：http://oo.shxzskj.cn

[R43] 按名字查找文件
来源：http://ea.gzmigu.cn

find . -name "*.log" -type f
来源：http://cx.wgjwhj.cn

[R44] 按修改时间查找
来源：http://jf.asd995.cn

find . -mtime -7 -type f
来源：http://jz.yuntaijiaju.cn

[R45] 批量删除
来源：http://js.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://ez.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://kw.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mo.shtwfgs.cn

[R47] sed 单行替换
来源：http://jx.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nj.yuexingan06.cn

[R48] awk 取指定列
来源：http://zg.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://cx.jianghongdianzi.cn

[R49] awk 带条件
来源：http://kl.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wt.hnjuh.cn

[R50] awk 求和
来源：http://gh.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vj.colortex.cn

[R51] 排序去重取前几
来源：http://zu.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://db.yuntaijiaju.cn

[R52] 统计行数
来源：http://bs.bjjhwx.cn

wc -l a.txt
来源：http://bo.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://tn.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ih.huixiangedu.cn

[R54] 比较两个文件
来源：http://cc.bookmarksfly.cn

diff a.txt b.txt
来源：http://uu.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://ok.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ol.jctech888.com.cn

[R56] 远程拷贝
来源：http://xs.yuexingan06.cn

scp file user@host:/path/
来源：http://tg.huixinmuqiang.cn

[R57] 远程执行命令
来源：http://tt.gzmigu.cn

ssh user@host 'uptime'
来源：http://eq.bookmarksfly.cn

[R58] 下载文件
来源：http://my.colortex.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ex.huixiangedu.cn

[R59] 发 POST JSON
来源：http://be.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://je.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://wl.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bj.panjiajie.cn

[R61] 磁盘占用
来源：http://fy.colortex.cn

df -h;  du -sh *
来源：http://xf.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://nz.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://oa.shxzukj.cn

[R63] 内存与进程
来源：http://ej.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://nv.chemitech.net.cn

[R64] 结束进程
来源：http://rk.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://wa.newstarts.cn

[R65] 查看端口占用
来源：http://ut.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xm.jctech888.com.cn

[R66] 定时任务
来源：http://jv.newstarts.cn

crontab -e;  crontab -l
来源：http://wg.newstarts.cn

[R67] 生成随机十六进制串
来源：http://ct.szsharing.cn

openssl rand -hex 16
来源：http://dx.bjjhwx.cn

[R68] 计算文件校验值
来源：http://zp.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rd.lnxyls.cn

[R69] 生成随机密码
来源：http://uf.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://vl.asd995.cn

[R70] 时间戳与互转
来源：http://kt.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://xk.shtwfgs.cn

[R71] 日期格式化
来源：http://nw.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vk.521024.cn

[R72] 等待端口就绪
来源：http://ps.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mf.newstarts.cn

[R73] 分割大日志
来源：http://mv.shxzukj.cn

split -l 1000 big.log part_
来源：http://km.yuexingan06.cn

[R74] 批量重命名
来源：http://by.gzmigu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nq.szxytkj.cn

[R75] 导出环境变量
来源：http://sk.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://bp.gzmigu.cn

[R76] 使用临时文件
来源：http://ir.asd995.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bf.lnxyls.cn

[R77] 读取用户输入
来源：http://tm.yuntaijiaju.cn

read -rp "请输入: " ans
来源：http://fu.nszjky.cn

[R78] 交互式菜单
来源：http://kk.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jp.521024.cn

[R79] 解析命令行选项
来源：http://yo.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://er.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://fm.huanxung.cn

time ./run.sh
来源：http://bn.bookmarksfly.cn

================================================================================
来源：http://py.asd995.cn

S. C / C++ 专题
来源：http://di.shxzukj.cn

================================================================================
来源：http://ee.jianghongdianzi.cn

[S01] C：Hello World
来源：http://sn.colortex.cn

#include <stdio.h>
来源：http://ho.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cz.9csxet.cn

[S02] C：变量与格式化输出
来源：http://sr.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://xj.shxzukj.cn

[S03] C：读入整数
来源：http://uv.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://rx.yuexingan06.cn

[S04] C：字符串复制
来源：http://tv.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ex.nszjky.cn

[S05] C：字符串长度
来源：http://za.huixinmuqiang.cn

strlen(s)
来源：http://lf.huixiangedu.cn

[S06] C：字符串比较
来源：http://fs.panjiajie.cn

strcmp(a, b) == 0
来源：http://ej.nszjky.cn

[S07] C：数组遍历求和
来源：http://in.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ye.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://tl.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ws.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://ra.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ms.chemitech.net.cn

[S10] C：指针与解引用
来源：http://wr.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://kw.huixiangedu.cn

[S11] C：逐行读文件
来源：http://qu.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://mg.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yl.szxytkj.cn

fclose(f);
来源：http://pi.yuntaijiaju.cn

[S12] C：写文件
来源：http://wr.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lb.chemitech.net.cn

[S13] C：宏定义
来源：http://cp.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bm.gzmigu.cn

[S14] C：枚举
来源：http://qh.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://nx.newstarts.cn

[S15] C：类型转换
来源：http://aw.wgjwhj.cn

(double) a / b
来源：http://ic.chemitech.net.cn

[S16] C：位操作置位
来源：http://bp.szxytkj.cn

x |= (1 << 3);
来源：http://gw.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://si.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xo.muxihuayi.cn

[S18] C：命令行参数
来源：http://tj.shxzukj.cn

int main(int argc, char **argv)
来源：http://od.muxihuayi.cn

[S19] C：快速排序
来源：http://gd.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zr.chemitech.net.cn

[S20] C：二分查找
来源：http://tw.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wq.wgjwhj.cn

[S21] C：字符类别判断
来源：http://rj.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hm.gzmigu.cn

[S22] C：字符串转数字
来源：http://hq.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xf.shxzskj.cn

[S23] C：随机数
来源：http://yd.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kl.wgjwhj.cn

[S24] C：获取本地时间
来源：http://eo.chemitech.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wg.asd995.cn

[S25] C：内存拷贝
来源：http://zm.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://se.szsharing.cn

[S26] C：内存清零
来源：http://oz.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://em.bookmarksfly.cn

[S27] C：定义常量
来源：http://rh.shxzukj.cn

const double PI = 3.14159;
来源：http://lo.shtwfgs.cn

[S28] C：静态变量
来源：http://eo.newstarts.cn

static int counter = 0;
来源：http://im.chemitech.net.cn

[S29] C：变参函数
来源：http://uq.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ez.bookmarksfly.cn

[S30] C：头文件保护
来源：http://er.huixiangedu.cn

#ifndef X_H
来源：http://wo.nszjky.cn

#define X_H
来源：http://ez.nicolike.cn

#endif
来源：http://jm.colortex.cn

[S31] C++：Hello World
来源：http://id.asd995.cn

#include <iostream>
来源：http://ts.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://lz.bjjhwx.cn

[S32] C++：字符串
来源：http://yn.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://qn.hahajie.cn

[S33] C++：vector 增删
来源：http://tu.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jq.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://uj.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://vn.haigaiapp.cn

[S35] C++：map
来源：http://uc.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tw.521024.cn

[S36] C++：unordered_map
来源：http://dv.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bo.colortex.cn

[S37] C++：set
来源：http://ny.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fo.521024.cn

[S38] C++：排序
来源：http://cg.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://rr.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://dk.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dx.wgjwhj.cn

[S40] C++：查找元素
来源：http://az.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tc.newstarts.cn

[S41] C++：类与构造函数
来源：http://kc.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://js.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://ur.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://ws.szsharing.cn

[S43] C++：智能指针
来源：http://zg.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://ky.jctech888.com.cn

[S44] C++：引用传参
来源：http://ja.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://za.panjiajie.cn

[S45] C++：lambda
来源：http://at.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://un.hnjuh.cn

[S46] C++：函数模板
来源：http://al.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cl.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://jt.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ab.haigaiapp.cn

[S48] C++：逐行读文件
来源：http://wg.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tz.newstarts.cn

while (std::getline(in, line)) { }
来源：http://se.nicolike.cn

[S49] C++：写文件
来源：http://iz.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bw.hahajie.cn

[S50] C++：格式化数字
来源：http://jv.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xz.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://yb.chemitech.net.cn

static_cast<double>(a) / b
来源：http://wy.asd995.cn

[S52] C++：const 与 noexcept
来源：http://uv.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://pp.9csxet.cn

[S53] C++：移动语义
来源：http://pb.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://nk.hnjuh.cn

[S54] C++：异常处理
来源：http://og.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ne.huanxung.cn

[S55] C++：结构化绑定
来源：http://qe.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ba.asd995.cn

[S56] C++：optional
来源：http://lj.9csxet.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kp.gzmigu.cn

[S57] C++：编译期常量
来源：http://rf.521024.cn

constexpr int N = 10;
来源：http://xo.wgjwhj.cn

[S58] C++：命名空间
来源：http://xr.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://sk.asd995.cn

[S59] C++：静态断言
来源：http://na.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cx.colortex.cn

[S60] C++：遍历并删除元素
来源：http://xl.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://in.haigaiapp.cn

================================================================================
来源：http://xv.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://at.huanxung.cn

================================================================================
来源：http://cz.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://gt.nszjky.cn

println("Hello")
来源：http://om.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://to.gzmigu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yl.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://bl.jctech888.com.cn

"值: $b"
来源：http://qv.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://yb.shxzukj.cn

val n: String? = null;  n?.length
来源：http://vx.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://hl.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lh.shxzukj.cn

[T06] Kotlin：集合映射
来源：http://xl.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bc.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://jn.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ub.huanxung.cn

[T08] Kotlin：数据类
来源：http://el.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://ts.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://ue.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://et.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://dk.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kq.panjiajie.cn

[T11] Kotlin：协程
来源：http://cv.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ux.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://mj.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://pd.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://ak.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://ug.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://if.szsharing.cn

for (i in 1..10) println(i)
来源：http://gw.shxzukj.cn

[T15] Kotlin：接口
来源：http://pt.newstarts.cn

interface Shape { fun area(): Double }
来源：http://dm.panjiajie.cn

[T16] Swift：Hello World
来源：http://pa.bookmarksfly.cn

print("Hello")
来源：http://mq.shxzukj.cn

[T17] Swift：变量与常量
来源：http://jm.bjjhwx.cn

var a = 1;  let b = 2
来源：http://sg.wgjwhj.cn

[T18] Swift：字符串插值
来源：http://pi.wgjwhj.cn

"值: \(b)"
来源：http://oz.newstarts.cn

[T19] Swift：可选绑定
来源：http://la.lnxyls.cn

if let n = opt { print(n) }
来源：http://pa.asd995.cn

[T20] Swift：数组操作
来源：http://tl.wgjwhj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tx.asd995.cn

[T21] Swift：遍历
来源：http://er.shxzskj.cn

for x in a { print(x) }
来源：http://rc.521024.cn

[T22] Swift：字典
来源：http://fx.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ek.szsharing.cn

[T23] Swift：函数
来源：http://jr.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vz.yuexingan06.cn

[T24] Swift：闭包
来源：http://pe.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fm.szsharing.cn

[T25] Swift：结构体
来源：http://zd.chemitech.net.cn

struct P { var x: Int }
来源：http://it.szsharing.cn

[T26] Swift：类与重写
来源：http://un.szxytkj.cn

class A: Base { override func f() {} }
来源：http://vt.newstarts.cn


<!-- 参考信息 -->