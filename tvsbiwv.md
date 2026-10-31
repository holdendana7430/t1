代发 wailian999

echo "${#arr[@]}"
来源：http://ws.hnjuh.cn

[R20] 关联数组（字典）
来源：http://nn.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nw.nszjky.cn

[R21] 字符串长度
来源：http://rz.lnxyls.cn

echo "${#s}"
来源：http://jo.yuntaijiaju.cn

[R22] 截取子串
来源：http://qp.szxytkj.cn

echo "${s:0:5}"
来源：http://qf.asd995.cn

[R23] 字符串替换
来源：http://dd.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sh.huixiangedu.cn

[R24] 大小写转换
来源：http://mi.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ti.huixinmuqiang.cn

[R25] 去后缀 / 去前缀
来源：http://ww.shtwfgs.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://et.shxzukj.cn

[R26] 命令替换
来源：http://wb.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://vu.colortex.cn

[R27] 算术展开
来源：http://ik.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://ir.haigaiapp.cn

[R28] 浮点运算
来源：http://nz.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://ar.newstarts.cn

[R29] 定义函数
来源：http://he.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wx.bjjhwx.cn

[R30] 函数返回状态码
来源：http://wl.shxzskj.cn

f() { return 0; }; f || echo "失败了"
来源：http://xd.huixinmuqiang.cn

[R31] 局部变量
来源：http://qo.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://xe.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://ay.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://db.yuntaijiaju.cn

[R33] 捕获错误并提示行号
来源：http://lp.asd995.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://aw.hnjuh.cn

[R34] 退出时清理
来源：http://ap.shtwfgs.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fx.huanxung.cn

[R35] 后台执行并等待
来源：http://db.szxytkj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ec.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://uu.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cm.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://mb.szxytkj.cn

files=$(ls -1)
来源：http://nm.nicolike.cn

[R38] 管道串联
来源：http://ow.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://jh.panjiajie.cn

[R39] 重定向标准输出与错误
来源：http://pk.shxzskj.cn

cmd > out.log 2>&1
来源：http://dn.521024.cn

[R40] 追加写日志
来源：http://ig.wgjwhj.cn

echo "log" >> out.log
来源：http://dc.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://ws.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://mk.jianghongdianzi.cn

[R42] 输入重定向
来源：http://zr.wgjwhj.cn

wc -l < a.txt
来源：http://nw.huixiangedu.cn

[R43] 按名字查找文件
来源：http://lv.gzmigu.cn

find . -name "*.log" -type f
来源：http://eb.chemitech.net.cn

[R44] 按修改时间查找
来源：http://sb.panjiajie.cn

find . -mtime -7 -type f
来源：http://yc.newstarts.cn

[R45] 批量删除
来源：http://ak.huanxung.cn

find . -name "*.tmp" -delete
来源：http://jf.colortex.cn

[R46] 递归替换文件内容
来源：http://cg.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cv.9csxet.cn

[R47] sed 单行替换
来源：http://mh.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hu.521024.cn

[R48] awk 取指定列
来源：http://yy.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://dq.huanxung.cn

[R49] awk 带条件
来源：http://xb.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cl.jctech888.com.cn

[R50] awk 求和
来源：http://dn.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://on.muxihuayi.cn

[R51] 排序去重取前几
来源：http://zq.gzmigu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jh.9csxet.cn

[R52] 统计行数
来源：http://hv.newstarts.cn

wc -l a.txt
来源：http://cf.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://vs.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oi.huixiangedu.cn

[R54] 比较两个文件
来源：http://ck.gzmigu.cn

diff a.txt b.txt
来源：http://vr.szxytkj.cn

[R55] 压缩与解压
来源：http://po.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dm.haigaiapp.cn

[R56] 远程拷贝
来源：http://qu.lnxyls.cn

scp file user@host:/path/
来源：http://cj.hahajie.cn

[R57] 远程执行命令
来源：http://uu.wgjwhj.cn

ssh user@host 'uptime'
来源：http://vj.jianghongdianzi.cn

[R58] 下载文件
来源：http://ea.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xf.colortex.cn

[R59] 发 POST JSON
来源：http://te.szxytkj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://db.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://oz.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ta.chemitech.net.cn

[R61] 磁盘占用
来源：http://nj.9csxet.cn

df -h;  du -sh *
来源：http://tg.shxzukj.cn

[R62] 找最占空间的文件
来源：http://vi.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://bf.521024.cn

[R63] 内存与进程
来源：http://zm.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://nq.jianghongdianzi.cn

