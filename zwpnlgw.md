代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://xs.jctech888.com.cn

[R32] 参数个数校验
来源：http://px.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lv.yuntaijiaju.cn

[R33] 捕获错误并提示行号
来源：http://qk.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ji.panjiajie.cn

[R34] 退出时清理
来源：http://wx.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bu.asd995.cn

[R35] 后台执行并等待
来源：http://dg.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zx.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://mu.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lp.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://wo.shtwfgs.cn

files=$(ls -1)
来源：http://zt.shtwfgs.cn

[R38] 管道串联
来源：http://ar.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://wd.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://pp.szxytkj.cn

cmd > out.log 2>&1
来源：http://cl.wgjwhj.cn

[R40] 追加写日志
来源：http://db.shtwfgs.cn

echo "log" >> out.log
来源：http://sc.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://ub.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://dp.bookmarksfly.cn

[R42] 输入重定向
来源：http://me.colortex.cn

wc -l < a.txt
来源：http://bd.gzmigu.cn

[R43] 按名字查找文件
来源：http://cf.yuexingan06.cn

find . -name "*.log" -type f
来源：http://gx.newstarts.cn

[R44] 按修改时间查找
来源：http://gr.bjjhwx.cn

find . -mtime -7 -type f
来源：http://jg.haigaiapp.cn

[R45] 批量删除
来源：http://al.szsharing.cn

find . -name "*.tmp" -delete
来源：http://yz.yuntaijiaju.cn

[R46] 递归替换文件内容
来源：http://oa.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qf.shxzskj.cn

[R47] sed 单行替换
来源：http://ky.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pb.jctech888.com.cn

[R48] awk 取指定列
来源：http://cj.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://hg.jctech888.com.cn

[R49] awk 带条件
来源：http://ss.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yq.huanxung.cn

[R50] awk 求和
来源：http://hs.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lg.9csxet.cn

[R51] 排序去重取前几
来源：http://ob.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mo.nszjky.cn

[R52] 统计行数
来源：http://vy.hnjuh.cn

wc -l a.txt
来源：http://wx.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://jj.gzmigu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yy.nszjky.cn

[R54] 比较两个文件
来源：http://ol.wgjwhj.cn

diff a.txt b.txt
来源：http://zh.asd995.cn

[R55] 压缩与解压
来源：http://yg.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mb.jctech888.com.cn

[R56] 远程拷贝
来源：http://yy.shxzukj.cn

scp file user@host:/path/
来源：http://nh.shxzskj.cn

[R57] 远程执行命令
来源：http://xa.panjiajie.cn

ssh user@host 'uptime'
来源：http://ul.asd995.cn

[R58] 下载文件
来源：http://iv.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xk.asd995.cn

[R59] 发 POST JSON
来源：http://yh.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ej.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://jn.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://or.panjiajie.cn

[R61] 磁盘占用
来源：http://dm.panjiajie.cn

df -h;  du -sh *
来源：http://ny.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://yi.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://vt.muxihuayi.cn

[R63] 内存与进程
来源：http://wm.521024.cn

free -h;  ps aux | grep nginx
来源：http://xl.asd995.cn

[R64] 结束进程
来源：http://kt.haigaiapp.cn

kill -9 $(pgrep -f app.py)
来源：http://id.chemitech.net.cn

[R65] 查看端口占用
来源：http://mc.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ha.muxihuayi.cn

[R66] 定时任务
来源：http://sy.huanxung.cn

crontab -e;  crontab -l
来源：http://ih.9csxet.cn

[R67] 生成随机十六进制串
来源：http://hx.huanxung.cn

openssl rand -hex 16
来源：http://gb.chemitech.net.cn

[R68] 计算文件校验值
来源：http://le.521024.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vp.szsharing.cn

[R69] 生成随机密码
来源：http://sz.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://sl.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://mw.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://aq.shxzukj.cn

[R71] 日期格式化
来源：http://fu.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rc.huixiangedu.cn

[R72] 等待端口就绪
来源：http://ae.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dm.huixiangedu.cn

[R73] 分割大日志
来源：http://lu.haigaiapp.cn

split -l 1000 big.log part_
来源：http://st.huixinmuqiang.cn

[R74] 批量重命名
来源：http://xb.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zk.hnjuh.cn

[R75] 导出环境变量
来源：http://sh.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://jn.hnjuh.cn

[R76] 使用临时文件
来源：http://rq.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gg.lnxyls.cn

[R77] 读取用户输入
来源：http://ao.hnjuh.cn

read -rp "请输入: " ans
来源：http://iw.colortex.cn

