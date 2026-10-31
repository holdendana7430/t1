代发 wailian999

echo "${#arr[@]}"
来源：http://rl.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://hv.nszjky.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rj.shtwfgs.cn

[R21] 字符串长度
来源：http://pu.huixinmuqiang.cn

echo "${#s}"
来源：http://va.gzmigu.cn

[R22] 截取子串
来源：http://op.shtwfgs.cn

echo "${s:0:5}"
来源：http://rk.9csxet.cn

[R23] 字符串替换
来源：http://hu.hahajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gr.gzmigu.cn

[R24] 大小写转换
来源：http://wc.nszjky.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qz.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://ug.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lr.bjjhwx.cn

[R26] 命令替换
来源：http://el.huixiangedu.cn

now=$(date +%F); echo "$now"
来源：http://sp.jctech888.com.cn

[R27] 算术展开
来源：http://ot.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://xk.nicolike.cn

[R28] 浮点运算
来源：http://ta.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://xm.nicolike.cn

[R29] 定义函数
来源：http://cy.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gn.bjjhwx.cn

[R30] 函数返回状态码
来源：http://ww.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://oy.szxytkj.cn

[R31] 局部变量
来源：http://bf.shxzukj.cn

f() { local x=1; echo "$x"; }
来源：http://fa.9csxet.cn

[R32] 参数个数校验
来源：http://rg.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ki.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://kz.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ly.huanxung.cn

[R34] 退出时清理
来源：http://xs.shtwfgs.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mt.521024.cn

[R35] 后台执行并等待
来源：http://sh.jianghongdianzi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hn.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://fy.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bn.shxzskj.cn

[R37] 把输出赋给变量
来源：http://zy.hnjuh.cn

files=$(ls -1)
来源：http://vf.jctech888.com.cn

[R38] 管道串联
来源：http://bf.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://lc.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://qq.muxihuayi.cn

cmd > out.log 2>&1
来源：http://we.wgjwhj.cn

[R40] 追加写日志
来源：http://yo.wgjwhj.cn

echo "log" >> out.log
来源：http://ku.huixiangedu.cn

[R41] 丢弃输出
来源：http://fi.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://ct.jianghongdianzi.cn

[R42] 输入重定向
来源：http://uq.asd995.cn

wc -l < a.txt
来源：http://rj.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://zc.huanxung.cn

find . -name "*.log" -type f
来源：http://id.wgjwhj.cn

[R44] 按修改时间查找
来源：http://aa.shtwfgs.cn

find . -mtime -7 -type f
来源：http://pg.shtwfgs.cn

[R45] 批量删除
来源：http://gm.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://rc.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://gy.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://de.chemitech.net.cn

[R47] sed 单行替换
来源：http://wa.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://go.bookmarksfly.cn

[R48] awk 取指定列
来源：http://lc.huixiangedu.cn

awk '{print $1, $3}' a.txt
来源：http://ps.newstarts.cn

[R49] awk 带条件
来源：http://bx.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xy.hahajie.cn

[R50] awk 求和
来源：http://vk.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bj.bjjhwx.cn

[R51] 排序去重取前几
来源：http://dr.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zt.hnjuh.cn

[R52] 统计行数
来源：http://hj.hahajie.cn

wc -l a.txt
来源：http://ty.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://dz.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://db.colortex.cn

[R54] 比较两个文件
来源：http://yk.szxytkj.cn

diff a.txt b.txt
来源：http://mm.asd995.cn

[R55] 压缩与解压
来源：http://pt.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zo.szsharing.cn

[R56] 远程拷贝
来源：http://xa.yuntaijiaju.cn

scp file user@host:/path/
来源：http://pl.lnxyls.cn

[R57] 远程执行命令
来源：http://rx.bookmarksfly.cn

ssh user@host 'uptime'
来源：http://nj.yuexingan06.cn

[R58] 下载文件
来源：http://ah.jianghongdianzi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ka.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://fm.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cz.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://eb.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oc.9csxet.cn

[R61] 磁盘占用
来源：http://sy.shtwfgs.cn

df -h;  du -sh *
来源：http://fw.9csxet.cn

[R62] 找最占空间的文件
来源：http://sx.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://sl.jianghongdianzi.cn

[R63] 内存与进程
来源：http://tc.asd995.cn

free -h;  ps aux | grep nginx
来源：http://na.yuntaijiaju.cn

