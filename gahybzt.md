代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://fc.panjiajie.cn

[R18] 遍历数组
来源：http://ko.szxytkj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ig.gzmigu.cn

[R19] 数组长度
来源：http://vc.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://lf.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://kb.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://li.muxihuayi.cn

[R21] 字符串长度
来源：http://al.muxihuayi.cn

echo "${#s}"
来源：http://kq.nicolike.cn

[R22] 截取子串
来源：http://pm.huanxung.cn

echo "${s:0:5}"
来源：http://tj.colortex.cn

[R23] 字符串替换
来源：http://et.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://br.asd995.cn

[R24] 大小写转换
来源：http://jo.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yt.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://xa.huanxung.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://iz.bjjhwx.cn

[R26] 命令替换
来源：http://ea.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://li.wgjwhj.cn

[R27] 算术展开
来源：http://ij.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://oz.chemitech.net.cn

[R28] 浮点运算
来源：http://ep.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://qd.szxytkj.cn

[R29] 定义函数
来源：http://hd.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fg.shxzskj.cn

[R30] 函数返回状态码
来源：http://wn.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://gt.jianghongdianzi.cn

[R31] 局部变量
来源：http://nu.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://ns.chemitech.net.cn

[R32] 参数个数校验
来源：http://rf.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mo.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://dh.hnjuh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mc.huixiangedu.cn

[R34] 退出时清理
来源：http://gl.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mw.nszjky.cn

[R35] 后台执行并等待
来源：http://zh.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dc.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://rb.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kv.colortex.cn

[R37] 把输出赋给变量
来源：http://km.panjiajie.cn

files=$(ls -1)
来源：http://ac.haigaiapp.cn

[R38] 管道串联
来源：http://fy.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://tu.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://wx.colortex.cn

cmd > out.log 2>&1
来源：http://zz.bjjhwx.cn

[R40] 追加写日志
来源：http://qz.yuntaijiaju.cn

echo "log" >> out.log
来源：http://uq.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://zc.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://yb.shxzskj.cn

[R42] 输入重定向
来源：http://wk.colortex.cn

wc -l < a.txt
来源：http://ud.bjjhwx.cn

[R43] 按名字查找文件
来源：http://zh.huanxung.cn

find . -name "*.log" -type f
来源：http://cb.yuexingan06.cn

[R44] 按修改时间查找
来源：http://pv.huanxung.cn

find . -mtime -7 -type f
来源：http://za.colortex.cn

[R45] 批量删除
来源：http://wo.colortex.cn

find . -name "*.tmp" -delete
来源：http://tj.huixiangedu.cn

[R46] 递归替换文件内容
来源：http://vi.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://op.nicolike.cn

[R47] sed 单行替换
来源：http://ww.panjiajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fg.shtwfgs.cn

[R48] awk 取指定列
来源：http://ab.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://hx.panjiajie.cn

[R49] awk 带条件
来源：http://ss.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nn.yuexingan06.cn

[R50] awk 求和
来源：http://af.bjjhwx.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ff.nszjky.cn

[R51] 排序去重取前几
来源：http://vc.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hl.gzmigu.cn

[R52] 统计行数
来源：http://ki.panjiajie.cn

wc -l a.txt
来源：http://sv.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://dr.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fi.wgjwhj.cn

[R54] 比较两个文件
来源：http://mv.haigaiapp.cn

diff a.txt b.txt
来源：http://oc.muxihuayi.cn

[R55] 压缩与解压
来源：http://ao.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hm.nszjky.cn

[R56] 远程拷贝
来源：http://gs.szxytkj.cn

scp file user@host:/path/
来源：http://yn.bookmarksfly.cn

[R57] 远程执行命令
来源：http://yb.jctech888.com.cn

ssh user@host 'uptime'
来源：http://sb.bookmarksfly.cn

[R58] 下载文件
来源：http://ju.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://no.wgjwhj.cn

[R59] 发 POST JSON
来源：http://jx.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ap.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://li.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iy.muxihuayi.cn

[R61] 磁盘占用
来源：http://zr.newstarts.cn

df -h;  du -sh *
来源：http://ry.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://cw.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://xz.shxzukj.cn

[R63] 内存与进程
来源：http://fk.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://ae.panjiajie.cn

[R64] 结束进程
来源：http://wg.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://sl.shxzskj.cn

[R65] 查看端口占用
来源：http://rq.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uf.hahajie.cn

