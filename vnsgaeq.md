代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://ws.huanxung.cn

[R36] 并发执行多个任务
来源：http://iz.shxzskj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://aq.szsharing.cn

[R37] 把输出赋给变量
来源：http://yy.yuntaijiaju.cn

files=$(ls -1)
来源：http://fw.shxzskj.cn

[R38] 管道串联
来源：http://dk.lnxyls.cn

cat a.txt | grep -i error | wc -l
来源：http://gz.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://xd.shxzskj.cn

cmd > out.log 2>&1
来源：http://jm.jianghongdianzi.cn

[R40] 追加写日志
来源：http://wt.hnjuh.cn

echo "log" >> out.log
来源：http://fh.lnxyls.cn

[R41] 丢弃输出
来源：http://yu.wgjwhj.cn

cmd >/dev/null 2>&1
来源：http://bi.szxytkj.cn

[R42] 输入重定向
来源：http://ml.chemitech.net.cn

wc -l < a.txt
来源：http://ne.panjiajie.cn

[R43] 按名字查找文件
来源：http://xm.yuexingan06.cn

find . -name "*.log" -type f
来源：http://ve.newstarts.cn

[R44] 按修改时间查找
来源：http://rc.newstarts.cn

find . -mtime -7 -type f
来源：http://pk.bookmarksfly.cn

[R45] 批量删除
来源：http://yq.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://gi.colortex.cn

[R46] 递归替换文件内容
来源：http://xp.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ra.nicolike.cn

[R47] sed 单行替换
来源：http://xv.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qt.yuexingan06.cn

[R48] awk 取指定列
来源：http://ss.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://ta.hahajie.cn

[R49] awk 带条件
来源：http://wu.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iz.panjiajie.cn

[R50] awk 求和
来源：http://he.bookmarksfly.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hx.colortex.cn

[R51] 排序去重取前几
来源：http://ir.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://eb.szsharing.cn

[R52] 统计行数
来源：http://cx.szsharing.cn

wc -l a.txt
来源：http://nv.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://ec.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dv.9csxet.cn

[R54] 比较两个文件
来源：http://vq.yuexingan06.cn

diff a.txt b.txt
来源：http://be.jctech888.com.cn

[R55] 压缩与解压
来源：http://ze.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rh.panjiajie.cn

[R56] 远程拷贝
来源：http://rv.hnjuh.cn

scp file user@host:/path/
来源：http://hp.lnxyls.cn

[R57] 远程执行命令
来源：http://if.newstarts.cn

ssh user@host 'uptime'
来源：http://nz.haigaiapp.cn

[R58] 下载文件
来源：http://kv.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dt.shtwfgs.cn

[R59] 发 POST JSON
来源：http://kp.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pd.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://ft.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xr.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://bu.yuexingan06.cn

df -h;  du -sh *
来源：http://zh.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://dc.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://cr.bjjhwx.cn

[R63] 内存与进程
来源：http://dw.yuntaijiaju.cn

free -h;  ps aux | grep nginx
来源：http://vo.muxihuayi.cn

[R64] 结束进程
来源：http://rt.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://rg.521024.cn

[R65] 查看端口占用
来源：http://vf.jctech888.com.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://im.9csxet.cn

[R66] 定时任务
来源：http://nf.hahajie.cn

crontab -e;  crontab -l
来源：http://is.jctech888.com.cn

[R67] 生成随机十六进制串
来源：http://cq.huanxung.cn

openssl rand -hex 16
来源：http://cm.lnxyls.cn

[R68] 计算文件校验值
来源：http://xa.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://is.nszjky.cn

[R69] 生成随机密码
来源：http://ik.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://uu.521024.cn

[R70] 时间戳与互转
来源：http://yo.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://hf.muxihuayi.cn

[R71] 日期格式化
来源：http://in.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uv.panjiajie.cn

[R72] 等待端口就绪
来源：http://si.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kn.nszjky.cn

[R73] 分割大日志
来源：http://tf.9csxet.cn

split -l 1000 big.log part_
来源：http://sp.panjiajie.cn

[R74] 批量重命名
来源：http://na.shxzskj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ul.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://lf.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://fg.lnxyls.cn

[R76] 使用临时文件
来源：http://zm.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hg.wgjwhj.cn

[R77] 读取用户输入
来源：http://kg.hnjuh.cn

read -rp "请输入: " ans
来源：http://mx.chemitech.net.cn

[R78] 交互式菜单
来源：http://ml.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oa.szsharing.cn

[R79] 解析命令行选项
来源：http://sq.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ze.shxzukj.cn

[R80] 查看脚本执行耗时
来源：http://nz.shtwfgs.cn

