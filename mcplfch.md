代发 wailian999

name="${1:-default}"
来源：http://xm.szsharing.cn

[R06] 判断命令是否存在
来源：http://sp.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rz.muxihuayi.cn

[R07] if 判断文件
来源：http://nf.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zs.lnxyls.cn

[R08] 数值比较
来源：http://dm.hahajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mi.colortex.cn

[R09] 字符串比较
来源：http://qz.bookmarksfly.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bg.wgjwhj.cn

[R10] 正则匹配
来源：http://ek.newstarts.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kj.huixinmuqiang.cn

[R11] case 多分支
来源：http://vt.szsharing.cn

case "$1" in
来源：http://tw.shxzukj.cn

start) echo "启动" ;;
来源：http://nn.hnjuh.cn

stop)  echo "停止" ;;
来源：http://ml.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://xn.colortex.cn

esac
来源：http://nu.hahajie.cn

[R12] for 遍历文件
来源：http://ml.szsharing.cn

for f in *.txt; do echo "$f"; done
来源：http://qf.huixinmuqiang.cn

[R13] for 计数循环
来源：http://yb.jianghongdianzi.cn

for i in {1..10}; do echo "$i"; done
来源：http://ah.huixiangedu.cn

[R14] C 风格 for
来源：http://lq.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://em.colortex.cn

[R15] while 逐行读文件
来源：http://da.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mo.shxzskj.cn

[R16] until 等待条件
来源：http://ha.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mm.newstarts.cn

[R17] 数组定义与取值
来源：http://bo.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mz.gzmigu.cn

[R18] 遍历数组
来源：http://as.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zc.yuexingan06.cn

[R19] 数组长度
来源：http://dx.jctech888.com.cn

echo "${#arr[@]}"
来源：http://oa.asd995.cn

[R20] 关联数组（字典）
来源：http://pz.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gb.jctech888.com.cn

[R21] 字符串长度
来源：http://vv.szsharing.cn

echo "${#s}"
来源：http://jh.jianghongdianzi.cn

[R22] 截取子串
来源：http://ck.9csxet.cn

echo "${s:0:5}"
来源：http://md.nszjky.cn

[R23] 字符串替换
来源：http://zo.szxytkj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bl.shxzukj.cn

[R24] 大小写转换
来源：http://km.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tx.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://do.huixiangedu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ex.bjjhwx.cn

[R26] 命令替换
来源：http://en.colortex.cn

now=$(date +%F); echo "$now"
来源：http://av.yuntaijiaju.cn

[R27] 算术展开
来源：http://iy.szsharing.cn

echo $((1 + 2 * 3))
来源：http://hm.jianghongdianzi.cn

[R28] 浮点运算
来源：http://ch.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://wa.yuntaijiaju.cn

[R29] 定义函数
来源：http://ma.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xi.asd995.cn

[R30] 函数返回状态码
来源：http://nn.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://to.yuntaijiaju.cn

[R31] 局部变量
来源：http://eb.hahajie.cn

f() { local x=1; echo "$x"; }
来源：http://ug.yuexingan06.cn

[R32] 参数个数校验
来源：http://xf.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ox.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://mp.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dh.bookmarksfly.cn

[R34] 退出时清理
来源：http://sf.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vi.wgjwhj.cn

[R35] 后台执行并等待
来源：http://ke.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xk.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://pu.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bm.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://ab.szsharing.cn

files=$(ls -1)
来源：http://yk.szsharing.cn

[R38] 管道串联
来源：http://qp.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://yo.asd995.cn

[R39] 重定向标准输出与错误
来源：http://rx.shtwfgs.cn

cmd > out.log 2>&1
来源：http://kd.panjiajie.cn

[R40] 追加写日志
来源：http://qb.huanxung.cn

echo "log" >> out.log
来源：http://qe.haigaiapp.cn

[R41] 丢弃输出
来源：http://un.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://rd.szxytkj.cn

[R42] 输入重定向
来源：http://ly.gzmigu.cn

wc -l < a.txt
来源：http://yy.jctech888.com.cn

[R43] 按名字查找文件
来源：http://rt.haigaiapp.cn

find . -name "*.log" -type f
来源：http://rr.newstarts.cn

[R44] 按修改时间查找
来源：http://rp.huixinmuqiang.cn

find . -mtime -7 -type f
来源：http://oc.bjjhwx.cn

[R45] 批量删除
来源：http://no.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://xp.asd995.cn

[R46] 递归替换文件内容
来源：http://zy.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hw.hnjuh.cn

[R47] sed 单行替换
来源：http://zl.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xk.szxytkj.cn

