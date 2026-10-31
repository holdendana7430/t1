代发 wailian999

echo "${#s}"
来源：http://yi.huanxung.cn

[R22] 截取子串
来源：http://df.szxytkj.cn

echo "${s:0:5}"
来源：http://xw.9csxet.cn

[R23] 字符串替换
来源：http://zr.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ju.panjiajie.cn

[R24] 大小写转换
来源：http://ff.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rp.bjjhwx.cn

[R25] 去后缀 / 去前缀
来源：http://kb.wgjwhj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qr.yuexingan06.cn

[R26] 命令替换
来源：http://ml.asd995.cn

now=$(date +%F); echo "$now"
来源：http://na.shtwfgs.cn

[R27] 算术展开
来源：http://ou.huanxung.cn

echo $((1 + 2 * 3))
来源：http://du.panjiajie.cn

[R28] 浮点运算
来源：http://fq.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://da.yuntaijiaju.cn

[R29] 定义函数
来源：http://eh.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jo.shxzukj.cn

[R30] 函数返回状态码
来源：http://na.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://xf.jctech888.com.cn

[R31] 局部变量
来源：http://vr.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://tr.bookmarksfly.cn

[R32] 参数个数校验
来源：http://oi.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ag.muxihuayi.cn

[R33] 捕获错误并提示行号
来源：http://gg.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uv.nicolike.cn

[R34] 退出时清理
来源：http://ho.huixinmuqiang.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zr.asd995.cn

[R35] 后台执行并等待
来源：http://cw.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://eu.shxzukj.cn

[R36] 并发执行多个任务
来源：http://hl.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cf.hnjuh.cn

[R37] 把输出赋给变量
来源：http://zl.asd995.cn

files=$(ls -1)
来源：http://it.szsharing.cn

[R38] 管道串联
来源：http://bz.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://pj.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://eq.wgjwhj.cn

cmd > out.log 2>&1
来源：http://ef.asd995.cn

[R40] 追加写日志
来源：http://ml.bjjhwx.cn

echo "log" >> out.log
来源：http://ei.9csxet.cn

[R41] 丢弃输出
来源：http://ma.9csxet.cn

cmd >/dev/null 2>&1
来源：http://yf.bookmarksfly.cn

[R42] 输入重定向
来源：http://kn.lnxyls.cn

wc -l < a.txt
来源：http://gf.shtwfgs.cn

[R43] 按名字查找文件
来源：http://tl.yuexingan06.cn

find . -name "*.log" -type f
来源：http://yl.shtwfgs.cn

[R44] 按修改时间查找
来源：http://qi.panjiajie.cn

find . -mtime -7 -type f
来源：http://jj.lnxyls.cn

[R45] 批量删除
来源：http://ef.jianghongdianzi.cn

find . -name "*.tmp" -delete
来源：http://qz.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://lk.muxihuayi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://st.colortex.cn

[R47] sed 单行替换
来源：http://rn.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ep.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://hw.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://lv.jianghongdianzi.cn

[R49] awk 带条件
来源：http://oq.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xy.shxzukj.cn

[R50] awk 求和
来源：http://sl.bjjhwx.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dz.shxzskj.cn

[R51] 排序去重取前几
来源：http://ov.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://be.huanxung.cn

[R52] 统计行数
来源：http://tr.panjiajie.cn

wc -l a.txt
来源：http://aw.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://fx.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pj.nszjky.cn

[R54] 比较两个文件
来源：http://jc.521024.cn

diff a.txt b.txt
来源：http://xk.shxzukj.cn

[R55] 压缩与解压
来源：http://wm.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vy.521024.cn

[R56] 远程拷贝
来源：http://yt.shxzskj.cn

scp file user@host:/path/
来源：http://lt.asd995.cn

[R57] 远程执行命令
来源：http://pd.hahajie.cn

ssh user@host 'uptime'
来源：http://sr.szxytkj.cn

[R58] 下载文件
来源：http://vi.colortex.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yh.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://vn.haigaiapp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sv.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://rf.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rf.9csxet.cn

[R61] 磁盘占用
来源：http://au.521024.cn

df -h;  du -sh *
来源：http://bc.hnjuh.cn

[R62] 找最占空间的文件
来源：http://iq.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://wm.bjjhwx.cn

[R63] 内存与进程
来源：http://ha.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://pm.shtwfgs.cn

[R64] 结束进程
来源：http://bn.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://rj.asd995.cn

[R65] 查看端口占用
来源：http://ho.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sa.panjiajie.cn

[R66] 定时任务
来源：http://xr.muxihuayi.cn

crontab -e;  crontab -l
来源：http://fb.521024.cn

[R67] 生成随机十六进制串
来源：http://dh.chemitech.net.cn