[R64] 结束进程
来源：http://eb.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://oq.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://th.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yg.huixiangedu.cn

[R66] 定时任务
来源：http://vo.colortex.cn

crontab -e;  crontab -l
来源：http://ov.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://wx.nicolike.cn

openssl rand -hex 16
来源：http://mj.huanxung.cn

[R68] 计算文件校验值
来源：http://go.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ja.nszjky.cn

[R69] 生成随机密码
来源：http://tu.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://jx.nicolike.cn

[R70] 时间戳与互转
来源：http://fw.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://vi.shxzukj.cn

[R71] 日期格式化
来源：http://zv.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uk.hahajie.cn

[R72] 等待端口就绪
来源：http://lu.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qo.hahajie.cn

[R73] 分割大日志
来源：http://ka.asd995.cn

split -l 1000 big.log part_
来源：http://iu.panjiajie.cn

[R74] 批量重命名
来源：http://qg.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rt.nicolike.cn

[R75] 导出环境变量
来源：http://cn.hnjuh.cn

export PATH="$HOME/bin:$PATH"
来源：http://ph.nszjky.cn

[R76] 使用临时文件
来源：http://fk.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://in.9csxet.cn

[R77] 读取用户输入
来源：http://cy.nicolike.cn

read -rp "请输入: " ans
来源：http://lh.shxzskj.cn

[R78] 交互式菜单
来源：http://gd.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mx.chemitech.net.cn

[R79] 解析命令行选项
来源：http://kj.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ag.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://cz.hnjuh.cn

time ./run.sh
来源：http://wf.wgjwhj.cn

================================================================================
来源：http://yh.bjjhwx.cn

S. C / C++ 专题
来源：http://wg.yuntaijiaju.cn

================================================================================
来源：http://ej.newstarts.cn

[S01] C：Hello World
来源：http://dh.haigaiapp.cn

#include <stdio.h>
来源：http://ra.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pl.huanxung.cn

[S02] C：变量与格式化输出
来源：http://ru.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://ta.haigaiapp.cn

[S03] C：读入整数
来源：http://sv.nszjky.cn

int x; scanf("%d", &x);
来源：http://co.shtwfgs.cn

[S04] C：字符串复制
来源：http://jp.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://og.colortex.cn

[S05] C：字符串长度
来源：http://mt.muxihuayi.cn

strlen(s)
来源：http://ai.shxzukj.cn

[S06] C：字符串比较
来源：http://el.muxihuayi.cn

strcmp(a, b) == 0
来源：http://bl.newstarts.cn

[S07] C：数组遍历求和
来源：http://vr.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lp.gzmigu.cn

[S08] C：动态内存分配与释放
来源：http://fa.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cn.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://ej.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qd.wgjwhj.cn

[S10] C：指针与解引用
来源：http://za.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://nr.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://nl.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://bd.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pl.bjjhwx.cn

fclose(f);
来源：http://vu.bookmarksfly.cn

[S12] C：写文件
来源：http://uy.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cf.hahajie.cn

[S13] C：宏定义
来源：http://kk.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ts.yuntaijiaju.cn

[S14] C：枚举
来源：http://du.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://og.panjiajie.cn

[S15] C：类型转换
来源：http://cd.szsharing.cn

(double) a / b
来源：http://cf.colortex.cn

[S16] C：位操作置位
来源：http://xf.jianghongdianzi.cn

x |= (1 << 3);
来源：http://vh.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://ye.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cz.haigaiapp.cn

[S18] C：命令行参数
来源：http://tb.lnxyls.cn

int main(int argc, char **argv)
来源：http://po.huixinmuqiang.cn

[S19] C：快速排序
来源：http://zg.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ky.yuntaijiaju.cn

[S20] C：二分查找
来源：http://br.hahajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://at.hahajie.cn

[S21] C：字符类别判断
来源：http://uf.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nf.shxzukj.cn

[S22] C：字符串转数字
来源：http://ec.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vr.bjjhwx.cn

[S23] C：随机数
来源：http://up.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lo.szxytkj.cn

[S24] C：获取本地时间
来源：http://eh.hahajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fy.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://qs.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://ow.jctech888.com.cn

[S26] C：内存清零
来源：http://lv.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://fe.nszjky.cn

[S27] C：定义常量
来源：http://ls.jianghongdianzi.cn

const double PI = 3.14159;
来源：http://dr.hnjuh.cn

[S28] C：静态变量
来源：http://gx.colortex.cn

