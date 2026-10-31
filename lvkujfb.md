代发 wailian999

set -euo pipefail
来源：http://qy.hnjuh.cn

[R02] 变量赋值与使用
来源：http://cb.nicolike.cn

name="Tom"; echo "$name"
来源：http://ej.hahajie.cn

[R03] 只读变量
来源：http://yj.bookmarksfly.cn

readonly PI=3.14
来源：http://hv.colortex.cn

[R04] 位置参数
来源：http://bb.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rg.shxzskj.cn

[R05] 参数默认值
来源：http://sm.newstarts.cn

name="${1:-default}"
来源：http://ew.newstarts.cn

[R06] 判断命令是否存在
来源：http://yu.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://np.gzmigu.cn

[R07] if 判断文件
来源：http://nc.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oc.colortex.cn

[R08] 数值比较
来源：http://bc.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xe.nszjky.cn

[R09] 字符串比较
来源：http://vt.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hu.chemitech.net.cn

[R10] 正则匹配
来源：http://oh.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gn.jctech888.com.cn

[R11] case 多分支
来源：http://zm.shxzskj.cn

case "$1" in
来源：http://iu.haigaiapp.cn

start) echo "启动" ;;
来源：http://fz.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://dy.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://gn.yuntaijiaju.cn

esac
来源：http://ba.shxzskj.cn

[R12] for 遍历文件
来源：http://xa.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://cv.colortex.cn

[R13] for 计数循环
来源：http://pp.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://qk.szsharing.cn

[R14] C 风格 for
来源：http://ji.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ls.hahajie.cn

[R15] while 逐行读文件
来源：http://sw.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jz.huixiangedu.cn

[R16] until 等待条件
来源：http://gi.521024.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mf.muxihuayi.cn

[R17] 数组定义与取值
来源：http://dw.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xs.wgjwhj.cn

[R18] 遍历数组
来源：http://yh.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oj.panjiajie.cn

[R19] 数组长度
来源：http://rt.hnjuh.cn

echo "${#arr[@]}"
来源：http://ba.lnxyls.cn

[R20] 关联数组（字典）
来源：http://en.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ag.shtwfgs.cn

[R21] 字符串长度
来源：http://fc.szsharing.cn

echo "${#s}"
来源：http://th.szxytkj.cn

[R22] 截取子串
来源：http://yu.colortex.cn

echo "${s:0:5}"
来源：http://tm.hahajie.cn

[R23] 字符串替换
来源：http://zt.lnxyls.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tj.lnxyls.cn

[R24] 大小写转换
来源：http://sz.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://oa.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://fd.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://os.colortex.cn

[R26] 命令替换
来源：http://jt.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://sj.huanxung.cn

[R27] 算术展开
来源：http://bs.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://ws.wgjwhj.cn

[R28] 浮点运算
来源：http://cr.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://fx.panjiajie.cn

[R29] 定义函数
来源：http://gs.bjjhwx.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vy.shxzskj.cn

[R30] 函数返回状态码
来源：http://lr.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://np.huanxung.cn

[R31] 局部变量
来源：http://al.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://ti.lnxyls.cn

[R32] 参数个数校验
来源：http://ms.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rb.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://rc.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mk.szxytkj.cn

[R34] 退出时清理
来源：http://gm.chemitech.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ej.szxytkj.cn

[R35] 后台执行并等待
来源：http://uw.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ct.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://rf.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ij.szsharing.cn

[R37] 把输出赋给变量
来源：http://je.yuntaijiaju.cn

files=$(ls -1)
来源：http://gc.shtwfgs.cn

[R38] 管道串联
来源：http://rf.huixiangedu.cn

cat a.txt | grep -i error | wc -l
来源：http://ol.colortex.cn

[R39] 重定向标准输出与错误
来源：http://nq.panjiajie.cn

cmd > out.log 2>&1
来源：http://xo.shxzukj.cn

[R40] 追加写日志
来源：http://wn.wgjwhj.cn

echo "log" >> out.log
来源：http://yt.wgjwhj.cn

[R41] 丢弃输出
来源：http://jj.521024.cn

cmd >/dev/null 2>&1
来源：http://wp.521024.cn

[R42] 输入重定向
来源：http://zo.huanxung.cn

wc -l < a.txt
来源：http://cq.nszjky.cn

[R43] 按名字查找文件
来源：http://xc.panjiajie.cn

find . -name "*.log" -type f
来源：http://df.521024.cn

[R44] 按修改时间查找
来源：http://an.huanxung.cn

find . -mtime -7 -type f
来源：http://gz.jianghongdianzi.cn

[R45] 批量删除
来源：http://nx.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://gk.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://rv.yuntaijiaju.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cr.shxzukj.cn

[R47] sed 单行替换
来源：http://yl.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xh.jctech888.com.cn