time ./run.sh
来源：http://wq.shtwfgs.cn

================================================================================
来源：http://bj.szsharing.cn

S. C / C++ 专题
来源：http://dx.yuntaijiaju.cn

================================================================================
来源：http://jq.huixinmuqiang.cn

[S01] C：Hello World
来源：http://tg.521024.cn

#include <stdio.h>
来源：http://np.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://it.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://fo.shxzukj.cn

int a = 10; printf("%d\n", a);
来源：http://se.shtwfgs.cn

[S03] C：读入整数
来源：http://rg.521024.cn

int x; scanf("%d", &x);
来源：http://se.shtwfgs.cn

[S04] C：字符串复制
来源：http://gq.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ma.huixiangedu.cn

[S05] C：字符串长度
来源：http://hl.yuexingan06.cn

strlen(s)
来源：http://ma.chemitech.net.cn

[S06] C：字符串比较
来源：http://qg.nszjky.cn

strcmp(a, b) == 0
来源：http://br.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://ad.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pq.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://lm.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://av.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://de.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jn.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://em.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://aq.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://ue.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://lo.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dm.huixinmuqiang.cn

fclose(f);
来源：http://xd.colortex.cn

[S12] C：写文件
来源：http://jc.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://px.huixiangedu.cn

[S13] C：宏定义
来源：http://ix.hnjuh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bq.hnjuh.cn

[S14] C：枚举
来源：http://kd.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://io.hnjuh.cn

[S15] C：类型转换
来源：http://ai.bjjhwx.cn

(double) a / b
来源：http://yp.bjjhwx.cn

[S16] C：位操作置位
来源：http://pv.jctech888.com.cn

x |= (1 << 3);
来源：http://fp.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://oo.muxihuayi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://se.yuexingan06.cn

[S18] C：命令行参数
来源：http://mz.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://qo.lnxyls.cn

[S19] C：快速排序
来源：http://aw.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bh.bjjhwx.cn

[S20] C：二分查找
来源：http://mh.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cs.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://tt.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xr.szsharing.cn

[S22] C：字符串转数字
来源：http://of.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hw.huixiangedu.cn

[S23] C：随机数
来源：http://ag.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hm.yuexingan06.cn

[S24] C：获取本地时间
来源：http://bb.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://im.wgjwhj.cn

[S25] C：内存拷贝
来源：http://zu.wgjwhj.cn

memcpy(dst, src, n);
来源：http://nz.yuntaijiaju.cn

[S26] C：内存清零
来源：http://ra.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://iu.shxzukj.cn

[S27] C：定义常量
来源：http://ca.colortex.cn

const double PI = 3.14159;
来源：http://qt.shxzskj.cn

[S28] C：静态变量
来源：http://lj.huixiangedu.cn

static int counter = 0;
来源：http://ud.huixiangedu.cn

[S29] C：变参函数
来源：http://yg.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vr.wgjwhj.cn

[S30] C：头文件保护
来源：http://sb.newstarts.cn

#ifndef X_H
来源：http://cx.lnxyls.cn

#define X_H
来源：http://tg.szxytkj.cn

#endif
来源：http://ye.panjiajie.cn

[S31] C++：Hello World
来源：http://qk.asd995.cn

#include <iostream>
来源：http://ot.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://hp.9csxet.cn

[S32] C++：字符串
来源：http://vc.hahajie.cn

std::string s = "hi";  s += "!";
来源：http://nz.shtwfgs.cn

[S33] C++：vector 增删
来源：http://wp.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wr.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://xg.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://az.huanxung.cn

[S35] C++：map
来源：http://wr.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pt.nszjky.cn

[S36] C++：unordered_map
来源：http://jd.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wt.shxzukj.cn

[S37] C++：set
来源：http://dk.jctech888.com.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eg.shxzskj.cn

[S38] C++：排序
来源：http://ad.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://vu.colortex.cn

[S39] C++：自定义比较器排序
来源：http://uc.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pn.huixiangedu.cn

[S40] C++：查找元素
来源：http://ya.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hj.colortex.cn

[S41] C++：类与构造函数
来源：http://fh.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yj.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://dv.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://fe.chemitech.net.cn

[S43] C++：智能指针
来源：http://ij.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://so.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://ic.nicolike.cn

void inc(int &x) { ++x; }
来源：http://df.9csxet.cn

[S45] C++：lambda
来源：http://cw.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xd.panjiajie.cn

[S46] C++：函数模板
来源：http://gl.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ld.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://ia.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sg.gzmigu.cn

[S48] C++：逐行读文件
来源：http://za.shxzskj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bb.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://cg.9csxet.cn

