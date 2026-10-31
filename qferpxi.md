代发 wailian999

esac
来源：http://jn.muxihuayi.cn

[R12] for 遍历文件
来源：http://mq.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://ej.bjjhwx.cn

[R13] for 计数循环
来源：http://kk.yuntaijiaju.cn

for i in {1..10}; do echo "$i"; done
来源：http://oa.nszjky.cn

[R14] C 风格 for
来源：http://za.yuntaijiaju.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zg.yuexingan06.cn

[R15] while 逐行读文件
来源：http://rg.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ps.panjiajie.cn

[R16] until 等待条件
来源：http://mv.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rm.9csxet.cn

[R17] 数组定义与取值
来源：http://kd.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ox.bjjhwx.cn

[R18] 遍历数组
来源：http://ow.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aw.haigaiapp.cn

[R19] 数组长度
来源：http://vl.newstarts.cn

echo "${#arr[@]}"
来源：http://oj.hahajie.cn

[R20] 关联数组（字典）
来源：http://nn.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ix.bjjhwx.cn

[R21] 字符串长度
来源：http://pe.muxihuayi.cn

echo "${#s}"
来源：http://wo.yuntaijiaju.cn

[R22] 截取子串
来源：http://ul.shtwfgs.cn

echo "${s:0:5}"
来源：http://pv.huixinmuqiang.cn

[R23] 字符串替换
来源：http://ux.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qv.colortex.cn

[R24] 大小写转换
来源：http://ob.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ql.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://zb.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xa.haigaiapp.cn

[R26] 命令替换
来源：http://dq.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://mu.huixiangedu.cn

[R27] 算术展开
来源：http://oi.hahajie.cn

echo $((1 + 2 * 3))
来源：http://zu.nicolike.cn

[R28] 浮点运算
来源：http://sl.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://og.521024.cn

[R29] 定义函数
来源：http://wa.yuntaijiaju.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dp.nicolike.cn

[R30] 函数返回状态码
来源：http://pu.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://wb.bjjhwx.cn

[R31] 局部变量
来源：http://ip.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://dc.gzmigu.cn

[R32] 参数个数校验
来源：http://ie.huixinmuqiang.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xv.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://iv.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ac.wgjwhj.cn

[R34] 退出时清理
来源：http://hi.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vu.521024.cn

[R35] 后台执行并等待
来源：http://tw.jianghongdianzi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fz.lnxyls.cn

[R36] 并发执行多个任务
来源：http://nu.shxzukj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eg.panjiajie.cn

[R37] 把输出赋给变量
来源：http://rr.szxytkj.cn

files=$(ls -1)
来源：http://ew.newstarts.cn

[R38] 管道串联
来源：http://uf.shxzukj.cn

cat a.txt | grep -i error | wc -l
来源：http://yi.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://yx.jctech888.com.cn

cmd > out.log 2>&1
来源：http://qg.jianghongdianzi.cn

[R40] 追加写日志
来源：http://ax.shxzskj.cn

echo "log" >> out.log
来源：http://qs.hnjuh.cn

[R41] 丢弃输出
来源：http://yf.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://bx.panjiajie.cn

[R42] 输入重定向
来源：http://lq.szxytkj.cn

wc -l < a.txt
来源：http://je.gzmigu.cn

[R43] 按名字查找文件
来源：http://qq.lnxyls.cn

find . -name "*.log" -type f
来源：http://uo.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://re.chemitech.net.cn

find . -mtime -7 -type f
来源：http://li.shtwfgs.cn

[R45] 批量删除
来源：http://py.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://jb.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://tv.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qn.hahajie.cn

[R47] sed 单行替换
来源：http://ka.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wv.shxzukj.cn

[R48] awk 取指定列
来源：http://cg.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://jv.lnxyls.cn

[R49] awk 带条件
来源：http://xl.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gv.hahajie.cn

[R50] awk 求和
来源：http://iw.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kp.shxzukj.cn

[R51] 排序去重取前几
来源：http://fr.huixiangedu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://do.nszjky.cn

[R52] 统计行数
来源：http://yi.jianghongdianzi.cn

wc -l a.txt
来源：http://nd.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://hb.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gh.hahajie.cn

[R54] 比较两个文件
来源：http://gg.wgjwhj.cn

diff a.txt b.txt
来源：http://oi.newstarts.cn

[R55] 压缩与解压
来源：http://at.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://my.huixiangedu.cn

[R56] 远程拷贝
来源：http://ud.gzmigu.cn

scp file user@host:/path/
来源：http://ey.shxzskj.cn

