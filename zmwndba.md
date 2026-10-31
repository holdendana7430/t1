代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://ao.gzmigu.cn

[R32] 参数个数校验
来源：http://av.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rz.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://re.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bi.huanxung.cn

[R34] 退出时清理
来源：http://qs.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cg.haigaiapp.cn

[R35] 后台执行并等待
来源：http://sk.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qc.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://tz.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dy.bjjhwx.cn

[R37] 把输出赋给变量
来源：http://qz.521024.cn

files=$(ls -1)
来源：http://xa.bookmarksfly.cn

[R38] 管道串联
来源：http://kj.nicolike.cn

cat a.txt | grep -i error | wc -l
来源：http://zs.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://rh.9csxet.cn

cmd > out.log 2>&1
来源：http://ww.huanxung.cn

[R40] 追加写日志
来源：http://bu.yuntaijiaju.cn

echo "log" >> out.log
来源：http://nm.szsharing.cn

[R41] 丢弃输出
来源：http://ns.nszjky.cn

cmd >/dev/null 2>&1
来源：http://lu.shtwfgs.cn

[R42] 输入重定向
来源：http://ni.huanxung.cn

wc -l < a.txt
来源：http://gu.jctech888.com.cn

[R43] 按名字查找文件
来源：http://kr.shxzskj.cn

find . -name "*.log" -type f
来源：http://dp.huanxung.cn

[R44] 按修改时间查找
来源：http://ah.colortex.cn

find . -mtime -7 -type f
来源：http://dt.bookmarksfly.cn

[R45] 批量删除
来源：http://ei.9csxet.cn

find . -name "*.tmp" -delete
来源：http://ql.lnxyls.cn

[R46] 递归替换文件内容
来源：http://zv.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wo.wgjwhj.cn

[R47] sed 单行替换
来源：http://lx.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dd.9csxet.cn

[R48] awk 取指定列
来源：http://il.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://id.521024.cn

[R49] awk 带条件
来源：http://mq.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zh.bjjhwx.cn

[R50] awk 求和
来源：http://mn.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wu.9csxet.cn

[R51] 排序去重取前几
来源：http://lc.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://el.gzmigu.cn

[R52] 统计行数
来源：http://pr.bjjhwx.cn

wc -l a.txt
来源：http://vy.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://ys.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qg.hnjuh.cn

[R54] 比较两个文件
来源：http://pd.huixiangedu.cn

diff a.txt b.txt
来源：http://cc.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://zu.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://of.chemitech.net.cn

[R56] 远程拷贝
来源：http://cq.hnjuh.cn

scp file user@host:/path/
来源：http://xh.hahajie.cn

[R57] 远程执行命令
来源：http://bo.lnxyls.cn

ssh user@host 'uptime'
来源：http://mb.shtwfgs.cn

[R58] 下载文件
来源：http://vw.bjjhwx.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bm.szxytkj.cn

[R59] 发 POST JSON
来源：http://em.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gf.colortex.cn

[R60] 只看 HTTP 状态码
来源：http://gk.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qy.nicolike.cn

[R61] 磁盘占用
来源：http://an.bookmarksfly.cn

df -h;  du -sh *
来源：http://oe.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://vq.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://zw.jctech888.com.cn

[R63] 内存与进程
来源：http://yh.haigaiapp.cn

free -h;  ps aux | grep nginx
来源：http://kr.szsharing.cn

[R64] 结束进程
来源：http://yx.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://bp.nicolike.cn

[R65] 查看端口占用
来源：http://yh.szxytkj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hb.huixiangedu.cn

[R66] 定时任务
来源：http://mr.shxzskj.cn

crontab -e;  crontab -l
来源：http://dw.nicolike.cn

[R67] 生成随机十六进制串
来源：http://au.nszjky.cn

openssl rand -hex 16
来源：http://zq.muxihuayi.cn

[R68] 计算文件校验值
来源：http://dp.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mf.521024.cn

[R69] 生成随机密码
来源：http://gg.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://ay.asd995.cn

[R70] 时间戳与互转
来源：http://fv.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://kb.colortex.cn

[R71] 日期格式化
来源：http://xx.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://so.huixinmuqiang.cn

[R72] 等待端口就绪
来源：http://za.huixinmuqiang.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://iw.nszjky.cn

[R73] 分割大日志
来源：http://rb.shtwfgs.cn

split -l 1000 big.log part_
来源：http://li.bjjhwx.cn

[R74] 批量重命名
来源：http://qy.gzmigu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hr.szsharing.cn

[R75] 导出环境变量
来源：http://ug.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://bg.huixiangedu.cn

