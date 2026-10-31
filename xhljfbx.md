代发 wailian999

case "$1" in
来源：http://tc.asd995.cn

start) echo "启动" ;;
来源：http://xf.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://ib.szsharing.cn

*)     echo "未知命令" ;;
来源：http://zh.yuntaijiaju.cn

esac
来源：http://zb.panjiajie.cn

[R12] for 遍历文件
来源：http://bb.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://tb.nszjky.cn

[R13] for 计数循环
来源：http://nu.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://ms.huixiangedu.cn

[R14] C 风格 for
来源：http://ou.huixiangedu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bc.szsharing.cn

[R15] while 逐行读文件
来源：http://nx.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yg.yuexingan06.cn

[R16] until 等待条件
来源：http://gm.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mt.shtwfgs.cn

[R17] 数组定义与取值
来源：http://fw.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sh.bookmarksfly.cn

[R18] 遍历数组
来源：http://jt.bookmarksfly.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pz.bjjhwx.cn

[R19] 数组长度
来源：http://bf.lnxyls.cn

echo "${#arr[@]}"
来源：http://wr.asd995.cn

[R20] 关联数组（字典）
来源：http://rt.panjiajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mj.panjiajie.cn

[R21] 字符串长度
来源：http://fb.chemitech.net.cn

echo "${#s}"
来源：http://ul.asd995.cn

[R22] 截取子串
来源：http://kh.shtwfgs.cn

echo "${s:0:5}"
来源：http://pc.hnjuh.cn

[R23] 字符串替换
来源：http://rk.yuexingan06.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pd.newstarts.cn

[R24] 大小写转换
来源：http://uj.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://je.bjjhwx.cn

[R25] 去后缀 / 去前缀
来源：http://nl.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lu.wgjwhj.cn

[R26] 命令替换
来源：http://kn.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://bp.jctech888.com.cn

[R27] 算术展开
来源：http://wp.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://gb.bookmarksfly.cn

[R28] 浮点运算
来源：http://da.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://vm.jianghongdianzi.cn

[R29] 定义函数
来源：http://vi.yuntaijiaju.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uk.521024.cn

[R30] 函数返回状态码
来源：http://gc.wgjwhj.cn

f() { return 0; }; f || echo "失败了"
来源：http://ab.huixinmuqiang.cn

[R31] 局部变量
来源：http://lb.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://ln.lnxyls.cn

[R32] 参数个数校验
来源：http://kx.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cn.muxihuayi.cn

[R33] 捕获错误并提示行号
来源：http://xy.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ey.huixiangedu.cn

[R34] 退出时清理
来源：http://df.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bx.panjiajie.cn

[R35] 后台执行并等待
来源：http://vm.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tm.shxzskj.cn

[R36] 并发执行多个任务
来源：http://du.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cn.hahajie.cn

[R37] 把输出赋给变量
来源：http://yx.shxzskj.cn

files=$(ls -1)
来源：http://ki.9csxet.cn

[R38] 管道串联
来源：http://fb.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://qi.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://iv.colortex.cn

cmd > out.log 2>&1
来源：http://yo.haigaiapp.cn

[R40] 追加写日志
来源：http://tq.jianghongdianzi.cn

echo "log" >> out.log
来源：http://ie.bjjhwx.cn

[R41] 丢弃输出
来源：http://gn.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://xa.shtwfgs.cn

[R42] 输入重定向
来源：http://vy.shxzukj.cn

wc -l < a.txt
来源：http://wx.haigaiapp.cn

[R43] 按名字查找文件
来源：http://pv.shxzukj.cn

find . -name "*.log" -type f
来源：http://me.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://xd.huanxung.cn

find . -mtime -7 -type f
来源：http://xi.lnxyls.cn

[R45] 批量删除
来源：http://ck.nicolike.cn

find . -name "*.tmp" -delete
来源：http://ff.nicolike.cn

[R46] 递归替换文件内容
来源：http://gu.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tf.shtwfgs.cn

[R47] sed 单行替换
来源：http://ht.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ku.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://na.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://dm.hnjuh.cn

[R49] awk 带条件
来源：http://fe.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dq.nszjky.cn

[R50] awk 求和
来源：http://ce.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jb.panjiajie.cn

[R51] 排序去重取前几
来源：http://sw.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lq.panjiajie.cn

[R52] 统计行数
来源：http://rn.szsharing.cn

wc -l a.txt
来源：http://jd.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://jm.colortex.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yk.szsharing.cn

[R54] 比较两个文件
来源：http://ob.chemitech.net.cn

diff a.txt b.txt
来源：http://jz.wgjwhj.cn

[R55] 压缩与解压
来源：http://sx.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nz.nszjky.cn

[R56] 远程拷贝
来源：http://sq.hahajie.cn

