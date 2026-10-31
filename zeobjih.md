代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lt.chemitech.net.cn

[R10] 正则匹配
来源：http://vp.newstarts.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sn.newstarts.cn

[R11] case 多分支
来源：http://kj.lnxyls.cn

case "$1" in
来源：http://ul.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://op.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://pj.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://sz.huixiangedu.cn

esac
来源：http://qc.muxihuayi.cn

[R12] for 遍历文件
来源：http://ig.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://wu.chemitech.net.cn

[R13] for 计数循环
来源：http://vt.shxzskj.cn

for i in {1..10}; do echo "$i"; done
来源：http://fm.bjjhwx.cn

[R14] C 风格 for
来源：http://lm.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wf.szxytkj.cn

[R15] while 逐行读文件
来源：http://zv.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ft.huixiangedu.cn

[R16] until 等待条件
来源：http://st.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ql.bjjhwx.cn

[R17] 数组定义与取值
来源：http://da.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tb.chemitech.net.cn

[R18] 遍历数组
来源：http://mg.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://os.nicolike.cn

[R19] 数组长度
来源：http://rz.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://ec.nszjky.cn

[R20] 关联数组（字典）
来源：http://jf.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cn.nicolike.cn

[R21] 字符串长度
来源：http://vb.yuntaijiaju.cn

echo "${#s}"
来源：http://iv.bookmarksfly.cn

[R22] 截取子串
来源：http://sq.haigaiapp.cn

echo "${s:0:5}"
来源：http://mm.haigaiapp.cn

[R23] 字符串替换
来源：http://mk.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rb.shxzukj.cn

[R24] 大小写转换
来源：http://bn.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wu.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://in.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qj.nicolike.cn

[R26] 命令替换
来源：http://ma.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://de.jctech888.com.cn

[R27] 算术展开
来源：http://nf.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://wv.colortex.cn

[R28] 浮点运算
来源：http://io.nszjky.cn

echo "scale=2; 10/3" | bc
来源：http://jb.panjiajie.cn

[R29] 定义函数
来源：http://eq.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oy.9csxet.cn

[R30] 函数返回状态码
来源：http://lh.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://bq.9csxet.cn

[R31] 局部变量
来源：http://tw.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://ek.lnxyls.cn

[R32] 参数个数校验
来源：http://pa.szxytkj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ew.bjjhwx.cn

[R33] 捕获错误并提示行号
来源：http://hb.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://co.wgjwhj.cn

[R34] 退出时清理
来源：http://tm.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vz.yuexingan06.cn

[R35] 后台执行并等待
来源：http://li.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sb.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://eu.shxzukj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ja.521024.cn

[R37] 把输出赋给变量
来源：http://cq.nszjky.cn

files=$(ls -1)
来源：http://mo.bjjhwx.cn

[R38] 管道串联
来源：http://vl.lnxyls.cn

cat a.txt | grep -i error | wc -l
来源：http://xf.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://cj.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://rb.muxihuayi.cn

[R40] 追加写日志
来源：http://tx.bjjhwx.cn

echo "log" >> out.log
来源：http://ra.wgjwhj.cn

[R41] 丢弃输出
来源：http://ej.521024.cn

cmd >/dev/null 2>&1
来源：http://se.9csxet.cn

[R42] 输入重定向
来源：http://cr.szxytkj.cn

wc -l < a.txt
来源：http://ky.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://rk.lnxyls.cn

find . -name "*.log" -type f
来源：http://zn.shtwfgs.cn

[R44] 按修改时间查找
来源：http://gz.bjjhwx.cn

find . -mtime -7 -type f
来源：http://he.nszjky.cn

[R45] 批量删除
来源：http://bm.colortex.cn

find . -name "*.tmp" -delete
来源：http://ul.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://it.hnjuh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ag.panjiajie.cn

[R47] sed 单行替换
来源：http://dd.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hi.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://tq.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://gd.szsharing.cn

[R49] awk 带条件
来源：http://kc.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ih.shtwfgs.cn

[R50] awk 求和
来源：http://pj.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ej.haigaiapp.cn

[R51] 排序去重取前几
来源：http://nx.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mm.wgjwhj.cn

[R52] 统计行数
来源：http://lf.szsharing.cn

wc -l a.txt
来源：http://ph.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://wd.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gm.521024.cn

[R54] 比较两个文件
来源：http://ro.nicolike.cn

diff a.txt b.txt
来源：http://ig.asd995.cn

[R55] 压缩与解压
来源：http://yn.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ha.bookmarksfly.cn

