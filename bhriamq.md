代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://zj.huixiangedu.cn

[R14] C 风格 for
来源：http://qg.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ix.jctech888.com.cn

[R15] while 逐行读文件
来源：http://ey.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hg.bjjhwx.cn

[R16] until 等待条件
来源：http://tf.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lt.colortex.cn

[R17] 数组定义与取值
来源：http://lp.hahajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tu.jianghongdianzi.cn

[R18] 遍历数组
来源：http://fz.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eq.colortex.cn

[R19] 数组长度
来源：http://bt.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://cr.521024.cn

[R20] 关联数组（字典）
来源：http://wg.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tt.yuexingan06.cn

[R21] 字符串长度
来源：http://gz.colortex.cn

echo "${#s}"
来源：http://ds.colortex.cn

[R22] 截取子串
来源：http://cj.shtwfgs.cn

echo "${s:0:5}"
来源：http://sz.szxytkj.cn

[R23] 字符串替换
来源：http://sv.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eu.panjiajie.cn

[R24] 大小写转换
来源：http://bp.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cd.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://up.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vd.shtwfgs.cn

[R26] 命令替换
来源：http://mz.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://do.9csxet.cn

[R27] 算术展开
来源：http://ug.nicolike.cn

echo $((1 + 2 * 3))
来源：http://de.huixiangedu.cn

[R28] 浮点运算
来源：http://ea.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://lh.huanxung.cn

[R29] 定义函数
来源：http://qn.colortex.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ap.asd995.cn

[R30] 函数返回状态码
来源：http://to.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://jf.nszjky.cn

[R31] 局部变量
来源：http://gn.shxzukj.cn

f() { local x=1; echo "$x"; }
来源：http://zm.szxytkj.cn

[R32] 参数个数校验
来源：http://bs.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vy.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://yt.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ld.gzmigu.cn

[R34] 退出时清理
来源：http://us.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yh.nicolike.cn

[R35] 后台执行并等待
来源：http://jz.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lj.panjiajie.cn

[R36] 并发执行多个任务
来源：http://ka.shxzskj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lp.panjiajie.cn

[R37] 把输出赋给变量
来源：http://pg.yuntaijiaju.cn

files=$(ls -1)
来源：http://zx.shxzukj.cn

[R38] 管道串联
来源：http://ig.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://ij.yuexingan06.cn

[R39] 重定向标准输出与错误
来源：http://yw.hnjuh.cn

cmd > out.log 2>&1
来源：http://ec.haigaiapp.cn

[R40] 追加写日志
来源：http://rs.szxytkj.cn

echo "log" >> out.log
来源：http://ep.huanxung.cn

[R41] 丢弃输出
来源：http://nj.colortex.cn

cmd >/dev/null 2>&1
来源：http://tx.colortex.cn

[R42] 输入重定向
来源：http://of.haigaiapp.cn

wc -l < a.txt
来源：http://oq.szxytkj.cn

[R43] 按名字查找文件
来源：http://gp.szsharing.cn

find . -name "*.log" -type f
来源：http://iu.wgjwhj.cn

[R44] 按修改时间查找
来源：http://pe.bjjhwx.cn

find . -mtime -7 -type f
来源：http://ai.huixinmuqiang.cn

[R45] 批量删除
来源：http://un.asd995.cn

find . -name "*.tmp" -delete
来源：http://sy.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://yi.shtwfgs.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ck.nicolike.cn

[R47] sed 单行替换
来源：http://ll.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ix.asd995.cn

[R48] awk 取指定列
来源：http://bf.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://rb.lnxyls.cn

[R49] awk 带条件
来源：http://nq.lnxyls.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bq.newstarts.cn

[R50] awk 求和
来源：http://ps.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dp.huixiangedu.cn

[R51] 排序去重取前几
来源：http://il.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kj.lnxyls.cn

[R52] 统计行数
来源：http://gg.521024.cn

wc -l a.txt
来源：http://km.huanxung.cn

[R53] 查看文件头与实时尾
来源：http://tr.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://eo.gzmigu.cn

[R54] 比较两个文件
来源：http://pm.9csxet.cn

diff a.txt b.txt
来源：http://ba.bjjhwx.cn

[R55] 压缩与解压
来源：http://iw.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://he.shtwfgs.cn

[R56] 远程拷贝
来源：http://oa.huanxung.cn

scp file user@host:/path/
来源：http://ai.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://fe.asd995.cn

ssh user@host 'uptime'
来源：http://xp.nszjky.cn

