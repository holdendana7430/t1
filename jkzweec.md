代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yu.chemitech.net.cn

[R24] 大小写转换
来源：http://ux.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zd.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://tu.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ol.panjiajie.cn

[R26] 命令替换
来源：http://aj.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://mk.szsharing.cn

[R27] 算术展开
来源：http://tv.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://yy.panjiajie.cn

[R28] 浮点运算
来源：http://ah.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://sy.nicolike.cn

[R29] 定义函数
来源：http://og.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qa.nszjky.cn

[R30] 函数返回状态码
来源：http://cp.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://xi.shxzukj.cn

[R31] 局部变量
来源：http://iv.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://zy.nicolike.cn

[R32] 参数个数校验
来源：http://tm.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hy.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://vi.asd995.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dr.panjiajie.cn

[R34] 退出时清理
来源：http://pw.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nr.jctech888.com.cn

[R35] 后台执行并等待
来源：http://hg.hnjuh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uz.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://cv.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yq.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://hf.521024.cn

files=$(ls -1)
来源：http://zk.haigaiapp.cn

[R38] 管道串联
来源：http://bj.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://rc.panjiajie.cn

[R39] 重定向标准输出与错误
来源：http://cm.haigaiapp.cn

cmd > out.log 2>&1
来源：http://ix.hahajie.cn

[R40] 追加写日志
来源：http://go.huanxung.cn

echo "log" >> out.log
来源：http://eo.panjiajie.cn

[R41] 丢弃输出
来源：http://xg.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://tw.nszjky.cn

[R42] 输入重定向
来源：http://wd.nszjky.cn

wc -l < a.txt
来源：http://so.haigaiapp.cn

[R43] 按名字查找文件
来源：http://ep.szsharing.cn

find . -name "*.log" -type f
来源：http://ir.chemitech.net.cn

[R44] 按修改时间查找
来源：http://ji.jctech888.com.cn

find . -mtime -7 -type f
来源：http://om.shxzukj.cn

[R45] 批量删除
来源：http://ud.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://cq.newstarts.cn

[R46] 递归替换文件内容
来源：http://rs.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wn.panjiajie.cn

[R47] sed 单行替换
来源：http://iv.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vb.asd995.cn

[R48] awk 取指定列
来源：http://yq.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://gp.jctech888.com.cn

[R49] awk 带条件
来源：http://jt.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pi.nicolike.cn

[R50] awk 求和
来源：http://hn.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ol.haigaiapp.cn

[R51] 排序去重取前几
来源：http://gn.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mh.jctech888.com.cn

[R52] 统计行数
来源：http://eh.szsharing.cn

wc -l a.txt
来源：http://ra.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://uv.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sl.szsharing.cn

[R54] 比较两个文件
来源：http://hp.jianghongdianzi.cn

diff a.txt b.txt
来源：http://ws.gzmigu.cn

[R55] 压缩与解压
来源：http://ly.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tz.bjjhwx.cn

[R56] 远程拷贝
来源：http://la.521024.cn

scp file user@host:/path/
来源：http://ot.huixiangedu.cn

[R57] 远程执行命令
来源：http://dq.chemitech.net.cn

ssh user@host 'uptime'
来源：http://iv.colortex.cn

[R58] 下载文件
来源：http://pt.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xr.nicolike.cn

[R59] 发 POST JSON
来源：http://bu.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pf.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://zx.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oe.huanxung.cn

[R61] 磁盘占用
来源：http://hs.shxzskj.cn

df -h;  du -sh *
来源：http://zr.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://qz.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://ki.chemitech.net.cn

[R63] 内存与进程
来源：http://vn.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://qd.szxytkj.cn

[R64] 结束进程
来源：http://vt.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://yy.nszjky.cn

[R65] 查看端口占用
来源：http://cz.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yi.lnxyls.cn

[R66] 定时任务
来源：http://zm.shtwfgs.cn

crontab -e;  crontab -l
来源：http://nc.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://yy.colortex.cn

openssl rand -hex 16
来源：http://ij.huanxung.cn

[R68] 计算文件校验值
来源：http://ja.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yu.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://so.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://be.shxzukj.cn

[R70] 时间戳与互转
来源：http://wt.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://mp.yuntaijiaju.cn

[R71] 日期格式化
来源：http://zd.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ky.nicolike.cn

[R72] 等待端口就绪
来源：http://xl.huixinmuqiang.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.panjiajie.cn

[R73] 分割大日志
来源：http://ef.hahajie.cn