openssl rand -hex 16
来源：http://wt.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://cc.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gn.asd995.cn

[R69] 生成随机密码
来源：http://os.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://dc.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://ch.colortex.cn

date +%s;  date -d @1700000000
来源：http://ra.muxihuayi.cn

[R71] 日期格式化
来源：http://os.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gy.szxytkj.cn

[R72] 等待端口就绪
来源：http://ov.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ry.colortex.cn

[R73] 分割大日志
来源：http://eb.colortex.cn

split -l 1000 big.log part_
来源：http://az.gzmigu.cn

[R74] 批量重命名
来源：http://vz.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nz.bookmarksfly.cn

[R75] 导出环境变量
来源：http://uo.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://xu.lnxyls.cn

[R76] 使用临时文件
来源：http://jg.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://da.bjjhwx.cn

[R77] 读取用户输入
来源：http://cz.colortex.cn

read -rp "请输入: " ans
来源：http://ct.gzmigu.cn

[R78] 交互式菜单
来源：http://uz.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sh.newstarts.cn

[R79] 解析命令行选项
来源：http://qh.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ci.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://wd.huixiangedu.cn

time ./run.sh
来源：http://xh.nszjky.cn

================================================================================
来源：http://to.hahajie.cn

S. C / C++ 专题
来源：http://se.huixiangedu.cn

================================================================================
来源：http://vg.newstarts.cn

[S01] C：Hello World
来源：http://kf.muxihuayi.cn

#include <stdio.h>
来源：http://di.panjiajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://li.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://lv.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://gz.shxzskj.cn

[S03] C：读入整数
来源：http://ij.hahajie.cn

int x; scanf("%d", &x);
来源：http://px.colortex.cn

[S04] C：字符串复制
来源：http://nl.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://da.yuexingan06.cn

[S05] C：字符串长度
来源：http://en.huixinmuqiang.cn

strlen(s)
来源：http://wh.wgjwhj.cn

[S06] C：字符串比较
来源：http://ib.bjjhwx.cn

strcmp(a, b) == 0
来源：http://pk.newstarts.cn

[S07] C：数组遍历求和
来源：http://hr.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://md.9csxet.cn

[S08] C：动态内存分配与释放
来源：http://tp.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dk.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://mx.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://re.9csxet.cn

[S10] C：指针与解引用
来源：http://ml.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://jv.haigaiapp.cn

[S11] C：逐行读文件
来源：http://pa.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://xq.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://oj.szxytkj.cn

fclose(f);
来源：http://zf.huanxung.cn

[S12] C：写文件
来源：http://dx.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tt.shxzskj.cn

[S13] C：宏定义
来源：http://yi.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oi.panjiajie.cn

[S14] C：枚举
来源：http://hb.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://ah.bjjhwx.cn

[S15] C：类型转换
来源：http://ko.haigaiapp.cn

(double) a / b
来源：http://yk.yuexingan06.cn

[S16] C：位操作置位
来源：http://dv.panjiajie.cn

x |= (1 << 3);
来源：http://bi.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://kq.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://un.hnjuh.cn

[S18] C：命令行参数
来源：http://uc.szxytkj.cn

int main(int argc, char **argv)
来源：http://sx.huixinmuqiang.cn

[S19] C：快速排序
来源：http://ip.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iz.521024.cn

[S20] C：二分查找
来源：http://qu.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ov.huanxung.cn

[S21] C：字符类别判断
来源：http://sn.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wu.nicolike.cn

[S22] C：字符串转数字
来源：http://tz.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zk.shxzukj.cn

[S23] C：随机数
来源：http://wq.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hf.shxzukj.cn

[S24] C：获取本地时间
来源：http://nc.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yu.nicolike.cn

[S25] C：内存拷贝
来源：http://ou.newstarts.cn

memcpy(dst, src, n);
来源：http://jl.huixiangedu.cn

[S26] C：内存清零
来源：http://gv.huanxung.cn

memset(a, 0, sizeof a);
来源：http://gf.newstarts.cn

[S27] C：定义常量
来源：http://pg.nszjky.cn

const double PI = 3.14159;
来源：http://sv.shtwfgs.cn

[S28] C：静态变量
来源：http://uh.huixiangedu.cn

static int counter = 0;
来源：http://gn.huixiangedu.cn

[S29] C：变参函数
来源：http://ic.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fn.colortex.cn

[S30] C：头文件保护
来源：http://tp.jctech888.com.cn

#ifndef X_H
来源：http://bx.shxzukj.cn

#define X_H
来源：http://bx.asd995.cn

#endif
来源：http://yb.bjjhwx.cn

[S31] C++：Hello World
来源：http://bq.wgjwhj.cn

#include <iostream>
来源：http://hj.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://ss.521024.cn

[S32] C++：字符串
来源：http://nj.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://ky.chemitech.net.cn

