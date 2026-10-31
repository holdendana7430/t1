代发 wailian999

case "$1" in
来源：http://uf.shxzskj.cn

start) echo "启动" ;;
来源：http://kr.huixiangedu.cn

stop)  echo "停止" ;;
来源：http://pg.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://zu.wgjwhj.cn

esac
来源：http://mh.jctech888.com.cn

[R12] for 遍历文件
来源：http://ys.szsharing.cn

for f in *.txt; do echo "$f"; done
来源：http://wd.hnjuh.cn

[R13] for 计数循环
来源：http://fk.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://cu.hahajie.cn

[R14] C 风格 for
来源：http://iz.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rv.wgjwhj.cn

[R15] while 逐行读文件
来源：http://sx.bjjhwx.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dp.nszjky.cn

[R16] until 等待条件
来源：http://ss.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ge.hnjuh.cn

[R17] 数组定义与取值
来源：http://mq.hahajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://td.haigaiapp.cn

[R18] 遍历数组
来源：http://rt.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tw.lnxyls.cn

[R19] 数组长度
来源：http://np.9csxet.cn

echo "${#arr[@]}"
来源：http://bh.bookmarksfly.cn

[R20] 关联数组（字典）
来源：http://jg.9csxet.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yb.chemitech.net.cn

[R21] 字符串长度
来源：http://si.521024.cn

echo "${#s}"
来源：http://mn.szsharing.cn

[R22] 截取子串
来源：http://eu.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://jb.hahajie.cn

[R23] 字符串替换
来源：http://fh.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ww.bjjhwx.cn

[R24] 大小写转换
来源：http://ec.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bz.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://kn.wgjwhj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fw.shxzukj.cn

[R26] 命令替换
来源：http://og.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://sy.shxzukj.cn

[R27] 算术展开
来源：http://nc.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://cg.shxzukj.cn

[R28] 浮点运算
来源：http://pe.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://ty.asd995.cn

[R29] 定义函数
来源：http://qf.haigaiapp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zn.haigaiapp.cn

[R30] 函数返回状态码
来源：http://nh.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://bt.hnjuh.cn

[R31] 局部变量
来源：http://uu.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://nf.gzmigu.cn

[R32] 参数个数校验
来源：http://lg.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dd.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://jw.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zu.nicolike.cn

[R34] 退出时清理
来源：http://he.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ib.panjiajie.cn

[R35] 后台执行并等待
来源：http://rv.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mf.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://bs.nszjky.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wr.szsharing.cn

[R37] 把输出赋给变量
来源：http://rm.bookmarksfly.cn

files=$(ls -1)
来源：http://jz.haigaiapp.cn

[R38] 管道串联
来源：http://pl.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://cf.panjiajie.cn

[R39] 重定向标准输出与错误
来源：http://ky.521024.cn

cmd > out.log 2>&1
来源：http://wx.szxytkj.cn

[R40] 追加写日志
来源：http://sz.jianghongdianzi.cn

echo "log" >> out.log
来源：http://ly.shxzukj.cn

[R41] 丢弃输出
来源：http://yb.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://ba.hnjuh.cn

[R42] 输入重定向
来源：http://dr.521024.cn

wc -l < a.txt
来源：http://wn.nicolike.cn

[R43] 按名字查找文件
来源：http://vb.wgjwhj.cn

find . -name "*.log" -type f
来源：http://tr.gzmigu.cn

[R44] 按修改时间查找
来源：http://jl.nicolike.cn

find . -mtime -7 -type f
来源：http://mm.jctech888.com.cn

[R45] 批量删除
来源：http://hg.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://xh.shxzskj.cn

[R46] 递归替换文件内容
来源：http://oz.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cq.colortex.cn

[R47] sed 单行替换
来源：http://ie.nszjky.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pn.bjjhwx.cn

[R48] awk 取指定列
来源：http://ok.gzmigu.cn

awk '{print $1, $3}' a.txt
来源：http://hd.huixinmuqiang.cn

[R49] awk 带条件
来源：http://yp.huixiangedu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ck.bookmarksfly.cn

[R50] awk 求和
来源：http://rj.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hg.nicolike.cn

[R51] 排序去重取前几
来源：http://fh.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ze.gzmigu.cn

[R52] 统计行数
来源：http://cv.colortex.cn

wc -l a.txt
来源：http://zs.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://nv.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xf.hnjuh.cn

[R54] 比较两个文件
来源：http://ju.szsharing.cn

diff a.txt b.txt
来源：http://xm.newstarts.cn

[R55] 压缩与解压
来源：http://ww.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gc.haigaiapp.cn

[R56] 远程拷贝
来源：http://ip.bookmarksfly.cn

