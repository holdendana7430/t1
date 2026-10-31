代发 wailian999

echo "${#arr[@]}"
来源：http://fl.shxzukj.cn

[R20] 关联数组（字典）
来源：http://of.huixinmuqiang.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qt.panjiajie.cn

[R21] 字符串长度
来源：http://as.shxzskj.cn

echo "${#s}"
来源：http://pz.chemitech.net.cn

[R22] 截取子串
来源：http://ba.shxzskj.cn

echo "${s:0:5}"
来源：http://by.yuntaijiaju.cn

[R23] 字符串替换
来源：http://fm.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://my.9csxet.cn

[R24] 大小写转换
来源：http://yz.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fl.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://hx.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kd.lnxyls.cn

[R26] 命令替换
来源：http://tv.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://bt.bookmarksfly.cn

[R27] 算术展开
来源：http://cc.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://nm.haigaiapp.cn

[R28] 浮点运算
来源：http://rg.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://re.521024.cn

[R29] 定义函数
来源：http://fs.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gy.colortex.cn

[R30] 函数返回状态码
来源：http://er.nicolike.cn

f() { return 0; }; f || echo "失败了"
来源：http://ie.521024.cn

[R31] 局部变量
来源：http://po.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://ep.wgjwhj.cn

[R32] 参数个数校验
来源：http://lr.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lx.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://ld.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ws.shxzskj.cn

[R34] 退出时清理
来源：http://wj.bjjhwx.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qe.bjjhwx.cn

[R35] 后台执行并等待
来源：http://rv.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jq.szsharing.cn

[R36] 并发执行多个任务
来源：http://wx.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nc.nicolike.cn

[R37] 把输出赋给变量
来源：http://nh.lnxyls.cn

files=$(ls -1)
来源：http://zm.bookmarksfly.cn

[R38] 管道串联
来源：http://pv.nszjky.cn

cat a.txt | grep -i error | wc -l
来源：http://yv.haigaiapp.cn

[R39] 重定向标准输出与错误
来源：http://bm.hnjuh.cn

cmd > out.log 2>&1
来源：http://uz.shxzukj.cn

[R40] 追加写日志
来源：http://vt.hahajie.cn

echo "log" >> out.log
来源：http://ws.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://nc.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://ze.colortex.cn

[R42] 输入重定向
来源：http://mi.nicolike.cn

wc -l < a.txt
来源：http://wf.hnjuh.cn

[R43] 按名字查找文件
来源：http://rk.521024.cn

find . -name "*.log" -type f
来源：http://kd.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://hk.gzmigu.cn

find . -mtime -7 -type f
来源：http://pk.nicolike.cn

[R45] 批量删除
来源：http://ns.szsharing.cn

find . -name "*.tmp" -delete
来源：http://cd.lnxyls.cn

[R46] 递归替换文件内容
来源：http://qc.hnjuh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jh.shxzukj.cn

[R47] sed 单行替换
来源：http://oi.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cm.bookmarksfly.cn

[R48] awk 取指定列
来源：http://bm.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://iy.shtwfgs.cn

[R49] awk 带条件
来源：http://ud.jianghongdianzi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wr.muxihuayi.cn

[R50] awk 求和
来源：http://ai.bookmarksfly.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fj.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://ie.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ek.jctech888.com.cn

[R52] 统计行数
来源：http://wy.yuntaijiaju.cn

wc -l a.txt
来源：http://lg.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://mc.lnxyls.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://do.hahajie.cn

[R54] 比较两个文件
来源：http://jg.gzmigu.cn

diff a.txt b.txt
来源：http://vg.shtwfgs.cn

[R55] 压缩与解压
来源：http://aq.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ay.chemitech.net.cn

[R56] 远程拷贝
来源：http://eq.huixiangedu.cn

scp file user@host:/path/
来源：http://qf.chemitech.net.cn

[R57] 远程执行命令
来源：http://eq.huixiangedu.cn

ssh user@host 'uptime'
来源：http://it.shxzukj.cn

[R58] 下载文件
来源：http://zw.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wo.lnxyls.cn

[R59] 发 POST JSON
来源：http://mk.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nj.jctech888.com.cn

[R60] 只看 HTTP 状态码
来源：http://lf.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ei.huanxung.cn

[R61] 磁盘占用
来源：http://tp.gzmigu.cn

df -h;  du -sh *
来源：http://co.szxytkj.cn

[R62] 找最占空间的文件
来源：http://gg.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://so.szxytkj.cn

[R63] 内存与进程
来源：http://xa.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://fi.hnjuh.cn

[R64] 结束进程
来源：http://gp.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://wp.521024.cn

[R65] 查看端口占用
来源：http://jq.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tf.yuexingan06.cn

