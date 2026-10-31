代发 wailian999

readonly PI=3.14
来源：http://en.9csxet.cn

[R04] 位置参数
来源：http://ek.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://em.shxzskj.cn

[R05] 参数默认值
来源：http://tb.lnxyls.cn

name="${1:-default}"
来源：http://gt.shtwfgs.cn

[R06] 判断命令是否存在
来源：http://lx.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ln.chemitech.net.cn

[R07] if 判断文件
来源：http://nl.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oh.shxzukj.cn

[R08] 数值比较
来源：http://yl.jianghongdianzi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ac.shxzskj.cn

[R09] 字符串比较
来源：http://dw.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://eg.muxihuayi.cn

[R10] 正则匹配
来源：http://ue.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qh.gzmigu.cn

[R11] case 多分支
来源：http://sv.shtwfgs.cn

case "$1" in
来源：http://st.bjjhwx.cn

start) echo "启动" ;;
来源：http://lj.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://pi.huanxung.cn

*)     echo "未知命令" ;;
来源：http://wc.gzmigu.cn

esac
来源：http://fo.shxzukj.cn

[R12] for 遍历文件
来源：http://yn.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://np.haigaiapp.cn

[R13] for 计数循环
来源：http://wm.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://xq.hahajie.cn

[R14] C 风格 for
来源：http://ab.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cm.wgjwhj.cn

[R15] while 逐行读文件
来源：http://xy.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bl.nicolike.cn

[R16] until 等待条件
来源：http://yr.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://go.hahajie.cn

[R17] 数组定义与取值
来源：http://ob.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gq.newstarts.cn

[R18] 遍历数组
来源：http://fv.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mr.shxzskj.cn

[R19] 数组长度
来源：http://il.jianghongdianzi.cn

echo "${#arr[@]}"
来源：http://cl.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://pm.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gn.muxihuayi.cn

[R21] 字符串长度
来源：http://re.newstarts.cn

echo "${#s}"
来源：http://wi.szsharing.cn

[R22] 截取子串
来源：http://bq.yuexingan06.cn

echo "${s:0:5}"
来源：http://nk.bookmarksfly.cn

[R23] 字符串替换
来源：http://jl.521024.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pa.haigaiapp.cn

[R24] 大小写转换
来源：http://qa.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hm.bjjhwx.cn

[R25] 去后缀 / 去前缀
来源：http://ow.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jo.bjjhwx.cn

[R26] 命令替换
来源：http://mn.huixiangedu.cn

now=$(date +%F); echo "$now"
来源：http://af.bjjhwx.cn

[R27] 算术展开
来源：http://em.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://go.shxzskj.cn

[R28] 浮点运算
来源：http://ua.asd995.cn

echo "scale=2; 10/3" | bc
来源：http://qm.nicolike.cn

[R29] 定义函数
来源：http://oz.bjjhwx.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lw.521024.cn

[R30] 函数返回状态码
来源：http://fc.newstarts.cn

f() { return 0; }; f || echo "失败了"
来源：http://lj.jianghongdianzi.cn

[R31] 局部变量
来源：http://je.521024.cn

f() { local x=1; echo "$x"; }
来源：http://iy.shtwfgs.cn

[R32] 参数个数校验
来源：http://ji.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tq.521024.cn

[R33] 捕获错误并提示行号
来源：http://gg.haigaiapp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gi.shxzukj.cn

[R34] 退出时清理
来源：http://tn.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ix.bookmarksfly.cn

[R35] 后台执行并等待
来源：http://lq.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gx.huanxung.cn

[R36] 并发执行多个任务
来源：http://lu.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qk.shxzukj.cn

[R37] 把输出赋给变量
来源：http://kq.shxzukj.cn

files=$(ls -1)
来源：http://zq.9csxet.cn

[R38] 管道串联
来源：http://dg.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://ne.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://ia.nicolike.cn

cmd > out.log 2>&1
来源：http://ng.gzmigu.cn

[R40] 追加写日志
来源：http://ws.huixinmuqiang.cn

echo "log" >> out.log
来源：http://fr.newstarts.cn

[R41] 丢弃输出
来源：http://rm.colortex.cn

cmd >/dev/null 2>&1
来源：http://en.jianghongdianzi.cn

[R42] 输入重定向
来源：http://mj.wgjwhj.cn

wc -l < a.txt
来源：http://xz.huanxung.cn

[R43] 按名字查找文件
来源：http://or.9csxet.cn

find . -name "*.log" -type f
来源：http://vr.shxzskj.cn

[R44] 按修改时间查找
来源：http://mi.chemitech.net.cn

find . -mtime -7 -type f
来源：http://or.hahajie.cn

[R45] 批量删除
来源：http://he.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://nc.nszjky.cn

