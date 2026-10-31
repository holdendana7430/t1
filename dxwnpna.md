代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://qx.wgjwhj.cn

[R18] 遍历数组
来源：http://kz.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ec.huixiangedu.cn

[R19] 数组长度
来源：http://kf.szxytkj.cn

echo "${#arr[@]}"
来源：http://lw.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://ue.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bq.hnjuh.cn

[R21] 字符串长度
来源：http://eu.hnjuh.cn

echo "${#s}"
来源：http://bb.szxytkj.cn

[R22] 截取子串
来源：http://nv.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://pn.newstarts.cn

[R23] 字符串替换
来源：http://jc.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xh.hahajie.cn

[R24] 大小写转换
来源：http://tz.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vz.yuntaijiaju.cn

[R25] 去后缀 / 去前缀
来源：http://fh.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ii.muxihuayi.cn

[R26] 命令替换
来源：http://fw.nicolike.cn

now=$(date +%F); echo "$now"
来源：http://rv.haigaiapp.cn

[R27] 算术展开
来源：http://ma.szsharing.cn

echo $((1 + 2 * 3))
来源：http://qp.nszjky.cn

[R28] 浮点运算
来源：http://ii.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://ma.szsharing.cn

[R29] 定义函数
来源：http://vc.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lb.lnxyls.cn

[R30] 函数返回状态码
来源：http://jz.muxihuayi.cn

f() { return 0; }; f || echo "失败了"
来源：http://dj.newstarts.cn

[R31] 局部变量
来源：http://fo.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://lf.panjiajie.cn

[R32] 参数个数校验
来源：http://hn.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tr.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://gr.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tx.shxzukj.cn

[R34] 退出时清理
来源：http://va.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://no.9csxet.cn

[R35] 后台执行并等待
来源：http://xn.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gb.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://mm.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wi.szsharing.cn

[R37] 把输出赋给变量
来源：http://br.shtwfgs.cn

files=$(ls -1)
来源：http://fj.shtwfgs.cn

[R38] 管道串联
来源：http://mu.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://ub.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://gz.jctech888.com.cn

cmd > out.log 2>&1
来源：http://pa.shtwfgs.cn

[R40] 追加写日志
来源：http://ff.9csxet.cn

echo "log" >> out.log
来源：http://hg.bookmarksfly.cn

[R41] 丢弃输出
来源：http://xn.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://bk.bjjhwx.cn

[R42] 输入重定向
来源：http://fp.panjiajie.cn

wc -l < a.txt
来源：http://zk.colortex.cn

[R43] 按名字查找文件
来源：http://gf.nszjky.cn

find . -name "*.log" -type f
来源：http://fy.newstarts.cn

[R44] 按修改时间查找
来源：http://mc.521024.cn

find . -mtime -7 -type f
来源：http://jh.asd995.cn

[R45] 批量删除
来源：http://pv.hahajie.cn

find . -name "*.tmp" -delete
来源：http://fm.nszjky.cn

[R46] 递归替换文件内容
来源：http://ef.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kx.nszjky.cn

[R47] sed 单行替换
来源：http://ty.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kt.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://as.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://wz.colortex.cn

[R49] awk 带条件
来源：http://uj.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vd.wgjwhj.cn

[R50] awk 求和
来源：http://cz.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ty.huixiangedu.cn

[R51] 排序去重取前几
来源：http://fd.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yl.bjjhwx.cn

[R52] 统计行数
来源：http://an.colortex.cn

wc -l a.txt
来源：http://ua.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://pg.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lq.huixiangedu.cn

[R54] 比较两个文件
来源：http://xw.newstarts.cn

diff a.txt b.txt
来源：http://ia.bookmarksfly.cn

[R55] 压缩与解压
来源：http://bw.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://or.hahajie.cn

[R56] 远程拷贝
来源：http://rh.shxzukj.cn

scp file user@host:/path/
来源：http://oc.colortex.cn

[R57] 远程执行命令
来源：http://ai.chemitech.net.cn

ssh user@host 'uptime'
来源：http://ku.colortex.cn

[R58] 下载文件
来源：http://lv.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sx.9csxet.cn

[R59] 发 POST JSON
来源：http://qc.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nm.nicolike.cn

[R60] 只看 HTTP 状态码
来源：http://jx.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://va.huanxung.cn

[R61] 磁盘占用
来源：http://dh.nicolike.cn

df -h;  du -sh *
来源：http://ew.szsharing.cn

[R62] 找最占空间的文件
来源：http://qo.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://yh.jianghongdianzi.cn

[R63] 内存与进程
来源：http://iz.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://yq.lnxyls.cn

[R64] 结束进程
来源：http://jk.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://gm.nicolike.cn