split -l 1000 big.log part_
来源：http://np.chemitech.net.cn

[R74] 批量重命名
来源：http://js.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nd.huanxung.cn

[R75] 导出环境变量
来源：http://bx.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://ul.huixiangedu.cn

[R76] 使用临时文件
来源：http://sm.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nb.asd995.cn

[R77] 读取用户输入
来源：http://qr.nicolike.cn

read -rp "请输入: " ans
来源：http://wa.shxzukj.cn

[R78] 交互式菜单
来源：http://cw.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qs.jctech888.com.cn

[R79] 解析命令行选项
来源：http://sk.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mh.yuntaijiaju.cn

[R80] 查看脚本执行耗时
来源：http://oo.panjiajie.cn

time ./run.sh
来源：http://ho.szsharing.cn

================================================================================
来源：http://wu.asd995.cn

S. C / C++ 专题
来源：http://dj.nszjky.cn

================================================================================
来源：http://ou.chemitech.net.cn

[S01] C：Hello World
来源：http://ig.9csxet.cn

#include <stdio.h>
来源：http://lu.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ad.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://cf.gzmigu.cn

int a = 10; printf("%d\n", a);
来源：http://gt.colortex.cn

[S03] C：读入整数
来源：http://sd.nicolike.cn

int x; scanf("%d", &x);
来源：http://ne.jctech888.com.cn

[S04] C：字符串复制
来源：http://et.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bc.asd995.cn

[S05] C：字符串长度
来源：http://uc.huixiangedu.cn

strlen(s)
来源：http://ne.bjjhwx.cn

[S06] C：字符串比较
来源：http://pc.wgjwhj.cn

strcmp(a, b) == 0
来源：http://jz.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://pc.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fl.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://dv.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jw.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://wo.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ys.muxihuayi.cn

[S10] C：指针与解引用
来源：http://mu.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://ty.nicolike.cn

[S11] C：逐行读文件
来源：http://ky.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://eg.hnjuh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wx.nszjky.cn

fclose(f);
来源：http://ou.hahajie.cn

[S12] C：写文件
来源：http://et.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tr.colortex.cn

[S13] C：宏定义
来源：http://hp.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ng.shtwfgs.cn

[S14] C：枚举
来源：http://rm.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://wk.jctech888.com.cn

[S15] C：类型转换
来源：http://dx.haigaiapp.cn

(double) a / b
来源：http://fj.521024.cn

[S16] C：位操作置位
来源：http://ao.521024.cn

x |= (1 << 3);
来源：http://he.9csxet.cn

[S17] C：安全拼接字符串
来源：http://gt.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aq.9csxet.cn

[S18] C：命令行参数
来源：http://zh.nszjky.cn

int main(int argc, char **argv)
来源：http://vj.huanxung.cn

[S19] C：快速排序
来源：http://et.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jg.muxihuayi.cn

[S20] C：二分查找
来源：http://ii.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kb.newstarts.cn

[S21] C：字符类别判断
来源：http://ki.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zp.lnxyls.cn

[S22] C：字符串转数字
来源：http://sa.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kf.jianghongdianzi.cn

[S23] C：随机数
来源：http://rd.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fx.shtwfgs.cn

[S24] C：获取本地时间
来源：http://nt.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oi.hahajie.cn

[S25] C：内存拷贝
来源：http://re.bjjhwx.cn

memcpy(dst, src, n);
来源：http://wj.521024.cn

[S26] C：内存清零
来源：http://po.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://rz.jianghongdianzi.cn

[S27] C：定义常量
来源：http://zr.shxzskj.cn

const double PI = 3.14159;
来源：http://uu.haigaiapp.cn

[S28] C：静态变量
来源：http://ko.chemitech.net.cn

static int counter = 0;
来源：http://dl.jctech888.com.cn

[S29] C：变参函数
来源：http://os.yuexingan06.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ss.chemitech.net.cn

[S30] C：头文件保护
来源：http://yc.haigaiapp.cn

#ifndef X_H
来源：http://mw.yuexingan06.cn

#define X_H
来源：http://uk.huixinmuqiang.cn

#endif
来源：http://ba.huanxung.cn

[S31] C++：Hello World
来源：http://tu.szxytkj.cn

#include <iostream>
来源：http://ia.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://zh.jianghongdianzi.cn

[S32] C++：字符串
来源：http://zc.colortex.cn

std::string s = "hi";  s += "!";
来源：http://ga.panjiajie.cn