scp file user@host:/path/
来源：http://xl.haigaiapp.cn

[R57] 远程执行命令
来源：http://pg.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://sn.szxytkj.cn

[R58] 下载文件
来源：http://qk.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ay.wgjwhj.cn

[R59] 发 POST JSON
来源：http://js.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tg.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://sz.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ex.9csxet.cn

[R61] 磁盘占用
来源：http://hh.bjjhwx.cn

df -h;  du -sh *
来源：http://dt.gzmigu.cn

[R62] 找最占空间的文件
来源：http://jl.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://qq.9csxet.cn

[R63] 内存与进程
来源：http://tq.521024.cn

free -h;  ps aux | grep nginx
来源：http://my.panjiajie.cn

[R64] 结束进程
来源：http://sa.muxihuayi.cn

kill -9 $(pgrep -f app.py)
来源：http://lw.shxzskj.cn

[R65] 查看端口占用
来源：http://ij.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nq.huanxung.cn

[R66] 定时任务
来源：http://yo.nszjky.cn

crontab -e;  crontab -l
来源：http://vy.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://cv.bookmarksfly.cn

openssl rand -hex 16
来源：http://uk.gzmigu.cn

[R68] 计算文件校验值
来源：http://za.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uv.colortex.cn

[R69] 生成随机密码
来源：http://hp.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://te.shtwfgs.cn

[R70] 时间戳与互转
来源：http://yq.huanxung.cn

date +%s;  date -d @1700000000
来源：http://ux.huixinmuqiang.cn

[R71] 日期格式化
来源：http://tk.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pl.szxytkj.cn

[R72] 等待端口就绪
来源：http://hu.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zl.shxzukj.cn

[R73] 分割大日志
来源：http://qe.shxzukj.cn

split -l 1000 big.log part_
来源：http://sz.yuexingan06.cn

[R74] 批量重命名
来源：http://lg.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jc.panjiajie.cn

[R75] 导出环境变量
来源：http://si.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://ni.muxihuayi.cn

[R76] 使用临时文件
来源：http://ty.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pg.nicolike.cn

[R77] 读取用户输入
来源：http://lh.gzmigu.cn

read -rp "请输入: " ans
来源：http://bh.lnxyls.cn

[R78] 交互式菜单
来源：http://pe.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ge.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://zq.521024.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nw.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://pu.shxzskj.cn

time ./run.sh
来源：http://lg.huixinmuqiang.cn

================================================================================
来源：http://nr.muxihuayi.cn

S. C / C++ 专题
来源：http://un.bjjhwx.cn

================================================================================
来源：http://kj.bjjhwx.cn

[S01] C：Hello World
来源：http://wq.shxzukj.cn

#include <stdio.h>
来源：http://lt.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tm.colortex.cn

[S02] C：变量与格式化输出
来源：http://rr.chemitech.net.cn

int a = 10; printf("%d\n", a);
来源：http://od.hahajie.cn

[S03] C：读入整数
来源：http://ge.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://cu.gzmigu.cn

[S04] C：字符串复制
来源：http://bf.huixinmuqiang.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ja.newstarts.cn

[S05] C：字符串长度
来源：http://ti.hahajie.cn

strlen(s)
来源：http://ro.lnxyls.cn

[S06] C：字符串比较
来源：http://ed.huixiangedu.cn

strcmp(a, b) == 0
来源：http://jj.521024.cn

[S07] C：数组遍历求和
来源：http://je.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ao.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://ow.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kq.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://xt.lnxyls.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jx.hnjuh.cn

[S10] C：指针与解引用
来源：http://oi.colortex.cn

int *p = &a;  *p = 5;
来源：http://gm.hahajie.cn

[S11] C：逐行读文件
来源：http://rv.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://xa.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ey.szxytkj.cn

fclose(f);
来源：http://ux.bookmarksfly.cn

[S12] C：写文件
来源：http://rt.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jr.panjiajie.cn

[S13] C：宏定义
来源：http://yj.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ws.bjjhwx.cn

[S14] C：枚举
来源：http://zh.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://ld.wgjwhj.cn

[S15] C：类型转换
来源：http://ey.lnxyls.cn

(double) a / b
来源：http://wt.chemitech.net.cn

[S16] C：位操作置位
来源：http://zh.chemitech.net.cn

x |= (1 << 3);
来源：http://sl.huanxung.cn

[S17] C：安全拼接字符串
来源：http://sl.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hm.shxzukj.cn

[S18] C：命令行参数
来源：http://tf.9csxet.cn

int main(int argc, char **argv)
来源：http://db.yuexingan06.cn

[S19] C：快速排序
来源：http://yz.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bv.asd995.cn

[S20] C：二分查找
来源：http://ha.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qf.nszjky.cn

[S21] C：字符类别判断
来源：http://db.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fh.521024.cn