[R64] 结束进程
来源：http://sy.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://fv.nszjky.cn

[R65] 查看端口占用
来源：http://tj.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ok.9csxet.cn

[R66] 定时任务
来源：http://os.nszjky.cn

crontab -e;  crontab -l
来源：http://lo.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://wb.colortex.cn

openssl rand -hex 16
来源：http://ro.yuntaijiaju.cn

[R68] 计算文件校验值
来源：http://si.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mw.gzmigu.cn

[R69] 生成随机密码
来源：http://dr.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://nq.bjjhwx.cn

[R70] 时间戳与互转
来源：http://uh.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://uu.hnjuh.cn

[R71] 日期格式化
来源：http://oe.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xf.muxihuayi.cn

[R72] 等待端口就绪
来源：http://do.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cm.lnxyls.cn

[R73] 分割大日志
来源：http://ye.muxihuayi.cn

split -l 1000 big.log part_
来源：http://rr.muxihuayi.cn

[R74] 批量重命名
来源：http://gh.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fo.huanxung.cn

[R75] 导出环境变量
来源：http://ie.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://eb.nszjky.cn

[R76] 使用临时文件
来源：http://ki.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zo.nszjky.cn

[R77] 读取用户输入
来源：http://fe.muxihuayi.cn

read -rp "请输入: " ans
来源：http://if.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://sy.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kv.asd995.cn

[R79] 解析命令行选项
来源：http://rj.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jj.asd995.cn

[R80] 查看脚本执行耗时
来源：http://rl.521024.cn

time ./run.sh
来源：http://dm.huixinmuqiang.cn

================================================================================
来源：http://zk.nszjky.cn

S. C / C++ 专题
来源：http://zj.huixiangedu.cn

================================================================================
来源：http://kx.hnjuh.cn

[S01] C：Hello World
来源：http://nv.521024.cn

#include <stdio.h>
来源：http://ca.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xx.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://pk.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://fn.bjjhwx.cn

[S03] C：读入整数
来源：http://zx.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://ys.newstarts.cn

[S04] C：字符串复制
来源：http://kf.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jh.chemitech.net.cn

[S05] C：字符串长度
来源：http://yz.yuexingan06.cn

strlen(s)
来源：http://va.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://nm.huixiangedu.cn

strcmp(a, b) == 0
来源：http://di.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://dm.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mc.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://tu.huixinmuqiang.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xi.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://be.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cw.asd995.cn

[S10] C：指针与解引用
来源：http://ut.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://iy.huixiangedu.cn

[S11] C：逐行读文件
来源：http://pr.yuexingan06.cn

FILE *f = fopen("a.txt", "r");
来源：http://pg.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wm.gzmigu.cn

fclose(f);
来源：http://zk.muxihuayi.cn

[S12] C：写文件
来源：http://go.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wd.newstarts.cn

[S13] C：宏定义
来源：http://xu.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nd.jctech888.com.cn

[S14] C：枚举
来源：http://li.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://uy.szsharing.cn

[S15] C：类型转换
来源：http://zt.yuntaijiaju.cn

(double) a / b
来源：http://tt.panjiajie.cn

[S16] C：位操作置位
来源：http://pa.bookmarksfly.cn

x |= (1 << 3);
来源：http://dw.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://ow.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ch.chemitech.net.cn

[S18] C：命令行参数
来源：http://is.panjiajie.cn

int main(int argc, char **argv)
来源：http://oh.asd995.cn

[S19] C：快速排序
来源：http://cx.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ss.szxytkj.cn

[S20] C：二分查找
来源：http://rz.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wl.colortex.cn

[S21] C：字符类别判断
来源：http://lz.wgjwhj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://in.nicolike.cn

[S22] C：字符串转数字
来源：http://gu.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tq.lnxyls.cn

[S23] C：随机数
来源：http://ip.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fr.haigaiapp.cn

[S24] C：获取本地时间
来源：http://vr.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lz.newstarts.cn

[S25] C：内存拷贝
来源：http://um.wgjwhj.cn

memcpy(dst, src, n);
来源：http://gy.asd995.cn

[S26] C：内存清零
来源：http://le.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://kb.bjjhwx.cn

[S27] C：定义常量
来源：http://vc.9csxet.cn

const double PI = 3.14159;
来源：http://nl.colortex.cn

[S28] C：静态变量
来源：http://xu.jianghongdianzi.cn

static int counter = 0;
来源：http://zd.panjiajie.cn

[S29] C：变参函数
来源：http://th.panjiajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bg.asd995.cn

