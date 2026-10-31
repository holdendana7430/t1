代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://cb.yuntaijiaju.cn

[R26] 命令替换
来源：http://bb.huixiangedu.cn

now=$(date +%F); echo "$now"
来源：http://hq.9csxet.cn

[R27] 算术展开
来源：http://id.newstarts.cn

echo $((1 + 2 * 3))
来源：http://gs.huixiangedu.cn

[R28] 浮点运算
来源：http://pd.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://zc.521024.cn

[R29] 定义函数
来源：http://ya.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gm.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://pw.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://pa.szxytkj.cn

[R31] 局部变量
来源：http://ce.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://nx.huixiangedu.cn

[R32] 参数个数校验
来源：http://ps.chemitech.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tt.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://zp.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xl.huixiangedu.cn

[R34] 退出时清理
来源：http://nn.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://za.9csxet.cn

[R35] 后台执行并等待
来源：http://nn.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ug.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://gh.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ki.szxytkj.cn

[R37] 把输出赋给变量
来源：http://fs.panjiajie.cn

files=$(ls -1)
来源：http://km.bjjhwx.cn

[R38] 管道串联
来源：http://se.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://mu.yuexingan06.cn

[R39] 重定向标准输出与错误
来源：http://mh.asd995.cn

cmd > out.log 2>&1
来源：http://qi.bjjhwx.cn

[R40] 追加写日志
来源：http://qa.chemitech.net.cn

echo "log" >> out.log
来源：http://hv.yuexingan06.cn

[R41] 丢弃输出
来源：http://wj.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://zd.newstarts.cn

[R42] 输入重定向
来源：http://ie.huixiangedu.cn

wc -l < a.txt
来源：http://ii.szsharing.cn

[R43] 按名字查找文件
来源：http://ng.hnjuh.cn

find . -name "*.log" -type f
来源：http://xe.bjjhwx.cn

[R44] 按修改时间查找
来源：http://mh.panjiajie.cn

find . -mtime -7 -type f
来源：http://vt.jctech888.com.cn

[R45] 批量删除
来源：http://cx.nicolike.cn

find . -name "*.tmp" -delete
来源：http://ey.newstarts.cn

[R46] 递归替换文件内容
来源：http://wk.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ri.haigaiapp.cn

[R47] sed 单行替换
来源：http://wk.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ro.szxytkj.cn

[R48] awk 取指定列
来源：http://fl.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://uj.colortex.cn

[R49] awk 带条件
来源：http://of.lnxyls.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fg.lnxyls.cn

[R50] awk 求和
来源：http://pb.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://su.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://nq.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ah.shxzskj.cn

[R52] 统计行数
来源：http://hd.shxzskj.cn

wc -l a.txt
来源：http://bb.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://cd.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kt.szsharing.cn

[R54] 比较两个文件
来源：http://vk.huanxung.cn

diff a.txt b.txt
来源：http://ch.jctech888.com.cn

[R55] 压缩与解压
来源：http://lo.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bd.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://rb.shxzukj.cn

scp file user@host:/path/
来源：http://xm.lnxyls.cn

[R57] 远程执行命令
来源：http://hd.wgjwhj.cn

ssh user@host 'uptime'
来源：http://gv.muxihuayi.cn

[R58] 下载文件
来源：http://et.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jz.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://ff.521024.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://it.jianghongdianzi.cn

[R60] 只看 HTTP 状态码
来源：http://nz.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qa.huixiangedu.cn

[R61] 磁盘占用
来源：http://au.chemitech.net.cn

df -h;  du -sh *
来源：http://lx.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://tw.chemitech.net.cn

du -ah . | sort -rh | head -10
来源：http://if.panjiajie.cn

[R63] 内存与进程
来源：http://tn.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://dh.huanxung.cn

[R64] 结束进程
来源：http://ca.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://jr.gzmigu.cn

[R65] 查看端口占用
来源：http://pt.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mn.szxytkj.cn

[R66] 定时任务
来源：http://lo.lnxyls.cn

crontab -e;  crontab -l
来源：http://ze.nicolike.cn

[R67] 生成随机十六进制串
来源：http://ih.asd995.cn

openssl rand -hex 16
来源：http://op.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://hh.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sm.shxzskj.cn

[R69] 生成随机密码
来源：http://xx.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://zp.huanxung.cn

[R70] 时间戳与互转
来源：http://vp.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://rl.hahajie.cn

[R71] 日期格式化
来源：http://lg.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://br.nicolike.cn

[R72] 等待端口就绪
来源：http://ns.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pr.lnxyls.cn

