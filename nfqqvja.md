代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://fq.shxzskj.cn

[R18] 遍历数组
来源：http://tl.newstarts.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qa.bookmarksfly.cn

[R19] 数组长度
来源：http://zu.nicolike.cn

echo "${#arr[@]}"
来源：http://ae.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://bw.panjiajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qt.jctech888.com.cn

[R21] 字符串长度
来源：http://kb.shxzskj.cn

echo "${#s}"
来源：http://sm.huanxung.cn

[R22] 截取子串
来源：http://ll.9csxet.cn

echo "${s:0:5}"
来源：http://wv.bjjhwx.cn

[R23] 字符串替换
来源：http://fe.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pk.panjiajie.cn

[R24] 大小写转换
来源：http://wp.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gh.wgjwhj.cn

[R25] 去后缀 / 去前缀
来源：http://fw.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kl.jianghongdianzi.cn

[R26] 命令替换
来源：http://dx.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://hn.bookmarksfly.cn

[R27] 算术展开
来源：http://ni.bookmarksfly.cn

echo $((1 + 2 * 3))
来源：http://vz.szsharing.cn

[R28] 浮点运算
来源：http://ly.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://rl.asd995.cn

[R29] 定义函数
来源：http://cn.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nt.hnjuh.cn

[R30] 函数返回状态码
来源：http://da.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://bh.hnjuh.cn

[R31] 局部变量
来源：http://iz.nszjky.cn

f() { local x=1; echo "$x"; }
来源：http://hk.huixiangedu.cn

[R32] 参数个数校验
来源：http://is.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://li.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://dw.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kk.shxzskj.cn

[R34] 退出时清理
来源：http://om.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://av.newstarts.cn

[R35] 后台执行并等待
来源：http://am.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://il.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://te.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://do.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://vu.bookmarksfly.cn

files=$(ls -1)
来源：http://ft.huixiangedu.cn

[R38] 管道串联
来源：http://fb.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://ac.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://zd.panjiajie.cn

cmd > out.log 2>&1
来源：http://sm.newstarts.cn

[R40] 追加写日志
来源：http://xj.newstarts.cn

echo "log" >> out.log
来源：http://di.colortex.cn

[R41] 丢弃输出
来源：http://ab.nszjky.cn

cmd >/dev/null 2>&1
来源：http://sw.shxzskj.cn

[R42] 输入重定向
来源：http://mr.asd995.cn

wc -l < a.txt
来源：http://wf.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://si.panjiajie.cn

find . -name "*.log" -type f
来源：http://wh.asd995.cn

[R44] 按修改时间查找
来源：http://qr.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://ok.panjiajie.cn

[R45] 批量删除
来源：http://vw.szsharing.cn

find . -name "*.tmp" -delete
来源：http://rr.yuexingan06.cn

[R46] 递归替换文件内容
来源：http://np.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oe.yuexingan06.cn

[R47] sed 单行替换
来源：http://tz.bjjhwx.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sh.jctech888.com.cn

[R48] awk 取指定列
来源：http://er.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://ic.huixiangedu.cn

[R49] awk 带条件
来源：http://ff.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zo.huanxung.cn

[R50] awk 求和
来源：http://ef.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xq.haigaiapp.cn

[R51] 排序去重取前几
来源：http://uy.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oa.9csxet.cn

[R52] 统计行数
来源：http://bh.szsharing.cn

wc -l a.txt
来源：http://kd.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://dn.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ad.szsharing.cn

[R54] 比较两个文件
来源：http://yr.shxzskj.cn

diff a.txt b.txt
来源：http://zl.521024.cn

[R55] 压缩与解压
来源：http://gb.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pz.newstarts.cn

[R56] 远程拷贝
来源：http://kv.colortex.cn

scp file user@host:/path/
来源：http://dn.newstarts.cn

[R57] 远程执行命令
来源：http://cs.jctech888.com.cn

ssh user@host 'uptime'
来源：http://na.huixinmuqiang.cn

[R58] 下载文件
来源：http://lf.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ka.colortex.cn

[R59] 发 POST JSON
来源：http://uq.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ez.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://jp.yuntaijiaju.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yr.colortex.cn

[R61] 磁盘占用
来源：http://et.lnxyls.cn

df -h;  du -sh *
来源：http://ru.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://cr.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://ys.shtwfgs.cn

[R63] 内存与进程
来源：http://dz.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://wh.9csxet.cn

[R64] 结束进程
来源：http://ki.nicolike.cn

kill -9 $(pgrep -f app.py)
来源：http://ux.9csxet.cn