[R46] 递归替换文件内容
来源：http://qi.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ge.nszjky.cn

[R47] sed 单行替换
来源：http://ie.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ge.huixiangedu.cn

[R48] awk 取指定列
来源：http://qy.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://sy.bookmarksfly.cn

[R49] awk 带条件
来源：http://bo.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kq.shtwfgs.cn

[R50] awk 求和
来源：http://sn.yuexingan06.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tr.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://uq.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ga.bookmarksfly.cn

[R52] 统计行数
来源：http://hy.hahajie.cn

wc -l a.txt
来源：http://pq.colortex.cn

[R53] 查看文件头与实时尾
来源：http://ct.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qa.shxzukj.cn

[R54] 比较两个文件
来源：http://hx.nicolike.cn

diff a.txt b.txt
来源：http://vl.gzmigu.cn

[R55] 压缩与解压
来源：http://vu.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ya.shxzukj.cn

[R56] 远程拷贝
来源：http://nr.shxzukj.cn

scp file user@host:/path/
来源：http://vh.chemitech.net.cn

[R57] 远程执行命令
来源：http://dy.panjiajie.cn

ssh user@host 'uptime'
来源：http://ji.asd995.cn

[R58] 下载文件
来源：http://mp.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ud.nicolike.cn

[R59] 发 POST JSON
来源：http://uu.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nd.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://if.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hl.bookmarksfly.cn

[R61] 磁盘占用
来源：http://mr.newstarts.cn

df -h;  du -sh *
来源：http://fl.shxzskj.cn

[R62] 找最占空间的文件
来源：http://qz.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://el.shtwfgs.cn

[R63] 内存与进程
来源：http://mo.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://js.gzmigu.cn

[R64] 结束进程
来源：http://ip.lnxyls.cn

kill -9 $(pgrep -f app.py)
来源：http://iq.shxzskj.cn

[R65] 查看端口占用
来源：http://ik.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vj.nszjky.cn

[R66] 定时任务
来源：http://dy.jctech888.com.cn

crontab -e;  crontab -l
来源：http://xj.huanxung.cn

[R67] 生成随机十六进制串
来源：http://vd.szxytkj.cn

openssl rand -hex 16
来源：http://zf.jctech888.com.cn

[R68] 计算文件校验值
来源：http://mn.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://st.lnxyls.cn

[R69] 生成随机密码
来源：http://vm.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://xl.huixiangedu.cn

[R70] 时间戳与互转
来源：http://mw.panjiajie.cn

date +%s;  date -d @1700000000
来源：http://lj.yuntaijiaju.cn

[R71] 日期格式化
来源：http://dh.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eb.nszjky.cn

[R72] 等待端口就绪
来源：http://qo.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ax.gzmigu.cn

[R73] 分割大日志
来源：http://vb.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://gj.521024.cn

[R74] 批量重命名
来源：http://uj.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iu.colortex.cn

[R75] 导出环境变量
来源：http://jf.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://ty.nszjky.cn

[R76] 使用临时文件
来源：http://sf.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bg.hahajie.cn

[R77] 读取用户输入
来源：http://lh.521024.cn

read -rp "请输入: " ans
来源：http://fv.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://tg.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qk.521024.cn

[R79] 解析命令行选项
来源：http://ey.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bw.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://bt.hnjuh.cn

time ./run.sh
来源：http://jg.yuexingan06.cn

================================================================================
来源：http://mw.wgjwhj.cn

S. C / C++ 专题
来源：http://mk.huixiangedu.cn

================================================================================
来源：http://wk.yuexingan06.cn

[S01] C：Hello World
来源：http://nf.bjjhwx.cn

#include <stdio.h>
来源：http://zy.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bw.521024.cn

[S02] C：变量与格式化输出
来源：http://gl.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://iq.shxzukj.cn

[S03] C：读入整数
来源：http://iz.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://hu.asd995.cn

[S04] C：字符串复制
来源：http://lt.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mb.bjjhwx.cn

[S05] C：字符串长度
来源：http://hl.gzmigu.cn

strlen(s)
来源：http://uz.9csxet.cn

[S06] C：字符串比较
来源：http://oy.szsharing.cn

strcmp(a, b) == 0
来源：http://if.gzmigu.cn

[S07] C：数组遍历求和
来源：http://uz.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ky.9csxet.cn

[S08] C：动态内存分配与释放
来源：http://zc.chemitech.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ko.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://lx.521024.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yh.huixiangedu.cn

[S10] C：指针与解引用
来源：http://za.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://ho.wgjwhj.cn

[S11] C：逐行读文件
来源：http://mq.lnxyls.cn

FILE *f = fopen("a.txt", "r");
来源：http://gz.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ju.shtwfgs.cn

fclose(f);
来源：http://hz.hnjuh.cn

