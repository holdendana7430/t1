代发 wailian999

echo $((1 + 2 * 3))
来源：http://tg.huixiangedu.cn

[R28] 浮点运算
来源：http://gi.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://pq.huanxung.cn

[R29] 定义函数
来源：http://ub.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://no.shxzskj.cn

[R30] 函数返回状态码
来源：http://nf.wgjwhj.cn

f() { return 0; }; f || echo "失败了"
来源：http://yr.muxihuayi.cn

[R31] 局部变量
来源：http://ll.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://nj.yuexingan06.cn

[R32] 参数个数校验
来源：http://yu.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qj.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://pa.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ix.shtwfgs.cn

[R34] 退出时清理
来源：http://tf.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ro.gzmigu.cn

[R35] 后台执行并等待
来源：http://ee.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ay.nicolike.cn

[R36] 并发执行多个任务
来源：http://ye.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gj.shxzskj.cn

[R37] 把输出赋给变量
来源：http://fz.wgjwhj.cn

files=$(ls -1)
来源：http://mh.9csxet.cn

[R38] 管道串联
来源：http://mj.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://el.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://pj.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://sp.9csxet.cn

[R40] 追加写日志
来源：http://lz.shxzskj.cn

echo "log" >> out.log
来源：http://ux.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://ii.asd995.cn

cmd >/dev/null 2>&1
来源：http://jz.haigaiapp.cn

[R42] 输入重定向
来源：http://du.huanxung.cn

wc -l < a.txt
来源：http://ar.huixiangedu.cn

[R43] 按名字查找文件
来源：http://gr.haigaiapp.cn

find . -name "*.log" -type f
来源：http://qi.chemitech.net.cn

[R44] 按修改时间查找
来源：http://cq.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://aa.muxihuayi.cn

[R45] 批量删除
来源：http://hs.hnjuh.cn

find . -name "*.tmp" -delete
来源：http://rm.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://lx.hnjuh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ur.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://fw.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dh.9csxet.cn

[R48] awk 取指定列
来源：http://jz.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://pr.szxytkj.cn

[R49] awk 带条件
来源：http://wm.lnxyls.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jo.nicolike.cn

[R50] awk 求和
来源：http://in.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://od.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://hc.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://px.asd995.cn

[R52] 统计行数
来源：http://mk.szxytkj.cn

wc -l a.txt
来源：http://qj.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://po.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cr.chemitech.net.cn

[R54] 比较两个文件
来源：http://rf.lnxyls.cn

diff a.txt b.txt
来源：http://km.nicolike.cn

[R55] 压缩与解压
来源：http://gx.hahajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://eh.521024.cn

[R56] 远程拷贝
来源：http://pd.gzmigu.cn

scp file user@host:/path/
来源：http://ic.jctech888.com.cn

[R57] 远程执行命令
来源：http://ep.jctech888.com.cn

ssh user@host 'uptime'
来源：http://lj.hnjuh.cn

[R58] 下载文件
来源：http://qi.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uu.shtwfgs.cn

[R59] 发 POST JSON
来源：http://sk.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zw.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://le.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dv.shxzskj.cn

[R61] 磁盘占用
来源：http://gn.newstarts.cn

df -h;  du -sh *
来源：http://yk.szsharing.cn

[R62] 找最占空间的文件
来源：http://px.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://qb.yuexingan06.cn

[R63] 内存与进程
来源：http://kx.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://sg.wgjwhj.cn

[R64] 结束进程
来源：http://et.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://xm.haigaiapp.cn

[R65] 查看端口占用
来源：http://te.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://td.yuntaijiaju.cn

[R66] 定时任务
来源：http://px.lnxyls.cn

crontab -e;  crontab -l
来源：http://pc.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://mb.gzmigu.cn

openssl rand -hex 16
来源：http://eh.nszjky.cn

[R68] 计算文件校验值
来源：http://ou.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pu.szsharing.cn

[R69] 生成随机密码
来源：http://gn.9csxet.cn

head -c 16 /dev/urandom | base64
来源：http://cs.bjjhwx.cn

[R70] 时间戳与互转
来源：http://kc.521024.cn

date +%s;  date -d @1700000000
来源：http://ns.jctech888.com.cn

[R71] 日期格式化
来源：http://rm.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vz.szxytkj.cn

[R72] 等待端口就绪
来源：http://py.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hy.szsharing.cn

[R73] 分割大日志
来源：http://zy.newstarts.cn

split -l 1000 big.log part_
来源：http://gu.colortex.cn

[R74] 批量重命名
来源：http://wq.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pf.gzmigu.cn

