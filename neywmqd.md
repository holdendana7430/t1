代发 wailian999

esac
来源：http://vx.shxzskj.cn

[R12] for 遍历文件
来源：http://eq.haigaiapp.cn

for f in *.txt; do echo "$f"; done
来源：http://kg.newstarts.cn

[R13] for 计数循环
来源：http://ue.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://sq.asd995.cn

[R14] C 风格 for
来源：http://lm.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lo.huanxung.cn

[R15] while 逐行读文件
来源：http://fj.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ms.yuexingan06.cn

[R16] until 等待条件
来源：http://ng.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wz.wgjwhj.cn

[R17] 数组定义与取值
来源：http://nh.jianghongdianzi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kg.521024.cn

[R18] 遍历数组
来源：http://fz.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fz.9csxet.cn

[R19] 数组长度
来源：http://kv.colortex.cn

echo "${#arr[@]}"
来源：http://mm.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://zk.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wo.nszjky.cn

[R21] 字符串长度
来源：http://in.huixinmuqiang.cn

echo "${#s}"
来源：http://vi.newstarts.cn

[R22] 截取子串
来源：http://ic.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://dl.huixinmuqiang.cn

[R23] 字符串替换
来源：http://jy.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lk.jianghongdianzi.cn

[R24] 大小写转换
来源：http://ay.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://se.panjiajie.cn

[R25] 去后缀 / 去前缀
来源：http://ij.wgjwhj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ii.hnjuh.cn

[R26] 命令替换
来源：http://un.yuexingan06.cn

now=$(date +%F); echo "$now"
来源：http://vd.nszjky.cn

[R27] 算术展开
来源：http://pu.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://rq.panjiajie.cn

[R28] 浮点运算
来源：http://ve.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://ks.wgjwhj.cn

[R29] 定义函数
来源：http://jw.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rf.chemitech.net.cn

[R30] 函数返回状态码
来源：http://lw.wgjwhj.cn

f() { return 0; }; f || echo "失败了"
来源：http://df.jianghongdianzi.cn

[R31] 局部变量
来源：http://nh.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://vg.muxihuayi.cn

[R32] 参数个数校验
来源：http://ab.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pv.asd995.cn

[R33] 捕获错误并提示行号
来源：http://wa.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yh.huanxung.cn

[R34] 退出时清理
来源：http://gs.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cf.bjjhwx.cn

[R35] 后台执行并等待
来源：http://fh.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ij.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://ao.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nt.panjiajie.cn

[R37] 把输出赋给变量
来源：http://oh.haigaiapp.cn

files=$(ls -1)
来源：http://fb.521024.cn

[R38] 管道串联
来源：http://qa.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://hz.haigaiapp.cn

[R39] 重定向标准输出与错误
来源：http://qu.huanxung.cn

cmd > out.log 2>&1
来源：http://vj.haigaiapp.cn

[R40] 追加写日志
来源：http://vm.bookmarksfly.cn

echo "log" >> out.log
来源：http://xu.newstarts.cn

[R41] 丢弃输出
来源：http://sr.asd995.cn

cmd >/dev/null 2>&1
来源：http://xd.huanxung.cn

[R42] 输入重定向
来源：http://yn.nszjky.cn

wc -l < a.txt
来源：http://nm.wgjwhj.cn

[R43] 按名字查找文件
来源：http://uf.yuexingan06.cn

find . -name "*.log" -type f
来源：http://ah.hnjuh.cn

[R44] 按修改时间查找
来源：http://ko.shtwfgs.cn

find . -mtime -7 -type f
来源：http://np.nszjky.cn

[R45] 批量删除
来源：http://yu.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://xq.huanxung.cn

[R46] 递归替换文件内容
来源：http://ln.nszjky.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kn.colortex.cn

[R47] sed 单行替换
来源：http://kh.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cr.nszjky.cn

[R48] awk 取指定列
来源：http://no.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://ka.nszjky.cn

[R49] awk 带条件
来源：http://vy.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yl.bjjhwx.cn

[R50] awk 求和
来源：http://yk.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ny.wgjwhj.cn

[R51] 排序去重取前几
来源：http://et.haigaiapp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wn.colortex.cn

[R52] 统计行数
来源：http://xp.bookmarksfly.cn

wc -l a.txt
来源：http://lx.asd995.cn

[R53] 查看文件头与实时尾
来源：http://sj.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wy.yuexingan06.cn

[R54] 比较两个文件
来源：http://cy.asd995.cn

diff a.txt b.txt
来源：http://ms.521024.cn

[R55] 压缩与解压
来源：http://wu.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bk.gzmigu.cn