[R66] 定时任务
来源：http://wc.lnxyls.cn

crontab -e;  crontab -l
来源：http://sk.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://yn.szxytkj.cn

openssl rand -hex 16
来源：http://yn.szsharing.cn

[R68] 计算文件校验值
来源：http://rs.lnxyls.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kf.panjiajie.cn

[R69] 生成随机密码
来源：http://az.9csxet.cn

head -c 16 /dev/urandom | base64
来源：http://cx.yuexingan06.cn

[R70] 时间戳与互转
来源：http://rf.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://pj.lnxyls.cn

[R71] 日期格式化
来源：http://vy.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://aw.nicolike.cn

[R72] 等待端口就绪
来源：http://oo.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bk.bjjhwx.cn

[R73] 分割大日志
来源：http://og.shxzukj.cn

split -l 1000 big.log part_
来源：http://gc.9csxet.cn

[R74] 批量重命名
来源：http://kj.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mg.hnjuh.cn

[R75] 导出环境变量
来源：http://jr.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://ih.521024.cn

[R76] 使用临时文件
来源：http://cl.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mf.bookmarksfly.cn

[R77] 读取用户输入
来源：http://gk.yuexingan06.cn

read -rp "请输入: " ans
来源：http://pu.colortex.cn

[R78] 交互式菜单
来源：http://av.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fd.shxzskj.cn

[R79] 解析命令行选项
来源：http://yt.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tt.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://sf.huixiangedu.cn

time ./run.sh
来源：http://fd.huixinmuqiang.cn

================================================================================
来源：http://ll.jianghongdianzi.cn

S. C / C++ 专题
来源：http://vf.bookmarksfly.cn

================================================================================
来源：http://hg.hnjuh.cn

[S01] C：Hello World
来源：http://ho.szsharing.cn

#include <stdio.h>
来源：http://wt.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fc.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://id.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://iz.shxzukj.cn

[S03] C：读入整数
来源：http://kw.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://gr.nszjky.cn

[S04] C：字符串复制
来源：http://jj.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ib.wgjwhj.cn

[S05] C：字符串长度
来源：http://vt.huixiangedu.cn

strlen(s)
来源：http://mr.shxzskj.cn

[S06] C：字符串比较
来源：http://yz.gzmigu.cn

strcmp(a, b) == 0
来源：http://ib.9csxet.cn

[S07] C：数组遍历求和
来源：http://ff.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://br.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://uh.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ds.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://re.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://of.szxytkj.cn

[S10] C：指针与解引用
来源：http://ye.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://px.szxytkj.cn

[S11] C：逐行读文件
来源：http://jv.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://dm.nicolike.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bq.huixiangedu.cn

fclose(f);
来源：http://pn.wgjwhj.cn

[S12] C：写文件
来源：http://er.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://al.jctech888.com.cn

[S13] C：宏定义
来源：http://ha.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zq.asd995.cn

[S14] C：枚举
来源：http://uy.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://by.haigaiapp.cn

[S15] C：类型转换
来源：http://ug.521024.cn

(double) a / b
来源：http://jg.szsharing.cn

[S16] C：位操作置位
来源：http://db.szsharing.cn

x |= (1 << 3);
来源：http://rb.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://de.muxihuayi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pa.hnjuh.cn

[S18] C：命令行参数
来源：http://oz.jctech888.com.cn

int main(int argc, char **argv)
来源：http://an.newstarts.cn

[S19] C：快速排序
来源：http://xo.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uv.gzmigu.cn

[S20] C：二分查找
来源：http://ln.521024.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://md.yuexingan06.cn

[S21] C：字符类别判断
来源：http://dx.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ly.szsharing.cn

[S22] C：字符串转数字
来源：http://ob.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cx.9csxet.cn

[S23] C：随机数
来源：http://vo.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ad.chemitech.net.cn

[S24] C：获取本地时间
来源：http://lr.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uf.wgjwhj.cn

[S25] C：内存拷贝
来源：http://ib.bjjhwx.cn

memcpy(dst, src, n);
来源：http://hd.9csxet.cn

[S26] C：内存清零
来源：http://hd.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://cr.9csxet.cn

[S27] C：定义常量
来源：http://rf.yuexingan06.cn

const double PI = 3.14159;
来源：http://vr.muxihuayi.cn

[S28] C：静态变量
来源：http://ky.shxzskj.cn

static int counter = 0;
来源：http://xw.huanxung.cn

[S29] C：变参函数
来源：http://gt.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jr.huixiangedu.cn

[S30] C：头文件保护
来源：http://wq.bjjhwx.cn

#ifndef X_H
来源：http://fq.nicolike.cn

