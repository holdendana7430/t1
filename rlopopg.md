代发 wailian999

case "$1" in
来源：http://ic.yuexingan06.cn

start) echo "启动" ;;
来源：http://cp.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://vn.wgjwhj.cn

*)     echo "未知命令" ;;
来源：http://zq.asd995.cn

esac
来源：http://hr.huixiangedu.cn

[R12] for 遍历文件
来源：http://hf.haigaiapp.cn

for f in *.txt; do echo "$f"; done
来源：http://aw.hnjuh.cn

[R13] for 计数循环
来源：http://cb.yuntaijiaju.cn

for i in {1..10}; do echo "$i"; done
来源：http://sx.shtwfgs.cn

[R14] C 风格 for
来源：http://qw.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ty.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://cu.yuexingan06.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nv.yuntaijiaju.cn

[R16] until 等待条件
来源：http://em.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ur.jianghongdianzi.cn

[R17] 数组定义与取值
来源：http://lr.hahajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nr.yuntaijiaju.cn

[R18] 遍历数组
来源：http://vi.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hn.jianghongdianzi.cn

[R19] 数组长度
来源：http://pj.yuexingan06.cn

echo "${#arr[@]}"
来源：http://cp.lnxyls.cn

[R20] 关联数组（字典）
来源：http://ml.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://na.chemitech.net.cn

[R21] 字符串长度
来源：http://vm.gzmigu.cn

echo "${#s}"
来源：http://pq.yuexingan06.cn

[R22] 截取子串
来源：http://ch.9csxet.cn

echo "${s:0:5}"
来源：http://bn.huixiangedu.cn

[R23] 字符串替换
来源：http://bm.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vg.hahajie.cn

[R24] 大小写转换
来源：http://za.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hb.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://vk.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xx.gzmigu.cn

[R26] 命令替换
来源：http://dx.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://en.wgjwhj.cn

[R27] 算术展开
来源：http://xm.wgjwhj.cn

echo $((1 + 2 * 3))
来源：http://lb.9csxet.cn

[R28] 浮点运算
来源：http://pp.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://uw.hahajie.cn

[R29] 定义函数
来源：http://ao.szxytkj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ep.9csxet.cn

[R30] 函数返回状态码
来源：http://hq.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://pl.huixinmuqiang.cn

[R31] 局部变量
来源：http://rm.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://zf.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://gq.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xx.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://zh.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cc.gzmigu.cn

[R34] 退出时清理
来源：http://lo.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fb.muxihuayi.cn

[R35] 后台执行并等待
来源：http://wj.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uj.asd995.cn

[R36] 并发执行多个任务
来源：http://tr.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ke.huanxung.cn

[R37] 把输出赋给变量
来源：http://eq.newstarts.cn

files=$(ls -1)
来源：http://pe.muxihuayi.cn

[R38] 管道串联
来源：http://zv.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://yo.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://jk.huanxung.cn

cmd > out.log 2>&1
来源：http://ng.gzmigu.cn

[R40] 追加写日志
来源：http://br.jianghongdianzi.cn

echo "log" >> out.log
来源：http://em.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://jw.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://hm.newstarts.cn

[R42] 输入重定向
来源：http://jx.chemitech.net.cn

wc -l < a.txt
来源：http://yt.jctech888.com.cn

[R43] 按名字查找文件
来源：http://gj.huixiangedu.cn

find . -name "*.log" -type f
来源：http://an.asd995.cn

[R44] 按修改时间查找
来源：http://ov.huixinmuqiang.cn

find . -mtime -7 -type f
来源：http://ql.asd995.cn

[R45] 批量删除
来源：http://vc.newstarts.cn

find . -name "*.tmp" -delete
来源：http://vn.newstarts.cn

[R46] 递归替换文件内容
来源：http://av.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://be.shxzskj.cn

[R47] sed 单行替换
来源：http://lx.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ew.bookmarksfly.cn

[R48] awk 取指定列
来源：http://ux.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://br.asd995.cn

[R49] awk 带条件
来源：http://il.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://px.colortex.cn

[R50] awk 求和
来源：http://ud.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lo.shtwfgs.cn

[R51] 排序去重取前几
来源：http://do.lnxyls.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://av.huanxung.cn

[R52] 统计行数
来源：http://nt.521024.cn

wc -l a.txt
来源：http://fw.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://xv.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zl.shxzukj.cn

[R54] 比较两个文件
来源：http://vo.hahajie.cn

diff a.txt b.txt
来源：http://pb.hahajie.cn

