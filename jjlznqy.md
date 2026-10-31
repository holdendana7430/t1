代发 wailian999

name="${1:-default}"
来源：http://bc.huanxung.cn

[R06] 判断命令是否存在
来源：http://kl.shtwfgs.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pb.haigaiapp.cn

[R07] if 判断文件
来源：http://uh.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jj.jianghongdianzi.cn

[R08] 数值比较
来源：http://dq.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zj.haigaiapp.cn

[R09] 字符串比较
来源：http://eb.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pm.jctech888.com.cn

[R10] 正则匹配
来源：http://rq.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mk.asd995.cn

[R11] case 多分支
来源：http://dz.colortex.cn

case "$1" in
来源：http://ex.lnxyls.cn

start) echo "启动" ;;
来源：http://xt.nicolike.cn

stop)  echo "停止" ;;
来源：http://to.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://xr.szsharing.cn

esac
来源：http://vn.521024.cn

[R12] for 遍历文件
来源：http://oz.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://ge.bookmarksfly.cn

[R13] for 计数循环
来源：http://yb.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://zp.shxzukj.cn

[R14] C 风格 for
来源：http://sd.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vu.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://mt.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ty.wgjwhj.cn

[R16] until 等待条件
来源：http://fc.521024.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mp.muxihuayi.cn

[R17] 数组定义与取值
来源：http://vs.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yy.yuexingan06.cn

[R18] 遍历数组
来源：http://bq.hnjuh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dz.panjiajie.cn

[R19] 数组长度
来源：http://vc.chemitech.net.cn

echo "${#arr[@]}"
来源：http://zu.lnxyls.cn

[R20] 关联数组（字典）
来源：http://yr.muxihuayi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gv.9csxet.cn

[R21] 字符串长度
来源：http://me.bookmarksfly.cn

echo "${#s}"
来源：http://tb.521024.cn

[R22] 截取子串
来源：http://wh.muxihuayi.cn

echo "${s:0:5}"
来源：http://fi.521024.cn

[R23] 字符串替换
来源：http://ow.lnxyls.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bq.chemitech.net.cn

[R24] 大小写转换
来源：http://yi.newstarts.cn

echo "${s^^}"; echo "${s,,}"
来源：http://za.bjjhwx.cn

[R25] 去后缀 / 去前缀
来源：http://rp.huanxung.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mz.nicolike.cn

[R26] 命令替换
来源：http://ik.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://zu.bjjhwx.cn

[R27] 算术展开
来源：http://oi.nszjky.cn

echo $((1 + 2 * 3))
来源：http://ub.panjiajie.cn

[R28] 浮点运算
来源：http://hj.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://ss.yuexingan06.cn

[R29] 定义函数
来源：http://kb.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bd.hnjuh.cn

[R30] 函数返回状态码
来源：http://wi.nicolike.cn

f() { return 0; }; f || echo "失败了"
来源：http://wi.colortex.cn

[R31] 局部变量
来源：http://qm.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://rq.haigaiapp.cn

[R32] 参数个数校验
来源：http://ow.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lh.jctech888.com.cn

[R33] 捕获错误并提示行号
来源：http://ki.muxihuayi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xa.shxzukj.cn

[R34] 退出时清理
来源：http://on.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uo.haigaiapp.cn

[R35] 后台执行并等待
来源：http://ae.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gl.szxytkj.cn

[R36] 并发执行多个任务
来源：http://aw.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://li.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://yl.hnjuh.cn

files=$(ls -1)
来源：http://mn.panjiajie.cn

[R38] 管道串联
来源：http://ws.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://pn.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://mt.panjiajie.cn

cmd > out.log 2>&1
来源：http://ki.shxzukj.cn

[R40] 追加写日志
来源：http://at.hahajie.cn

echo "log" >> out.log
来源：http://sj.hnjuh.cn

[R41] 丢弃输出
来源：http://se.huanxung.cn

cmd >/dev/null 2>&1
来源：http://xr.lnxyls.cn

[R42] 输入重定向
来源：http://ks.nicolike.cn

wc -l < a.txt
来源：http://cd.huanxung.cn

[R43] 按名字查找文件
来源：http://hj.chemitech.net.cn

find . -name "*.log" -type f
来源：http://kq.wgjwhj.cn

[R44] 按修改时间查找
来源：http://fw.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://vp.lnxyls.cn

[R45] 批量删除
来源：http://gx.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://jz.panjiajie.cn

[R46] 递归替换文件内容
来源：http://rf.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pw.wgjwhj.cn

[R47] sed 单行替换
来源：http://cv.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ai.bookmarksfly.cn

[R48] awk 取指定列
来源：http://wg.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://ou.9csxet.cn