[R65] 查看端口占用
来源：http://sj.szxytkj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tl.gzmigu.cn

[R66] 定时任务
来源：http://xy.nszjky.cn

crontab -e;  crontab -l
来源：http://dn.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://mp.jctech888.com.cn

openssl rand -hex 16
来源：http://bi.szsharing.cn

[R68] 计算文件校验值
来源：http://sn.hnjuh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xb.muxihuayi.cn

[R69] 生成随机密码
来源：http://dv.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://ln.colortex.cn

[R70] 时间戳与互转
来源：http://eo.newstarts.cn

date +%s;  date -d @1700000000
来源：http://zm.nicolike.cn

[R71] 日期格式化
来源：http://fe.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xb.9csxet.cn

[R72] 等待端口就绪
来源：http://uy.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cr.hnjuh.cn

[R73] 分割大日志
来源：http://yq.gzmigu.cn

split -l 1000 big.log part_
来源：http://kd.yuexingan06.cn

[R74] 批量重命名
来源：http://ae.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vl.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://lv.wgjwhj.cn

export PATH="$HOME/bin:$PATH"
来源：http://kc.panjiajie.cn

[R76] 使用临时文件
来源：http://nr.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wh.hnjuh.cn

[R77] 读取用户输入
来源：http://fw.shxzukj.cn

read -rp "请输入: " ans
来源：http://ix.muxihuayi.cn

[R78] 交互式菜单
来源：http://ej.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jl.jctech888.com.cn

[R79] 解析命令行选项
来源：http://pe.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lm.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://nw.chemitech.net.cn

time ./run.sh
来源：http://qd.huixinmuqiang.cn

================================================================================
来源：http://ld.panjiajie.cn

S. C / C++ 专题
来源：http://jj.hnjuh.cn

================================================================================
来源：http://jh.yuexingan06.cn

[S01] C：Hello World
来源：http://rx.bookmarksfly.cn

#include <stdio.h>
来源：http://ag.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pk.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://kg.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://pv.jctech888.com.cn

[S03] C：读入整数
来源：http://zi.jianghongdianzi.cn

int x; scanf("%d", &x);
来源：http://vq.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://yo.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cy.wgjwhj.cn

[S05] C：字符串长度
来源：http://rv.yuexingan06.cn

strlen(s)
来源：http://yo.newstarts.cn

[S06] C：字符串比较
来源：http://dj.bjjhwx.cn

strcmp(a, b) == 0
来源：http://bz.szxytkj.cn

[S07] C：数组遍历求和
来源：http://tr.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wp.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://oy.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ix.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://pk.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pg.shxzukj.cn

[S10] C：指针与解引用
来源：http://gt.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://ry.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://hk.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://es.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fj.nicolike.cn

fclose(f);
来源：http://pm.muxihuayi.cn

[S12] C：写文件
来源：http://pc.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dh.haigaiapp.cn

[S13] C：宏定义
来源：http://fq.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oi.chemitech.net.cn

[S14] C：枚举
来源：http://pf.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://ns.colortex.cn

[S15] C：类型转换
来源：http://rm.muxihuayi.cn

(double) a / b
来源：http://dp.colortex.cn

[S16] C：位操作置位
来源：http://kb.bjjhwx.cn

x |= (1 << 3);
来源：http://gv.nszjky.cn

[S17] C：安全拼接字符串
来源：http://qw.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jd.hnjuh.cn

[S18] C：命令行参数
来源：http://fc.asd995.cn

int main(int argc, char **argv)
来源：http://bf.shxzukj.cn

[S19] C：快速排序
来源：http://hg.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cw.bjjhwx.cn

[S20] C：二分查找
来源：http://mj.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nu.muxihuayi.cn

[S21] C：字符类别判断
来源：http://gs.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ab.asd995.cn

[S22] C：字符串转数字
来源：http://rm.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bn.asd995.cn

[S23] C：随机数
来源：http://ki.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pj.9csxet.cn

[S24] C：获取本地时间
来源：http://yg.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lv.szxytkj.cn

[S25] C：内存拷贝
来源：http://lg.shxzskj.cn

memcpy(dst, src, n);
来源：http://af.nicolike.cn

[S26] C：内存清零
来源：http://yp.szsharing.cn

memset(a, 0, sizeof a);
来源：http://er.huanxung.cn

[S27] C：定义常量
来源：http://ni.chemitech.net.cn

const double PI = 3.14159;
来源：http://zm.yuntaijiaju.cn

[S28] C：静态变量
来源：http://jz.yuntaijiaju.cn

static int counter = 0;
来源：http://vt.bookmarksfly.cn

[S29] C：变参函数
来源：http://ve.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://de.szxytkj.cn