[S22] C：字符串转数字
来源：http://uq.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vv.shtwfgs.cn

[S23] C：随机数
来源：http://rc.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://iy.panjiajie.cn

[S24] C：获取本地时间
来源：http://cm.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xk.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://oq.haigaiapp.cn

memcpy(dst, src, n);
来源：http://iw.bjjhwx.cn

[S26] C：内存清零
来源：http://xq.9csxet.cn

memset(a, 0, sizeof a);
来源：http://xm.wgjwhj.cn

[S27] C：定义常量
来源：http://lr.newstarts.cn

const double PI = 3.14159;
来源：http://lp.shtwfgs.cn

[S28] C：静态变量
来源：http://jw.shxzukj.cn

static int counter = 0;
来源：http://je.shtwfgs.cn

[S29] C：变参函数
来源：http://gk.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ec.bjjhwx.cn

[S30] C：头文件保护
来源：http://lz.haigaiapp.cn

#ifndef X_H
来源：http://at.szxytkj.cn

#define X_H
来源：http://ag.bookmarksfly.cn

#endif
来源：http://sx.nicolike.cn

[S31] C++：Hello World
来源：http://cc.yuntaijiaju.cn

#include <iostream>
来源：http://wi.huixiangedu.cn

int main() { std::cout << "Hello\n"; }
来源：http://jy.panjiajie.cn

[S32] C++：字符串
来源：http://gf.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://is.asd995.cn

[S33] C++：vector 增删
来源：http://wh.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://is.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://fs.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://yp.lnxyls.cn

[S35] C++：map
来源：http://kz.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lc.521024.cn

[S36] C++：unordered_map
来源：http://rk.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ca.yuntaijiaju.cn

[S37] C++：set
来源：http://ut.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qv.521024.cn

[S38] C++：排序
来源：http://ea.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://on.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://is.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wa.szsharing.cn

[S40] C++：查找元素
来源：http://nc.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qo.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://rm.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nf.hahajie.cn

[S42] C++：继承与虚函数
来源：http://ur.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://zh.gzmigu.cn

[S43] C++：智能指针
来源：http://bo.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://hk.hahajie.cn

[S44] C++：引用传参
来源：http://li.shtwfgs.cn

void inc(int &x) { ++x; }
来源：http://cn.nszjky.cn

[S45] C++：lambda
来源：http://lk.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://al.shxzukj.cn

[S46] C++：函数模板
来源：http://ud.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ww.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://rr.9csxet.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eu.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://re.shxzukj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ow.nicolike.cn

while (std::getline(in, line)) { }
来源：http://xl.yuexingan06.cn

[S49] C++：写文件
来源：http://vl.colortex.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eu.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://hu.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dr.nicolike.cn

[S51] C++：显式类型转换
来源：http://dd.huanxung.cn

static_cast<double>(a) / b
来源：http://sn.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://bx.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://wq.nszjky.cn

[S53] C++：移动语义
来源：http://nj.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://dh.szsharing.cn

[S54] C++：异常处理
来源：http://nn.muxihuayi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://di.521024.cn

[S55] C++：结构化绑定
来源：http://wc.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ay.huixinmuqiang.cn

[S56] C++：optional
来源：http://lm.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vk.chemitech.net.cn

[S57] C++：编译期常量
来源：http://lq.chemitech.net.cn

constexpr int N = 10;
来源：http://ex.szxytkj.cn

[S58] C++：命名空间
来源：http://oe.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://ci.bjjhwx.cn

[S59] C++：静态断言
来源：http://tk.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://go.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://ke.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tu.szsharing.cn

================================================================================
来源：http://em.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fq.nszjky.cn

================================================================================
来源：http://qz.newstarts.cn

[T01] Kotlin：Hello World
来源：http://oq.szxytkj.cn

println("Hello")
来源：http://hv.haigaiapp.cn

[T02] Kotlin：变量
来源：http://ho.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yv.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://ss.szsharing.cn

"值: $b"
来源：http://pe.newstarts.cn

[T04] Kotlin：空安全
来源：http://in.szsharing.cn

val n: String? = null;  n?.length
来源：http://gb.colortex.cn

[T05] Kotlin：when 表达式
来源：http://jr.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gs.asd995.cn

[T06] Kotlin：集合映射
来源：http://hh.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rh.asd995.cn

[T07] Kotlin：集合过滤
来源：http://bl.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ic.521024.cn

[T08] Kotlin：数据类
来源：http://et.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://ir.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://oe.521024.cn

fun String.exclaim() = this + "!"
来源：http://ky.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://ax.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xu.wgjwhj.cn

[T11] Kotlin：协程
来源：http://hl.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ct.huanxung.cn

[T12] Kotlin：解构声明
来源：http://jw.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://dn.jianghongdianzi.cn


<!-- 参考信息 -->