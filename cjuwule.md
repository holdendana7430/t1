代发 wailian999

echo "${#s}"
来源：http://ml.521024.cn

[R22] 截取子串
来源：http://nv.jctech888.com.cn

echo "${s:0:5}"
来源：http://vz.hnjuh.cn

[R23] 字符串替换
来源：http://qi.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ya.wgjwhj.cn

[R24] 大小写转换
来源：http://gx.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fh.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://ji.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yy.chemitech.net.cn

[R26] 命令替换
来源：http://nb.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://xh.colortex.cn

[R27] 算术展开
来源：http://hk.nicolike.cn

echo $((1 + 2 * 3))
来源：http://vn.newstarts.cn

[R28] 浮点运算
来源：http://gn.colortex.cn

echo "scale=2; 10/3" | bc
来源：http://so.9csxet.cn

[R29] 定义函数
来源：http://vu.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qq.szsharing.cn

[R30] 函数返回状态码
来源：http://hg.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://ei.9csxet.cn

[R31] 局部变量
来源：http://sz.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://uq.shxzukj.cn

[R32] 参数个数校验
来源：http://ay.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wj.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://gd.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vv.bjjhwx.cn

[R34] 退出时清理
来源：http://zh.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jk.panjiajie.cn

[R35] 后台执行并等待
来源：http://nn.yuexingan06.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gz.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://pe.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cj.nszjky.cn

[R37] 把输出赋给变量
来源：http://sw.shtwfgs.cn

files=$(ls -1)
来源：http://xv.shxzskj.cn

[R38] 管道串联
来源：http://vj.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://ka.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://aq.bjjhwx.cn

cmd > out.log 2>&1
来源：http://pa.shxzskj.cn

[R40] 追加写日志
来源：http://mv.shxzskj.cn

echo "log" >> out.log
来源：http://xf.panjiajie.cn

[R41] 丢弃输出
来源：http://ym.asd995.cn

cmd >/dev/null 2>&1
来源：http://tu.panjiajie.cn

[R42] 输入重定向
来源：http://dm.chemitech.net.cn

wc -l < a.txt
来源：http://dd.panjiajie.cn

[R43] 按名字查找文件
来源：http://jf.colortex.cn

find . -name "*.log" -type f
来源：http://ff.asd995.cn

[R44] 按修改时间查找
来源：http://ps.yuexingan06.cn

find . -mtime -7 -type f
来源：http://ic.huanxung.cn

[R45] 批量删除
来源：http://ql.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://kb.muxihuayi.cn

[R46] 递归替换文件内容
来源：http://na.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rm.panjiajie.cn

[R47] sed 单行替换
来源：http://hk.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dr.shtwfgs.cn

[R48] awk 取指定列
来源：http://tv.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://uo.gzmigu.cn

[R49] awk 带条件
来源：http://nd.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ii.szxytkj.cn

[R50] awk 求和
来源：http://yu.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fi.nicolike.cn

[R51] 排序去重取前几
来源：http://am.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hu.shtwfgs.cn

[R52] 统计行数
来源：http://hl.shtwfgs.cn

wc -l a.txt
来源：http://qd.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://hz.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://my.bookmarksfly.cn

[R54] 比较两个文件
来源：http://ub.yuntaijiaju.cn

diff a.txt b.txt
来源：http://jo.hahajie.cn

[R55] 压缩与解压
来源：http://hs.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gt.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://fn.huanxung.cn

scp file user@host:/path/
来源：http://os.huixinmuqiang.cn

[R57] 远程执行命令
来源：http://gv.bjjhwx.cn

ssh user@host 'uptime'
来源：http://kq.jctech888.com.cn

[R58] 下载文件
来源：http://nk.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ig.9csxet.cn

[R59] 发 POST JSON
来源：http://hm.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rl.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://pn.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ux.nszjky.cn

[R61] 磁盘占用
来源：http://bw.bjjhwx.cn

df -h;  du -sh *
来源：http://vj.lnxyls.cn

[R62] 找最占空间的文件
来源：http://ml.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://cd.bookmarksfly.cn

[R63] 内存与进程
来源：http://mc.panjiajie.cn

free -h;  ps aux | grep nginx
来源：http://ha.521024.cn

[R64] 结束进程
来源：http://jd.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://qn.szsharing.cn

[R65] 查看端口占用
来源：http://dl.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gs.9csxet.cn

[R66] 定时任务
来源：http://pv.hahajie.cn

crontab -e;  crontab -l
来源：http://wi.newstarts.cn

[R67] 生成随机十六进制串
来源：http://xi.huixiangedu.cn

openssl rand -hex 16
来源：http://fy.colortex.cn