[R48] awk 取指定列
来源：http://ku.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://dy.huanxung.cn

[R49] awk 带条件
来源：http://rr.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sp.haigaiapp.cn

[R50] awk 求和
来源：http://nv.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://px.lnxyls.cn

[R51] 排序去重取前几
来源：http://pt.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://td.521024.cn

[R52] 统计行数
来源：http://bh.huanxung.cn

wc -l a.txt
来源：http://lk.asd995.cn

[R53] 查看文件头与实时尾
来源：http://sh.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sg.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://gx.haigaiapp.cn

diff a.txt b.txt
来源：http://cg.szxytkj.cn

[R55] 压缩与解压
来源：http://cj.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gs.wgjwhj.cn

[R56] 远程拷贝
来源：http://mo.nicolike.cn

scp file user@host:/path/
来源：http://zm.521024.cn

[R57] 远程执行命令
来源：http://cd.huixiangedu.cn

ssh user@host 'uptime'
来源：http://bl.huanxung.cn

[R58] 下载文件
来源：http://tt.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fn.9csxet.cn

[R59] 发 POST JSON
来源：http://bx.jianghongdianzi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ib.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://ab.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://av.szsharing.cn

[R61] 磁盘占用
来源：http://ch.521024.cn

df -h;  du -sh *
来源：http://hq.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://gm.colortex.cn

du -ah . | sort -rh | head -10
来源：http://tu.shxzskj.cn

[R63] 内存与进程
来源：http://vh.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://ar.asd995.cn

[R64] 结束进程
来源：http://rz.haigaiapp.cn

kill -9 $(pgrep -f app.py)
来源：http://ki.bjjhwx.cn

[R65] 查看端口占用
来源：http://cv.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fg.colortex.cn

[R66] 定时任务
来源：http://nt.bookmarksfly.cn

crontab -e;  crontab -l
来源：http://aa.hahajie.cn

[R67] 生成随机十六进制串
来源：http://fh.hnjuh.cn

openssl rand -hex 16
来源：http://vv.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://na.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sd.szxytkj.cn

[R69] 生成随机密码
来源：http://eq.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://am.asd995.cn

[R70] 时间戳与互转
来源：http://wr.colortex.cn

date +%s;  date -d @1700000000
来源：http://nz.huixiangedu.cn

[R71] 日期格式化
来源：http://om.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gp.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://yv.huixinmuqiang.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mt.bjjhwx.cn

[R73] 分割大日志
来源：http://ql.hahajie.cn

split -l 1000 big.log part_
来源：http://ld.muxihuayi.cn

[R74] 批量重命名
来源：http://ng.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cm.huixiangedu.cn

[R75] 导出环境变量
来源：http://yb.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://st.shxzukj.cn

[R76] 使用临时文件
来源：http://fb.shxzskj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wy.bjjhwx.cn

[R77] 读取用户输入
来源：http://eb.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://qk.shxzukj.cn

[R78] 交互式菜单
来源：http://nr.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fy.shxzskj.cn

[R79] 解析命令行选项
来源：http://ec.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://so.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://zg.nicolike.cn

time ./run.sh
来源：http://fy.huixiangedu.cn

================================================================================
来源：http://ht.huixiangedu.cn

S. C / C++ 专题
来源：http://vk.yuntaijiaju.cn

================================================================================
来源：http://ev.nicolike.cn

[S01] C：Hello World
来源：http://rn.wgjwhj.cn

#include <stdio.h>
来源：http://xj.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xf.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://rh.lnxyls.cn

int a = 10; printf("%d\n", a);
来源：http://tk.asd995.cn

[S03] C：读入整数
来源：http://fc.newstarts.cn

int x; scanf("%d", &x);
来源：http://qe.hahajie.cn

[S04] C：字符串复制
来源：http://ba.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ga.asd995.cn

[S05] C：字符串长度
来源：http://zy.bjjhwx.cn

strlen(s)
来源：http://um.chemitech.net.cn

[S06] C：字符串比较
来源：http://xo.hahajie.cn

strcmp(a, b) == 0
来源：http://eo.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://kj.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zs.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://rn.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ln.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://tg.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qt.hnjuh.cn

[S10] C：指针与解引用
来源：http://cj.newstarts.cn

int *p = &a;  *p = 5;
来源：http://at.huixiangedu.cn

[S11] C：逐行读文件
来源：http://zw.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://ba.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rb.haigaiapp.cn

fclose(f);
来源：http://mb.hahajie.cn

[S12] C：写文件
来源：http://lr.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hx.chemitech.net.cn

[S13] C：宏定义
来源：http://id.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uj.szsharing.cn