[R73] 分割大日志
来源：http://ok.asd995.cn

split -l 1000 big.log part_
来源：http://kz.asd995.cn

[R74] 批量重命名
来源：http://du.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lm.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://bp.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://hr.huanxung.cn

[R76] 使用临时文件
来源：http://lp.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://od.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://ww.huanxung.cn

read -rp "请输入: " ans
来源：http://gm.colortex.cn

[R78] 交互式菜单
来源：http://rb.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ox.shxzukj.cn

[R79] 解析命令行选项
来源：http://tr.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rg.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://fq.szsharing.cn

time ./run.sh
来源：http://ha.jianghongdianzi.cn

================================================================================
来源：http://dq.hahajie.cn

S. C / C++ 专题
来源：http://sh.panjiajie.cn

================================================================================
来源：http://lo.shxzskj.cn

[S01] C：Hello World
来源：http://ws.wgjwhj.cn

#include <stdio.h>
来源：http://ld.huixiangedu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vh.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://gx.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://bw.huixinmuqiang.cn

[S03] C：读入整数
来源：http://ek.lnxyls.cn

int x; scanf("%d", &x);
来源：http://tl.nszjky.cn

[S04] C：字符串复制
来源：http://tu.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kd.huixiangedu.cn

[S05] C：字符串长度
来源：http://na.szsharing.cn

strlen(s)
来源：http://zh.asd995.cn

[S06] C：字符串比较
来源：http://rw.gzmigu.cn

strcmp(a, b) == 0
来源：http://dc.lnxyls.cn

[S07] C：数组遍历求和
来源：http://ec.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zj.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://hc.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pn.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://yf.hnjuh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tw.haigaiapp.cn

[S10] C：指针与解引用
来源：http://vn.hahajie.cn

int *p = &a;  *p = 5;
来源：http://do.wgjwhj.cn

[S11] C：逐行读文件
来源：http://dx.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://pc.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ro.shtwfgs.cn

fclose(f);
来源：http://yy.colortex.cn

[S12] C：写文件
来源：http://yp.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rg.nszjky.cn

[S13] C：宏定义
来源：http://le.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oa.lnxyls.cn

[S14] C：枚举
来源：http://zq.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://fh.yuexingan06.cn

[S15] C：类型转换
来源：http://bb.hahajie.cn

(double) a / b
来源：http://tc.521024.cn

[S16] C：位操作置位
来源：http://xx.huixinmuqiang.cn

x |= (1 << 3);
来源：http://ez.newstarts.cn

[S17] C：安全拼接字符串
来源：http://zo.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://um.wgjwhj.cn

[S18] C：命令行参数
来源：http://kn.hahajie.cn

int main(int argc, char **argv)
来源：http://th.muxihuayi.cn

[S19] C：快速排序
来源：http://ak.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mk.yuntaijiaju.cn

[S20] C：二分查找
来源：http://xk.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zf.521024.cn

[S21] C：字符类别判断
来源：http://ve.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hv.yuexingan06.cn

[S22] C：字符串转数字
来源：http://fk.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ut.newstarts.cn

[S23] C：随机数
来源：http://rc.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rm.shxzukj.cn

[S24] C：获取本地时间
来源：http://yl.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jp.panjiajie.cn

[S25] C：内存拷贝
来源：http://va.gzmigu.cn

memcpy(dst, src, n);
来源：http://mn.huixiangedu.cn

[S26] C：内存清零
来源：http://rn.huanxung.cn

memset(a, 0, sizeof a);
来源：http://cr.jianghongdianzi.cn

[S27] C：定义常量
来源：http://ka.colortex.cn

const double PI = 3.14159;
来源：http://pg.jianghongdianzi.cn

[S28] C：静态变量
来源：http://sw.huanxung.cn

static int counter = 0;
来源：http://cd.hnjuh.cn

[S29] C：变参函数
来源：http://ru.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://un.shxzukj.cn

[S30] C：头文件保护
来源：http://vu.hnjuh.cn

#ifndef X_H
来源：http://ti.nicolike.cn

#define X_H
来源：http://cq.gzmigu.cn

#endif
来源：http://bq.shxzskj.cn

[S31] C++：Hello World
来源：http://on.huixiangedu.cn

#include <iostream>
来源：http://dq.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://dr.jianghongdianzi.cn

[S32] C++：字符串
来源：http://ij.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://qr.nicolike.cn

[S33] C++：vector 增删
来源：http://am.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wu.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://ad.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://gm.szsharing.cn

[S35] C++：map
来源：http://gv.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kq.haigaiapp.cn

