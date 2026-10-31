代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rs.yuntaijiaju.cn

[R08] 数值比较
来源：http://me.panjiajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uk.haigaiapp.cn

[R09] 字符串比较
来源：http://ls.chemitech.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ec.shxzskj.cn

[R10] 正则匹配
来源：http://bg.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fl.hahajie.cn

[R11] case 多分支
来源：http://zk.szsharing.cn

case "$1" in
来源：http://yf.9csxet.cn

start) echo "启动" ;;
来源：http://bt.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://gj.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://jc.nszjky.cn

esac
来源：http://ce.huixiangedu.cn

[R12] for 遍历文件
来源：http://qg.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://tv.521024.cn

[R13] for 计数循环
来源：http://cx.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://lh.nicolike.cn

[R14] C 风格 for
来源：http://oo.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ag.huanxung.cn

[R15] while 逐行读文件
来源：http://az.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://en.shxzukj.cn

[R16] until 等待条件
来源：http://ua.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xl.gzmigu.cn

[R17] 数组定义与取值
来源：http://ry.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jn.521024.cn

[R18] 遍历数组
来源：http://yw.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rx.shxzukj.cn

[R19] 数组长度
来源：http://im.muxihuayi.cn

echo "${#arr[@]}"
来源：http://en.nicolike.cn

[R20] 关联数组（字典）
来源：http://yu.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://td.szsharing.cn

[R21] 字符串长度
来源：http://bq.wgjwhj.cn

echo "${#s}"
来源：http://cx.hnjuh.cn

[R22] 截取子串
来源：http://is.newstarts.cn

echo "${s:0:5}"
来源：http://cl.bjjhwx.cn

[R23] 字符串替换
来源：http://xu.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://se.9csxet.cn

[R24] 大小写转换
来源：http://ax.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bp.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://fj.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://go.colortex.cn

[R26] 命令替换
来源：http://gc.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://lj.yuexingan06.cn

[R27] 算术展开
来源：http://mw.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://gj.nicolike.cn

[R28] 浮点运算
来源：http://mq.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://qu.asd995.cn

[R29] 定义函数
来源：http://ck.colortex.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wm.muxihuayi.cn

[R30] 函数返回状态码
来源：http://ze.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://mr.shtwfgs.cn

[R31] 局部变量
来源：http://ff.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://wh.9csxet.cn

[R32] 参数个数校验
来源：http://ba.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uq.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://fn.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ge.nicolike.cn

[R34] 退出时清理
来源：http://wd.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jb.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://tn.szxytkj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xv.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://av.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oc.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://ry.szxytkj.cn

files=$(ls -1)
来源：http://fb.gzmigu.cn

[R38] 管道串联
来源：http://ky.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://gt.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://ts.szxytkj.cn

cmd > out.log 2>&1
来源：http://ni.yuexingan06.cn

[R40] 追加写日志
来源：http://mf.521024.cn

echo "log" >> out.log
来源：http://xx.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://jt.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://ql.shxzukj.cn

[R42] 输入重定向
来源：http://ja.yuexingan06.cn

wc -l < a.txt
来源：http://av.muxihuayi.cn

[R43] 按名字查找文件
来源：http://ej.szxytkj.cn

find . -name "*.log" -type f
来源：http://xd.bjjhwx.cn

[R44] 按修改时间查找
来源：http://dx.jctech888.com.cn

find . -mtime -7 -type f
来源：http://qt.muxihuayi.cn

[R45] 批量删除
来源：http://pw.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://hu.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://ao.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ey.huixiangedu.cn

[R47] sed 单行替换
来源：http://dq.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hs.huanxung.cn

[R48] awk 取指定列
来源：http://oi.521024.cn

awk '{print $1, $3}' a.txt
来源：http://oh.jianghongdianzi.cn

[R49] awk 带条件
来源：http://cf.chemitech.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://og.yuntaijiaju.cn

[R50] awk 求和
来源：http://bb.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ek.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://sv.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zx.shxzskj.cn

[R52] 统计行数
来源：http://hw.muxihuayi.cn

wc -l a.txt
来源：http://ns.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://rd.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xn.shtwfgs.cn

[R54] 比较两个文件
来源：http://hw.huixiangedu.cn

diff a.txt b.txt
来源：http://ur.lnxyls.cn

[R55] 压缩与解压
来源：http://hm.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://se.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://kz.nicolike.cn

scp file user@host:/path/
来源：http://mo.jctech888.com.cn