[R65] 查看端口占用
来源：http://ae.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hr.colortex.cn

[R66] 定时任务
来源：http://tf.huanxung.cn

crontab -e;  crontab -l
来源：http://vb.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://wl.yuntaijiaju.cn

openssl rand -hex 16
来源：http://yo.lnxyls.cn

[R68] 计算文件校验值
来源：http://cc.lnxyls.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wu.9csxet.cn

[R69] 生成随机密码
来源：http://lx.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://jj.shtwfgs.cn

[R70] 时间戳与互转
来源：http://xb.huixiangedu.cn

date +%s;  date -d @1700000000
来源：http://gl.yuexingan06.cn

[R71] 日期格式化
来源：http://ih.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://om.muxihuayi.cn

[R72] 等待端口就绪
来源：http://gu.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ml.newstarts.cn

[R73] 分割大日志
来源：http://vm.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://kw.chemitech.net.cn

[R74] 批量重命名
来源：http://li.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nu.jctech888.com.cn

[R75] 导出环境变量
来源：http://af.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://wh.panjiajie.cn

[R76] 使用临时文件
来源：http://ip.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://er.szsharing.cn

[R77] 读取用户输入
来源：http://tn.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://dn.colortex.cn

[R78] 交互式菜单
来源：http://wq.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xx.hnjuh.cn

[R79] 解析命令行选项
来源：http://xe.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mf.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://zr.bookmarksfly.cn

time ./run.sh
来源：http://jm.jianghongdianzi.cn

================================================================================
来源：http://db.bookmarksfly.cn

S. C / C++ 专题
来源：http://ig.szxytkj.cn

================================================================================
来源：http://md.newstarts.cn

[S01] C：Hello World
来源：http://xw.huanxung.cn

#include <stdio.h>
来源：http://yp.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mv.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://rj.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://tp.shxzukj.cn

[S03] C：读入整数
来源：http://it.szxytkj.cn

int x; scanf("%d", &x);
来源：http://ae.lnxyls.cn

[S04] C：字符串复制
来源：http://jh.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jk.hahajie.cn

[S05] C：字符串长度
来源：http://em.muxihuayi.cn

strlen(s)
来源：http://ny.colortex.cn

[S06] C：字符串比较
来源：http://un.yuexingan06.cn

strcmp(a, b) == 0
来源：http://cy.jctech888.com.cn

[S07] C：数组遍历求和
来源：http://xy.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dg.asd995.cn

[S08] C：动态内存分配与释放
来源：http://eh.jctech888.com.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tl.bjjhwx.cn

[S09] C：结构体定义与初始化
来源：http://fo.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nn.szsharing.cn

[S10] C：指针与解引用
来源：http://fj.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://ef.521024.cn

[S11] C：逐行读文件
来源：http://cv.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://lw.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jm.wgjwhj.cn

fclose(f);
来源：http://cl.nszjky.cn

[S12] C：写文件
来源：http://nr.hnjuh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ne.521024.cn

[S13] C：宏定义
来源：http://gb.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rs.huanxung.cn

[S14] C：枚举
来源：http://pg.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://bs.haigaiapp.cn

[S15] C：类型转换
来源：http://uz.muxihuayi.cn

(double) a / b
来源：http://sp.yuexingan06.cn

[S16] C：位操作置位
来源：http://sx.nicolike.cn

x |= (1 << 3);
来源：http://gh.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://vl.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rz.shxzukj.cn

[S18] C：命令行参数
来源：http://ya.colortex.cn

int main(int argc, char **argv)
来源：http://je.panjiajie.cn

[S19] C：快速排序
来源：http://ha.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ks.muxihuayi.cn

[S20] C：二分查找
来源：http://zh.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bq.huixiangedu.cn

[S21] C：字符类别判断
来源：http://js.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ap.panjiajie.cn

[S22] C：字符串转数字
来源：http://vw.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xr.nicolike.cn

[S23] C：随机数
来源：http://ky.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ri.asd995.cn

[S24] C：获取本地时间
来源：http://al.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vd.shxzskj.cn

[S25] C：内存拷贝
来源：http://ok.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://fi.huixiangedu.cn

[S26] C：内存清零
来源：http://fv.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://ih.lnxyls.cn

[S27] C：定义常量
来源：http://eb.newstarts.cn

const double PI = 3.14159;
来源：http://dn.szxytkj.cn

[S28] C：静态变量
来源：http://ze.521024.cn

static int counter = 0;
来源：http://pw.521024.cn