[R75] 导出环境变量
来源：http://da.hnjuh.cn

export PATH="$HOME/bin:$PATH"
来源：http://vm.bookmarksfly.cn

[R76] 使用临时文件
来源：http://mq.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ej.9csxet.cn

[R77] 读取用户输入
来源：http://nv.colortex.cn

read -rp "请输入: " ans
来源：http://gi.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://go.hahajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kc.huixiangedu.cn

[R79] 解析命令行选项
来源：http://ke.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jz.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://dm.hahajie.cn

time ./run.sh
来源：http://qz.huixiangedu.cn

================================================================================
来源：http://gg.asd995.cn

S. C / C++ 专题
来源：http://mh.shxzskj.cn

================================================================================
来源：http://nc.lnxyls.cn

[S01] C：Hello World
来源：http://ve.hnjuh.cn

#include <stdio.h>
来源：http://ut.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ph.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://fz.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://ar.muxihuayi.cn

[S03] C：读入整数
来源：http://fo.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://xk.shxzskj.cn

[S04] C：字符串复制
来源：http://vo.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kk.shxzskj.cn

[S05] C：字符串长度
来源：http://xa.panjiajie.cn

strlen(s)
来源：http://va.szsharing.cn

[S06] C：字符串比较
来源：http://lk.muxihuayi.cn

strcmp(a, b) == 0
来源：http://dw.huanxung.cn

[S07] C：数组遍历求和
来源：http://jd.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mh.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://wy.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oa.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://yv.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ie.nicolike.cn

[S10] C：指针与解引用
来源：http://kr.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://vo.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://fz.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://wt.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mw.shtwfgs.cn

fclose(f);
来源：http://px.wgjwhj.cn

[S12] C：写文件
来源：http://fe.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zn.9csxet.cn

[S13] C：宏定义
来源：http://ya.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ef.huixinmuqiang.cn

[S14] C：枚举
来源：http://ci.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://ma.shxzskj.cn

[S15] C：类型转换
来源：http://qx.szxytkj.cn

(double) a / b
来源：http://as.huixiangedu.cn

[S16] C：位操作置位
来源：http://gl.nicolike.cn

x |= (1 << 3);
来源：http://cb.colortex.cn

[S17] C：安全拼接字符串
来源：http://zq.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ui.521024.cn

[S18] C：命令行参数
来源：http://td.jctech888.com.cn

int main(int argc, char **argv)
来源：http://xf.hnjuh.cn

[S19] C：快速排序
来源：http://bb.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hv.shxzukj.cn

[S20] C：二分查找
来源：http://iw.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://py.hahajie.cn

[S21] C：字符类别判断
来源：http://vk.wgjwhj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://az.nicolike.cn

[S22] C：字符串转数字
来源：http://gm.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ys.hahajie.cn

[S23] C：随机数
来源：http://od.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kf.colortex.cn

[S24] C：获取本地时间
来源：http://nf.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jq.nicolike.cn

[S25] C：内存拷贝
来源：http://sb.szxytkj.cn

memcpy(dst, src, n);
来源：http://bh.wgjwhj.cn

[S26] C：内存清零
来源：http://qr.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://kz.chemitech.net.cn

[S27] C：定义常量
来源：http://wt.muxihuayi.cn

const double PI = 3.14159;
来源：http://ye.nicolike.cn

[S28] C：静态变量
来源：http://nd.szxytkj.cn

static int counter = 0;
来源：http://wu.haigaiapp.cn

[S29] C：变参函数
来源：http://ma.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rk.szxytkj.cn

[S30] C：头文件保护
来源：http://md.hahajie.cn

#ifndef X_H
来源：http://rg.jianghongdianzi.cn

#define X_H
来源：http://sq.shxzskj.cn

#endif
来源：http://qu.huixiangedu.cn

[S31] C++：Hello World
来源：http://lz.yuntaijiaju.cn

#include <iostream>
来源：http://qu.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://mb.shxzukj.cn

[S32] C++：字符串
来源：http://pa.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://bu.yuexingan06.cn

[S33] C++：vector 增删
来源：http://zp.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yr.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://df.yuntaijiaju.cn

for (auto &x : v) { std::cout << x; }
来源：http://ce.szsharing.cn

[S35] C++：map
来源：http://qe.lnxyls.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yg.szsharing.cn

[S36] C++：unordered_map
来源：http://yy.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://se.huixiangedu.cn

[S37] C++：set
来源：http://mn.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://co.hnjuh.cn

[S38] C++：排序
来源：http://uv.asd995.cn

std::sort(v.begin(), v.end());
来源：http://oc.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://ty.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mz.wgjwhj.cn