[S14] C：枚举
来源：http://ll.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://yr.yuexingan06.cn

[S15] C：类型转换
来源：http://xk.szsharing.cn

(double) a / b
来源：http://zy.jctech888.com.cn

[S16] C：位操作置位
来源：http://dw.yuntaijiaju.cn

x |= (1 << 3);
来源：http://iv.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://ls.bjjhwx.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://if.panjiajie.cn

[S18] C：命令行参数
来源：http://wo.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://zh.jianghongdianzi.cn

[S19] C：快速排序
来源：http://yw.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tc.szxytkj.cn

[S20] C：二分查找
来源：http://lb.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ve.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://tp.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ad.yuexingan06.cn

[S22] C：字符串转数字
来源：http://or.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hk.hnjuh.cn

[S23] C：随机数
来源：http://jz.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lx.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://wy.hahajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wr.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://eh.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://wp.jianghongdianzi.cn

[S26] C：内存清零
来源：http://hx.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://pm.chemitech.net.cn

[S27] C：定义常量
来源：http://se.newstarts.cn

const double PI = 3.14159;
来源：http://om.lnxyls.cn

[S28] C：静态变量
来源：http://pj.panjiajie.cn

static int counter = 0;
来源：http://xu.huixinmuqiang.cn

[S29] C：变参函数
来源：http://sh.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hh.haigaiapp.cn

[S30] C：头文件保护
来源：http://wg.hahajie.cn

#ifndef X_H
来源：http://nh.nszjky.cn

#define X_H
来源：http://wr.panjiajie.cn

#endif
来源：http://ed.wgjwhj.cn

[S31] C++：Hello World
来源：http://jf.szsharing.cn

#include <iostream>
来源：http://gc.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://bt.lnxyls.cn

[S32] C++：字符串
来源：http://tq.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://oj.szsharing.cn

[S33] C++：vector 增删
来源：http://nj.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://td.huanxung.cn

[S34] C++：遍历 vector
来源：http://ys.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://pg.huanxung.cn

[S35] C++：map
来源：http://js.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nz.huixiangedu.cn

[S36] C++：unordered_map
来源：http://ko.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yd.huanxung.cn

[S37] C++：set
来源：http://qa.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xp.jctech888.com.cn

[S38] C++：排序
来源：http://uo.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://zd.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://vd.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://da.jctech888.com.cn

[S40] C++：查找元素
来源：http://de.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ww.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://fv.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uc.nszjky.cn

[S42] C++：继承与虚函数
来源：http://lf.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://uj.newstarts.cn

[S43] C++：智能指针
来源：http://mo.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://lo.shxzukj.cn

[S44] C++：引用传参
来源：http://xu.nszjky.cn

void inc(int &x) { ++x; }
来源：http://bf.nszjky.cn

[S45] C++：lambda
来源：http://gn.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pq.haigaiapp.cn

[S46] C++：函数模板
来源：http://dd.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ux.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://ai.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wo.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://zj.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ac.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://eh.muxihuayi.cn

[S49] C++：写文件
来源：http://ck.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mi.nszjky.cn

[S50] C++：格式化数字
来源：http://xt.shtwfgs.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rl.szxytkj.cn

[S51] C++：显式类型转换
来源：http://ue.huixiangedu.cn

static_cast<double>(a) / b
来源：http://nt.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://mh.shxzukj.cn

int size() const noexcept { return n_; }
来源：http://ma.szsharing.cn

[S53] C++：移动语义
来源：http://pb.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://lj.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://fh.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ds.9csxet.cn

[S55] C++：结构化绑定
来源：http://ko.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://eu.asd995.cn

[S56] C++：optional
来源：http://ex.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rl.wgjwhj.cn

[S57] C++：编译期常量
来源：http://ey.lnxyls.cn

constexpr int N = 10;
来源：http://wg.9csxet.cn

[S58] C++：命名空间
来源：http://tf.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://pb.huanxung.cn

[S59] C++：静态断言
来源：http://wn.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ox.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://im.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yn.521024.cn

================================================================================
来源：http://lr.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pd.shxzskj.cn

================================================================================
来源：http://os.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://sj.jctech888.com.cn

println("Hello")
来源：http://xn.yuexingan06.cn

[T02] Kotlin：变量
来源：http://ht.gzmigu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dj.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://oc.chemitech.net.cn

"值: $b"
来源：http://cg.shxzskj.cn

[T04] Kotlin：空安全
来源：http://sn.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://ak.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://fk.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rf.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://eh.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gm.haigaiapp.cn


<!-- 参考信息 -->