[R57] 远程执行命令
来源：http://zx.lnxyls.cn

ssh user@host 'uptime'
来源：http://sv.bookmarksfly.cn

[R58] 下载文件
来源：http://sd.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qg.gzmigu.cn

[R59] 发 POST JSON
来源：http://gs.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ke.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://gi.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ez.panjiajie.cn

[R61] 磁盘占用
来源：http://kg.colortex.cn

df -h;  du -sh *
来源：http://be.huanxung.cn

[R62] 找最占空间的文件
来源：http://ck.521024.cn

du -ah . | sort -rh | head -10
来源：http://qj.jctech888.com.cn

[R63] 内存与进程
来源：http://wt.colortex.cn

free -h;  ps aux | grep nginx
来源：http://zo.hnjuh.cn

[R64] 结束进程
来源：http://xi.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://ca.panjiajie.cn

[R65] 查看端口占用
来源：http://uk.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zu.huanxung.cn

[R66] 定时任务
来源：http://kq.lnxyls.cn

crontab -e;  crontab -l
来源：http://ah.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://ar.haigaiapp.cn

openssl rand -hex 16
来源：http://pw.9csxet.cn

[R68] 计算文件校验值
来源：http://xt.gzmigu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bt.lnxyls.cn

[R69] 生成随机密码
来源：http://ug.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://pv.colortex.cn

[R70] 时间戳与互转
来源：http://wq.hahajie.cn

date +%s;  date -d @1700000000
来源：http://ba.shxzukj.cn

[R71] 日期格式化
来源：http://kj.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sz.huixiangedu.cn

[R72] 等待端口就绪
来源：http://or.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dp.huixinmuqiang.cn

[R73] 分割大日志
来源：http://hu.colortex.cn

split -l 1000 big.log part_
来源：http://yj.gzmigu.cn

[R74] 批量重命名
来源：http://ty.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hg.shxzukj.cn

[R75] 导出环境变量
来源：http://sa.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://la.hahajie.cn

[R76] 使用临时文件
来源：http://jz.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ov.szsharing.cn

[R77] 读取用户输入
来源：http://ci.huanxung.cn

read -rp "请输入: " ans
来源：http://qx.haigaiapp.cn

[R78] 交互式菜单
来源：http://nx.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://om.yuexingan06.cn

[R79] 解析命令行选项
来源：http://we.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rd.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://ig.muxihuayi.cn

time ./run.sh
来源：http://mx.yuexingan06.cn

================================================================================
来源：http://va.lnxyls.cn

S. C / C++ 专题
来源：http://pk.bjjhwx.cn

================================================================================
来源：http://bo.chemitech.net.cn

[S01] C：Hello World
来源：http://uf.521024.cn

#include <stdio.h>
来源：http://jm.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ru.gzmigu.cn

[S02] C：变量与格式化输出
来源：http://wt.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://oo.muxihuayi.cn

[S03] C：读入整数
来源：http://nn.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://kt.hnjuh.cn

[S04] C：字符串复制
来源：http://ey.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ow.521024.cn

[S05] C：字符串长度
来源：http://hx.huanxung.cn

strlen(s)
来源：http://mo.bjjhwx.cn

[S06] C：字符串比较
来源：http://gv.haigaiapp.cn

strcmp(a, b) == 0
来源：http://gh.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://mh.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fp.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://tu.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pt.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://ob.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pu.hahajie.cn

[S10] C：指针与解引用
来源：http://cc.521024.cn

int *p = &a;  *p = 5;
来源：http://yi.nicolike.cn

[S11] C：逐行读文件
来源：http://xc.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://xc.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fx.szxytkj.cn

fclose(f);
来源：http://hv.newstarts.cn

[S12] C：写文件
来源：http://wi.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ni.yuntaijiaju.cn

[S13] C：宏定义
来源：http://ap.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nh.jctech888.com.cn

[S14] C：枚举
来源：http://ar.shxzukj.cn

enum Color { RED, GREEN, BLUE };
来源：http://ds.hahajie.cn

[S15] C：类型转换
来源：http://en.haigaiapp.cn

(double) a / b
来源：http://qd.newstarts.cn

[S16] C：位操作置位
来源：http://st.huixiangedu.cn

x |= (1 << 3);
来源：http://zz.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://ub.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vl.bookmarksfly.cn

[S18] C：命令行参数
来源：http://qs.lnxyls.cn

int main(int argc, char **argv)
来源：http://ns.9csxet.cn