[R78] 交互式菜单
来源：http://pn.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://la.nszjky.cn

[R79] 解析命令行选项
来源：http://kn.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lt.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://df.panjiajie.cn

time ./run.sh
来源：http://ae.shxzukj.cn

================================================================================
来源：http://uj.hnjuh.cn

S. C / C++ 专题
来源：http://yq.shxzskj.cn

================================================================================
来源：http://cg.shxzskj.cn

[S01] C：Hello World
来源：http://to.nszjky.cn

#include <stdio.h>
来源：http://ty.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://to.szsharing.cn

[S02] C：变量与格式化输出
来源：http://oh.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://lv.yuntaijiaju.cn

[S03] C：读入整数
来源：http://kc.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://lv.jctech888.com.cn

[S04] C：字符串复制
来源：http://uf.huixiangedu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://se.newstarts.cn

[S05] C：字符串长度
来源：http://ws.shxzskj.cn

strlen(s)
来源：http://kf.huixiangedu.cn

[S06] C：字符串比较
来源：http://sv.yuexingan06.cn

strcmp(a, b) == 0
来源：http://bo.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://ds.szxytkj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dq.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://yh.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gq.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://qm.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ti.lnxyls.cn

[S10] C：指针与解引用
来源：http://cx.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://df.szxytkj.cn

[S11] C：逐行读文件
来源：http://uw.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://ng.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cg.9csxet.cn

fclose(f);
来源：http://zt.shxzukj.cn

[S12] C：写文件
来源：http://hi.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wj.colortex.cn

[S13] C：宏定义
来源：http://pk.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fz.hnjuh.cn

[S14] C：枚举
来源：http://dc.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://mq.shtwfgs.cn

[S15] C：类型转换
来源：http://er.yuexingan06.cn

(double) a / b
来源：http://sy.chemitech.net.cn

[S16] C：位操作置位
来源：http://cd.muxihuayi.cn

x |= (1 << 3);
来源：http://xh.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://re.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sl.newstarts.cn

[S18] C：命令行参数
来源：http://jf.yuexingan06.cn

int main(int argc, char **argv)
来源：http://ia.shtwfgs.cn

[S19] C：快速排序
来源：http://bp.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wr.lnxyls.cn

[S20] C：二分查找
来源：http://ij.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xq.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://ye.jianghongdianzi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://op.shtwfgs.cn

[S22] C：字符串转数字
来源：http://ez.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hm.hahajie.cn

[S23] C：随机数
来源：http://ow.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bq.gzmigu.cn

[S24] C：获取本地时间
来源：http://ef.521024.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wg.szxytkj.cn

[S25] C：内存拷贝
来源：http://ah.szsharing.cn

memcpy(dst, src, n);
来源：http://op.shtwfgs.cn

[S26] C：内存清零
来源：http://fa.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://qp.nszjky.cn

[S27] C：定义常量
来源：http://am.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://tt.haigaiapp.cn

[S28] C：静态变量
来源：http://zw.yuexingan06.cn

static int counter = 0;
来源：http://yc.muxihuayi.cn

[S29] C：变参函数
来源：http://ho.9csxet.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lc.gzmigu.cn

[S30] C：头文件保护
来源：http://av.shxzukj.cn

#ifndef X_H
来源：http://mj.huanxung.cn

#define X_H
来源：http://zr.muxihuayi.cn

#endif
来源：http://nx.shxzukj.cn

[S31] C++：Hello World
来源：http://yk.colortex.cn

#include <iostream>
来源：http://cy.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://db.haigaiapp.cn

[S32] C++：字符串
来源：http://vu.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://sw.hahajie.cn

[S33] C++：vector 增删
来源：http://qd.wgjwhj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vx.521024.cn

[S34] C++：遍历 vector
来源：http://gr.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://wm.hahajie.cn

[S35] C++：map
来源：http://js.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eb.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://pb.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://me.9csxet.cn

[S37] C++：set
来源：http://yn.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yp.panjiajie.cn

[S38] C++：排序
来源：http://fk.asd995.cn

std::sort(v.begin(), v.end());
来源：http://kk.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://lw.huixinmuqiang.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vp.bjjhwx.cn

[S40] C++：查找元素
来源：http://aw.jianghongdianzi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://aq.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://tx.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://of.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://jw.nszjky.cn

class B : public Base { public: void f() override {} };
来源：http://wx.hahajie.cn

[S43] C++：智能指针
来源：http://ad.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://xr.panjiajie.cn

[S44] C++：引用传参
来源：http://vw.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://ot.yuexingan06.cn