[R56] 远程拷贝
来源：http://zx.wgjwhj.cn

scp file user@host:/path/
来源：http://fg.bjjhwx.cn

[R57] 远程执行命令
来源：http://my.hnjuh.cn

ssh user@host 'uptime'
来源：http://nk.shxzukj.cn

[R58] 下载文件
来源：http://dm.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qt.wgjwhj.cn

[R59] 发 POST JSON
来源：http://by.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xc.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://kk.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bu.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://rj.nszjky.cn

df -h;  du -sh *
来源：http://dw.521024.cn

[R62] 找最占空间的文件
来源：http://oy.bjjhwx.cn

du -ah . | sort -rh | head -10
来源：http://xz.haigaiapp.cn

[R63] 内存与进程
来源：http://fo.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://fq.hahajie.cn

[R64] 结束进程
来源：http://fs.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://zh.szxytkj.cn

[R65] 查看端口占用
来源：http://mh.colortex.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ju.panjiajie.cn

[R66] 定时任务
来源：http://rw.shxzskj.cn

crontab -e;  crontab -l
来源：http://eg.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://ww.shxzskj.cn

openssl rand -hex 16
来源：http://df.gzmigu.cn

[R68] 计算文件校验值
来源：http://rs.521024.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uu.nicolike.cn

[R69] 生成随机密码
来源：http://xs.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://qe.chemitech.net.cn

[R70] 时间戳与互转
来源：http://re.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://qx.521024.cn

[R71] 日期格式化
来源：http://fj.jianghongdianzi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dz.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://wr.newstarts.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ia.jianghongdianzi.cn

[R73] 分割大日志
来源：http://jw.asd995.cn

split -l 1000 big.log part_
来源：http://xp.gzmigu.cn

[R74] 批量重命名
来源：http://ug.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xs.gzmigu.cn

[R75] 导出环境变量
来源：http://jh.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://bh.colortex.cn

[R76] 使用临时文件
来源：http://tx.szxytkj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vl.hahajie.cn

[R77] 读取用户输入
来源：http://un.szxytkj.cn

read -rp "请输入: " ans
来源：http://yg.shxzskj.cn

[R78] 交互式菜单
来源：http://kx.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lv.colortex.cn

[R79] 解析命令行选项
来源：http://wl.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bu.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://tk.haigaiapp.cn

time ./run.sh
来源：http://ll.521024.cn

================================================================================
来源：http://es.yuntaijiaju.cn

S. C / C++ 专题
来源：http://lv.hahajie.cn

================================================================================
来源：http://wt.asd995.cn

[S01] C：Hello World
来源：http://vy.colortex.cn

#include <stdio.h>
来源：http://hg.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hi.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://ly.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://vc.nszjky.cn

[S03] C：读入整数
来源：http://kf.panjiajie.cn

int x; scanf("%d", &x);
来源：http://jf.haigaiapp.cn

[S04] C：字符串复制
来源：http://di.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zx.newstarts.cn

[S05] C：字符串长度
来源：http://ed.bookmarksfly.cn

strlen(s)
来源：http://lw.haigaiapp.cn

[S06] C：字符串比较
来源：http://ca.haigaiapp.cn

strcmp(a, b) == 0
来源：http://bj.9csxet.cn

[S07] C：数组遍历求和
来源：http://th.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qi.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://dw.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qi.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://fj.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qh.szsharing.cn

[S10] C：指针与解引用
来源：http://lf.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://gj.nicolike.cn

[S11] C：逐行读文件
来源：http://vg.muxihuayi.cn

FILE *f = fopen("a.txt", "r");
来源：http://rm.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://az.lnxyls.cn

fclose(f);
来源：http://ck.szsharing.cn

[S12] C：写文件
来源：http://cn.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fj.521024.cn

[S13] C：宏定义
来源：http://dk.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cp.huixiangedu.cn

[S14] C：枚举
来源：http://wc.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://zt.bookmarksfly.cn

[S15] C：类型转换
来源：http://up.shxzukj.cn

(double) a / b
来源：http://ej.muxihuayi.cn

[S16] C：位操作置位
来源：http://an.9csxet.cn

x |= (1 << 3);
来源：http://hc.asd995.cn

[S17] C：安全拼接字符串
来源：http://qp.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sh.muxihuayi.cn

[S18] C：命令行参数
来源：http://xw.szxytkj.cn

int main(int argc, char **argv)
来源：http://rn.gzmigu.cn

[S19] C：快速排序
来源：http://ia.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jr.lnxyls.cn

[S20] C：二分查找
来源：http://td.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mj.szxytkj.cn