[R76] 使用临时文件
来源：http://ny.jianghongdianzi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xs.chemitech.net.cn

[R77] 读取用户输入
来源：http://js.shxzukj.cn

read -rp "请输入: " ans
来源：http://pk.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://tw.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yk.gzmigu.cn

[R79] 解析命令行选项
来源：http://vb.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ro.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://of.colortex.cn

time ./run.sh
来源：http://ae.bjjhwx.cn

================================================================================
来源：http://pn.shtwfgs.cn

S. C / C++ 专题
来源：http://oc.bjjhwx.cn

================================================================================
来源：http://zo.bookmarksfly.cn

[S01] C：Hello World
来源：http://cn.colortex.cn

#include <stdio.h>
来源：http://zw.huixiangedu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mz.szxytkj.cn

[S02] C：变量与格式化输出
来源：http://az.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://yx.jianghongdianzi.cn

[S03] C：读入整数
来源：http://qn.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://et.bookmarksfly.cn

[S04] C：字符串复制
来源：http://ci.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fx.panjiajie.cn

[S05] C：字符串长度
来源：http://me.nicolike.cn

strlen(s)
来源：http://ku.shtwfgs.cn

[S06] C：字符串比较
来源：http://gn.asd995.cn

strcmp(a, b) == 0
来源：http://ud.jctech888.com.cn

[S07] C：数组遍历求和
来源：http://wd.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ii.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://bv.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://un.bjjhwx.cn

[S09] C：结构体定义与初始化
来源：http://sg.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cf.nicolike.cn

[S10] C：指针与解引用
来源：http://ij.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://sq.nicolike.cn

[S11] C：逐行读文件
来源：http://ii.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://so.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jv.panjiajie.cn

fclose(f);
来源：http://pc.wgjwhj.cn

[S12] C：写文件
来源：http://ci.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hw.hahajie.cn

[S13] C：宏定义
来源：http://bi.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ig.bjjhwx.cn

[S14] C：枚举
来源：http://qz.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://lk.muxihuayi.cn

[S15] C：类型转换
来源：http://lk.bjjhwx.cn

(double) a / b
来源：http://ke.szxytkj.cn

[S16] C：位操作置位
来源：http://xq.newstarts.cn

x |= (1 << 3);
来源：http://oh.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://ma.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ak.gzmigu.cn

[S18] C：命令行参数
来源：http://pg.9csxet.cn

int main(int argc, char **argv)
来源：http://bw.9csxet.cn

[S19] C：快速排序
来源：http://nt.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ie.yuntaijiaju.cn

[S20] C：二分查找
来源：http://aa.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uf.hahajie.cn

[S21] C：字符类别判断
来源：http://sa.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hh.yuexingan06.cn

[S22] C：字符串转数字
来源：http://uh.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cw.nszjky.cn

[S23] C：随机数
来源：http://cj.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ct.haigaiapp.cn

[S24] C：获取本地时间
来源：http://ek.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ci.jctech888.com.cn

[S25] C：内存拷贝
来源：http://kv.jctech888.com.cn

memcpy(dst, src, n);
来源：http://nu.nszjky.cn

[S26] C：内存清零
来源：http://xk.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://xx.bookmarksfly.cn

[S27] C：定义常量
来源：http://id.jctech888.com.cn

const double PI = 3.14159;
来源：http://wk.bookmarksfly.cn

[S28] C：静态变量
来源：http://uf.yuexingan06.cn

static int counter = 0;
来源：http://zs.wgjwhj.cn

[S29] C：变参函数
来源：http://bz.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://an.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://hr.521024.cn

#ifndef X_H
来源：http://ix.colortex.cn

#define X_H
来源：http://lz.gzmigu.cn

#endif
来源：http://gf.panjiajie.cn

[S31] C++：Hello World
来源：http://mj.huanxung.cn

#include <iostream>
来源：http://pc.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://qn.nicolike.cn

[S32] C++：字符串
来源：http://bj.colortex.cn

std::string s = "hi";  s += "!";
来源：http://nd.huixiangedu.cn

[S33] C++：vector 增删
来源：http://nk.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://np.shxzukj.cn

[S34] C++：遍历 vector
来源：http://iv.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://zx.szsharing.cn

[S35] C++：map
来源：http://jv.lnxyls.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qa.lnxyls.cn

[S36] C++：unordered_map
来源：http://uv.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cf.bjjhwx.cn

[S37] C++：set
来源：http://zb.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gg.hahajie.cn

[S38] C++：排序
来源：http://gj.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://vg.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://te.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vo.lnxyls.cn

[S40] C++：查找元素
来源：http://pm.nicolike.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uk.szxytkj.cn