[S30] C：头文件保护
来源：http://rb.shxzskj.cn

#ifndef X_H
来源：http://bq.9csxet.cn

#define X_H
来源：http://wm.yuexingan06.cn

#endif
来源：http://jf.muxihuayi.cn

[S31] C++：Hello World
来源：http://lb.yuexingan06.cn

#include <iostream>
来源：http://xe.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://cq.shxzukj.cn

[S32] C++：字符串
来源：http://dw.521024.cn

std::string s = "hi";  s += "!";
来源：http://ka.newstarts.cn

[S33] C++：vector 增删
来源：http://dg.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pm.hnjuh.cn

[S34] C++：遍历 vector
来源：http://rs.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://pt.panjiajie.cn

[S35] C++：map
来源：http://zo.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hi.hahajie.cn

[S36] C++：unordered_map
来源：http://dh.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tf.bjjhwx.cn

[S37] C++：set
来源：http://al.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wx.bjjhwx.cn

[S38] C++：排序
来源：http://dk.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://el.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://fy.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ew.szxytkj.cn

[S40] C++：查找元素
来源：http://vx.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ly.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://jb.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nz.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://mz.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://sw.bjjhwx.cn

[S43] C++：智能指针
来源：http://op.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://zg.huanxung.cn

[S44] C++：引用传参
来源：http://tc.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://bb.hnjuh.cn

[S45] C++：lambda
来源：http://yd.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tr.nszjky.cn

[S46] C++：函数模板
来源：http://fa.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fi.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://vo.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ev.9csxet.cn

[S48] C++：逐行读文件
来源：http://ng.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qn.nszjky.cn

while (std::getline(in, line)) { }
来源：http://qj.yuntaijiaju.cn

[S49] C++：写文件
来源：http://xc.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hr.hnjuh.cn

[S50] C++：格式化数字
来源：http://ho.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zg.hnjuh.cn

[S51] C++：显式类型转换
来源：http://ox.9csxet.cn

static_cast<double>(a) / b
来源：http://qy.huixinmuqiang.cn

[S52] C++：const 与 noexcept
来源：http://id.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://xl.huixiangedu.cn

[S53] C++：移动语义
来源：http://eh.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://vi.lnxyls.cn

[S54] C++：异常处理
来源：http://rq.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tr.newstarts.cn

[S55] C++：结构化绑定
来源：http://xk.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fg.521024.cn

[S56] C++：optional
来源：http://uj.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ng.szsharing.cn

[S57] C++：编译期常量
来源：http://tp.hnjuh.cn

constexpr int N = 10;
来源：http://ni.nszjky.cn

[S58] C++：命名空间
来源：http://mq.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://dx.shxzukj.cn

[S59] C++：静态断言
来源：http://eg.shxzukj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hd.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://yx.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dy.szsharing.cn

================================================================================
来源：http://xc.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://su.chemitech.net.cn

================================================================================
来源：http://yg.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://ws.jctech888.com.cn

println("Hello")
来源：http://pu.asd995.cn

[T02] Kotlin：变量
来源：http://vh.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ls.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://cw.newstarts.cn

"值: $b"
来源：http://rk.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://nd.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://fp.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://wz.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vj.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://rb.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ct.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://ms.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wj.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://xw.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://sf.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://vi.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://ls.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://ji.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zi.chemitech.net.cn

[T11] Kotlin：协程
来源：http://gn.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ul.colortex.cn

[T12] Kotlin：解构声明
来源：http://de.chemitech.net.cn

val (a, b) = Pair(1, 2)
来源：http://zv.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://fn.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://ym.yuexingan06.cn

[T14] Kotlin：循环
来源：http://vr.521024.cn

for (i in 1..10) println(i)
来源：http://ip.chemitech.net.cn

[T15] Kotlin：接口
来源：http://xu.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://kt.shxzskj.cn

[T16] Swift：Hello World
来源：http://gr.yuexingan06.cn

print("Hello")
来源：http://qj.nicolike.cn

[T17] Swift：变量与常量
来源：http://fc.jctech888.com.cn

var a = 1;  let b = 2
来源：http://px.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://wx.huixiangedu.cn

"值: \(b)"
来源：http://ll.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://jw.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://lj.huixiangedu.cn

[T20] Swift：数组操作
来源：http://ir.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wx.jctech888.com.cn

[T21] Swift：遍历
来源：http://av.szxytkj.cn

for x in a { print(x) }
来源：http://xt.nicolike.cn

[T22] Swift：字典
来源：http://sz.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rj.jctech888.com.cn


<!-- 参考信息 -->