[S19] C：快速排序
来源：http://cc.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://td.gzmigu.cn

[S20] C：二分查找
来源：http://ew.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lh.jctech888.com.cn

[S21] C：字符类别判断
来源：http://jb.wgjwhj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zg.wgjwhj.cn

[S22] C：字符串转数字
来源：http://zo.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yr.521024.cn

[S23] C：随机数
来源：http://jj.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vz.newstarts.cn

[S24] C：获取本地时间
来源：http://bq.yuexingan06.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dh.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://dm.wgjwhj.cn

memcpy(dst, src, n);
来源：http://yc.colortex.cn

[S26] C：内存清零
来源：http://hg.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://yk.shxzskj.cn

[S27] C：定义常量
来源：http://ct.nszjky.cn

const double PI = 3.14159;
来源：http://zs.shxzukj.cn

[S28] C：静态变量
来源：http://ms.bjjhwx.cn

static int counter = 0;
来源：http://cr.521024.cn

[S29] C：变参函数
来源：http://ao.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cd.shxzukj.cn

[S30] C：头文件保护
来源：http://zk.jctech888.com.cn

#ifndef X_H
来源：http://aq.nicolike.cn

#define X_H
来源：http://ae.chemitech.net.cn

#endif
来源：http://ck.asd995.cn

[S31] C++：Hello World
来源：http://lz.yuexingan06.cn

#include <iostream>
来源：http://ux.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://by.colortex.cn

[S32] C++：字符串
来源：http://ud.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://mx.shxzskj.cn

[S33] C++：vector 增删
来源：http://mt.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dg.shtwfgs.cn

[S34] C++：遍历 vector
来源：http://kn.asd995.cn

for (auto &x : v) { std::cout << x; }
来源：http://jw.haigaiapp.cn

[S35] C++：map
来源：http://kt.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bk.wgjwhj.cn

[S36] C++：unordered_map
来源：http://ae.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ge.newstarts.cn

[S37] C++：set
来源：http://ez.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ez.gzmigu.cn

[S38] C++：排序
来源：http://mq.shxzukj.cn

std::sort(v.begin(), v.end());
来源：http://lh.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://zq.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rb.newstarts.cn

[S40] C++：查找元素
来源：http://oa.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gg.szxytkj.cn

[S41] C++：类与构造函数
来源：http://bw.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lg.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://ph.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://kr.gzmigu.cn

[S43] C++：智能指针
来源：http://jz.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://cd.bjjhwx.cn

[S44] C++：引用传参
来源：http://zr.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://ud.huanxung.cn

[S45] C++：lambda
来源：http://ds.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pk.huanxung.cn

[S46] C++：函数模板
来源：http://lu.asd995.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ky.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://nt.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dk.521024.cn

[S48] C++：逐行读文件
来源：http://cc.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nz.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://sk.wgjwhj.cn

[S49] C++：写文件
来源：http://io.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qc.haigaiapp.cn

[S50] C++：格式化数字
来源：http://fj.huanxung.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gh.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://yo.szxytkj.cn

static_cast<double>(a) / b
来源：http://oz.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://tm.newstarts.cn

int size() const noexcept { return n_; }
来源：http://qt.panjiajie.cn

[S53] C++：移动语义
来源：http://dn.panjiajie.cn

std::vector<int> w = std::move(v);
来源：http://cv.newstarts.cn

[S54] C++：异常处理
来源：http://ng.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ym.shxzukj.cn

[S55] C++：结构化绑定
来源：http://un.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nc.wgjwhj.cn

[S56] C++：optional
来源：http://su.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jq.yuexingan06.cn

[S57] C++：编译期常量
来源：http://jt.nszjky.cn

constexpr int N = 10;
来源：http://pr.muxihuayi.cn

[S58] C++：命名空间
来源：http://yf.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://fy.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://xy.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hq.521024.cn

[S60] C++：遍历并删除元素
来源：http://tz.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hw.shxzskj.cn

================================================================================
来源：http://fu.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lw.panjiajie.cn

================================================================================
来源：http://nq.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://th.huixinmuqiang.cn

println("Hello")
来源：http://mk.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://xe.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://be.colortex.cn

[T03] Kotlin：字符串模板
来源：http://ox.huixiangedu.cn

"值: $b"
来源：http://wo.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://vh.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://dv.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://ug.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dz.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://nc.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ve.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://br.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://or.panjiajie.cn

[T08] Kotlin：数据类
来源：http://eb.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://ij.newstarts.cn


<!-- 参考信息 -->