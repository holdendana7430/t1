代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wa.jctech888.com.cn

[R16] until 等待条件
来源：http://zx.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mj.huixiangedu.cn

[R17] 数组定义与取值
来源：http://ls.bjjhwx.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qx.huixinmuqiang.cn

[R18] 遍历数组
来源：http://rz.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ls.muxihuayi.cn

[R19] 数组长度
来源：http://gu.huanxung.cn

echo "${#arr[@]}"
来源：http://rj.nszjky.cn

[R20] 关联数组（字典）
来源：http://ms.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aj.yuntaijiaju.cn

[R21] 字符串长度
来源：http://am.newstarts.cn

echo "${#s}"
来源：http://wa.szsharing.cn

[R22] 截取子串
来源：http://wj.newstarts.cn

echo "${s:0:5}"
来源：http://ym.nszjky.cn

[R23] 字符串替换
来源：http://an.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sj.lnxyls.cn

[R24] 大小写转换
来源：http://sd.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qo.bjjhwx.cn

[R25] 去后缀 / 去前缀
来源：http://xg.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fl.colortex.cn

[R26] 命令替换
来源：http://as.szxytkj.cn

now=$(date +%F); echo "$now"
来源：http://ya.jianghongdianzi.cn

[R27] 算术展开
来源：http://if.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://qq.bookmarksfly.cn

[R28] 浮点运算
来源：http://nt.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://xo.shxzukj.cn

[R29] 定义函数
来源：http://te.colortex.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oi.jctech888.com.cn

[R30] 函数返回状态码
来源：http://bd.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://qc.shxzukj.cn

[R31] 局部变量
来源：http://xb.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://nu.huixiangedu.cn

[R32] 参数个数校验
来源：http://fn.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ig.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://vh.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gw.wgjwhj.cn

[R34] 退出时清理
来源：http://hd.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tp.lnxyls.cn

[R35] 后台执行并等待
来源：http://qh.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uv.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://ge.shxzskj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jz.huixinmuqiang.cn

[R37] 把输出赋给变量
来源：http://ji.9csxet.cn

files=$(ls -1)
来源：http://nm.yuntaijiaju.cn

[R38] 管道串联
来源：http://ee.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://iy.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://tw.shxzukj.cn

cmd > out.log 2>&1
来源：http://ul.szsharing.cn

[R40] 追加写日志
来源：http://lx.muxihuayi.cn

echo "log" >> out.log
来源：http://ge.shtwfgs.cn

[R41] 丢弃输出
来源：http://na.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://xs.nszjky.cn

[R42] 输入重定向
来源：http://sl.shtwfgs.cn

wc -l < a.txt
来源：http://pp.chemitech.net.cn

[R43] 按名字查找文件
来源：http://rh.jctech888.com.cn

find . -name "*.log" -type f
来源：http://xw.yuexingan06.cn

[R44] 按修改时间查找
来源：http://nk.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://sm.yuexingan06.cn

[R45] 批量删除
来源：http://gi.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://sf.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://zl.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pc.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://lp.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qv.shxzskj.cn

[R48] awk 取指定列
来源：http://ld.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://ni.bjjhwx.cn

[R49] awk 带条件
来源：http://ri.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zd.521024.cn

[R50] awk 求和
来源：http://do.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hl.nicolike.cn

[R51] 排序去重取前几
来源：http://rs.huixiangedu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cp.nszjky.cn

[R52] 统计行数
来源：http://vj.szsharing.cn

wc -l a.txt
来源：http://ar.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://rp.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fv.nszjky.cn

[R54] 比较两个文件
来源：http://zo.wgjwhj.cn

diff a.txt b.txt
来源：http://ie.chemitech.net.cn

[R55] 压缩与解压
来源：http://gd.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qu.muxihuayi.cn

[R56] 远程拷贝
来源：http://kp.szsharing.cn

scp file user@host:/path/
来源：http://lt.nszjky.cn

[R57] 远程执行命令
来源：http://wv.shxzukj.cn

ssh user@host 'uptime'
来源：http://gf.szxytkj.cn

[R58] 下载文件
来源：http://xe.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tg.hnjuh.cn

[R59] 发 POST JSON
来源：http://gu.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yu.yuexingan06.cn

[R60] 只看 HTTP 状态码
来源：http://ch.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fz.asd995.cn

[R61] 磁盘占用
来源：http://tp.gzmigu.cn

df -h;  du -sh *
来源：http://zz.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://vr.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://vi.jctech888.com.cn