[R57] 远程执行命令
来源：http://zy.wgjwhj.cn

ssh user@host 'uptime'
来源：http://ji.wgjwhj.cn

[R58] 下载文件
来源：http://im.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sf.szxytkj.cn

[R59] 发 POST JSON
来源：http://cu.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ma.jianghongdianzi.cn

[R60] 只看 HTTP 状态码
来源：http://ml.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://va.szsharing.cn

[R61] 磁盘占用
来源：http://gn.shxzskj.cn

df -h;  du -sh *
来源：http://om.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://qc.521024.cn

du -ah . | sort -rh | head -10
来源：http://yy.bjjhwx.cn

[R63] 内存与进程
来源：http://om.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://vs.bookmarksfly.cn

[R64] 结束进程
来源：http://zd.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://fd.chemitech.net.cn

[R65] 查看端口占用
来源：http://kv.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vg.asd995.cn

[R66] 定时任务
来源：http://pg.panjiajie.cn

crontab -e;  crontab -l
来源：http://me.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://jt.nszjky.cn

openssl rand -hex 16
来源：http://tm.huanxung.cn

[R68] 计算文件校验值
来源：http://yi.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ud.newstarts.cn

[R69] 生成随机密码
来源：http://hl.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://ic.colortex.cn

[R70] 时间戳与互转
来源：http://md.asd995.cn

date +%s;  date -d @1700000000
来源：http://me.shtwfgs.cn

[R71] 日期格式化
来源：http://kt.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xe.hahajie.cn

[R72] 等待端口就绪
来源：http://ft.jianghongdianzi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ei.muxihuayi.cn

[R73] 分割大日志
来源：http://zz.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://zi.hnjuh.cn

[R74] 批量重命名
来源：http://qa.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nx.jctech888.com.cn

[R75] 导出环境变量
来源：http://ks.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://uj.newstarts.cn

[R76] 使用临时文件
来源：http://fg.shxzukj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tx.521024.cn

[R77] 读取用户输入
来源：http://gt.hahajie.cn

read -rp "请输入: " ans
来源：http://fg.asd995.cn

[R78] 交互式菜单
来源：http://sv.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mr.shtwfgs.cn

[R79] 解析命令行选项
来源：http://hh.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zj.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://rc.chemitech.net.cn

time ./run.sh
来源：http://do.gzmigu.cn

================================================================================
来源：http://ay.bookmarksfly.cn

S. C / C++ 专题
来源：http://da.521024.cn

================================================================================
来源：http://nv.lnxyls.cn

[S01] C：Hello World
来源：http://dm.jianghongdianzi.cn

#include <stdio.h>
来源：http://xk.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ep.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://yz.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://pn.nicolike.cn

[S03] C：读入整数
来源：http://qc.521024.cn

int x; scanf("%d", &x);
来源：http://hd.huanxung.cn

[S04] C：字符串复制
来源：http://lm.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://av.wgjwhj.cn

[S05] C：字符串长度
来源：http://zn.hahajie.cn

strlen(s)
来源：http://xf.bjjhwx.cn

[S06] C：字符串比较
来源：http://vy.9csxet.cn

strcmp(a, b) == 0
来源：http://xr.521024.cn

[S07] C：数组遍历求和
来源：http://hw.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lr.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://ko.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jo.colortex.cn

[S09] C：结构体定义与初始化
来源：http://jv.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://el.bjjhwx.cn

[S10] C：指针与解引用
来源：http://kj.asd995.cn

int *p = &a;  *p = 5;
来源：http://fe.nicolike.cn

[S11] C：逐行读文件
来源：http://he.haigaiapp.cn

FILE *f = fopen("a.txt", "r");
来源：http://sk.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ri.wgjwhj.cn

fclose(f);
来源：http://no.haigaiapp.cn

[S12] C：写文件
来源：http://mu.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rz.haigaiapp.cn

[S13] C：宏定义
来源：http://lc.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qi.asd995.cn

[S14] C：枚举
来源：http://vm.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://ax.huixinmuqiang.cn

[S15] C：类型转换
来源：http://ee.haigaiapp.cn

(double) a / b
来源：http://tr.lnxyls.cn

[S16] C：位操作置位
来源：http://mg.bookmarksfly.cn

x |= (1 << 3);
来源：http://ok.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://ef.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hn.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://md.haigaiapp.cn

int main(int argc, char **argv)
来源：http://cu.bookmarksfly.cn

[S19] C：快速排序
来源：http://wq.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zu.szsharing.cn