[S45] C++：lambda
来源：http://bc.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hi.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://ul.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zq.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://it.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gb.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://ib.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ca.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://qr.jianghongdianzi.cn

[S49] C++：写文件
来源：http://bk.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vr.colortex.cn

[S50] C++：格式化数字
来源：http://hn.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ah.hnjuh.cn

[S51] C++：显式类型转换
来源：http://no.lnxyls.cn

static_cast<double>(a) / b
来源：http://me.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://na.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://lw.shxzukj.cn

[S53] C++：移动语义
来源：http://hm.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://kf.shxzukj.cn

[S54] C++：异常处理
来源：http://gs.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ds.hnjuh.cn

[S55] C++：结构化绑定
来源：http://ht.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xq.newstarts.cn

[S56] C++：optional
来源：http://dn.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jo.chemitech.net.cn

[S57] C++：编译期常量
来源：http://yb.yuexingan06.cn

constexpr int N = 10;
来源：http://cp.lnxyls.cn

[S58] C++：命名空间
来源：http://tt.jianghongdianzi.cn

namespace ns { int f() { return 1; } }
来源：http://es.hnjuh.cn

[S59] C++：静态断言
来源：http://nh.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pn.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://dz.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://re.yuexingan06.cn

================================================================================
来源：http://pi.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lx.hahajie.cn

================================================================================
来源：http://yk.hahajie.cn

[T01] Kotlin：Hello World
来源：http://yh.huanxung.cn

println("Hello")
来源：http://op.szxytkj.cn

[T02] Kotlin：变量
来源：http://pp.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rx.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://dk.muxihuayi.cn

"值: $b"
来源：http://op.asd995.cn

[T04] Kotlin：空安全
来源：http://fq.colortex.cn

val n: String? = null;  n?.length
来源：http://tf.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://bo.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mn.521024.cn

[T06] Kotlin：集合映射
来源：http://kc.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xe.huixinmuqiang.cn

[T07] Kotlin：集合过滤
来源：http://ev.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ao.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://po.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://zs.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://bz.asd995.cn

fun String.exclaim() = this + "!"
来源：http://iv.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://hn.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ra.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://jr.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tq.yuexingan06.cn

[T12] Kotlin：解构声明
来源：http://vb.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://qf.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://rf.colortex.cn

val m = mapOf("a" to 1)
来源：http://oy.panjiajie.cn

[T14] Kotlin：循环
来源：http://ep.gzmigu.cn

for (i in 1..10) println(i)
来源：http://ry.haigaiapp.cn

[T15] Kotlin：接口
来源：http://hr.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://on.521024.cn

[T16] Swift：Hello World
来源：http://wa.shxzskj.cn

print("Hello")
来源：http://as.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://lk.wgjwhj.cn

var a = 1;  let b = 2
来源：http://gu.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://yc.nicolike.cn

"值: \(b)"
来源：http://wx.lnxyls.cn

[T19] Swift：可选绑定
来源：http://zi.shxzukj.cn

if let n = opt { print(n) }
来源：http://ow.yuexingan06.cn

[T20] Swift：数组操作
来源：http://kd.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xh.muxihuayi.cn

[T21] Swift：遍历
来源：http://id.shtwfgs.cn

for x in a { print(x) }
来源：http://kz.chemitech.net.cn

[T22] Swift：字典
来源：http://zg.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fk.asd995.cn

[T23] Swift：函数
来源：http://kd.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cw.lnxyls.cn

[T24] Swift：闭包
来源：http://ex.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rp.hnjuh.cn

[T25] Swift：结构体
来源：http://im.huixinmuqiang.cn

struct P { var x: Int }
来源：http://bc.szxytkj.cn

[T26] Swift：类与重写
来源：http://cl.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://gf.asd995.cn

[T27] Swift：错误处理
来源：http://de.nicolike.cn

do { try f() } catch { print(error) }
来源：http://fd.huanxung.cn

[T28] Swift：枚举
来源：http://kh.shxzskj.cn

enum Color { case red, green }
来源：http://fw.shtwfgs.cn

[T29] Swift：guard 提前返回
来源：http://on.jctech888.com.cn

guard let x = opt else { return }
来源：http://jh.hnjuh.cn

[T30] Swift：协议
来源：http://wn.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://pf.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://jz.huanxung.cn

print("Hello")
来源：http://ya.hnjuh.cn

[T32] Lua：局部变量
来源：http://wf.521024.cn

local a = 1
来源：http://vb.newstarts.cn

[T33] Lua：表（数组）
来源：http://mi.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tk.chemitech.net.cn

[T34] Lua：遍历表
来源：http://yu.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nw.shxzskj.cn


<!-- 参考信息 -->