scp file user@host:/path/
来源：http://hi.szsharing.cn

[R57] 远程执行命令
来源：http://ty.chemitech.net.cn

ssh user@host 'uptime'
来源：http://kn.jctech888.com.cn

[R58] 下载文件
来源：http://st.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://us.shtwfgs.cn

[R59] 发 POST JSON
来源：http://sr.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qj.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://zc.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://an.haigaiapp.cn

[R61] 磁盘占用
来源：http://ci.jctech888.com.cn

df -h;  du -sh *
来源：http://xa.nicolike.cn

[R62] 找最占空间的文件
来源：http://ec.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://zn.lnxyls.cn

[R63] 内存与进程
来源：http://bp.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://bl.bookmarksfly.cn

[R64] 结束进程
来源：http://zi.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://ye.huanxung.cn

[R65] 查看端口占用
来源：http://qb.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tl.jianghongdianzi.cn

[R66] 定时任务
来源：http://ml.panjiajie.cn

crontab -e;  crontab -l
来源：http://zx.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://jd.521024.cn

openssl rand -hex 16
来源：http://ml.szsharing.cn

[R68] 计算文件校验值
来源：http://hs.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://iz.haigaiapp.cn

[R69] 生成随机密码
来源：http://hs.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://jt.9csxet.cn

[R70] 时间戳与互转
来源：http://ut.colortex.cn

date +%s;  date -d @1700000000
来源：http://qh.521024.cn

[R71] 日期格式化
来源：http://ph.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rq.shxzukj.cn

[R72] 等待端口就绪
来源：http://hx.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vb.shxzukj.cn

[R73] 分割大日志
来源：http://zw.szsharing.cn

split -l 1000 big.log part_
来源：http://dr.muxihuayi.cn

[R74] 批量重命名
来源：http://rv.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uq.szxytkj.cn

[R75] 导出环境变量
来源：http://xs.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://aq.panjiajie.cn

[R76] 使用临时文件
来源：http://sj.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xm.bookmarksfly.cn

[R77] 读取用户输入
来源：http://kw.jctech888.com.cn

read -rp "请输入: " ans
来源：http://pw.bookmarksfly.cn

[R78] 交互式菜单
来源：http://qe.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wv.bjjhwx.cn

[R79] 解析命令行选项
来源：http://gg.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jp.shxzukj.cn

[R80] 查看脚本执行耗时
来源：http://dd.jianghongdianzi.cn

time ./run.sh
来源：http://fp.szxytkj.cn

================================================================================
来源：http://ar.huixinmuqiang.cn

S. C / C++ 专题
来源：http://uk.shxzskj.cn

================================================================================
来源：http://ar.bookmarksfly.cn

[S01] C：Hello World
来源：http://hj.9csxet.cn

#include <stdio.h>
来源：http://xh.newstarts.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dd.szsharing.cn

[S02] C：变量与格式化输出
来源：http://jq.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://kt.shxzukj.cn

[S03] C：读入整数
来源：http://if.9csxet.cn

int x; scanf("%d", &x);
来源：http://to.muxihuayi.cn

[S04] C：字符串复制
来源：http://os.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cb.hnjuh.cn

[S05] C：字符串长度
来源：http://qr.hnjuh.cn

strlen(s)
来源：http://ml.shxzukj.cn

[S06] C：字符串比较
来源：http://pe.jctech888.com.cn

strcmp(a, b) == 0
来源：http://yw.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://jg.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://di.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://vr.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ks.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://hm.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vf.panjiajie.cn

[S10] C：指针与解引用
来源：http://zx.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://rr.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://fc.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://sx.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lg.yuexingan06.cn

fclose(f);
来源：http://nm.yuexingan06.cn

[S12] C：写文件
来源：http://cg.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dx.huixinmuqiang.cn

[S13] C：宏定义
来源：http://ja.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zb.bjjhwx.cn

[S14] C：枚举
来源：http://ec.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://yu.huixinmuqiang.cn

[S15] C：类型转换
来源：http://wk.nszjky.cn

(double) a / b
来源：http://gr.szxytkj.cn

[S16] C：位操作置位
来源：http://wo.muxihuayi.cn

x |= (1 << 3);
来源：http://xn.szsharing.cn

[S17] C：安全拼接字符串
来源：http://kg.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fm.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://ea.shxzskj.cn

int main(int argc, char **argv)
来源：http://rt.shtwfgs.cn

[S19] C：快速排序
来源：http://qy.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ru.szsharing.cn

[S20] C：二分查找
来源：http://cx.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xv.muxihuayi.cn

[S21] C：字符类别判断
来源：http://qz.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ci.huanxung.cn