static int counter = 0;
来源：http://ii.hahajie.cn

[S29] C：变参函数
来源：http://rc.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ou.hahajie.cn

[S30] C：头文件保护
来源：http://hk.colortex.cn

#ifndef X_H
来源：http://lk.nszjky.cn

#define X_H
来源：http://dx.521024.cn

#endif
来源：http://er.szsharing.cn

[S31] C++：Hello World
来源：http://sd.jianghongdianzi.cn

#include <iostream>
来源：http://de.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://ja.shxzukj.cn

[S32] C++：字符串
来源：http://hb.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://ng.hahajie.cn

[S33] C++：vector 增删
来源：http://az.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kk.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://qq.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://ml.wgjwhj.cn

[S35] C++：map
来源：http://bs.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://df.lnxyls.cn

[S36] C++：unordered_map
来源：http://vh.9csxet.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ad.haigaiapp.cn

[S37] C++：set
来源：http://qb.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sy.nszjky.cn

[S38] C++：排序
来源：http://jr.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://ep.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://gj.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tb.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://zt.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fk.521024.cn

[S41] C++：类与构造函数
来源：http://kl.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mw.asd995.cn

[S42] C++：继承与虚函数
来源：http://wu.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://vs.chemitech.net.cn

[S43] C++：智能指针
来源：http://ov.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://xx.nicolike.cn

[S44] C++：引用传参
来源：http://bx.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://zt.haigaiapp.cn

[S45] C++：lambda
来源：http://pk.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://iz.jctech888.com.cn

[S46] C++：函数模板
来源：http://gr.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qm.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://ri.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yi.lnxyls.cn

[S48] C++：逐行读文件
来源：http://ic.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kq.newstarts.cn

while (std::getline(in, line)) { }
来源：http://kq.szsharing.cn

[S49] C++：写文件
来源：http://so.huixinmuqiang.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tv.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://rt.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ko.szxytkj.cn

[S51] C++：显式类型转换
来源：http://mv.nszjky.cn

static_cast<double>(a) / b
来源：http://uv.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://wf.521024.cn

int size() const noexcept { return n_; }
来源：http://xx.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://sw.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://yj.muxihuayi.cn

[S54] C++：异常处理
来源：http://pu.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://df.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://ld.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tm.nicolike.cn

[S56] C++：optional
来源：http://bg.jctech888.com.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://st.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://ia.colortex.cn

constexpr int N = 10;
来源：http://gb.newstarts.cn

[S58] C++：命名空间
来源：http://wu.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://kc.huixiangedu.cn

[S59] C++：静态断言
来源：http://gz.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bh.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://km.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ak.szxytkj.cn

================================================================================
来源：http://yq.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gh.bjjhwx.cn

================================================================================
来源：http://vv.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://cu.nszjky.cn

println("Hello")
来源：http://yu.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://ri.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zu.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://md.huixiangedu.cn

"值: $b"
来源：http://jo.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://ou.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://lu.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://id.wgjwhj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://th.hahajie.cn

[T06] Kotlin：集合映射
来源：http://gr.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://uc.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://fy.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://al.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://av.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://iq.colortex.cn

[T09] Kotlin：扩展函数
来源：http://ia.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://pc.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://bs.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rz.shxzukj.cn

[T11] Kotlin：协程
来源：http://ms.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hg.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://ux.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://fo.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://pz.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://mi.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://tx.jctech888.com.cn

for (i in 1..10) println(i)
来源：http://pv.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://sp.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://xz.haigaiapp.cn

[T16] Swift：Hello World
来源：http://rp.huixinmuqiang.cn

print("Hello")
来源：http://yr.newstarts.cn

[T17] Swift：变量与常量
来源：http://qk.asd995.cn

var a = 1;  let b = 2
来源：http://pi.szsharing.cn

[T18] Swift：字符串插值
来源：http://ju.colortex.cn

"值: \(b)"
来源：http://vq.szxytkj.cn

[T19] Swift：可选绑定
来源：http://qt.szxytkj.cn

if let n = opt { print(n) }
来源：http://ln.521024.cn

[T20] Swift：数组操作
来源：http://eg.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xj.newstarts.cn

[T21] Swift：遍历
来源：http://qr.jianghongdianzi.cn

for x in a { print(x) }
来源：http://rx.wgjwhj.cn

[T22] Swift：字典
来源：http://bh.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cr.huixinmuqiang.cn


<!-- 参考信息 -->