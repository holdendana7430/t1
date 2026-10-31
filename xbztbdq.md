代发 wailian999

echo "${#arr[@]}"
来源：http://rb.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://bo.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zi.huixiangedu.cn

[R21] 字符串长度
来源：http://rd.szsharing.cn

echo "${#s}"
来源：http://ir.jctech888.com.cn

[R22] 截取子串
来源：http://pn.panjiajie.cn

echo "${s:0:5}"
来源：http://qq.hahajie.cn

[R23] 字符串替换
来源：http://rz.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fh.jianghongdianzi.cn

[R24] 大小写转换
来源：http://ui.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tt.shtwfgs.cn

[R25] 去后缀 / 去前缀
来源：http://wg.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://se.yuntaijiaju.cn

[R26] 命令替换
来源：http://oz.yuexingan06.cn

now=$(date +%F); echo "$now"
来源：http://yl.lnxyls.cn

[R27] 算术展开
来源：http://eb.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://mm.hahajie.cn

[R28] 浮点运算
来源：http://cg.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://by.nszjky.cn

[R29] 定义函数
来源：http://mm.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ms.huanxung.cn

[R30] 函数返回状态码
来源：http://lx.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://ig.szsharing.cn

[R31] 局部变量
来源：http://ih.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://bb.bjjhwx.cn

[R32] 参数个数校验
来源：http://hq.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oy.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://ni.muxihuayi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ul.szxytkj.cn

[R34] 退出时清理
来源：http://im.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ss.yuexingan06.cn

[R35] 后台执行并等待
来源：http://az.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xt.9csxet.cn

[R36] 并发执行多个任务
来源：http://nm.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kp.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://dp.gzmigu.cn

files=$(ls -1)
来源：http://dx.nszjky.cn

[R38] 管道串联
来源：http://gh.shxzukj.cn

cat a.txt | grep -i error | wc -l
来源：http://ix.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://pt.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://xc.hahajie.cn

[R40] 追加写日志
来源：http://ko.jctech888.com.cn

echo "log" >> out.log
来源：http://fw.colortex.cn

[R41] 丢弃输出
来源：http://qg.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://qm.hnjuh.cn

[R42] 输入重定向
来源：http://qm.newstarts.cn

wc -l < a.txt
来源：http://lg.huixiangedu.cn

[R43] 按名字查找文件
来源：http://ld.521024.cn

find . -name "*.log" -type f
来源：http://yg.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://ns.shxzukj.cn

find . -mtime -7 -type f
来源：http://sy.hahajie.cn

[R45] 批量删除
来源：http://yp.nicolike.cn

find . -name "*.tmp" -delete
来源：http://dz.hahajie.cn

[R46] 递归替换文件内容
来源：http://tt.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nt.gzmigu.cn

[R47] sed 单行替换
来源：http://nr.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bi.shxzukj.cn

[R48] awk 取指定列
来源：http://cu.huixiangedu.cn

awk '{print $1, $3}' a.txt
来源：http://wi.huixiangedu.cn

[R49] awk 带条件
来源：http://ji.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fp.huixiangedu.cn

[R50] awk 求和
来源：http://gh.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wb.asd995.cn

[R51] 排序去重取前几
来源：http://to.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://km.bookmarksfly.cn

[R52] 统计行数
来源：http://cs.lnxyls.cn

wc -l a.txt
来源：http://nw.521024.cn

[R53] 查看文件头与实时尾
来源：http://bb.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ct.lnxyls.cn

[R54] 比较两个文件
来源：http://pn.huanxung.cn

diff a.txt b.txt
来源：http://jy.jianghongdianzi.cn

[R55] 压缩与解压
来源：http://rp.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ua.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://zp.yuexingan06.cn

scp file user@host:/path/
来源：http://vu.gzmigu.cn

[R57] 远程执行命令
来源：http://xt.bjjhwx.cn

ssh user@host 'uptime'
来源：http://mr.panjiajie.cn

[R58] 下载文件
来源：http://js.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sm.szsharing.cn

[R59] 发 POST JSON
来源：http://vu.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uv.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://yn.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xr.9csxet.cn

[R61] 磁盘占用
来源：http://br.szxytkj.cn

df -h;  du -sh *
来源：http://fm.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://yz.chemitech.net.cn

du -ah . | sort -rh | head -10
来源：http://tk.hahajie.cn

[R63] 内存与进程
来源：http://qy.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://th.521024.cn

[R64] 结束进程
来源：http://zv.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://pk.huixiangedu.cn

[R65] 查看端口占用
来源：http://mq.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mv.muxihuayi.cn

[R66] 定时任务
来源：http://il.muxihuayi.cn