[R63] 内存与进程
来源：http://ps.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://wp.nicolike.cn

[R64] 结束进程
来源：http://aa.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://tm.szxytkj.cn

[R65] 查看端口占用
来源：http://qu.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eb.szsharing.cn

[R66] 定时任务
来源：http://ut.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://iu.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://uh.asd995.cn

openssl rand -hex 16
来源：http://mm.muxihuayi.cn

[R68] 计算文件校验值
来源：http://na.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rj.szxytkj.cn

[R69] 生成随机密码
来源：http://qy.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://mp.nszjky.cn

[R70] 时间戳与互转
来源：http://zy.asd995.cn

date +%s;  date -d @1700000000
来源：http://ku.shxzskj.cn

[R71] 日期格式化
来源：http://wj.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fq.9csxet.cn

[R72] 等待端口就绪
来源：http://ie.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://so.szsharing.cn

[R73] 分割大日志
来源：http://pf.jctech888.com.cn

split -l 1000 big.log part_
来源：http://qb.nicolike.cn

[R74] 批量重命名
来源：http://ai.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yg.muxihuayi.cn

[R75] 导出环境变量
来源：http://sd.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://pc.9csxet.cn

[R76] 使用临时文件
来源：http://ab.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://me.521024.cn

[R77] 读取用户输入
来源：http://wy.asd995.cn

read -rp "请输入: " ans
来源：http://uc.colortex.cn

[R78] 交互式菜单
来源：http://no.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://iy.muxihuayi.cn

[R79] 解析命令行选项
来源：http://nx.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xa.yuntaijiaju.cn

[R80] 查看脚本执行耗时
来源：http://fm.szxytkj.cn

time ./run.sh
来源：http://bp.yuexingan06.cn

================================================================================
来源：http://xi.huanxung.cn

S. C / C++ 专题
来源：http://sf.szxytkj.cn

================================================================================
来源：http://wu.szxytkj.cn

[S01] C：Hello World
来源：http://mf.yuexingan06.cn

#include <stdio.h>
来源：http://kq.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jx.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://ad.chemitech.net.cn

int a = 10; printf("%d\n", a);
来源：http://vc.szsharing.cn

[S03] C：读入整数
来源：http://no.hahajie.cn

int x; scanf("%d", &x);
来源：http://lv.shtwfgs.cn

[S04] C：字符串复制
来源：http://ak.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hd.haigaiapp.cn

[S05] C：字符串长度
来源：http://yb.jianghongdianzi.cn

strlen(s)
来源：http://wv.huixiangedu.cn

[S06] C：字符串比较
来源：http://gu.bjjhwx.cn

strcmp(a, b) == 0
来源：http://gx.nszjky.cn

[S07] C：数组遍历求和
来源：http://ra.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lh.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://xh.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ys.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://kl.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rd.shtwfgs.cn

[S10] C：指针与解引用
来源：http://xg.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://bz.szsharing.cn

[S11] C：逐行读文件
来源：http://wl.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://ad.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bk.yuexingan06.cn

fclose(f);
来源：http://gj.muxihuayi.cn

[S12] C：写文件
来源：http://ny.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ql.hahajie.cn

[S13] C：宏定义
来源：http://cu.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pn.bookmarksfly.cn

[S14] C：枚举
来源：http://yo.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://yd.muxihuayi.cn

[S15] C：类型转换
来源：http://qn.shtwfgs.cn

(double) a / b
来源：http://ll.yuexingan06.cn

[S16] C：位操作置位
来源：http://ub.shxzukj.cn

x |= (1 << 3);
来源：http://rt.9csxet.cn

[S17] C：安全拼接字符串
来源：http://uz.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ee.panjiajie.cn

[S18] C：命令行参数
来源：http://ur.nszjky.cn

int main(int argc, char **argv)
来源：http://sv.521024.cn

[S19] C：快速排序
来源：http://lu.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dn.bjjhwx.cn

[S20] C：二分查找
来源：http://ol.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vd.yuexingan06.cn

[S21] C：字符类别判断
来源：http://kr.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ur.haigaiapp.cn

[S22] C：字符串转数字
来源：http://rr.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jianghongdianzi.cn

[S23] C：随机数
来源：http://ei.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nx.gzmigu.cn

[S24] C：获取本地时间
来源：http://oc.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://de.muxihuayi.cn

[S25] C：内存拷贝
来源：http://ad.nszjky.cn

memcpy(dst, src, n);
来源：http://gq.huixinmuqiang.cn

[S26] C：内存清零
来源：http://ma.nicolike.cn