[R55] 压缩与解压
来源：http://oi.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xc.chemitech.net.cn

[R56] 远程拷贝
来源：http://ww.haigaiapp.cn

scp file user@host:/path/
来源：http://za.bookmarksfly.cn

[R57] 远程执行命令
来源：http://hq.hahajie.cn

ssh user@host 'uptime'
来源：http://yt.asd995.cn

[R58] 下载文件
来源：http://jh.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iw.lnxyls.cn

[R59] 发 POST JSON
来源：http://kf.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cq.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://ib.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iy.hahajie.cn

[R61] 磁盘占用
来源：http://kq.yuexingan06.cn

df -h;  du -sh *
来源：http://ne.newstarts.cn

[R62] 找最占空间的文件
来源：http://vx.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://zy.bookmarksfly.cn

[R63] 内存与进程
来源：http://an.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://hw.shtwfgs.cn

[R64] 结束进程
来源：http://rr.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://my.colortex.cn

[R65] 查看端口占用
来源：http://ja.muxihuayi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kr.colortex.cn

[R66] 定时任务
来源：http://zo.gzmigu.cn

crontab -e;  crontab -l
来源：http://dh.huanxung.cn

[R67] 生成随机十六进制串
来源：http://zd.newstarts.cn

openssl rand -hex 16
来源：http://zp.jctech888.com.cn

[R68] 计算文件校验值
来源：http://jn.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bj.szsharing.cn

[R69] 生成随机密码
来源：http://mj.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://un.asd995.cn

[R70] 时间戳与互转
来源：http://wx.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://wi.yuntaijiaju.cn

[R71] 日期格式化
来源：http://ra.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qq.panjiajie.cn

[R72] 等待端口就绪
来源：http://im.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vc.shxzskj.cn

[R73] 分割大日志
来源：http://ka.9csxet.cn

split -l 1000 big.log part_
来源：http://ez.huixiangedu.cn

[R74] 批量重命名
来源：http://lp.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yn.huanxung.cn

[R75] 导出环境变量
来源：http://ti.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://ll.jctech888.com.cn

[R76] 使用临时文件
来源：http://xs.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ui.nicolike.cn

[R77] 读取用户输入
来源：http://im.jctech888.com.cn

read -rp "请输入: " ans
来源：http://ua.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://cy.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xy.lnxyls.cn

[R79] 解析命令行选项
来源：http://xc.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bv.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://bu.panjiajie.cn

time ./run.sh
来源：http://dt.wgjwhj.cn

================================================================================
来源：http://fh.newstarts.cn

S. C / C++ 专题
来源：http://ee.nicolike.cn

================================================================================
来源：http://hh.panjiajie.cn

[S01] C：Hello World
来源：http://ks.shtwfgs.cn

#include <stdio.h>
来源：http://ig.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://js.nszjky.cn

[S02] C：变量与格式化输出
来源：http://ez.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://ro.haigaiapp.cn

[S03] C：读入整数
来源：http://xn.szsharing.cn

int x; scanf("%d", &x);
来源：http://nz.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://ss.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jf.panjiajie.cn

[S05] C：字符串长度
来源：http://uy.colortex.cn

strlen(s)
来源：http://eq.newstarts.cn

[S06] C：字符串比较
来源：http://tk.nicolike.cn

strcmp(a, b) == 0
来源：http://gb.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://oh.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://or.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://zk.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ic.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://kk.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mi.shxzskj.cn

[S10] C：指针与解引用
来源：http://re.nicolike.cn

int *p = &a;  *p = 5;
来源：http://qp.hahajie.cn

[S11] C：逐行读文件
来源：http://ur.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://fw.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lw.chemitech.net.cn

fclose(f);
来源：http://fx.huixiangedu.cn

[S12] C：写文件
来源：http://kc.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ue.newstarts.cn

[S13] C：宏定义
来源：http://dw.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cb.9csxet.cn

[S14] C：枚举
来源：http://ou.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://bu.521024.cn

[S15] C：类型转换
来源：http://ou.chemitech.net.cn

(double) a / b
来源：http://dk.hahajie.cn

[S16] C：位操作置位
来源：http://il.bookmarksfly.cn

x |= (1 << 3);
来源：http://np.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://kl.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fq.9csxet.cn

[S18] C：命令行参数
来源：http://ry.hahajie.cn

int main(int argc, char **argv)
来源：http://lk.wgjwhj.cn

[S19] C：快速排序
来源：http://ft.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vi.bjjhwx.cn

[S20] C：二分查找
来源：http://eb.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gt.9csxet.cn