[S40] C++：查找元素
来源：http://sp.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cz.shxzukj.cn

[S41] C++：类与构造函数
来源：http://pz.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sa.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://fs.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://cd.newstarts.cn

[S43] C++：智能指针
来源：http://zi.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://sn.huanxung.cn

[S44] C++：引用传参
来源：http://lw.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://cm.hnjuh.cn

[S45] C++：lambda
来源：http://yp.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qc.chemitech.net.cn

[S46] C++：函数模板
来源：http://tb.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://el.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://gv.huanxung.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xf.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://bs.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://un.asd995.cn

while (std::getline(in, line)) { }
来源：http://jr.nszjky.cn

[S49] C++：写文件
来源：http://tu.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kx.panjiajie.cn

[S50] C++：格式化数字
来源：http://io.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qg.panjiajie.cn

[S51] C++：显式类型转换
来源：http://tv.szsharing.cn

static_cast<double>(a) / b
来源：http://bn.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://xm.asd995.cn

int size() const noexcept { return n_; }
来源：http://ny.chemitech.net.cn

[S53] C++：移动语义
来源：http://gm.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://wh.gzmigu.cn

[S54] C++：异常处理
来源：http://kf.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fx.lnxyls.cn

[S55] C++：结构化绑定
来源：http://qm.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://co.9csxet.cn

[S56] C++：optional
来源：http://ob.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ta.szsharing.cn

[S57] C++：编译期常量
来源：http://bf.jctech888.com.cn

constexpr int N = 10;
来源：http://lg.haigaiapp.cn

[S58] C++：命名空间
来源：http://wm.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://cv.hahajie.cn

[S59] C++：静态断言
来源：http://by.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bl.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://kk.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jq.nszjky.cn

================================================================================
来源：http://tz.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://as.colortex.cn

================================================================================
来源：http://uu.newstarts.cn

[T01] Kotlin：Hello World
来源：http://ki.bjjhwx.cn

println("Hello")
来源：http://cj.huixiangedu.cn

[T02] Kotlin：变量
来源：http://up.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qq.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://au.panjiajie.cn

"值: $b"
来源：http://ia.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://to.nicolike.cn

val n: String? = null;  n?.length
来源：http://lt.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://go.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xq.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://zp.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://op.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://gg.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jl.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://wa.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://fj.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://dd.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://qa.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://oa.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qv.panjiajie.cn

[T11] Kotlin：协程
来源：http://ma.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yy.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://fv.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://xh.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://kg.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://bk.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://nn.hahajie.cn

for (i in 1..10) println(i)
来源：http://xo.9csxet.cn

[T15] Kotlin：接口
来源：http://pn.newstarts.cn

interface Shape { fun area(): Double }
来源：http://mf.panjiajie.cn

[T16] Swift：Hello World
来源：http://po.gzmigu.cn

print("Hello")
来源：http://xs.asd995.cn

[T17] Swift：变量与常量
来源：http://hn.hnjuh.cn

var a = 1;  let b = 2
来源：http://xw.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://mo.nszjky.cn

"值: \(b)"
来源：http://gc.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://xb.shtwfgs.cn

if let n = opt { print(n) }
来源：http://xy.nszjky.cn

[T20] Swift：数组操作
来源：http://ss.gzmigu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bz.colortex.cn

[T21] Swift：遍历
来源：http://sv.nicolike.cn

for x in a { print(x) }
来源：http://bb.huixinmuqiang.cn

[T22] Swift：字典
来源：http://sr.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bd.muxihuayi.cn

[T23] Swift：函数
来源：http://pi.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rq.hnjuh.cn

[T24] Swift：闭包
来源：http://hw.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mw.wgjwhj.cn

[T25] Swift：结构体
来源：http://el.nszjky.cn

struct P { var x: Int }
来源：http://sd.hahajie.cn

[T26] Swift：类与重写
来源：http://ur.huanxung.cn

class A: Base { override func f() {} }
来源：http://xw.9csxet.cn

[T27] Swift：错误处理
来源：http://tb.asd995.cn

do { try f() } catch { print(error) }
来源：http://rp.wgjwhj.cn

[T28] Swift：枚举
来源：http://kv.huanxung.cn

enum Color { case red, green }
来源：http://tm.colortex.cn

[T29] Swift：guard 提前返回
来源：http://bc.jctech888.com.cn

guard let x = opt else { return }
来源：http://da.wgjwhj.cn

[T30] Swift：协议
来源：http://za.521024.cn

protocol Shape { func area() -> Double }
来源：http://kr.szxytkj.cn


<!-- 参考信息 -->