[S22] C：字符串转数字
来源：http://ul.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xs.asd995.cn

[S23] C：随机数
来源：http://yg.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wc.lnxyls.cn

[S24] C：获取本地时间
来源：http://ze.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bz.haigaiapp.cn

[S25] C：内存拷贝
来源：http://hv.jctech888.com.cn

memcpy(dst, src, n);
来源：http://qq.yuntaijiaju.cn

[S26] C：内存清零
来源：http://db.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://tw.gzmigu.cn

[S27] C：定义常量
来源：http://xg.shxzukj.cn

const double PI = 3.14159;
来源：http://ur.shxzskj.cn

[S28] C：静态变量
来源：http://qa.bjjhwx.cn

static int counter = 0;
来源：http://az.521024.cn

[S29] C：变参函数
来源：http://ui.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oq.szxytkj.cn

[S30] C：头文件保护
来源：http://nc.szxytkj.cn

#ifndef X_H
来源：http://xi.huanxung.cn

#define X_H
来源：http://ye.huixinmuqiang.cn

#endif
来源：http://ci.hahajie.cn

[S31] C++：Hello World
来源：http://lu.shxzskj.cn

#include <iostream>
来源：http://nx.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ym.newstarts.cn

[S32] C++：字符串
来源：http://oq.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://vl.asd995.cn

[S33] C++：vector 增删
来源：http://qz.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cf.huanxung.cn

[S34] C++：遍历 vector
来源：http://ux.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://qi.yuntaijiaju.cn

[S35] C++：map
来源：http://lh.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vb.jctech888.com.cn

[S36] C++：unordered_map
来源：http://pp.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ov.jianghongdianzi.cn

[S37] C++：set
来源：http://hr.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ps.shxzukj.cn

[S38] C++：排序
来源：http://xl.asd995.cn

std::sort(v.begin(), v.end());
来源：http://np.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://di.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aj.9csxet.cn

[S40] C++：查找元素
来源：http://li.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eq.gzmigu.cn

[S41] C++：类与构造函数
来源：http://lu.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://og.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://ag.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://rj.yuexingan06.cn

[S43] C++：智能指针
来源：http://vv.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://jf.hnjuh.cn

[S44] C++：引用传参
来源：http://uw.lnxyls.cn

void inc(int &x) { ++x; }
来源：http://bo.hahajie.cn

[S45] C++：lambda
来源：http://tk.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pu.asd995.cn

[S46] C++：函数模板
来源：http://dx.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qn.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://ux.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kc.asd995.cn

[S48] C++：逐行读文件
来源：http://eh.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wg.szsharing.cn

while (std::getline(in, line)) { }
来源：http://yp.panjiajie.cn

[S49] C++：写文件
来源：http://zt.huixinmuqiang.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ib.hnjuh.cn

[S50] C++：格式化数字
来源：http://yg.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ia.chemitech.net.cn

[S51] C++：显式类型转换
来源：http://uu.bjjhwx.cn

static_cast<double>(a) / b
来源：http://yb.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://oa.nszjky.cn

int size() const noexcept { return n_; }
来源：http://ls.hahajie.cn

[S53] C++：移动语义
来源：http://mu.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://rj.9csxet.cn

[S54] C++：异常处理
来源：http://au.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vi.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://ra.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fw.huixiangedu.cn

[S56] C++：optional
来源：http://mq.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kw.chemitech.net.cn

[S57] C++：编译期常量
来源：http://qr.yuntaijiaju.cn

constexpr int N = 10;
来源：http://ym.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://tf.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://ea.shtwfgs.cn

[S59] C++：静态断言
来源：http://oz.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ao.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://cv.huixinmuqiang.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wh.newstarts.cn

================================================================================
来源：http://vf.jctech888.com.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yn.muxihuayi.cn

================================================================================
来源：http://xm.huanxung.cn

[T01] Kotlin：Hello World
来源：http://lv.9csxet.cn

println("Hello")
来源：http://io.haigaiapp.cn

[T02] Kotlin：变量
来源：http://nn.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yf.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://vt.9csxet.cn

"值: $b"
来源：http://ss.nszjky.cn

[T04] Kotlin：空安全
来源：http://yr.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://ob.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://bm.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mi.hahajie.cn

[T06] Kotlin：集合映射
来源：http://sm.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vd.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://yn.jianghongdianzi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://og.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://ft.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://dh.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://fs.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://sw.nicolike.cn

[T10] Kotlin：默认参数
来源：http://xg.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vm.hahajie.cn

[T11] Kotlin：协程
来源：http://qf.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ah.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://de.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://jb.hnjuh.cn


<!-- 参考信息 -->