[R48] awk 取指定列
来源：http://vj.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://nz.chemitech.net.cn

[R49] awk 带条件
来源：http://lz.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://as.shxzukj.cn

[R50] awk 求和
来源：http://no.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gg.panjiajie.cn

[R51] 排序去重取前几
来源：http://xy.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ho.yuexingan06.cn

[R52] 统计行数
来源：http://zh.panjiajie.cn

wc -l a.txt
来源：http://ak.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://ec.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hg.haigaiapp.cn

[R54] 比较两个文件
来源：http://le.huixiangedu.cn

diff a.txt b.txt
来源：http://fn.shxzskj.cn

[R55] 压缩与解压
来源：http://xz.jctech888.com.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ps.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://yo.haigaiapp.cn

scp file user@host:/path/
来源：http://wo.panjiajie.cn

[R57] 远程执行命令
来源：http://wb.jctech888.com.cn

ssh user@host 'uptime'
来源：http://sr.panjiajie.cn

[R58] 下载文件
来源：http://xm.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cx.muxihuayi.cn

[R59] 发 POST JSON
来源：http://eu.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ck.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://sx.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yt.szxytkj.cn

[R61] 磁盘占用
来源：http://ko.huanxung.cn

df -h;  du -sh *
来源：http://uk.panjiajie.cn

[R62] 找最占空间的文件
来源：http://zi.jctech888.com.cn

du -ah . | sort -rh | head -10
来源：http://fl.colortex.cn

[R63] 内存与进程
来源：http://dd.panjiajie.cn

free -h;  ps aux | grep nginx
来源：http://kl.colortex.cn

[R64] 结束进程
来源：http://cj.lnxyls.cn

kill -9 $(pgrep -f app.py)
来源：http://nm.bookmarksfly.cn

[R65] 查看端口占用
来源：http://mu.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ks.bjjhwx.cn

[R66] 定时任务
来源：http://mj.muxihuayi.cn

crontab -e;  crontab -l
来源：http://qx.colortex.cn

[R67] 生成随机十六进制串
来源：http://tw.521024.cn

openssl rand -hex 16
来源：http://gk.szxytkj.cn

[R68] 计算文件校验值
来源：http://to.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://we.gzmigu.cn

[R69] 生成随机密码
来源：http://ye.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://sx.bjjhwx.cn

[R70] 时间戳与互转
来源：http://fe.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://ej.nszjky.cn

[R71] 日期格式化
来源：http://na.nszjky.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cl.9csxet.cn

[R72] 等待端口就绪
来源：http://qk.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jd.521024.cn

[R73] 分割大日志
来源：http://re.bjjhwx.cn

split -l 1000 big.log part_
来源：http://vi.szxytkj.cn

[R74] 批量重命名
来源：http://jr.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ua.lnxyls.cn

[R75] 导出环境变量
来源：http://zh.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://hr.9csxet.cn

[R76] 使用临时文件
来源：http://xm.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pd.colortex.cn

[R77] 读取用户输入
来源：http://om.haigaiapp.cn

read -rp "请输入: " ans
来源：http://rr.hnjuh.cn

[R78] 交互式菜单
来源：http://tf.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zv.muxihuayi.cn

[R79] 解析命令行选项
来源：http://lk.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fi.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://ef.yuexingan06.cn

time ./run.sh
来源：http://wb.521024.cn

================================================================================
来源：http://no.shxzskj.cn

S. C / C++ 专题
来源：http://gf.bookmarksfly.cn

================================================================================
来源：http://tr.szxytkj.cn

[S01] C：Hello World
来源：http://jh.huixiangedu.cn

#include <stdio.h>
来源：http://aa.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xh.newstarts.cn

[S02] C：变量与格式化输出
来源：http://yb.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://es.hahajie.cn

[S03] C：读入整数
来源：http://dg.colortex.cn

int x; scanf("%d", &x);
来源：http://wy.bookmarksfly.cn

[S04] C：字符串复制
来源：http://xm.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dq.huanxung.cn

[S05] C：字符串长度
来源：http://qf.szsharing.cn

strlen(s)
来源：http://mo.newstarts.cn

[S06] C：字符串比较
来源：http://tv.shxzskj.cn

strcmp(a, b) == 0
来源：http://da.jctech888.com.cn

[S07] C：数组遍历求和
来源：http://fs.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mv.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://aj.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fm.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://wn.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pr.szxytkj.cn

[S10] C：指针与解引用
来源：http://ov.nszjky.cn

int *p = &a;  *p = 5;
来源：http://pq.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://ag.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://lu.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vg.hnjuh.cn

fclose(f);
来源：http://ho.haigaiapp.cn

[S12] C：写文件
来源：http://oc.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yq.gzmigu.cn