[R68] 计算文件校验值
来源：http://ql.gzmigu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bq.lnxyls.cn

[R69] 生成随机密码
来源：http://xc.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://wx.hnjuh.cn

[R70] 时间戳与互转
来源：http://ob.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://td.shtwfgs.cn

[R71] 日期格式化
来源：http://zv.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ae.colortex.cn

[R72] 等待端口就绪
来源：http://ou.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cb.yuexingan06.cn

[R73] 分割大日志
来源：http://ho.shxzskj.cn

split -l 1000 big.log part_
来源：http://jv.lnxyls.cn

[R74] 批量重命名
来源：http://ps.jianghongdianzi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vp.muxihuayi.cn

[R75] 导出环境变量
来源：http://eg.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://ad.hahajie.cn

[R76] 使用临时文件
来源：http://ph.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ok.wgjwhj.cn

[R77] 读取用户输入
来源：http://zh.521024.cn

read -rp "请输入: " ans
来源：http://hl.szsharing.cn

[R78] 交互式菜单
来源：http://mn.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ou.9csxet.cn

[R79] 解析命令行选项
来源：http://or.colortex.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jf.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://oo.huixiangedu.cn

time ./run.sh
来源：http://fw.huixiangedu.cn

================================================================================
来源：http://ov.muxihuayi.cn

S. C / C++ 专题
来源：http://to.jianghongdianzi.cn

================================================================================
来源：http://ja.huixiangedu.cn

[S01] C：Hello World
来源：http://mv.huixinmuqiang.cn

#include <stdio.h>
来源：http://ie.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vu.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://hz.panjiajie.cn

int a = 10; printf("%d\n", a);
来源：http://ug.asd995.cn

[S03] C：读入整数
来源：http://zw.gzmigu.cn

int x; scanf("%d", &x);
来源：http://ie.bjjhwx.cn

[S04] C：字符串复制
来源：http://aw.nicolike.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wt.chemitech.net.cn

[S05] C：字符串长度
来源：http://hg.colortex.cn

strlen(s)
来源：http://tz.shxzskj.cn

[S06] C：字符串比较
来源：http://bi.shtwfgs.cn

strcmp(a, b) == 0
来源：http://qs.hnjuh.cn

[S07] C：数组遍历求和
来源：http://co.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ry.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://zz.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fc.colortex.cn

[S09] C：结构体定义与初始化
来源：http://bl.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vv.shxzukj.cn

[S10] C：指针与解引用
来源：http://dn.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://jr.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://iw.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://hq.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mk.nszjky.cn

fclose(f);
来源：http://xv.nszjky.cn

[S12] C：写文件
来源：http://sn.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yr.521024.cn

[S13] C：宏定义
来源：http://wc.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jw.chemitech.net.cn

[S14] C：枚举
来源：http://gb.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://rw.colortex.cn

[S15] C：类型转换
来源：http://ht.shxzskj.cn

(double) a / b
来源：http://ej.gzmigu.cn

[S16] C：位操作置位
来源：http://zp.jianghongdianzi.cn

x |= (1 << 3);
来源：http://zg.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://ct.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zy.wgjwhj.cn

[S18] C：命令行参数
来源：http://av.nicolike.cn

int main(int argc, char **argv)
来源：http://uy.jianghongdianzi.cn

[S19] C：快速排序
来源：http://bo.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jn.lnxyls.cn

[S20] C：二分查找
来源：http://ar.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zo.shtwfgs.cn

[S21] C：字符类别判断
来源：http://ro.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://en.wgjwhj.cn

[S22] C：字符串转数字
来源：http://my.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hq.chemitech.net.cn

[S23] C：随机数
来源：http://ao.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ip.szxytkj.cn

[S24] C：获取本地时间
来源：http://wt.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zu.bjjhwx.cn

[S25] C：内存拷贝
来源：http://oj.nicolike.cn

memcpy(dst, src, n);
来源：http://sg.haigaiapp.cn

[S26] C：内存清零
来源：http://bc.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://uz.shxzukj.cn

[S27] C：定义常量
来源：http://om.bjjhwx.cn

const double PI = 3.14159;
来源：http://ob.bookmarksfly.cn

[S28] C：静态变量
来源：http://dq.asd995.cn

static int counter = 0;
来源：http://aq.bjjhwx.cn

[S29] C：变参函数
来源：http://jp.huixinmuqiang.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ib.nszjky.cn

[S30] C：头文件保护
来源：http://cb.jctech888.com.cn

#ifndef X_H
来源：http://bi.szxytkj.cn

#define X_H
来源：http://bd.yuexingan06.cn

#endif
来源：http://dh.yuexingan06.cn