[S20] C：二分查找
来源：http://wn.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sn.yuexingan06.cn

[S21] C：字符类别判断
来源：http://da.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://in.hahajie.cn

[S22] C：字符串转数字
来源：http://zc.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hq.huanxung.cn

[S23] C：随机数
来源：http://hk.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://do.panjiajie.cn

[S24] C：获取本地时间
来源：http://kh.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qd.asd995.cn

[S25] C：内存拷贝
来源：http://uy.lnxyls.cn

memcpy(dst, src, n);
来源：http://mq.gzmigu.cn

[S26] C：内存清零
来源：http://ou.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://qd.szxytkj.cn

[S27] C：定义常量
来源：http://vc.panjiajie.cn

const double PI = 3.14159;
来源：http://gq.bjjhwx.cn

[S28] C：静态变量
来源：http://eu.panjiajie.cn

static int counter = 0;
来源：http://bx.asd995.cn

[S29] C：变参函数
来源：http://fi.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sx.szsharing.cn

[S30] C：头文件保护
来源：http://zd.shtwfgs.cn

#ifndef X_H
来源：http://zs.wgjwhj.cn

#define X_H
来源：http://at.huanxung.cn

#endif
来源：http://tn.bjjhwx.cn

[S31] C++：Hello World
来源：http://px.lnxyls.cn

#include <iostream>
来源：http://st.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://fi.bookmarksfly.cn

[S32] C++：字符串
来源：http://yf.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://tv.colortex.cn

[S33] C++：vector 增删
来源：http://ph.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iw.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://ms.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://lm.asd995.cn

[S35] C++：map
来源：http://nt.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ki.wgjwhj.cn

[S36] C++：unordered_map
来源：http://sc.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xy.gzmigu.cn

[S37] C++：set
来源：http://jr.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tq.shxzukj.cn

[S38] C++：排序
来源：http://ng.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://rl.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://qz.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uo.bjjhwx.cn

[S40] C++：查找元素
来源：http://mz.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cj.newstarts.cn

[S41] C++：类与构造函数
来源：http://tw.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ni.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://ah.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://ha.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://fw.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://xf.hnjuh.cn

[S44] C++：引用传参
来源：http://dm.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://hj.yuexingan06.cn

[S45] C++：lambda
来源：http://ap.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ek.newstarts.cn

[S46] C++：函数模板
来源：http://jr.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nv.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://oi.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://di.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://sm.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xp.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://qg.huanxung.cn

[S49] C++：写文件
来源：http://bw.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nn.huanxung.cn

[S50] C++：格式化数字
来源：http://gf.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fy.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://ba.hahajie.cn

static_cast<double>(a) / b
来源：http://oi.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://uv.521024.cn

int size() const noexcept { return n_; }
来源：http://be.bjjhwx.cn

[S53] C++：移动语义
来源：http://fu.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://kq.asd995.cn

[S54] C++：异常处理
来源：http://aj.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hy.521024.cn

[S55] C++：结构化绑定
来源：http://if.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ts.colortex.cn

[S56] C++：optional
来源：http://if.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rv.shtwfgs.cn

[S57] C++：编译期常量
来源：http://mu.bookmarksfly.cn

constexpr int N = 10;
来源：http://zx.wgjwhj.cn

[S58] C++：命名空间
来源：http://fc.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://go.nicolike.cn

[S59] C++：静态断言
来源：http://ht.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uq.huixinmuqiang.cn

[S60] C++：遍历并删除元素
来源：http://nl.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vw.jctech888.com.cn

================================================================================
来源：http://lg.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rl.shtwfgs.cn

================================================================================
来源：http://hi.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://fx.panjiajie.cn

println("Hello")
来源：http://bl.hnjuh.cn

[T02] Kotlin：变量
来源：http://ke.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fn.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://ss.huixiangedu.cn

"值: $b"
来源：http://af.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://ot.hahajie.cn

val n: String? = null;  n?.length
来源：http://do.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://vd.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bv.hahajie.cn

[T06] Kotlin：集合映射
来源：http://xp.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oz.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://yl.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fc.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://ym.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://ws.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://an.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://mz.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://wj.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://al.gzmigu.cn

[T11] Kotlin：协程
来源：http://io.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ok.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://fi.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://aa.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://tt.nszjky.cn

val m = mapOf("a" to 1)
来源：http://kr.huixiangedu.cn

[T14] Kotlin：循环
来源：http://aj.jctech888.com.cn

for (i in 1..10) println(i)
来源：http://od.bjjhwx.cn


<!-- 参考信息 -->