[S29] C：变参函数
来源：http://cu.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oh.hahajie.cn

[S30] C：头文件保护
来源：http://jn.shxzskj.cn

#ifndef X_H
来源：http://qk.huixiangedu.cn

#define X_H
来源：http://jc.521024.cn

#endif
来源：http://ve.newstarts.cn

[S31] C++：Hello World
来源：http://qp.jianghongdianzi.cn

#include <iostream>
来源：http://hc.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://pd.wgjwhj.cn

[S32] C++：字符串
来源：http://sm.huixinmuqiang.cn

std::string s = "hi";  s += "!";
来源：http://eu.gzmigu.cn

[S33] C++：vector 增删
来源：http://as.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mi.shtwfgs.cn

[S34] C++：遍历 vector
来源：http://nd.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://ex.yuntaijiaju.cn

[S35] C++：map
来源：http://xy.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lo.szsharing.cn

[S36] C++：unordered_map
来源：http://jm.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://il.huanxung.cn

[S37] C++：set
来源：http://rg.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iv.bookmarksfly.cn

[S38] C++：排序
来源：http://tn.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://zw.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://ey.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cu.gzmigu.cn

[S40] C++：查找元素
来源：http://dc.521024.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wn.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://uf.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ho.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://un.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://vk.muxihuayi.cn

[S43] C++：智能指针
来源：http://lj.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://gb.9csxet.cn

[S44] C++：引用传参
来源：http://ak.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://by.newstarts.cn

[S45] C++：lambda
来源：http://me.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qe.asd995.cn

[S46] C++：函数模板
来源：http://zr.shxzukj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lw.wgjwhj.cn

[S47] C++：结构化绑定遍历
来源：http://pj.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ww.gzmigu.cn

[S48] C++：逐行读文件
来源：http://fz.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qi.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://kl.shxzukj.cn

[S49] C++：写文件
来源：http://xf.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://li.lnxyls.cn

[S50] C++：格式化数字
来源：http://zl.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fw.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://vt.521024.cn

static_cast<double>(a) / b
来源：http://iu.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://nl.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://ee.bookmarksfly.cn

[S53] C++：移动语义
来源：http://es.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://be.haigaiapp.cn

[S54] C++：异常处理
来源：http://hr.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qa.szsharing.cn

[S55] C++：结构化绑定
来源：http://ld.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://db.521024.cn

[S56] C++：optional
来源：http://ij.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hy.yuexingan06.cn

[S57] C++：编译期常量
来源：http://ra.nicolike.cn

constexpr int N = 10;
来源：http://il.shtwfgs.cn

[S58] C++：命名空间
来源：http://wz.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://qd.chemitech.net.cn

[S59] C++：静态断言
来源：http://my.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://us.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://wy.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gu.nicolike.cn

================================================================================
来源：http://rp.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xd.newstarts.cn

================================================================================
来源：http://am.szxytkj.cn

[T01] Kotlin：Hello World
来源：http://uz.yuntaijiaju.cn

println("Hello")
来源：http://bw.9csxet.cn

[T02] Kotlin：变量
来源：http://is.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oa.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://am.bookmarksfly.cn

"值: $b"
来源：http://fa.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://jm.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://vk.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://ra.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fu.huanxung.cn

[T06] Kotlin：集合映射
来源：http://ef.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hh.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://il.jianghongdianzi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uo.lnxyls.cn

[T08] Kotlin：数据类
来源：http://ss.asd995.cn

data class User(val name: String, val age: Int)
来源：http://vh.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://wg.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://uz.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://rg.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nk.hahajie.cn

[T11] Kotlin：协程
来源：http://mw.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gu.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://uc.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://ii.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://sm.huanxung.cn

val m = mapOf("a" to 1)
来源：http://fa.hahajie.cn

[T14] Kotlin：循环
来源：http://cy.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://wc.bjjhwx.cn

[T15] Kotlin：接口
来源：http://to.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://nx.muxihuayi.cn

[T16] Swift：Hello World
来源：http://ny.nicolike.cn

print("Hello")
来源：http://ff.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://sh.wgjwhj.cn

var a = 1;  let b = 2
来源：http://ej.lnxyls.cn

[T18] Swift：字符串插值
来源：http://eo.asd995.cn

"值: \(b)"
来源：http://az.hnjuh.cn

[T19] Swift：可选绑定
来源：http://au.yuexingan06.cn

if let n = opt { print(n) }
来源：http://jy.huixiangedu.cn

[T20] Swift：数组操作
来源：http://qr.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dp.shxzukj.cn


<!-- 参考信息 -->