crontab -e;  crontab -l
来源：http://qp.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://sv.muxihuayi.cn

openssl rand -hex 16
来源：http://oh.gzmigu.cn

[R68] 计算文件校验值
来源：http://no.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bw.nicolike.cn

[R69] 生成随机密码
来源：http://xr.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://xb.nszjky.cn

[R70] 时间戳与互转
来源：http://ak.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://ss.jianghongdianzi.cn

[R71] 日期格式化
来源：http://qm.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rd.lnxyls.cn

[R72] 等待端口就绪
来源：http://yz.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bm.nszjky.cn

[R73] 分割大日志
来源：http://tr.newstarts.cn

split -l 1000 big.log part_
来源：http://kn.nicolike.cn

[R74] 批量重命名
来源：http://ea.haigaiapp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fx.lnxyls.cn

[R75] 导出环境变量
来源：http://jv.szsharing.cn

export PATH="$HOME/bin:$PATH"
来源：http://kx.shxzukj.cn

[R76] 使用临时文件
来源：http://sv.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zf.colortex.cn

[R77] 读取用户输入
来源：http://ps.szsharing.cn

read -rp "请输入: " ans
来源：http://lm.panjiajie.cn

[R78] 交互式菜单
来源：http://du.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ic.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://li.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lr.521024.cn

[R80] 查看脚本执行耗时
来源：http://el.521024.cn

time ./run.sh
来源：http://zd.shxzskj.cn

================================================================================
来源：http://rf.shxzskj.cn

S. C / C++ 专题
来源：http://fn.shxzskj.cn

================================================================================
来源：http://ut.colortex.cn

[S01] C：Hello World
来源：http://dn.shxzskj.cn

#include <stdio.h>
来源：http://qh.newstarts.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ff.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://mm.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://mi.haigaiapp.cn

[S03] C：读入整数
来源：http://kr.shxzskj.cn

int x; scanf("%d", &x);
来源：http://un.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://tu.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mn.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://sc.wgjwhj.cn

strlen(s)
来源：http://zi.nicolike.cn

[S06] C：字符串比较
来源：http://mn.panjiajie.cn

strcmp(a, b) == 0
来源：http://df.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://ft.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nh.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://br.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eu.521024.cn

[S09] C：结构体定义与初始化
来源：http://oq.521024.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://el.gzmigu.cn

[S10] C：指针与解引用
来源：http://wr.9csxet.cn

int *p = &a;  *p = 5;
来源：http://gm.colortex.cn

[S11] C：逐行读文件
来源：http://yw.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://jb.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://et.haigaiapp.cn

fclose(f);
来源：http://xw.haigaiapp.cn

[S12] C：写文件
来源：http://zi.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rz.wgjwhj.cn

[S13] C：宏定义
来源：http://xp.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sl.huixinmuqiang.cn

[S14] C：枚举
来源：http://xc.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://zw.huanxung.cn

[S15] C：类型转换
来源：http://jb.shtwfgs.cn

(double) a / b
来源：http://qf.wgjwhj.cn

[S16] C：位操作置位
来源：http://pv.shxzukj.cn

x |= (1 << 3);
来源：http://qc.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://lt.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://np.haigaiapp.cn

[S18] C：命令行参数
来源：http://zt.nicolike.cn

int main(int argc, char **argv)
来源：http://uu.szsharing.cn

[S19] C：快速排序
来源：http://za.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hu.jctech888.com.cn

[S20] C：二分查找
来源：http://xb.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mk.szxytkj.cn

[S21] C：字符类别判断
来源：http://xi.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uo.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://wd.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zy.shxzukj.cn

[S23] C：随机数
来源：http://oy.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://eq.szsharing.cn

[S24] C：获取本地时间
来源：http://mx.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wk.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://rh.521024.cn

memcpy(dst, src, n);
来源：http://vz.muxihuayi.cn

[S26] C：内存清零
来源：http://nz.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://do.lnxyls.cn

[S27] C：定义常量
来源：http://wk.bjjhwx.cn

const double PI = 3.14159;
来源：http://qe.haigaiapp.cn

[S28] C：静态变量
来源：http://wf.lnxyls.cn

static int counter = 0;
来源：http://hx.shxzukj.cn

[S29] C：变参函数
来源：http://gm.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ki.haigaiapp.cn

[S30] C：头文件保护
来源：http://ep.colortex.cn

#ifndef X_H
来源：http://gt.yuexingan06.cn

#define X_H
来源：http://mc.panjiajie.cn

#endif
来源：http://pj.9csxet.cn

[S31] C++：Hello World
来源：http://zt.yuntaijiaju.cn