[S33] C++：vector 增删
来源：http://zi.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fr.huanxung.cn

[S34] C++：遍历 vector
来源：http://ow.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://ck.shtwfgs.cn

[S35] C++：map
来源：http://dm.lnxyls.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bz.newstarts.cn

[S36] C++：unordered_map
来源：http://re.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xf.shtwfgs.cn

[S37] C++：set
来源：http://ys.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bu.gzmigu.cn

[S38] C++：排序
来源：http://fq.521024.cn

std::sort(v.begin(), v.end());
来源：http://ax.gzmigu.cn

[S39] C++：自定义比较器排序
来源：http://qe.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://im.huanxung.cn

[S40] C++：查找元素
来源：http://qv.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yw.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://eb.bookmarksfly.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xj.yuntaijiaju.cn

[S42] C++：继承与虚函数
来源：http://mx.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://lo.bjjhwx.cn

[S43] C++：智能指针
来源：http://xa.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://qo.shxzukj.cn

[S44] C++：引用传参
来源：http://dt.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://wm.lnxyls.cn

[S45] C++：lambda
来源：http://jv.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bz.shtwfgs.cn

[S46] C++：函数模板
来源：http://em.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://so.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://wo.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vy.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://dz.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cn.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://ul.colortex.cn

[S49] C++：写文件
来源：http://nv.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ma.jctech888.com.cn

[S50] C++：格式化数字
来源：http://yl.shxzukj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ng.colortex.cn

[S51] C++：显式类型转换
来源：http://su.asd995.cn

static_cast<double>(a) / b
来源：http://bl.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://td.newstarts.cn

int size() const noexcept { return n_; }
来源：http://bh.bookmarksfly.cn

[S53] C++：移动语义
来源：http://ao.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://ee.huixiangedu.cn

[S54] C++：异常处理
来源：http://mw.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ls.nszjky.cn

[S55] C++：结构化绑定
来源：http://pe.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ql.muxihuayi.cn

[S56] C++：optional
来源：http://ce.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tk.hahajie.cn

[S57] C++：编译期常量
来源：http://dy.jctech888.com.cn

constexpr int N = 10;
来源：http://lt.colortex.cn

[S58] C++：命名空间
来源：http://fw.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://lz.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://io.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qy.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://bz.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dp.newstarts.cn

================================================================================
来源：http://xa.gzmigu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tf.yuntaijiaju.cn

================================================================================
来源：http://wu.521024.cn

[T01] Kotlin：Hello World
来源：http://du.hahajie.cn

println("Hello")
来源：http://ca.colortex.cn

[T02] Kotlin：变量
来源：http://kk.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://db.asd995.cn

[T03] Kotlin：字符串模板
来源：http://lu.521024.cn

"值: $b"
来源：http://ve.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://xm.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://ff.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://iv.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jb.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://um.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rb.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://mm.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nx.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://ox.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://yf.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://oz.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://gf.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://em.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xt.chemitech.net.cn

[T11] Kotlin：协程
来源：http://ct.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bn.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://rg.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://yd.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://pl.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://am.shxzskj.cn

[T14] Kotlin：循环
来源：http://yd.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://yy.panjiajie.cn

[T15] Kotlin：接口
来源：http://mg.yuexingan06.cn

interface Shape { fun area(): Double }
来源：http://bp.hahajie.cn

[T16] Swift：Hello World
来源：http://ew.yuntaijiaju.cn

print("Hello")
来源：http://sb.huanxung.cn

[T17] Swift：变量与常量
来源：http://fl.haigaiapp.cn

var a = 1;  let b = 2
来源：http://yi.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://ai.shxzskj.cn

"值: \(b)"
来源：http://cl.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://st.nicolike.cn

if let n = opt { print(n) }
来源：http://oi.hnjuh.cn

[T20] Swift：数组操作
来源：http://xn.shxzskj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ma.szxytkj.cn

[T21] Swift：遍历
来源：http://ui.panjiajie.cn

for x in a { print(x) }
来源：http://yg.huanxung.cn

[T22] Swift：字典
来源：http://yt.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jo.szsharing.cn

[T23] Swift：函数
来源：http://sj.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dn.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://km.hahajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://za.gzmigu.cn

[T25] Swift：结构体
来源：http://io.nszjky.cn

struct P { var x: Int }
来源：http://nq.szxytkj.cn

[T26] Swift：类与重写
来源：http://ua.hnjuh.cn

class A: Base { override func f() {} }
来源：http://eq.szsharing.cn


<!-- 参考信息 -->