[R58] 下载文件
来源：http://bx.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://es.lnxyls.cn

[R59] 发 POST JSON
来源：http://fz.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cd.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://tr.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pm.bjjhwx.cn

[R61] 磁盘占用
来源：http://um.chemitech.net.cn

df -h;  du -sh *
来源：http://cm.nszjky.cn

[R62] 找最占空间的文件
来源：http://jz.521024.cn

du -ah . | sort -rh | head -10
来源：http://xd.szxytkj.cn

[R63] 内存与进程
来源：http://hi.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://jd.jianghongdianzi.cn

[R64] 结束进程
来源：http://yn.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://ym.shxzskj.cn

[R65] 查看端口占用
来源：http://uz.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wh.521024.cn

[R66] 定时任务
来源：http://af.wgjwhj.cn

crontab -e;  crontab -l
来源：http://pp.haigaiapp.cn

[R67] 生成随机十六进制串
来源：http://cw.panjiajie.cn

openssl rand -hex 16
来源：http://qy.nszjky.cn

[R68] 计算文件校验值
来源：http://mz.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ik.hahajie.cn

[R69] 生成随机密码
来源：http://ix.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://xq.gzmigu.cn

[R70] 时间戳与互转
来源：http://yk.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://at.bookmarksfly.cn

[R71] 日期格式化
来源：http://na.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uq.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://ca.yuexingan06.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ry.hahajie.cn

[R73] 分割大日志
来源：http://dq.hahajie.cn

split -l 1000 big.log part_
来源：http://al.gzmigu.cn

[R74] 批量重命名
来源：http://rv.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fm.gzmigu.cn

[R75] 导出环境变量
来源：http://mp.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://vd.lnxyls.cn

[R76] 使用临时文件
来源：http://oz.jianghongdianzi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ff.hnjuh.cn

[R77] 读取用户输入
来源：http://zp.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://im.nszjky.cn

[R78] 交互式菜单
来源：http://as.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gp.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://in.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eq.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://or.bookmarksfly.cn

time ./run.sh
来源：http://ou.haigaiapp.cn

================================================================================
来源：http://dz.huixinmuqiang.cn

S. C / C++ 专题
来源：http://wd.hnjuh.cn

================================================================================
来源：http://xa.jctech888.com.cn

[S01] C：Hello World
来源：http://rl.szxytkj.cn

#include <stdio.h>
来源：http://rc.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://te.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://mt.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://vs.huixiangedu.cn

[S03] C：读入整数
来源：http://qx.nszjky.cn

int x; scanf("%d", &x);
来源：http://xi.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://oh.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ge.shxzskj.cn

[S05] C：字符串长度
来源：http://ms.nszjky.cn

strlen(s)
来源：http://ci.szxytkj.cn

[S06] C：字符串比较
来源：http://go.shxzukj.cn

strcmp(a, b) == 0
来源：http://km.hnjuh.cn

[S07] C：数组遍历求和
来源：http://bp.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oa.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://mx.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zt.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://bv.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vm.szsharing.cn

[S10] C：指针与解引用
来源：http://ft.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://id.muxihuayi.cn

[S11] C：逐行读文件
来源：http://hw.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://nd.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nu.szxytkj.cn

fclose(f);
来源：http://zg.huanxung.cn

[S12] C：写文件
来源：http://yy.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gf.muxihuayi.cn

[S13] C：宏定义
来源：http://ar.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ai.asd995.cn

[S14] C：枚举
来源：http://jf.huanxung.cn

enum Color { RED, GREEN, BLUE };
来源：http://oa.chemitech.net.cn

[S15] C：类型转换
来源：http://ve.wgjwhj.cn

(double) a / b
来源：http://iw.shxzukj.cn

[S16] C：位操作置位
来源：http://rx.hahajie.cn

x |= (1 << 3);
来源：http://go.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://bf.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fe.bookmarksfly.cn

[S18] C：命令行参数
来源：http://jh.lnxyls.cn

int main(int argc, char **argv)
来源：http://kp.szsharing.cn

[S19] C：快速排序
来源：http://og.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://op.hnjuh.cn

[S20] C：二分查找
来源：http://kq.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jy.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://om.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fb.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://ha.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://md.huixiangedu.cn

[S23] C：随机数
来源：http://hq.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zg.hnjuh.cn

[S24] C：获取本地时间
来源：http://gr.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gc.9csxet.cn

[S25] C：内存拷贝
来源：http://wl.haigaiapp.cn