[S31] C++：Hello World
来源：http://xv.haigaiapp.cn

#include <iostream>
来源：http://vm.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://ip.chemitech.net.cn

[S32] C++：字符串
来源：http://ub.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://pk.wgjwhj.cn

[S33] C++：vector 增删
来源：http://jx.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hd.panjiajie.cn

[S34] C++：遍历 vector
来源：http://nj.szxytkj.cn

for (auto &x : v) { std::cout << x; }
来源：http://uv.wgjwhj.cn

[S35] C++：map
来源：http://xi.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ph.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://jt.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wa.panjiajie.cn

[S37] C++：set
来源：http://dc.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pd.hahajie.cn

[S38] C++：排序
来源：http://pk.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://al.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://wk.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gd.gzmigu.cn

[S40] C++：查找元素
来源：http://ku.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pg.nicolike.cn

[S41] C++：类与构造函数
来源：http://re.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dq.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://rp.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://dp.wgjwhj.cn

[S43] C++：智能指针
来源：http://hs.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://ek.jctech888.com.cn

[S44] C++：引用传参
来源：http://ju.szsharing.cn

void inc(int &x) { ++x; }
来源：http://oq.9csxet.cn

[S45] C++：lambda
来源：http://ul.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gr.yuexingan06.cn

[S46] C++：函数模板
来源：http://do.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ks.bjjhwx.cn

[S47] C++：结构化绑定遍历
来源：http://cf.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ui.szsharing.cn

[S48] C++：逐行读文件
来源：http://fs.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hz.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://gl.shxzukj.cn

[S49] C++：写文件
来源：http://vx.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hy.shxzukj.cn

[S50] C++：格式化数字
来源：http://ql.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ah.hahajie.cn

[S51] C++：显式类型转换
来源：http://gt.nszjky.cn

static_cast<double>(a) / b
来源：http://ka.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://dy.colortex.cn

int size() const noexcept { return n_; }
来源：http://rh.yuexingan06.cn

[S53] C++：移动语义
来源：http://uz.wgjwhj.cn

std::vector<int> w = std::move(v);
来源：http://un.newstarts.cn

[S54] C++：异常处理
来源：http://wm.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://os.shxzukj.cn

[S55] C++：结构化绑定
来源：http://ll.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jf.huanxung.cn

[S56] C++：optional
来源：http://ze.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oe.shtwfgs.cn

[S57] C++：编译期常量
来源：http://jo.nszjky.cn

constexpr int N = 10;
来源：http://wd.chemitech.net.cn

[S58] C++：命名空间
来源：http://hb.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://dg.bookmarksfly.cn

[S59] C++：静态断言
来源：http://ai.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ev.bjjhwx.cn

[S60] C++：遍历并删除元素
来源：http://dv.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zo.szsharing.cn

================================================================================
来源：http://nf.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nq.521024.cn

================================================================================
来源：http://pd.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://sq.newstarts.cn

println("Hello")
来源：http://vx.shxzskj.cn

[T02] Kotlin：变量
来源：http://hf.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yu.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://uy.huixinmuqiang.cn

"值: $b"
来源：http://ac.newstarts.cn

[T04] Kotlin：空安全
来源：http://of.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://vv.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://ko.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://io.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://yg.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qc.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://wq.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ab.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://gw.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://ml.colortex.cn

[T09] Kotlin：扩展函数
来源：http://rf.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://dy.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://qr.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kk.9csxet.cn

[T11] Kotlin：协程
来源：http://qn.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ex.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://gn.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://ep.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://de.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://fc.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://nl.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://ny.lnxyls.cn

[T15] Kotlin：接口
来源：http://uk.nszjky.cn

interface Shape { fun area(): Double }
来源：http://xe.jctech888.com.cn

[T16] Swift：Hello World
来源：http://zp.shtwfgs.cn

print("Hello")
来源：http://sx.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://ei.panjiajie.cn

var a = 1;  let b = 2
来源：http://zd.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://fr.chemitech.net.cn

"值: \(b)"
来源：http://jb.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://bv.asd995.cn

if let n = opt { print(n) }
来源：http://ca.gzmigu.cn

[T20] Swift：数组操作
来源：http://of.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cn.nicolike.cn

[T21] Swift：遍历
来源：http://ie.huixiangedu.cn

for x in a { print(x) }
来源：http://ko.9csxet.cn

[T22] Swift：字典
来源：http://vq.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wc.muxihuayi.cn

[T23] Swift：函数
来源：http://lt.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pz.muxihuayi.cn

[T24] Swift：闭包
来源：http://kg.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ky.yuexingan06.cn


<!-- 参考信息 -->