[S49] C++：写文件
来源：http://hv.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qx.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://mi.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://af.shxzukj.cn

[S51] C++：显式类型转换
来源：http://xa.hahajie.cn

static_cast<double>(a) / b
来源：http://wf.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://ph.szsharing.cn

int size() const noexcept { return n_; }
来源：http://pz.shxzukj.cn

[S53] C++：移动语义
来源：http://uw.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://gy.shxzskj.cn

[S54] C++：异常处理
来源：http://xm.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kz.asd995.cn

[S55] C++：结构化绑定
来源：http://wy.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ki.colortex.cn

[S56] C++：optional
来源：http://xx.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://va.chemitech.net.cn

[S57] C++：编译期常量
来源：http://cg.9csxet.cn

constexpr int N = 10;
来源：http://wo.9csxet.cn

[S58] C++：命名空间
来源：http://tp.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://es.shxzukj.cn

[S59] C++：静态断言
来源：http://vz.shtwfgs.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yw.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://ya.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fd.shxzukj.cn

================================================================================
来源：http://ci.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nl.huixiangedu.cn

================================================================================
来源：http://qh.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://zd.bjjhwx.cn

println("Hello")
来源：http://xb.panjiajie.cn

[T02] Kotlin：变量
来源：http://go.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vi.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://as.jctech888.com.cn

"值: $b"
来源：http://kt.521024.cn

[T04] Kotlin：空安全
来源：http://om.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://yy.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://rg.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kd.huanxung.cn

[T06] Kotlin：集合映射
来源：http://cy.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jm.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://re.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dq.bookmarksfly.cn

[T08] Kotlin：数据类
来源：http://tu.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://wn.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://bw.colortex.cn

fun String.exclaim() = this + "!"
来源：http://ao.colortex.cn

[T10] Kotlin：默认参数
来源：http://oi.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tr.9csxet.cn

[T11] Kotlin：协程
来源：http://xi.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://im.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://ei.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://ux.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://hy.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://lv.szxytkj.cn

[T14] Kotlin：循环
来源：http://ir.521024.cn

for (i in 1..10) println(i)
来源：http://rs.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://yz.nicolike.cn

interface Shape { fun area(): Double }
来源：http://rd.gzmigu.cn

[T16] Swift：Hello World
来源：http://ls.jianghongdianzi.cn

print("Hello")
来源：http://ys.9csxet.cn

[T17] Swift：变量与常量
来源：http://nx.colortex.cn

var a = 1;  let b = 2
来源：http://va.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://gt.szxytkj.cn

"值: \(b)"
来源：http://pb.colortex.cn

[T19] Swift：可选绑定
来源：http://mc.hahajie.cn

if let n = opt { print(n) }
来源：http://wp.yuexingan06.cn

[T20] Swift：数组操作
来源：http://tz.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wr.asd995.cn

[T21] Swift：遍历
来源：http://hn.wgjwhj.cn

for x in a { print(x) }
来源：http://jo.jianghongdianzi.cn

[T22] Swift：字典
来源：http://hv.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wx.wgjwhj.cn

[T23] Swift：函数
来源：http://xb.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qe.bookmarksfly.cn

[T24] Swift：闭包
来源：http://dx.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pp.shxzukj.cn

[T25] Swift：结构体
来源：http://ku.shxzukj.cn

struct P { var x: Int }
来源：http://vs.lnxyls.cn

[T26] Swift：类与重写
来源：http://cc.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://vu.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://rb.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://yr.bjjhwx.cn

[T28] Swift：枚举
来源：http://xs.nicolike.cn

enum Color { case red, green }
来源：http://ip.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://jo.gzmigu.cn

guard let x = opt else { return }
来源：http://nz.jctech888.com.cn

[T30] Swift：协议
来源：http://pf.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://id.lnxyls.cn

[T31] Lua：Hello World
来源：http://ym.nicolike.cn

print("Hello")
来源：http://hk.panjiajie.cn

[T32] Lua：局部变量
来源：http://bw.chemitech.net.cn

local a = 1
来源：http://ow.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://yn.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://he.bjjhwx.cn

[T34] Lua：遍历表
来源：http://sv.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ob.szxytkj.cn

[T35] Lua：字典表
来源：http://gr.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://av.shtwfgs.cn

[T36] Lua：函数
来源：http://zn.panjiajie.cn

function add(a, b) return a + b end
来源：http://im.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://xn.9csxet.cn

"a" .. "b"
来源：http://lu.yuexingan06.cn

[T38] Lua：条件
来源：http://iv.muxihuayi.cn

if x > 0 then print("正") end
来源：http://nr.shtwfgs.cn


<!-- 参考信息 -->