[R49] awk 带条件
来源：http://qb.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jm.szxytkj.cn

[R50] awk 求和
来源：http://dg.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hk.colortex.cn

[R51] 排序去重取前几
来源：http://ii.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ff.jctech888.com.cn

[R52] 统计行数
来源：http://et.huanxung.cn

wc -l a.txt
来源：http://wp.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://fh.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uk.9csxet.cn

[R54] 比较两个文件
来源：http://sh.newstarts.cn

diff a.txt b.txt
来源：http://yx.panjiajie.cn

[R55] 压缩与解压
来源：http://xs.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fy.szsharing.cn

[R56] 远程拷贝
来源：http://ek.yuntaijiaju.cn

scp file user@host:/path/
来源：http://di.huixiangedu.cn

[R57] 远程执行命令
来源：http://ad.jianghongdianzi.cn

ssh user@host 'uptime'
来源：http://zt.haigaiapp.cn

[R58] 下载文件
来源：http://mj.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vb.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://ja.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xb.nicolike.cn

[R60] 只看 HTTP 状态码
来源：http://xd.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ib.shxzukj.cn

[R61] 磁盘占用
来源：http://rl.szxytkj.cn

df -h;  du -sh *
来源：http://nm.lnxyls.cn

[R62] 找最占空间的文件
来源：http://rj.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://kh.newstarts.cn

[R63] 内存与进程
来源：http://hw.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://dl.szsharing.cn

[R64] 结束进程
来源：http://ib.lnxyls.cn

kill -9 $(pgrep -f app.py)
来源：http://ph.bookmarksfly.cn

[R65] 查看端口占用
来源：http://iu.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://if.yuntaijiaju.cn

[R66] 定时任务
来源：http://ax.szxytkj.cn

crontab -e;  crontab -l
来源：http://km.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://iz.nicolike.cn

openssl rand -hex 16
来源：http://ir.shxzskj.cn

[R68] 计算文件校验值
来源：http://te.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://no.panjiajie.cn

[R69] 生成随机密码
来源：http://ie.9csxet.cn

head -c 16 /dev/urandom | base64
来源：http://fk.9csxet.cn

[R70] 时间戳与互转
来源：http://yf.huanxung.cn

date +%s;  date -d @1700000000
来源：http://wg.9csxet.cn

[R71] 日期格式化
来源：http://oi.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ao.nszjky.cn

[R72] 等待端口就绪
来源：http://xk.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cu.yuexingan06.cn

[R73] 分割大日志
来源：http://xm.muxihuayi.cn

split -l 1000 big.log part_
来源：http://lg.haigaiapp.cn

[R74] 批量重命名
来源：http://fk.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://su.huixiangedu.cn

[R75] 导出环境变量
来源：http://vn.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://sl.lnxyls.cn

[R76] 使用临时文件
来源：http://nb.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ne.nicolike.cn

[R77] 读取用户输入
来源：http://sz.haigaiapp.cn

read -rp "请输入: " ans
来源：http://bo.chemitech.net.cn

[R78] 交互式菜单
来源：http://vn.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lj.newstarts.cn

[R79] 解析命令行选项
来源：http://ij.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pk.521024.cn

[R80] 查看脚本执行耗时
来源：http://bo.yuexingan06.cn

time ./run.sh
来源：http://bo.panjiajie.cn

================================================================================
来源：http://tt.szsharing.cn

S. C / C++ 专题
来源：http://xc.shxzukj.cn

================================================================================
来源：http://gr.huixinmuqiang.cn

[S01] C：Hello World
来源：http://zy.lnxyls.cn

#include <stdio.h>
来源：http://mv.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ty.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://ei.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://vw.nszjky.cn

[S03] C：读入整数
来源：http://zp.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://kd.gzmigu.cn

[S04] C：字符串复制
来源：http://wa.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wh.chemitech.net.cn

[S05] C：字符串长度
来源：http://pi.huixinmuqiang.cn

strlen(s)
来源：http://dx.yuexingan06.cn

[S06] C：字符串比较
来源：http://ik.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://hw.shxzskj.cn

[S07] C：数组遍历求和
来源：http://ie.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qc.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://tw.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ep.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://hw.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rn.bjjhwx.cn

[S10] C：指针与解引用
来源：http://sj.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://dt.muxihuayi.cn

[S11] C：逐行读文件
来源：http://ve.haigaiapp.cn

FILE *f = fopen("a.txt", "r");
来源：http://cp.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://po.colortex.cn

fclose(f);
来源：http://hj.haigaiapp.cn

[S12] C：写文件
来源：http://oc.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://to.chemitech.net.cn

[S13] C：宏定义
来源：http://an.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qg.hahajie.cn

[S14] C：枚举
来源：http://es.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://vp.gzmigu.cn