[S13] C：宏定义
来源：http://xg.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bm.hahajie.cn

[S14] C：枚举
来源：http://yy.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://xu.521024.cn

[S15] C：类型转换
来源：http://vd.muxihuayi.cn

(double) a / b
来源：http://pm.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://uj.newstarts.cn

x |= (1 << 3);
来源：http://mv.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://cu.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gd.jctech888.com.cn

[S18] C：命令行参数
来源：http://cu.huixiangedu.cn

int main(int argc, char **argv)
来源：http://by.panjiajie.cn

[S19] C：快速排序
来源：http://pb.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iu.shxzukj.cn

[S20] C：二分查找
来源：http://pd.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pb.bookmarksfly.cn

[S21] C：字符类别判断
来源：http://gm.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ah.wgjwhj.cn

[S22] C：字符串转数字
来源：http://na.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://el.shxzukj.cn

[S23] C：随机数
来源：http://hp.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nv.yuexingan06.cn

[S24] C：获取本地时间
来源：http://jr.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jb.shtwfgs.cn

[S25] C：内存拷贝
来源：http://kg.huixiangedu.cn

memcpy(dst, src, n);
来源：http://yw.yuntaijiaju.cn

[S26] C：内存清零
来源：http://sx.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://us.shxzskj.cn

[S27] C：定义常量
来源：http://lt.muxihuayi.cn

const double PI = 3.14159;
来源：http://om.huixinmuqiang.cn

[S28] C：静态变量
来源：http://du.asd995.cn

static int counter = 0;
来源：http://yk.bookmarksfly.cn

[S29] C：变参函数
来源：http://po.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bn.jctech888.com.cn

[S30] C：头文件保护
来源：http://kj.shxzskj.cn

#ifndef X_H
来源：http://xo.shtwfgs.cn

#define X_H
来源：http://mf.nicolike.cn

#endif
来源：http://ep.haigaiapp.cn

[S31] C++：Hello World
来源：http://hf.huixiangedu.cn

#include <iostream>
来源：http://do.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://ud.huanxung.cn

[S32] C++：字符串
来源：http://es.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://to.huanxung.cn

[S33] C++：vector 增删
来源：http://au.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wn.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://jc.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://zi.hahajie.cn

[S35] C++：map
来源：http://xa.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aq.jctech888.com.cn

[S36] C++：unordered_map
来源：http://qe.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ca.shxzukj.cn

[S37] C++：set
来源：http://un.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bn.nicolike.cn

[S38] C++：排序
来源：http://kt.colortex.cn

std::sort(v.begin(), v.end());
来源：http://dl.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://uz.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uz.9csxet.cn

[S40] C++：查找元素
来源：http://vm.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jv.hahajie.cn

[S41] C++：类与构造函数
来源：http://iy.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://my.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://nk.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://di.bookmarksfly.cn

[S43] C++：智能指针
来源：http://fe.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://ud.huixiangedu.cn

[S44] C++：引用传参
来源：http://gt.nicolike.cn

void inc(int &x) { ++x; }
来源：http://zo.panjiajie.cn

[S45] C++：lambda
来源：http://ms.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hc.huixiangedu.cn

[S46] C++：函数模板
来源：http://hp.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xg.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://vu.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pb.nicolike.cn

[S48] C++：逐行读文件
来源：http://ty.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gn.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://cu.asd995.cn

[S49] C++：写文件
来源：http://fu.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jf.lnxyls.cn

[S50] C++：格式化数字
来源：http://ei.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sz.shxzskj.cn

[S51] C++：显式类型转换
来源：http://rv.nszjky.cn

static_cast<double>(a) / b
来源：http://af.521024.cn

[S52] C++：const 与 noexcept
来源：http://ch.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://bi.colortex.cn

[S53] C++：移动语义
来源：http://ce.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://lw.wgjwhj.cn

[S54] C++：异常处理
来源：http://yk.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cw.lnxyls.cn

[S55] C++：结构化绑定
来源：http://sl.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hp.shxzukj.cn

[S56] C++：optional
来源：http://bh.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rd.jctech888.com.cn

[S57] C++：编译期常量
来源：http://hh.jianghongdianzi.cn

constexpr int N = 10;
来源：http://nq.muxihuayi.cn

[S58] C++：命名空间
来源：http://wb.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://rg.wgjwhj.cn

[S59] C++：静态断言
来源：http://uv.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zx.colortex.cn

[S60] C++：遍历并删除元素
来源：http://vd.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yw.shxzukj.cn

================================================================================
来源：http://nd.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mk.colortex.cn

================================================================================
来源：http://ow.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://sz.shxzskj.cn

println("Hello")
来源：http://cr.shxzskj.cn

[T02] Kotlin：变量
来源：http://ce.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qx.gzmigu.cn


<!-- 参考信息 -->