[S41] C++：类与构造函数
来源：http://wh.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nv.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://uf.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://ko.hnjuh.cn

[S43] C++：智能指针
来源：http://dv.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://tb.9csxet.cn

[S44] C++：引用传参
来源：http://nd.9csxet.cn

void inc(int &x) { ++x; }
来源：http://uk.shtwfgs.cn

[S45] C++：lambda
来源：http://ve.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ef.bjjhwx.cn

[S46] C++：函数模板
来源：http://ii.yuntaijiaju.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ad.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://ou.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ef.hahajie.cn

[S48] C++：逐行读文件
来源：http://fp.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ac.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://mr.521024.cn

[S49] C++：写文件
来源：http://cy.huixinmuqiang.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tw.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://nd.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pp.huanxung.cn

[S51] C++：显式类型转换
来源：http://xz.521024.cn

static_cast<double>(a) / b
来源：http://ll.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://vv.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://ay.panjiajie.cn

[S53] C++：移动语义
来源：http://kr.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://mj.yuexingan06.cn

[S54] C++：异常处理
来源：http://gq.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ix.colortex.cn

[S55] C++：结构化绑定
来源：http://aj.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tt.bjjhwx.cn

[S56] C++：optional
来源：http://cq.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sk.huixiangedu.cn

[S57] C++：编译期常量
来源：http://rd.jianghongdianzi.cn

constexpr int N = 10;
来源：http://bu.wgjwhj.cn

[S58] C++：命名空间
来源：http://vp.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://zj.huixiangedu.cn

[S59] C++：静态断言
来源：http://dx.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bd.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://li.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uf.jianghongdianzi.cn

================================================================================
来源：http://bj.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qe.huixiangedu.cn

================================================================================
来源：http://ic.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://zs.huixinmuqiang.cn

println("Hello")
来源：http://so.nicolike.cn

[T02] Kotlin：变量
来源：http://oc.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yi.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://ct.szxytkj.cn

"值: $b"
来源：http://pi.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://gg.9csxet.cn

val n: String? = null;  n?.length
来源：http://oj.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://fv.9csxet.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wn.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://lm.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rx.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://kx.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ku.bookmarksfly.cn

[T08] Kotlin：数据类
来源：http://pq.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://ui.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://yk.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://ge.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://hc.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zt.haigaiapp.cn

[T11] Kotlin：协程
来源：http://bx.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kh.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://sq.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://jf.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://gg.colortex.cn

val m = mapOf("a" to 1)
来源：http://ez.huixiangedu.cn

[T14] Kotlin：循环
来源：http://wo.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://fz.nszjky.cn

[T15] Kotlin：接口
来源：http://jw.asd995.cn

interface Shape { fun area(): Double }
来源：http://ox.chemitech.net.cn

[T16] Swift：Hello World
来源：http://eo.nszjky.cn

print("Hello")
来源：http://mv.nszjky.cn

[T17] Swift：变量与常量
来源：http://fz.nicolike.cn

var a = 1;  let b = 2
来源：http://ck.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://ds.521024.cn

"值: \(b)"
来源：http://fr.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://mj.nszjky.cn

if let n = opt { print(n) }
来源：http://xe.shxzskj.cn

[T20] Swift：数组操作
来源：http://lb.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rg.hnjuh.cn

[T21] Swift：遍历
来源：http://gs.huixiangedu.cn

for x in a { print(x) }
来源：http://hs.szxytkj.cn

[T22] Swift：字典
来源：http://it.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uf.lnxyls.cn

[T23] Swift：函数
来源：http://cn.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rs.shxzskj.cn

[T24] Swift：闭包
来源：http://qy.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qy.nicolike.cn

[T25] Swift：结构体
来源：http://it.newstarts.cn

struct P { var x: Int }
来源：http://ar.nszjky.cn

[T26] Swift：类与重写
来源：http://qg.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://ya.hahajie.cn

[T27] Swift：错误处理
来源：http://kk.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://ei.huixiangedu.cn

[T28] Swift：枚举
来源：http://eu.chemitech.net.cn

enum Color { case red, green }
来源：http://lf.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://nk.haigaiapp.cn

guard let x = opt else { return }
来源：http://qw.panjiajie.cn

[T30] Swift：协议
来源：http://go.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://ys.huixiangedu.cn

[T31] Lua：Hello World
来源：http://hd.hahajie.cn

print("Hello")
来源：http://ca.jctech888.com.cn

[T32] Lua：局部变量
来源：http://qo.huixiangedu.cn

local a = 1
来源：http://fu.gzmigu.cn

[T33] Lua：表（数组）
来源：http://jq.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ve.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://qm.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ta.nicolike.cn


<!-- 参考信息 -->