[S12] C：写文件
来源：http://vw.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eh.wgjwhj.cn

[S13] C：宏定义
来源：http://ic.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jm.haigaiapp.cn

[S14] C：枚举
来源：http://ut.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://lx.jianghongdianzi.cn

[S15] C：类型转换
来源：http://hj.shtwfgs.cn

(double) a / b
来源：http://gs.colortex.cn

[S16] C：位操作置位
来源：http://od.521024.cn

x |= (1 << 3);
来源：http://wk.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://fg.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sn.wgjwhj.cn

[S18] C：命令行参数
来源：http://zm.huixiangedu.cn

int main(int argc, char **argv)
来源：http://rv.colortex.cn

[S19] C：快速排序
来源：http://yn.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zj.szsharing.cn

[S20] C：二分查找
来源：http://pa.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ft.newstarts.cn

[S21] C：字符类别判断
来源：http://fl.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qh.9csxet.cn

[S22] C：字符串转数字
来源：http://wq.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ij.wgjwhj.cn

[S23] C：随机数
来源：http://rd.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://us.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://vc.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kf.nicolike.cn

[S25] C：内存拷贝
来源：http://kq.nszjky.cn

memcpy(dst, src, n);
来源：http://fm.szsharing.cn

[S26] C：内存清零
来源：http://tp.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://nq.colortex.cn

[S27] C：定义常量
来源：http://ds.muxihuayi.cn

const double PI = 3.14159;
来源：http://ng.wgjwhj.cn

[S28] C：静态变量
来源：http://dg.asd995.cn

static int counter = 0;
来源：http://ww.9csxet.cn

[S29] C：变参函数
来源：http://vn.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pl.bjjhwx.cn

[S30] C：头文件保护
来源：http://ez.nicolike.cn

#ifndef X_H
来源：http://fs.521024.cn

#define X_H
来源：http://gk.muxihuayi.cn

#endif
来源：http://uz.hahajie.cn

[S31] C++：Hello World
来源：http://dk.colortex.cn

#include <iostream>
来源：http://ld.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://ec.9csxet.cn

[S32] C++：字符串
来源：http://kj.colortex.cn

std::string s = "hi";  s += "!";
来源：http://kp.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://ri.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zx.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://ib.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://at.521024.cn

[S35] C++：map
来源：http://sq.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ij.lnxyls.cn

[S36] C++：unordered_map
来源：http://dh.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cz.yuexingan06.cn

[S37] C++：set
来源：http://lq.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qm.huixinmuqiang.cn

[S38] C++：排序
来源：http://ow.521024.cn

std::sort(v.begin(), v.end());
来源：http://hx.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://cz.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bg.shtwfgs.cn

[S40] C++：查找元素
来源：http://ho.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jb.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://bd.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yn.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://js.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://fm.wgjwhj.cn

[S43] C++：智能指针
来源：http://uu.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://od.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://ih.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://yf.yuntaijiaju.cn

[S45] C++：lambda
来源：http://kz.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wf.lnxyls.cn

[S46] C++：函数模板
来源：http://pe.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dx.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://sn.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vt.nszjky.cn

[S48] C++：逐行读文件
来源：http://fa.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jf.521024.cn

while (std::getline(in, line)) { }
来源：http://cn.nszjky.cn

[S49] C++：写文件
来源：http://ok.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lt.9csxet.cn

[S50] C++：格式化数字
来源：http://fd.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://im.szxytkj.cn

[S51] C++：显式类型转换
来源：http://lw.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://sb.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://jd.asd995.cn

int size() const noexcept { return n_; }
来源：http://fa.hahajie.cn

[S53] C++：移动语义
来源：http://gy.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://jj.newstarts.cn

[S54] C++：异常处理
来源：http://aj.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ri.asd995.cn

[S55] C++：结构化绑定
来源：http://oh.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ct.szsharing.cn

[S56] C++：optional
来源：http://qf.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://am.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://rt.shxzukj.cn

constexpr int N = 10;
来源：http://re.yuexingan06.cn

[S58] C++：命名空间
来源：http://pq.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://tc.521024.cn

[S59] C++：静态断言
来源：http://fc.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hd.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://mk.huixinmuqiang.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://av.huixinmuqiang.cn

================================================================================
来源：http://dd.gzmigu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eb.gzmigu.cn

================================================================================
来源：http://no.szxytkj.cn

[T01] Kotlin：Hello World
来源：http://pj.hnjuh.cn

println("Hello")
来源：http://ga.hnjuh.cn

[T02] Kotlin：变量
来源：http://wg.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pr.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://bj.colortex.cn

"值: $b"
来源：http://jl.bjjhwx.cn

[T04] Kotlin：空安全
来源：http://bk.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://vv.shxzskj.cn


<!-- 参考信息 -->