[R66] 定时任务
来源：http://vm.yuexingan06.cn

crontab -e;  crontab -l
来源：http://vg.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://bj.huixiangedu.cn

openssl rand -hex 16
来源：http://ne.szxytkj.cn

[R68] 计算文件校验值
来源：http://jh.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xd.haigaiapp.cn

[R69] 生成随机密码
来源：http://vx.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://xa.panjiajie.cn

[R70] 时间戳与互转
来源：http://st.521024.cn

date +%s;  date -d @1700000000
来源：http://sp.521024.cn

[R71] 日期格式化
来源：http://zb.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://aw.szxytkj.cn

[R72] 等待端口就绪
来源：http://fh.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xe.haigaiapp.cn

[R73] 分割大日志
来源：http://wj.hahajie.cn

split -l 1000 big.log part_
来源：http://te.szxytkj.cn

[R74] 批量重命名
来源：http://da.9csxet.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zo.muxihuayi.cn

[R75] 导出环境变量
来源：http://nu.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://pd.huanxung.cn

[R76] 使用临时文件
来源：http://ev.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yb.szsharing.cn

[R77] 读取用户输入
来源：http://st.hnjuh.cn

read -rp "请输入: " ans
来源：http://aq.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://fc.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://de.haigaiapp.cn

[R79] 解析命令行选项
来源：http://mi.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cp.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://fl.szxytkj.cn

time ./run.sh
来源：http://no.jianghongdianzi.cn

================================================================================
来源：http://sz.huixinmuqiang.cn

S. C / C++ 专题
来源：http://al.yuntaijiaju.cn

================================================================================
来源：http://ay.bookmarksfly.cn

[S01] C：Hello World
来源：http://df.lnxyls.cn

#include <stdio.h>
来源：http://mo.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://de.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://ez.521024.cn

int a = 10; printf("%d\n", a);
来源：http://ku.shxzskj.cn

[S03] C：读入整数
来源：http://fy.szsharing.cn

int x; scanf("%d", &x);
来源：http://ah.shxzskj.cn

[S04] C：字符串复制
来源：http://ot.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lz.newstarts.cn

[S05] C：字符串长度
来源：http://yv.shtwfgs.cn

strlen(s)
来源：http://tf.newstarts.cn

[S06] C：字符串比较
来源：http://oc.huanxung.cn

strcmp(a, b) == 0
来源：http://kr.hnjuh.cn

[S07] C：数组遍历求和
来源：http://zj.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hd.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://mm.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ji.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://cb.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rj.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://vs.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://tg.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://mp.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://pn.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nv.szsharing.cn

fclose(f);
来源：http://ho.huixiangedu.cn

[S12] C：写文件
来源：http://kj.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ia.haigaiapp.cn

[S13] C：宏定义
来源：http://yx.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bz.bjjhwx.cn

[S14] C：枚举
来源：http://in.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://vi.haigaiapp.cn

[S15] C：类型转换
来源：http://rq.shxzukj.cn

(double) a / b
来源：http://ml.bjjhwx.cn

[S16] C：位操作置位
来源：http://ng.huixinmuqiang.cn

x |= (1 << 3);
来源：http://wu.huanxung.cn

[S17] C：安全拼接字符串
来源：http://uf.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fp.hnjuh.cn

[S18] C：命令行参数
来源：http://qk.muxihuayi.cn

int main(int argc, char **argv)
来源：http://te.yuntaijiaju.cn

[S19] C：快速排序
来源：http://gf.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kr.shxzskj.cn

[S20] C：二分查找
来源：http://ss.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jf.muxihuayi.cn

[S21] C：字符类别判断
来源：http://en.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eu.9csxet.cn

[S22] C：字符串转数字
来源：http://ka.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hw.bjjhwx.cn

[S23] C：随机数
来源：http://jm.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xc.szsharing.cn

[S24] C：获取本地时间
来源：http://rc.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sb.shtwfgs.cn

[S25] C：内存拷贝
来源：http://hg.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://xn.gzmigu.cn

[S26] C：内存清零
来源：http://nj.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://uo.szsharing.cn

[S27] C：定义常量
来源：http://vz.jianghongdianzi.cn

const double PI = 3.14159;
来源：http://ir.asd995.cn

[S28] C：静态变量
来源：http://qn.lnxyls.cn

static int counter = 0;
来源：http://vu.shtwfgs.cn