memcpy(dst, src, n);
来源：http://wk.bjjhwx.cn

[S26] C：内存清零
来源：http://xv.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://rn.shxzskj.cn

[S27] C：定义常量
来源：http://lz.wgjwhj.cn

const double PI = 3.14159;
来源：http://xw.huixiangedu.cn

[S28] C：静态变量
来源：http://nw.muxihuayi.cn

static int counter = 0;
来源：http://az.nszjky.cn

[S29] C：变参函数
来源：http://zh.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ce.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://an.nicolike.cn

#ifndef X_H
来源：http://fw.shxzukj.cn

#define X_H
来源：http://dd.chemitech.net.cn

#endif
来源：http://tr.hnjuh.cn

[S31] C++：Hello World
来源：http://fe.nszjky.cn

#include <iostream>
来源：http://ua.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://ko.hahajie.cn

[S32] C++：字符串
来源：http://vk.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://hw.gzmigu.cn

[S33] C++：vector 增删
来源：http://et.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rp.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://ew.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://fj.shtwfgs.cn

[S35] C++：map
来源：http://mo.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bg.521024.cn

[S36] C++：unordered_map
来源：http://ma.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ff.szxytkj.cn

[S37] C++：set
来源：http://ng.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mx.bookmarksfly.cn

[S38] C++：排序
来源：http://ry.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://zt.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://ye.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bi.yuexingan06.cn

[S40] C++：查找元素
来源：http://vn.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bx.9csxet.cn

[S41] C++：类与构造函数
来源：http://hw.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bb.szsharing.cn

[S42] C++：继承与虚函数
来源：http://tt.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://se.lnxyls.cn

[S43] C++：智能指针
来源：http://ib.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://ci.521024.cn

[S44] C++：引用传参
来源：http://oa.nicolike.cn

void inc(int &x) { ++x; }
来源：http://hv.nicolike.cn

[S45] C++：lambda
来源：http://id.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fg.jctech888.com.cn

[S46] C++：函数模板
来源：http://bn.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pd.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://ma.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xq.hahajie.cn

[S48] C++：逐行读文件
来源：http://ts.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://up.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://xc.nicolike.cn

[S49] C++：写文件
来源：http://tv.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yk.shxzskj.cn

[S50] C++：格式化数字
来源：http://ia.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sg.colortex.cn

[S51] C++：显式类型转换
来源：http://vs.huanxung.cn

static_cast<double>(a) / b
来源：http://bn.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://uj.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://je.chemitech.net.cn

[S53] C++：移动语义
来源：http://ls.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://au.shtwfgs.cn

[S54] C++：异常处理
来源：http://yg.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fm.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://iv.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mp.yuexingan06.cn

[S56] C++：optional
来源：http://pv.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://id.bjjhwx.cn

[S57] C++：编译期常量
来源：http://js.jianghongdianzi.cn

constexpr int N = 10;
来源：http://jq.shxzukj.cn

[S58] C++：命名空间
来源：http://pa.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://hy.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://ve.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kt.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://ym.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pm.muxihuayi.cn

================================================================================
来源：http://ij.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nd.nicolike.cn

================================================================================
来源：http://gi.nszjky.cn

[T01] Kotlin：Hello World
来源：http://js.muxihuayi.cn

println("Hello")
来源：http://gx.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://hz.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oe.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://uq.asd995.cn

"值: $b"
来源：http://lb.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://iq.newstarts.cn

val n: String? = null;  n?.length
来源：http://hh.521024.cn

[T05] Kotlin：when 表达式
来源：http://yo.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ta.newstarts.cn

[T06] Kotlin：集合映射
来源：http://is.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nj.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://zb.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ew.jctech888.com.cn

[T08] Kotlin：数据类
来源：http://sj.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://lk.gzmigu.cn

[T09] Kotlin：扩展函数
来源：http://ur.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://tz.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://sz.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://iv.chemitech.net.cn

[T11] Kotlin：协程
来源：http://gx.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://om.huanxung.cn

[T12] Kotlin：解构声明
来源：http://rc.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://xa.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://gh.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://wl.hnjuh.cn

[T14] Kotlin：循环
来源：http://yc.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://xd.asd995.cn

[T15] Kotlin：接口
来源：http://aa.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://qe.jctech888.com.cn

[T16] Swift：Hello World
来源：http://tx.jctech888.com.cn

print("Hello")
来源：http://ls.huixinmuqiang.cn


<!-- 参考信息 -->