[R56] 远程拷贝
来源：http://sk.shxzskj.cn

scp file user@host:/path/
来源：http://yv.panjiajie.cn

[R57] 远程执行命令
来源：http://yz.yuntaijiaju.cn

ssh user@host 'uptime'
来源：http://tj.jianghongdianzi.cn

[R58] 下载文件
来源：http://kk.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nj.haigaiapp.cn

[R59] 发 POST JSON
来源：http://ds.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lm.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://zo.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cu.huixiangedu.cn

[R61] 磁盘占用
来源：http://jb.jianghongdianzi.cn

df -h;  du -sh *
来源：http://zk.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://kn.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://it.chemitech.net.cn

[R63] 内存与进程
来源：http://we.colortex.cn

free -h;  ps aux | grep nginx
来源：http://xq.hnjuh.cn

[R64] 结束进程
来源：http://sq.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://re.szxytkj.cn

[R65] 查看端口占用
来源：http://bo.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yh.yuntaijiaju.cn

[R66] 定时任务
来源：http://hj.newstarts.cn

crontab -e;  crontab -l
来源：http://us.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://qz.lnxyls.cn

openssl rand -hex 16
来源：http://qz.muxihuayi.cn

[R68] 计算文件校验值
来源：http://ua.lnxyls.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ao.jctech888.com.cn

[R69] 生成随机密码
来源：http://yr.9csxet.cn

head -c 16 /dev/urandom | base64
来源：http://ws.huixiangedu.cn

[R70] 时间戳与互转
来源：http://cl.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://dg.521024.cn

[R71] 日期格式化
来源：http://vw.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fb.9csxet.cn

[R72] 等待端口就绪
来源：http://hh.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xv.huixinmuqiang.cn

[R73] 分割大日志
来源：http://rg.colortex.cn

split -l 1000 big.log part_
来源：http://xf.jianghongdianzi.cn

[R74] 批量重命名
来源：http://ug.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ez.wgjwhj.cn

[R75] 导出环境变量
来源：http://op.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://ro.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://ca.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hr.wgjwhj.cn

[R77] 读取用户输入
来源：http://id.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://iq.newstarts.cn

[R78] 交互式菜单
来源：http://vh.panjiajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ep.newstarts.cn

[R79] 解析命令行选项
来源：http://ix.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yo.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://tf.jctech888.com.cn

time ./run.sh
来源：http://gc.muxihuayi.cn

================================================================================
来源：http://jp.colortex.cn

S. C / C++ 专题
来源：http://vp.hahajie.cn

================================================================================
来源：http://nw.9csxet.cn

[S01] C：Hello World
来源：http://cv.huixiangedu.cn

#include <stdio.h>
来源：http://da.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vb.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://vc.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://au.hnjuh.cn

[S03] C：读入整数
来源：http://nv.hnjuh.cn

int x; scanf("%d", &x);
来源：http://zx.szxytkj.cn

[S04] C：字符串复制
来源：http://qk.panjiajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gm.chemitech.net.cn

[S05] C：字符串长度
来源：http://lu.panjiajie.cn

strlen(s)
来源：http://zj.szxytkj.cn

[S06] C：字符串比较
来源：http://qa.hnjuh.cn

strcmp(a, b) == 0
来源：http://cs.lnxyls.cn

[S07] C：数组遍历求和
来源：http://wy.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yq.colortex.cn

[S08] C：动态内存分配与释放
来源：http://hz.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vk.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://nw.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ji.shxzukj.cn

[S10] C：指针与解引用
来源：http://bm.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://og.nszjky.cn

[S11] C：逐行读文件
来源：http://gs.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://nx.nicolike.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fi.asd995.cn

fclose(f);
来源：http://kp.hnjuh.cn

[S12] C：写文件
来源：http://un.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bl.asd995.cn

[S13] C：宏定义
来源：http://zf.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tl.huanxung.cn

[S14] C：枚举
来源：http://vc.shxzukj.cn

enum Color { RED, GREEN, BLUE };
来源：http://gu.bookmarksfly.cn

[S15] C：类型转换
来源：http://zv.huixiangedu.cn

(double) a / b
来源：http://jg.gzmigu.cn

[S16] C：位操作置位
来源：http://lm.hahajie.cn

x |= (1 << 3);
来源：http://ai.newstarts.cn

[S17] C：安全拼接字符串
来源：http://nr.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jt.nicolike.cn

[S18] C：命令行参数
来源：http://db.nszjky.cn

int main(int argc, char **argv)
来源：http://xi.panjiajie.cn