[S21] C：字符类别判断
来源：http://ci.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xo.shxzskj.cn

[S22] C：字符串转数字
来源：http://kv.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nb.szxytkj.cn

[S23] C：随机数
来源：http://ev.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ms.shtwfgs.cn

[S24] C：获取本地时间
来源：http://gu.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pc.chemitech.net.cn

[S25] C：内存拷贝
来源：http://jj.shxzskj.cn

memcpy(dst, src, n);
来源：http://fo.szxytkj.cn

[S26] C：内存清零
来源：http://lf.szsharing.cn

memset(a, 0, sizeof a);
来源：http://uf.asd995.cn

[S27] C：定义常量
来源：http://lt.hnjuh.cn

const double PI = 3.14159;
来源：http://jz.huanxung.cn

[S28] C：静态变量
来源：http://qb.jctech888.com.cn

static int counter = 0;
来源：http://yt.huixiangedu.cn

[S29] C：变参函数
来源：http://zk.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ge.lnxyls.cn

[S30] C：头文件保护
来源：http://rb.yuntaijiaju.cn

#ifndef X_H
来源：http://yi.9csxet.cn

#define X_H
来源：http://iy.shxzskj.cn

#endif
来源：http://zd.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://lb.hnjuh.cn

#include <iostream>
来源：http://ck.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://qr.haigaiapp.cn

[S32] C++：字符串
来源：http://ig.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://qv.shtwfgs.cn

[S33] C++：vector 增删
来源：http://ky.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nz.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://hd.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://zm.jctech888.com.cn

[S35] C++：map
来源：http://sr.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wq.nicolike.cn

[S36] C++：unordered_map
来源：http://yv.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qi.chemitech.net.cn

[S37] C++：set
来源：http://qv.521024.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lo.colortex.cn

[S38] C++：排序
来源：http://xr.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://bv.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://bp.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://if.colortex.cn

[S40] C++：查找元素
来源：http://vw.521024.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://le.gzmigu.cn

[S41] C++：类与构造函数
来源：http://jg.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qo.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://ao.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://rt.panjiajie.cn

[S43] C++：智能指针
来源：http://cv.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://hj.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://ku.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://ev.shtwfgs.cn

[S45] C++：lambda
来源：http://uo.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vp.muxihuayi.cn

[S46] C++：函数模板
来源：http://ti.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ow.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://cx.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bc.9csxet.cn

[S48] C++：逐行读文件
来源：http://fl.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ub.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://oo.521024.cn

[S49] C++：写文件
来源：http://nc.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ow.huanxung.cn

[S50] C++：格式化数字
来源：http://vw.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cp.newstarts.cn

[S51] C++：显式类型转换
来源：http://nf.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://hc.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://ax.huanxung.cn

int size() const noexcept { return n_; }
来源：http://cf.lnxyls.cn

[S53] C++：移动语义
来源：http://vs.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://ug.szsharing.cn

[S54] C++：异常处理
来源：http://os.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dk.huixiangedu.cn

[S55] C++：结构化绑定
来源：http://nk.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xf.521024.cn

[S56] C++：optional
来源：http://dm.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ju.muxihuayi.cn

[S57] C++：编译期常量
来源：http://pu.jctech888.com.cn

constexpr int N = 10;
来源：http://wh.colortex.cn

[S58] C++：命名空间
来源：http://ct.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://zn.panjiajie.cn

[S59] C++：静态断言
来源：http://we.nszjky.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oc.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://gw.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xr.huixinmuqiang.cn

================================================================================
来源：http://es.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ih.gzmigu.cn

================================================================================
来源：http://wg.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://vg.chemitech.net.cn

println("Hello")
来源：http://jt.szsharing.cn

[T02] Kotlin：变量
来源：http://nf.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mx.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://jz.yuexingan06.cn

"值: $b"
来源：http://xi.huanxung.cn

[T04] Kotlin：空安全
来源：http://gn.shxzukj.cn

val n: String? = null;  n?.length
来源：http://vc.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://jk.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dj.nszjky.cn

[T06] Kotlin：集合映射
来源：http://zd.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ah.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://yj.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gt.asd995.cn

[T08] Kotlin：数据类
来源：http://rw.hahajie.cn

data class User(val name: String, val age: Int)
来源：http://ob.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://si.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://nm.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://vr.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://em.shxzukj.cn

[T11] Kotlin：协程
来源：http://pz.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qq.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://jt.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://kj.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://vk.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://kk.lnxyls.cn

[T14] Kotlin：循环
来源：http://zk.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://xd.newstarts.cn


<!-- 参考信息 -->