[S29] C：变参函数
来源：http://zb.yuexingan06.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xn.bjjhwx.cn

[S30] C：头文件保护
来源：http://xj.shxzukj.cn

#ifndef X_H
来源：http://mr.jctech888.com.cn

#define X_H
来源：http://pj.yuexingan06.cn

#endif
来源：http://kl.szsharing.cn

[S31] C++：Hello World
来源：http://dq.chemitech.net.cn

#include <iostream>
来源：http://yu.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://mm.colortex.cn

[S32] C++：字符串
来源：http://qg.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://kw.gzmigu.cn

[S33] C++：vector 增删
来源：http://oa.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cp.asd995.cn

[S34] C++：遍历 vector
来源：http://zt.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://yw.szsharing.cn

[S35] C++：map
来源：http://on.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wp.gzmigu.cn

[S36] C++：unordered_map
来源：http://uo.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ls.panjiajie.cn

[S37] C++：set
来源：http://ez.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ho.muxihuayi.cn

[S38] C++：排序
来源：http://jy.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://sw.521024.cn

[S39] C++：自定义比较器排序
来源：http://ia.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ni.chemitech.net.cn

[S40] C++：查找元素
来源：http://tx.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hq.shxzukj.cn

[S41] C++：类与构造函数
来源：http://tf.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mh.yuntaijiaju.cn

[S42] C++：继承与虚函数
来源：http://qi.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://aa.shxzskj.cn

[S43] C++：智能指针
来源：http://og.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://yy.hahajie.cn

[S44] C++：引用传参
来源：http://rl.9csxet.cn

void inc(int &x) { ++x; }
来源：http://gu.bookmarksfly.cn

[S45] C++：lambda
来源：http://cj.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ac.shxzskj.cn

[S46] C++：函数模板
来源：http://du.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eh.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://kt.9csxet.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hi.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://lh.shxzskj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vp.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://gl.gzmigu.cn

[S49] C++：写文件
来源：http://yb.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ev.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://jk.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kt.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://sv.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://vl.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://xc.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://jb.szxytkj.cn

[S53] C++：移动语义
来源：http://je.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://we.panjiajie.cn

[S54] C++：异常处理
来源：http://qs.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dr.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://ru.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wr.jianghongdianzi.cn

[S56] C++：optional
来源：http://lf.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xm.521024.cn

[S57] C++：编译期常量
来源：http://md.wgjwhj.cn

constexpr int N = 10;
来源：http://dm.9csxet.cn

[S58] C++：命名空间
来源：http://hb.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://ze.shxzskj.cn

[S59] C++：静态断言
来源：http://ac.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fy.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://at.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zn.gzmigu.cn

================================================================================
来源：http://aq.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oe.haigaiapp.cn

================================================================================
来源：http://of.colortex.cn

[T01] Kotlin：Hello World
来源：http://ke.yuexingan06.cn

println("Hello")
来源：http://vj.gzmigu.cn

[T02] Kotlin：变量
来源：http://uq.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qc.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://rp.muxihuayi.cn

"值: $b"
来源：http://vk.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://yv.szxytkj.cn

val n: String? = null;  n?.length
来源：http://zx.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://jb.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tc.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://wk.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wv.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://xf.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ys.nszjky.cn

[T08] Kotlin：数据类
来源：http://vt.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://qh.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://sh.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://vu.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://hk.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fq.521024.cn

[T11] Kotlin：协程
来源：http://lf.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xz.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://da.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://tl.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://gf.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://wd.muxihuayi.cn

[T14] Kotlin：循环
来源：http://pz.shxzukj.cn

for (i in 1..10) println(i)
来源：http://mn.nicolike.cn

[T15] Kotlin：接口
来源：http://hf.bjjhwx.cn

interface Shape { fun area(): Double }
来源：http://yd.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://qe.huixinmuqiang.cn

print("Hello")
来源：http://dz.nszjky.cn

[T17] Swift：变量与常量
来源：http://qf.shxzskj.cn

var a = 1;  let b = 2
来源：http://ox.hnjuh.cn

[T18] Swift：字符串插值
来源：http://wy.huixinmuqiang.cn

"值: \(b)"
来源：http://ei.hahajie.cn

[T19] Swift：可选绑定
来源：http://bq.haigaiapp.cn

if let n = opt { print(n) }
来源：http://jn.colortex.cn

[T20] Swift：数组操作
来源：http://cp.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uu.nicolike.cn


<!-- 参考信息 -->