[S19] C：快速排序
来源：http://kk.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://em.hnjuh.cn

[S20] C：二分查找
来源：http://hk.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nf.nicolike.cn

[S21] C：字符类别判断
来源：http://lw.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://no.shxzukj.cn

[S22] C：字符串转数字
来源：http://em.nszjky.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ow.jctech888.com.cn

[S23] C：随机数
来源：http://zq.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://da.shxzskj.cn

[S24] C：获取本地时间
来源：http://nt.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fh.hnjuh.cn

[S25] C：内存拷贝
来源：http://xt.shtwfgs.cn

memcpy(dst, src, n);
来源：http://oe.521024.cn

[S26] C：内存清零
来源：http://hb.nicolike.cn

memset(a, 0, sizeof a);
来源：http://nv.yuntaijiaju.cn

[S27] C：定义常量
来源：http://sb.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://lk.chemitech.net.cn

[S28] C：静态变量
来源：http://mv.gzmigu.cn

static int counter = 0;
来源：http://tm.shtwfgs.cn

[S29] C：变参函数
来源：http://ug.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iy.muxihuayi.cn

[S30] C：头文件保护
来源：http://hv.bookmarksfly.cn

#ifndef X_H
来源：http://du.huixinmuqiang.cn

#define X_H
来源：http://up.huanxung.cn

#endif
来源：http://tp.lnxyls.cn

[S31] C++：Hello World
来源：http://mx.yuexingan06.cn

#include <iostream>
来源：http://qd.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ap.bjjhwx.cn

[S32] C++：字符串
来源：http://ai.colortex.cn

std::string s = "hi";  s += "!";
来源：http://zw.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://ba.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kl.szxytkj.cn

[S34] C++：遍历 vector
来源：http://ul.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://fk.hnjuh.cn

[S35] C++：map
来源：http://ci.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://el.newstarts.cn

[S36] C++：unordered_map
来源：http://vo.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jw.wgjwhj.cn

[S37] C++：set
来源：http://pj.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bg.jianghongdianzi.cn

[S38] C++：排序
来源：http://sr.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://qf.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://xz.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nq.szsharing.cn

[S40] C++：查找元素
来源：http://yn.521024.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gi.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://jf.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pe.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://ee.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://vk.lnxyls.cn

[S43] C++：智能指针
来源：http://rf.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://qx.shtwfgs.cn

[S44] C++：引用传参
来源：http://vx.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://ux.huixiangedu.cn

[S45] C++：lambda
来源：http://qs.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cb.colortex.cn

[S46] C++：函数模板
来源：http://mg.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nu.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://dw.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kj.panjiajie.cn

[S48] C++：逐行读文件
来源：http://hb.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qi.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://eh.jianghongdianzi.cn

[S49] C++：写文件
来源：http://ff.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ar.newstarts.cn

[S50] C++：格式化数字
来源：http://lm.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sx.9csxet.cn

[S51] C++：显式类型转换
来源：http://re.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://fi.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://ts.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://ah.szxytkj.cn

[S53] C++：移动语义
来源：http://iw.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://fx.shxzskj.cn

[S54] C++：异常处理
来源：http://ny.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mt.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://bl.muxihuayi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zt.lnxyls.cn

[S56] C++：optional
来源：http://ow.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uy.wgjwhj.cn

[S57] C++：编译期常量
来源：http://kj.yuexingan06.cn

constexpr int N = 10;
来源：http://yw.nicolike.cn

[S58] C++：命名空间
来源：http://dh.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://lu.huanxung.cn

[S59] C++：静态断言
来源：http://gf.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bn.521024.cn

[S60] C++：遍历并删除元素
来源：http://vz.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fl.panjiajie.cn

================================================================================
来源：http://fy.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xm.shxzskj.cn

================================================================================
来源：http://bb.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://vv.nicolike.cn

println("Hello")
来源：http://yo.szxytkj.cn

[T02] Kotlin：变量
来源：http://dn.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ke.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://ax.nicolike.cn

"值: $b"
来源：http://vj.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://uq.9csxet.cn

val n: String? = null;  n?.length
来源：http://or.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://xh.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pa.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://ag.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ig.panjiajie.cn

[T07] Kotlin：集合过滤
来源：http://su.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://eu.nicolike.cn

[T08] Kotlin：数据类
来源：http://wk.asd995.cn

data class User(val name: String, val age: Int)
来源：http://tp.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://oa.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://tx.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://sk.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wq.yuntaijiaju.cn


<!-- 参考信息 -->