#include <iostream>
来源：http://jb.huixiangedu.cn

int main() { std::cout << "Hello\n"; }
来源：http://nt.jianghongdianzi.cn

[S32] C++：字符串
来源：http://uv.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://cd.jctech888.com.cn

[S33] C++：vector 增删
来源：http://un.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://va.gzmigu.cn

[S34] C++：遍历 vector
来源：http://wn.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://bo.nszjky.cn

[S35] C++：map
来源：http://kb.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nq.huixiangedu.cn

[S36] C++：unordered_map
来源：http://xl.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tu.hahajie.cn

[S37] C++：set
来源：http://jv.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wj.huixinmuqiang.cn

[S38] C++：排序
来源：http://an.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://yc.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://vb.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zy.yuexingan06.cn

[S40] C++：查找元素
来源：http://iw.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://us.gzmigu.cn

[S41] C++：类与构造函数
来源：http://rh.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ur.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://wc.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://gb.bjjhwx.cn

[S43] C++：智能指针
来源：http://ba.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://df.nszjky.cn

[S44] C++：引用传参
来源：http://le.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://hb.yuexingan06.cn

[S45] C++：lambda
来源：http://ug.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vx.bookmarksfly.cn

[S46] C++：函数模板
来源：http://dm.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sk.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://kw.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gj.shxzukj.cn

[S48] C++：逐行读文件
来源：http://my.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bp.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://re.gzmigu.cn

[S49] C++：写文件
来源：http://wi.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wk.colortex.cn

[S50] C++：格式化数字
来源：http://jr.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://on.asd995.cn

[S51] C++：显式类型转换
来源：http://bi.yuexingan06.cn

static_cast<double>(a) / b
来源：http://lr.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://ho.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://wy.shxzskj.cn

[S53] C++：移动语义
来源：http://wt.panjiajie.cn

std::vector<int> w = std::move(v);
来源：http://wg.szsharing.cn

[S54] C++：异常处理
来源：http://va.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ts.521024.cn

[S55] C++：结构化绑定
来源：http://fk.muxihuayi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zr.huixinmuqiang.cn

[S56] C++：optional
来源：http://ra.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yt.huixinmuqiang.cn

[S57] C++：编译期常量
来源：http://nb.colortex.cn

constexpr int N = 10;
来源：http://tg.yuexingan06.cn

[S58] C++：命名空间
来源：http://ow.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://bf.yuexingan06.cn

[S59] C++：静态断言
来源：http://nv.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zo.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://pc.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jf.bookmarksfly.cn

================================================================================
来源：http://kn.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yg.panjiajie.cn

================================================================================
来源：http://bp.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://qm.newstarts.cn

println("Hello")
来源：http://yp.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://ux.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gy.colortex.cn

[T03] Kotlin：字符串模板
来源：http://oc.yuexingan06.cn

"值: $b"
来源：http://ab.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://ms.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://hi.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://ce.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ag.huanxung.cn

[T06] Kotlin：集合映射
来源：http://sv.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lg.521024.cn

[T07] Kotlin：集合过滤
来源：http://nu.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ea.nszjky.cn

[T08] Kotlin：数据类
来源：http://xp.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://aj.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://vz.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://lb.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://cj.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://by.huixiangedu.cn

[T11] Kotlin：协程
来源：http://ke.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gm.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://gc.chemitech.net.cn

val (a, b) = Pair(1, 2)
来源：http://np.asd995.cn

[T13] Kotlin：只读 Map
来源：http://sh.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://mv.huixiangedu.cn

[T14] Kotlin：循环
来源：http://iu.9csxet.cn

for (i in 1..10) println(i)
来源：http://vf.gzmigu.cn

[T15] Kotlin：接口
来源：http://dj.huixinmuqiang.cn

interface Shape { fun area(): Double }
来源：http://bj.yuexingan06.cn

[T16] Swift：Hello World
来源：http://xa.shtwfgs.cn

print("Hello")
来源：http://od.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://un.lnxyls.cn

var a = 1;  let b = 2
来源：http://yy.lnxyls.cn

[T18] Swift：字符串插值
来源：http://ch.huixinmuqiang.cn

"值: \(b)"
来源：http://eq.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://fx.panjiajie.cn

if let n = opt { print(n) }
来源：http://qv.jctech888.com.cn

[T20] Swift：数组操作
来源：http://dd.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jl.521024.cn

[T21] Swift：遍历
来源：http://es.hahajie.cn

for x in a { print(x) }
来源：http://iv.bookmarksfly.cn

[T22] Swift：字典
来源：http://sl.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pj.szsharing.cn


<!-- 参考信息 -->