[S36] C++：unordered_map
来源：http://ts.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wo.chemitech.net.cn

[S37] C++：set
来源：http://ca.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nw.bookmarksfly.cn

[S38] C++：排序
来源：http://sj.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://ex.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://wl.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ho.shtwfgs.cn

[S40] C++：查找元素
来源：http://hs.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nv.newstarts.cn

[S41] C++：类与构造函数
来源：http://zu.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yy.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://gh.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://ra.huixiangedu.cn

[S43] C++：智能指针
来源：http://fw.521024.cn

auto p = std::make_unique<int>(5);
来源：http://lv.muxihuayi.cn

[S44] C++：引用传参
来源：http://op.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://zv.bjjhwx.cn

[S45] C++：lambda
来源：http://ri.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://as.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://mr.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ke.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://rd.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://as.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://oe.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ag.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://lv.hahajie.cn

[S49] C++：写文件
来源：http://cr.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://la.shxzukj.cn

[S50] C++：格式化数字
来源：http://wi.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qp.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://zy.hnjuh.cn

static_cast<double>(a) / b
来源：http://sg.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://id.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://ou.szsharing.cn

[S53] C++：移动语义
来源：http://qp.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://li.hnjuh.cn

[S54] C++：异常处理
来源：http://wi.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bu.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://io.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vm.hnjuh.cn

[S56] C++：optional
来源：http://vi.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bd.jctech888.com.cn

[S57] C++：编译期常量
来源：http://rh.521024.cn

constexpr int N = 10;
来源：http://ks.huanxung.cn

[S58] C++：命名空间
来源：http://cn.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://cu.hahajie.cn

[S59] C++：静态断言
来源：http://pv.yuntaijiaju.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://he.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://zr.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ut.hahajie.cn

================================================================================
来源：http://ti.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ma.asd995.cn

================================================================================
来源：http://kk.nszjky.cn

[T01] Kotlin：Hello World
来源：http://um.yuexingan06.cn

println("Hello")
来源：http://jj.chemitech.net.cn

[T02] Kotlin：变量
来源：http://ii.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pl.asd995.cn

[T03] Kotlin：字符串模板
来源：http://of.bjjhwx.cn

"值: $b"
来源：http://zt.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://ej.shxzskj.cn

val n: String? = null;  n?.length
来源：http://mv.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://lz.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qs.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://qm.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pb.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://pd.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zm.panjiajie.cn

[T08] Kotlin：数据类
来源：http://ju.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://yp.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://rj.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://re.nszjky.cn

[T10] Kotlin：默认参数
来源：http://xz.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dd.newstarts.cn

[T11] Kotlin：协程
来源：http://gj.bookmarksfly.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xs.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://ew.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://ng.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://oq.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://nb.9csxet.cn

[T14] Kotlin：循环
来源：http://xf.jctech888.com.cn

for (i in 1..10) println(i)
来源：http://hh.shxzukj.cn

[T15] Kotlin：接口
来源：http://mx.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://yl.shxzukj.cn

[T16] Swift：Hello World
来源：http://bm.chemitech.net.cn

print("Hello")
来源：http://ak.huanxung.cn

[T17] Swift：变量与常量
来源：http://ej.huanxung.cn

var a = 1;  let b = 2
来源：http://uf.bookmarksfly.cn

[T18] Swift：字符串插值
来源：http://km.huixinmuqiang.cn

"值: \(b)"
来源：http://wr.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://nm.newstarts.cn

if let n = opt { print(n) }
来源：http://jy.jctech888.com.cn

[T20] Swift：数组操作
来源：http://vd.shxzskj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ge.szsharing.cn

[T21] Swift：遍历
来源：http://fg.jianghongdianzi.cn

for x in a { print(x) }
来源：http://lx.huanxung.cn

[T22] Swift：字典
来源：http://kq.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://de.huanxung.cn

[T23] Swift：函数
来源：http://vq.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hj.chemitech.net.cn

[T24] Swift：闭包
来源：http://vx.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qp.szxytkj.cn

[T25] Swift：结构体
来源：http://yd.shtwfgs.cn

struct P { var x: Int }
来源：http://cs.nszjky.cn

[T26] Swift：类与重写
来源：http://yl.asd995.cn

class A: Base { override func f() {} }
来源：http://hs.chemitech.net.cn

[T27] Swift：错误处理
来源：http://po.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://mo.bookmarksfly.cn

[T28] Swift：枚举
来源：http://tw.jctech888.com.cn

enum Color { case red, green }
来源：http://xr.szsharing.cn


<!-- 参考信息 -->