[S33] C++：vector 增删
来源：http://iz.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://es.521024.cn

[S34] C++：遍历 vector
来源：http://ue.szsharing.cn

for (auto &x : v) { std::cout << x; }
来源：http://ku.hahajie.cn

[S35] C++：map
来源：http://ao.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vl.wgjwhj.cn

[S36] C++：unordered_map
来源：http://is.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xv.huixiangedu.cn

[S37] C++：set
来源：http://oe.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ym.nszjky.cn

[S38] C++：排序
来源：http://mj.shxzukj.cn

std::sort(v.begin(), v.end());
来源：http://iu.huixinmuqiang.cn

[S39] C++：自定义比较器排序
来源：http://xe.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dj.newstarts.cn

[S40] C++：查找元素
来源：http://et.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nm.szxytkj.cn

[S41] C++：类与构造函数
来源：http://et.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zp.newstarts.cn

[S42] C++：继承与虚函数
来源：http://cc.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://dr.szsharing.cn

[S43] C++：智能指针
来源：http://hi.huixinmuqiang.cn

auto p = std::make_unique<int>(5);
来源：http://ce.shxzukj.cn

[S44] C++：引用传参
来源：http://gz.lnxyls.cn

void inc(int &x) { ++x; }
来源：http://pf.szsharing.cn

[S45] C++：lambda
来源：http://qv.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kn.lnxyls.cn

[S46] C++：函数模板
来源：http://fq.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sc.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://wu.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xw.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://et.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kw.nszjky.cn

while (std::getline(in, line)) { }
来源：http://xy.shtwfgs.cn

[S49] C++：写文件
来源：http://ir.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ef.bjjhwx.cn

[S50] C++：格式化数字
来源：http://ki.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bo.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://lg.nszjky.cn

static_cast<double>(a) / b
来源：http://lz.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://yd.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://zx.haigaiapp.cn

[S53] C++：移动语义
来源：http://er.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://hx.nszjky.cn

[S54] C++：异常处理
来源：http://mu.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ic.szxytkj.cn

[S55] C++：结构化绑定
来源：http://gc.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qo.bjjhwx.cn

[S56] C++：optional
来源：http://xy.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hl.lnxyls.cn

[S57] C++：编译期常量
来源：http://xj.newstarts.cn

constexpr int N = 10;
来源：http://xu.gzmigu.cn

[S58] C++：命名空间
来源：http://ds.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://zp.521024.cn

[S59] C++：静态断言
来源：http://bm.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xs.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://jf.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://st.newstarts.cn

================================================================================
来源：http://gi.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ve.chemitech.net.cn

================================================================================
来源：http://nq.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://pp.nszjky.cn

println("Hello")
来源：http://cz.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://ki.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yk.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://kn.shtwfgs.cn

"值: $b"
来源：http://ta.huanxung.cn

[T04] Kotlin：空安全
来源：http://pa.szxytkj.cn

val n: String? = null;  n?.length
来源：http://tm.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://nw.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cf.nicolike.cn

[T06] Kotlin：集合映射
来源：http://lm.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oz.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://qf.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zb.shxzukj.cn

[T08] Kotlin：数据类
来源：http://se.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://wq.lnxyls.cn

[T09] Kotlin：扩展函数
来源：http://an.hahajie.cn

fun String.exclaim() = this + "!"
来源：http://rk.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://tm.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rx.521024.cn

[T11] Kotlin：协程
来源：http://hu.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bd.nszjky.cn

[T12] Kotlin：解构声明
来源：http://oo.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://dl.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://yf.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://nn.chemitech.net.cn

[T14] Kotlin：循环
来源：http://rc.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://hg.hnjuh.cn

[T15] Kotlin：接口
来源：http://hx.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://il.521024.cn

[T16] Swift：Hello World
来源：http://qs.huixiangedu.cn

print("Hello")
来源：http://zu.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://zc.9csxet.cn

var a = 1;  let b = 2
来源：http://ev.newstarts.cn

[T18] Swift：字符串插值
来源：http://sc.asd995.cn

"值: \(b)"
来源：http://yb.gzmigu.cn

[T19] Swift：可选绑定
来源：http://zy.szsharing.cn

if let n = opt { print(n) }
来源：http://em.hahajie.cn

[T20] Swift：数组操作
来源：http://cs.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ws.colortex.cn

[T21] Swift：遍历
来源：http://wi.yuexingan06.cn

for x in a { print(x) }
来源：http://kq.colortex.cn

[T22] Swift：字典
来源：http://gb.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hg.jctech888.com.cn

[T23] Swift：函数
来源：http://ro.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sp.szxytkj.cn

[T24] Swift：闭包
来源：http://tn.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ml.szxytkj.cn


<!-- 参考信息 -->