[S21] C：字符类别判断
来源：http://lw.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hp.hahajie.cn

[S22] C：字符串转数字
来源：http://tk.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://iz.shxzukj.cn

[S23] C：随机数
来源：http://xb.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nu.shtwfgs.cn

[S24] C：获取本地时间
来源：http://ov.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wu.shtwfgs.cn

[S25] C：内存拷贝
来源：http://vi.szxytkj.cn

memcpy(dst, src, n);
来源：http://qq.nszjky.cn

[S26] C：内存清零
来源：http://zo.nszjky.cn

memset(a, 0, sizeof a);
来源：http://na.jctech888.com.cn

[S27] C：定义常量
来源：http://lw.szxytkj.cn

const double PI = 3.14159;
来源：http://xs.yuntaijiaju.cn

[S28] C：静态变量
来源：http://zw.shtwfgs.cn

static int counter = 0;
来源：http://sj.bookmarksfly.cn

[S29] C：变参函数
来源：http://ty.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dp.bookmarksfly.cn

[S30] C：头文件保护
来源：http://pl.jctech888.com.cn

#ifndef X_H
来源：http://tp.bookmarksfly.cn

#define X_H
来源：http://ww.huanxung.cn

#endif
来源：http://kr.bjjhwx.cn

[S31] C++：Hello World
来源：http://fq.szsharing.cn

#include <iostream>
来源：http://jv.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://ld.szsharing.cn

[S32] C++：字符串
来源：http://gh.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://nx.szsharing.cn

[S33] C++：vector 增删
来源：http://vn.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xc.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://xf.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://ql.shxzukj.cn

[S35] C++：map
来源：http://vd.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://no.nszjky.cn

[S36] C++：unordered_map
来源：http://cd.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wp.szxytkj.cn

[S37] C++：set
来源：http://ek.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kg.chemitech.net.cn

[S38] C++：排序
来源：http://xk.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://by.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://lj.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ad.chemitech.net.cn

[S40] C++：查找元素
来源：http://co.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://so.asd995.cn

[S41] C++：类与构造函数
来源：http://zs.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://be.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://vq.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://cf.haigaiapp.cn

[S43] C++：智能指针
来源：http://vz.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://op.nszjky.cn

[S44] C++：引用传参
来源：http://hy.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://aj.asd995.cn

[S45] C++：lambda
来源：http://se.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pl.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://ct.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wh.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://py.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dc.asd995.cn

[S48] C++：逐行读文件
来源：http://uz.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qm.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://er.wgjwhj.cn

[S49] C++：写文件
来源：http://rq.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lu.9csxet.cn

[S50] C++：格式化数字
来源：http://vd.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kg.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://fa.huixiangedu.cn

static_cast<double>(a) / b
来源：http://mz.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://we.521024.cn

int size() const noexcept { return n_; }
来源：http://bt.shxzskj.cn

[S53] C++：移动语义
来源：http://ey.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://fn.bookmarksfly.cn

[S54] C++：异常处理
来源：http://hd.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eh.nszjky.cn

[S55] C++：结构化绑定
来源：http://cf.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cj.jianghongdianzi.cn

[S56] C++：optional
来源：http://bl.shxzskj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vi.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://bd.jianghongdianzi.cn

constexpr int N = 10;
来源：http://wh.shxzukj.cn

[S58] C++：命名空间
来源：http://aw.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://xw.shxzskj.cn

[S59] C++：静态断言
来源：http://kv.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://we.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://ix.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qw.hnjuh.cn

================================================================================
来源：http://bm.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fn.muxihuayi.cn

================================================================================
来源：http://si.bjjhwx.cn

[T01] Kotlin：Hello World
来源：http://dc.bookmarksfly.cn

println("Hello")
来源：http://mb.521024.cn

[T02] Kotlin：变量
来源：http://gv.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nj.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://jr.yuexingan06.cn

"值: $b"
来源：http://jy.nszjky.cn

[T04] Kotlin：空安全
来源：http://gv.lnxyls.cn

val n: String? = null;  n?.length
来源：http://ng.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://by.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://md.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://tr.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qv.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://pf.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cz.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://nl.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://ku.asd995.cn

[T09] Kotlin：扩展函数
来源：http://cn.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://bv.colortex.cn

[T10] Kotlin：默认参数
来源：http://wa.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gp.shxzukj.cn

[T11] Kotlin：协程
来源：http://me.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lg.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://wx.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://zm.muxihuayi.cn


<!-- 参考信息 -->