#define X_H
来源：http://mn.bjjhwx.cn

#endif
来源：http://ml.huixiangedu.cn

[S31] C++：Hello World
来源：http://xe.haigaiapp.cn

#include <iostream>
来源：http://cs.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://mf.hnjuh.cn

[S32] C++：字符串
来源：http://gh.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://kj.muxihuayi.cn

[S33] C++：vector 增删
来源：http://wh.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ta.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://fd.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://fs.asd995.cn

[S35] C++：map
来源：http://wf.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ew.shxzukj.cn

[S36] C++：unordered_map
来源：http://fz.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tf.wgjwhj.cn

[S37] C++：set
来源：http://mr.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nj.lnxyls.cn

[S38] C++：排序
来源：http://wq.shxzukj.cn

std::sort(v.begin(), v.end());
来源：http://wc.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://fq.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ti.521024.cn

[S40] C++：查找元素
来源：http://vl.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rj.hahajie.cn

[S41] C++：类与构造函数
来源：http://gg.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gd.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://vc.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://jr.shxzukj.cn

[S43] C++：智能指针
来源：http://fj.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://dw.jctech888.com.cn

[S44] C++：引用传参
来源：http://dq.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://xq.chemitech.net.cn

[S45] C++：lambda
来源：http://tq.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ef.hnjuh.cn

[S46] C++：函数模板
来源：http://fi.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fr.yuntaijiaju.cn

[S47] C++：结构化绑定遍历
来源：http://ed.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bs.colortex.cn

[S48] C++：逐行读文件
来源：http://jr.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ip.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://xq.shxzskj.cn

[S49] C++：写文件
来源：http://yf.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sk.9csxet.cn

[S50] C++：格式化数字
来源：http://rk.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zc.hahajie.cn

[S51] C++：显式类型转换
来源：http://ty.szsharing.cn

static_cast<double>(a) / b
来源：http://fq.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://lw.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://rj.lnxyls.cn

[S53] C++：移动语义
来源：http://vx.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://nn.chemitech.net.cn

[S54] C++：异常处理
来源：http://bl.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://so.huanxung.cn

[S55] C++：结构化绑定
来源：http://zf.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bf.shtwfgs.cn

[S56] C++：optional
来源：http://bf.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ou.shtwfgs.cn

[S57] C++：编译期常量
来源：http://fc.szsharing.cn

constexpr int N = 10;
来源：http://hk.hahajie.cn

[S58] C++：命名空间
来源：http://dg.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://vq.colortex.cn

[S59] C++：静态断言
来源：http://ed.shtwfgs.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qx.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://vr.huixinmuqiang.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nt.nszjky.cn

================================================================================
来源：http://zl.jctech888.com.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nv.yuexingan06.cn

================================================================================
来源：http://rb.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://qk.muxihuayi.cn

println("Hello")
来源：http://cg.panjiajie.cn

[T02] Kotlin：变量
来源：http://we.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qy.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://so.bookmarksfly.cn

"值: $b"
来源：http://dg.szxytkj.cn

[T04] Kotlin：空安全
来源：http://xu.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://wy.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://xu.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qj.hahajie.cn

[T06] Kotlin：集合映射
来源：http://op.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hm.panjiajie.cn

[T07] Kotlin：集合过滤
来源：http://tk.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xz.asd995.cn

[T08] Kotlin：数据类
来源：http://um.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://ds.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://lz.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://wv.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://lh.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zg.nicolike.cn

[T11] Kotlin：协程
来源：http://bo.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qm.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://sv.521024.cn

val (a, b) = Pair(1, 2)
来源：http://zy.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://ma.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://cc.szsharing.cn

[T14] Kotlin：循环
来源：http://lx.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://or.szxytkj.cn

[T15] Kotlin：接口
来源：http://yh.colortex.cn

interface Shape { fun area(): Double }
来源：http://og.jctech888.com.cn

[T16] Swift：Hello World
来源：http://wn.newstarts.cn

print("Hello")
来源：http://ux.hahajie.cn

[T17] Swift：变量与常量
来源：http://cb.colortex.cn

var a = 1;  let b = 2
来源：http://di.shxzukj.cn

[T18] Swift：字符串插值
来源：http://cm.nicolike.cn

"值: \(b)"
来源：http://bq.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://zd.haigaiapp.cn

if let n = opt { print(n) }
来源：http://ag.colortex.cn

[T20] Swift：数组操作
来源：http://tz.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qf.colortex.cn

[T21] Swift：遍历
来源：http://uk.jianghongdianzi.cn

for x in a { print(x) }
来源：http://xe.yuntaijiaju.cn

[T22] Swift：字典
来源：http://id.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hw.hahajie.cn


<!-- 参考信息 -->