memset(a, 0, sizeof a);
来源：http://fw.bookmarksfly.cn

[S27] C：定义常量
来源：http://qs.asd995.cn

const double PI = 3.14159;
来源：http://dk.nicolike.cn

[S28] C：静态变量
来源：http://xq.huixinmuqiang.cn

static int counter = 0;
来源：http://nj.jctech888.com.cn

[S29] C：变参函数
来源：http://ia.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sq.haigaiapp.cn

[S30] C：头文件保护
来源：http://zp.shxzskj.cn

#ifndef X_H
来源：http://vq.panjiajie.cn

#define X_H
来源：http://hy.muxihuayi.cn

#endif
来源：http://iu.521024.cn

[S31] C++：Hello World
来源：http://rw.9csxet.cn

#include <iostream>
来源：http://ns.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://zc.shxzukj.cn

[S32] C++：字符串
来源：http://xn.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://fc.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://rd.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rp.huanxung.cn

[S34] C++：遍历 vector
来源：http://qr.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://ij.newstarts.cn

[S35] C++：map
来源：http://dz.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lz.bjjhwx.cn

[S36] C++：unordered_map
来源：http://bp.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ip.gzmigu.cn

[S37] C++：set
来源：http://ij.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bd.asd995.cn

[S38] C++：排序
来源：http://pi.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://iw.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://fx.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bi.muxihuayi.cn

[S40] C++：查找元素
来源：http://qi.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ql.hahajie.cn

[S41] C++：类与构造函数
来源：http://ag.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://di.9csxet.cn

[S42] C++：继承与虚函数
来源：http://ev.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://lq.shxzukj.cn

[S43] C++：智能指针
来源：http://ko.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://iv.muxihuayi.cn

[S44] C++：引用传参
来源：http://sj.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://zk.huixiangedu.cn

[S45] C++：lambda
来源：http://md.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lb.szsharing.cn

[S46] C++：函数模板
来源：http://si.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sp.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://su.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gs.gzmigu.cn

[S48] C++：逐行读文件
来源：http://ti.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://us.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://fd.shtwfgs.cn

[S49] C++：写文件
来源：http://lr.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jt.lnxyls.cn

[S50] C++：格式化数字
来源：http://ym.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jb.gzmigu.cn

[S51] C++：显式类型转换
来源：http://gd.shtwfgs.cn

static_cast<double>(a) / b
来源：http://fm.gzmigu.cn

[S52] C++：const 与 noexcept
来源：http://ae.colortex.cn

int size() const noexcept { return n_; }
来源：http://hg.haigaiapp.cn

[S53] C++：移动语义
来源：http://gr.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://tv.nszjky.cn

[S54] C++：异常处理
来源：http://pi.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pi.lnxyls.cn

[S55] C++：结构化绑定
来源：http://nn.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tm.bjjhwx.cn

[S56] C++：optional
来源：http://wk.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cp.nszjky.cn

[S57] C++：编译期常量
来源：http://mx.shxzskj.cn

constexpr int N = 10;
来源：http://dd.chemitech.net.cn

[S58] C++：命名空间
来源：http://eu.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://si.newstarts.cn

[S59] C++：静态断言
来源：http://ds.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jf.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://xu.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dk.shxzskj.cn

================================================================================
来源：http://mz.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vn.lnxyls.cn

================================================================================
来源：http://pq.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://xf.yuexingan06.cn

println("Hello")
来源：http://kl.shtwfgs.cn

[T02] Kotlin：变量
来源：http://dq.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rc.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://vh.9csxet.cn

"值: $b"
来源：http://mj.521024.cn

[T04] Kotlin：空安全
来源：http://oe.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://ww.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://az.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ec.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://us.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hv.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://tb.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ca.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://zn.colortex.cn

data class User(val name: String, val age: Int)
来源：http://ky.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://jt.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://or.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://ur.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kn.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://yh.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bq.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://cd.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://bf.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://ao.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://ey.nszjky.cn

[T14] Kotlin：循环
来源：http://fg.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://tj.hnjuh.cn

[T15] Kotlin：接口
来源：http://oy.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://ik.yuexingan06.cn

[T16] Swift：Hello World
来源：http://by.bookmarksfly.cn

print("Hello")
来源：http://ax.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://ou.shxzskj.cn

var a = 1;  let b = 2
来源：http://vy.huanxung.cn

[T18] Swift：字符串插值
来源：http://fb.521024.cn

"值: \(b)"
来源：http://tf.9csxet.cn


<!-- 参考信息 -->