[S30] C：头文件保护
来源：http://zy.szsharing.cn

#ifndef X_H
来源：http://wn.haigaiapp.cn

#define X_H
来源：http://xo.panjiajie.cn

#endif
来源：http://wu.nszjky.cn

[S31] C++：Hello World
来源：http://ji.nicolike.cn

#include <iostream>
来源：http://ao.bookmarksfly.cn

int main() { std::cout << "Hello\n"; }
来源：http://kb.szxytkj.cn

[S32] C++：字符串
来源：http://uz.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://ck.chemitech.net.cn

[S33] C++：vector 增删
来源：http://cp.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ol.gzmigu.cn

[S34] C++：遍历 vector
来源：http://ko.szsharing.cn

for (auto &x : v) { std::cout << x; }
来源：http://xa.panjiajie.cn

[S35] C++：map
来源：http://re.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://px.szsharing.cn

[S36] C++：unordered_map
来源：http://zn.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cl.huixiangedu.cn

[S37] C++：set
来源：http://nh.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ds.shxzukj.cn

[S38] C++：排序
来源：http://oy.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://gr.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://uo.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hs.muxihuayi.cn

[S40] C++：查找元素
来源：http://bx.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oq.panjiajie.cn

[S41] C++：类与构造函数
来源：http://yy.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fh.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://zj.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://gb.chemitech.net.cn

[S43] C++：智能指针
来源：http://if.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://oj.newstarts.cn

[S44] C++：引用传参
来源：http://po.shtwfgs.cn

void inc(int &x) { ++x; }
来源：http://ma.bjjhwx.cn

[S45] C++：lambda
来源：http://zv.colortex.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dk.szxytkj.cn

[S46] C++：函数模板
来源：http://mf.jianghongdianzi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qf.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://tb.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bj.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://ld.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tx.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://zc.hahajie.cn

[S49] C++：写文件
来源：http://on.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lb.gzmigu.cn

[S50] C++：格式化数字
来源：http://el.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fx.panjiajie.cn

[S51] C++：显式类型转换
来源：http://ag.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://qa.521024.cn

[S52] C++：const 与 noexcept
来源：http://iz.colortex.cn

int size() const noexcept { return n_; }
来源：http://tz.szsharing.cn

[S53] C++：移动语义
来源：http://sp.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://eg.521024.cn

[S54] C++：异常处理
来源：http://zl.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lr.shxzskj.cn

[S55] C++：结构化绑定
来源：http://qj.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ho.huixiangedu.cn

[S56] C++：optional
来源：http://mv.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fn.asd995.cn

[S57] C++：编译期常量
来源：http://wp.jctech888.com.cn

constexpr int N = 10;
来源：http://dv.wgjwhj.cn

[S58] C++：命名空间
来源：http://rt.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://mg.shtwfgs.cn

[S59] C++：静态断言
来源：http://gs.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gi.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://hy.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zz.bookmarksfly.cn

================================================================================
来源：http://pg.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fr.nicolike.cn

================================================================================
来源：http://zy.9csxet.cn

[T01] Kotlin：Hello World
来源：http://lg.bookmarksfly.cn

println("Hello")
来源：http://th.huanxung.cn

[T02] Kotlin：变量
来源：http://fl.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ye.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://ap.yuexingan06.cn

"值: $b"
来源：http://ne.colortex.cn

[T04] Kotlin：空安全
来源：http://ir.newstarts.cn

val n: String? = null;  n?.length
来源：http://sc.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://if.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ae.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://sb.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://od.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://fo.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://od.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://jz.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://sz.gzmigu.cn

[T09] Kotlin：扩展函数
来源：http://tz.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://fq.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://jw.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yb.colortex.cn

[T11] Kotlin：协程
来源：http://iw.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://om.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://pj.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://dy.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://ck.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://xr.haigaiapp.cn

[T14] Kotlin：循环
来源：http://xn.nszjky.cn

for (i in 1..10) println(i)
来源：http://yd.9csxet.cn

[T15] Kotlin：接口
来源：http://fi.asd995.cn

interface Shape { fun area(): Double }
来源：http://ez.haigaiapp.cn

[T16] Swift：Hello World
来源：http://xz.shxzukj.cn

print("Hello")
来源：http://pb.panjiajie.cn

[T17] Swift：变量与常量
来源：http://ew.nszjky.cn

var a = 1;  let b = 2
来源：http://mb.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://fr.gzmigu.cn

"值: \(b)"
来源：http://lb.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://ov.jctech888.com.cn

if let n = opt { print(n) }
来源：http://oz.hnjuh.cn

[T20] Swift：数组操作
来源：http://kd.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mf.wgjwhj.cn


<!-- 参考信息 -->