[S15] C：类型转换
来源：http://ek.yuexingan06.cn

(double) a / b
来源：http://lx.haigaiapp.cn

[S16] C：位操作置位
来源：http://qh.muxihuayi.cn

x |= (1 << 3);
来源：http://iz.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://cz.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vs.yuexingan06.cn

[S18] C：命令行参数
来源：http://fy.gzmigu.cn

int main(int argc, char **argv)
来源：http://cn.panjiajie.cn

[S19] C：快速排序
来源：http://qy.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sr.bjjhwx.cn

[S20] C：二分查找
来源：http://mw.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ng.panjiajie.cn

[S21] C：字符类别判断
来源：http://zg.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dh.lnxyls.cn

[S22] C：字符串转数字
来源：http://mk.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kx.shxzukj.cn

[S23] C：随机数
来源：http://qb.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fo.9csxet.cn

[S24] C：获取本地时间
来源：http://hg.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wu.nicolike.cn

[S25] C：内存拷贝
来源：http://js.jctech888.com.cn

memcpy(dst, src, n);
来源：http://wa.bjjhwx.cn

[S26] C：内存清零
来源：http://ci.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://iz.muxihuayi.cn

[S27] C：定义常量
来源：http://ru.wgjwhj.cn

const double PI = 3.14159;
来源：http://wy.chemitech.net.cn

[S28] C：静态变量
来源：http://dz.bjjhwx.cn

static int counter = 0;
来源：http://mw.521024.cn

[S29] C：变参函数
来源：http://zb.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://io.hahajie.cn

[S30] C：头文件保护
来源：http://pk.bjjhwx.cn

#ifndef X_H
来源：http://du.lnxyls.cn

#define X_H
来源：http://wh.gzmigu.cn

#endif
来源：http://il.colortex.cn

[S31] C++：Hello World
来源：http://fn.colortex.cn

#include <iostream>
来源：http://ks.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://jx.yuexingan06.cn

[S32] C++：字符串
来源：http://zr.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://sg.hahajie.cn

[S33] C++：vector 增删
来源：http://zg.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ri.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://nm.szxytkj.cn

for (auto &x : v) { std::cout << x; }
来源：http://wy.wgjwhj.cn

[S35] C++：map
来源：http://kj.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eb.huanxung.cn

[S36] C++：unordered_map
来源：http://ny.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ox.asd995.cn

[S37] C++：set
来源：http://np.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fm.nszjky.cn

[S38] C++：排序
来源：http://db.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://lz.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://wy.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ct.chemitech.net.cn

[S40] C++：查找元素
来源：http://ix.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://an.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://th.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zv.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://zf.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://hi.lnxyls.cn

[S43] C++：智能指针
来源：http://xs.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://kt.haigaiapp.cn

[S44] C++：引用传参
来源：http://ls.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://sd.colortex.cn

[S45] C++：lambda
来源：http://li.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hx.9csxet.cn

[S46] C++：函数模板
来源：http://cp.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dw.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://tu.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://as.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://le.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://aj.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://xw.nicolike.cn

[S49] C++：写文件
来源：http://tu.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yg.lnxyls.cn

[S50] C++：格式化数字
来源：http://bi.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sx.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://sm.shxzskj.cn

static_cast<double>(a) / b
来源：http://fh.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://qp.shxzukj.cn

int size() const noexcept { return n_; }
来源：http://bp.shxzukj.cn

[S53] C++：移动语义
来源：http://tq.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://ml.hnjuh.cn

[S54] C++：异常处理
来源：http://gc.yuntaijiaju.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sp.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://ms.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ep.gzmigu.cn

[S56] C++：optional
来源：http://dx.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kq.szxytkj.cn

[S57] C++：编译期常量
来源：http://om.jctech888.com.cn

constexpr int N = 10;
来源：http://mu.hahajie.cn

[S58] C++：命名空间
来源：http://cz.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://dl.haigaiapp.cn

[S59] C++：静态断言
来源：http://qy.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mx.huixinmuqiang.cn

[S60] C++：遍历并删除元素
来源：http://ef.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kh.szsharing.cn

================================================================================
来源：http://vy.haigaiapp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ad.wgjwhj.cn

================================================================================
来源：http://pd.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://on.gzmigu.cn

println("Hello")
来源：http://ju.panjiajie.cn

[T02] Kotlin：变量
来源：http://yv.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wp.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://tp.yuntaijiaju.cn

"值: $b"
来源：http://jr.gzmigu.cn

[T04] Kotlin：空安全
来源：http://we.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://er.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://vm.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bj.huanxung.cn

[T06] Kotlin：集合映射
来源：http://ym.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ai.huixiangedu.cn


<!-- 参考信息 -->