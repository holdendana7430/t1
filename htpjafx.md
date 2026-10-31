代发 wailian999

readonly PI=3.14
来源：http://mz.nicolike.cn

[R04] 位置参数
来源：http://df.bjjhwx.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oy.chemitech.net.cn

[R05] 参数默认值
来源：http://ct.szsharing.cn

name="${1:-default}"
来源：http://yi.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://fh.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qk.huanxung.cn

[R07] if 判断文件
来源：http://mc.nszjky.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ej.hahajie.cn

[R08] 数值比较
来源：http://fs.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ba.lnxyls.cn

[R09] 字符串比较
来源：http://yb.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yq.bjjhwx.cn

[R10] 正则匹配
来源：http://sz.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uo.hahajie.cn

[R11] case 多分支
来源：http://rb.bookmarksfly.cn

case "$1" in
来源：http://wu.yuexingan06.cn

start) echo "启动" ;;
来源：http://zf.panjiajie.cn

stop)  echo "停止" ;;
来源：http://bf.shtwfgs.cn

*)     echo "未知命令" ;;
来源：http://fj.huanxung.cn

esac
来源：http://uz.bookmarksfly.cn

[R12] for 遍历文件
来源：http://vv.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://yk.lnxyls.cn

[R13] for 计数循环
来源：http://an.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://ch.szsharing.cn

[R14] C 风格 for
来源：http://mo.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rf.panjiajie.cn

[R15] while 逐行读文件
来源：http://yk.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://in.yuntaijiaju.cn

[R16] until 等待条件
来源：http://no.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mx.bjjhwx.cn

[R17] 数组定义与取值
来源：http://df.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dr.shxzskj.cn

[R18] 遍历数组
来源：http://se.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ox.jctech888.com.cn

[R19] 数组长度
来源：http://mb.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://ic.newstarts.cn

[R20] 关联数组（字典）
来源：http://mn.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rj.521024.cn

[R21] 字符串长度
来源：http://ze.nszjky.cn

echo "${#s}"
来源：http://av.jianghongdianzi.cn

[R22] 截取子串
来源：http://lx.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://pf.yuntaijiaju.cn

[R23] 字符串替换
来源：http://fs.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xk.9csxet.cn

[R24] 大小写转换
来源：http://bs.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://be.szxytkj.cn

[R25] 去后缀 / 去前缀
来源：http://qe.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qk.newstarts.cn

[R26] 命令替换
来源：http://qs.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://bg.huixiangedu.cn

[R27] 算术展开
来源：http://ut.huanxung.cn

echo $((1 + 2 * 3))
来源：http://ih.jctech888.com.cn

[R28] 浮点运算
来源：http://wg.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://ab.gzmigu.cn

[R29] 定义函数
来源：http://sq.yuexingan06.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pe.shxzukj.cn

[R30] 函数返回状态码
来源：http://kr.newstarts.cn

f() { return 0; }; f || echo "失败了"
来源：http://dy.newstarts.cn

[R31] 局部变量
来源：http://aa.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://bj.hnjuh.cn

[R32] 参数个数校验
来源：http://bq.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cw.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://gk.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sa.newstarts.cn

[R34] 退出时清理
来源：http://ox.chemitech.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vv.chemitech.net.cn

[R35] 后台执行并等待
来源：http://av.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lg.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://rr.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qn.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://yk.haigaiapp.cn

files=$(ls -1)
来源：http://au.chemitech.net.cn

[R38] 管道串联
来源：http://ob.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://sk.yuexingan06.cn

[R39] 重定向标准输出与错误
来源：http://ih.bjjhwx.cn

cmd > out.log 2>&1
来源：http://mi.wgjwhj.cn

[R40] 追加写日志
来源：http://iz.szxytkj.cn

echo "log" >> out.log
来源：http://gs.haigaiapp.cn

[R41] 丢弃输出
来源：http://rb.jctech888.com.cn

cmd >/dev/null 2>&1
来源：http://ev.huixiangedu.cn

[R42] 输入重定向
来源：http://tk.gzmigu.cn

wc -l < a.txt
来源：http://nr.szxytkj.cn

[R43] 按名字查找文件
来源：http://oa.lnxyls.cn

find . -name "*.log" -type f
来源：http://sp.gzmigu.cn

[R44] 按修改时间查找
来源：http://ns.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://sr.haigaiapp.cn

[R45] 批量删除
来源：http://tz.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://zi.yuntaijiaju.cn

[R46] 递归替换文件内容
来源：http://jv.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://je.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://ws.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bn.bjjhwx.cn

[R48] awk 取指定列
来源：http://fw.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://so.yuexingan06.cn

[R49] awk 带条件
来源：http://wv.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ih.hahajie.cn

[R50] awk 求和
来源：http://xe.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://js.szxytkj.cn

[R51] 排序去重取前几
来源：http://eu.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ta.newstarts.cn

[R52] 统计行数
来源：http://tq.shxzukj.cn

wc -l a.txt
来源：http://jt.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://gx.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hg.521024.cn

[R54] 比较两个文件
来源：http://pp.huixinmuqiang.cn

diff a.txt b.txt
来源：http://nh.hnjuh.cn

[R55] 压缩与解压
来源：http://tz.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uc.nicolike.cn

[R56] 远程拷贝
来源：http://ym.chemitech.net.cn

scp file user@host:/path/
来源：http://vq.nicolike.cn

[R57] 远程执行命令
来源：http://kd.lnxyls.cn

ssh user@host 'uptime'
来源：http://cq.newstarts.cn

[R58] 下载文件
来源：http://ty.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zf.jctech888.com.cn

[R59] 发 POST JSON
来源：http://bw.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ny.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://zq.huanxung.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zd.szxytkj.cn

[R61] 磁盘占用
来源：http://nj.bjjhwx.cn

df -h;  du -sh *
来源：http://ks.huixinmuqiang.cn

[R62] 找最占空间的文件
来源：http://uy.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://cu.nszjky.cn

[R63] 内存与进程
来源：http://ie.521024.cn

free -h;  ps aux | grep nginx
来源：http://ol.hahajie.cn

[R64] 结束进程
来源：http://me.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://pg.panjiajie.cn

[R65] 查看端口占用
来源：http://bo.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wi.huixinmuqiang.cn

[R66] 定时任务
来源：http://xk.hahajie.cn

crontab -e;  crontab -l
来源：http://qd.jctech888.com.cn

[R67] 生成随机十六进制串
来源：http://qs.nicolike.cn

openssl rand -hex 16
来源：http://tj.shxzukj.cn

[R68] 计算文件校验值
来源：http://gv.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cp.nicolike.cn

[R69] 生成随机密码
来源：http://yw.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://ti.asd995.cn

[R70] 时间戳与互转
来源：http://fy.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://df.huixiangedu.cn

[R71] 日期格式化
来源：http://oy.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ai.szxytkj.cn

[R72] 等待端口就绪
来源：http://dy.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wo.gzmigu.cn

[R73] 分割大日志
来源：http://df.lnxyls.cn

split -l 1000 big.log part_
来源：http://du.9csxet.cn

[R74] 批量重命名
来源：http://vq.gzmigu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ut.lnxyls.cn

[R75] 导出环境变量
来源：http://on.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://vd.hahajie.cn

[R76] 使用临时文件
来源：http://ue.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://po.szxytkj.cn

[R77] 读取用户输入
来源：http://kt.huixiangedu.cn

read -rp "请输入: " ans
来源：http://eu.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://jj.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qp.jctech888.com.cn

[R79] 解析命令行选项
来源：http://fg.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://as.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://dv.asd995.cn

time ./run.sh
来源：http://oc.muxihuayi.cn

================================================================================
来源：http://fp.wgjwhj.cn

S. C / C++ 专题
来源：http://bb.panjiajie.cn

================================================================================
来源：http://ey.szsharing.cn

[S01] C：Hello World
来源：http://jt.lnxyls.cn

#include <stdio.h>
来源：http://xi.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yg.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://cj.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://yf.panjiajie.cn

[S03] C：读入整数
来源：http://br.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://jc.hnjuh.cn

[S04] C：字符串复制
来源：http://kz.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zy.haigaiapp.cn

[S05] C：字符串长度
来源：http://ne.jctech888.com.cn

strlen(s)
来源：http://mv.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://jt.shxzskj.cn

strcmp(a, b) == 0
来源：http://gh.bookmarksfly.cn

[S07] C：数组遍历求和
来源：http://hd.521024.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bp.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://dt.chemitech.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ui.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://bq.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qi.szsharing.cn

[S10] C：指针与解引用
来源：http://rb.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://zw.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://dx.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://pc.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://oz.jctech888.com.cn

fclose(f);
来源：http://mb.shxzukj.cn

[S12] C：写文件
来源：http://py.hnjuh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pp.asd995.cn

[S13] C：宏定义
来源：http://iw.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hs.muxihuayi.cn

[S14] C：枚举
来源：http://qo.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://tz.hnjuh.cn

[S15] C：类型转换
来源：http://yi.hnjuh.cn

(double) a / b
来源：http://lb.521024.cn

[S16] C：位操作置位
来源：http://jz.bjjhwx.cn

x |= (1 << 3);
来源：http://de.szsharing.cn

[S17] C：安全拼接字符串
来源：http://hy.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lh.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://as.szxytkj.cn

int main(int argc, char **argv)
来源：http://hk.shxzukj.cn

[S19] C：快速排序
来源：http://zv.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xv.haigaiapp.cn

[S20] C：二分查找
来源：http://co.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://an.muxihuayi.cn

[S21] C：字符类别判断
来源：http://ij.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://si.haigaiapp.cn

[S22] C：字符串转数字
来源：http://sq.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wh.colortex.cn

[S23] C：随机数
来源：http://vd.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ip.newstarts.cn

[S24] C：获取本地时间
来源：http://ce.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ds.huanxung.cn

[S25] C：内存拷贝
来源：http://mi.nicolike.cn

memcpy(dst, src, n);
来源：http://ou.wgjwhj.cn

[S26] C：内存清零
来源：http://ob.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://ev.521024.cn

[S27] C：定义常量
来源：http://lb.panjiajie.cn

const double PI = 3.14159;
来源：http://ia.huanxung.cn

[S28] C：静态变量
来源：http://vt.bjjhwx.cn

static int counter = 0;
来源：http://bc.shxzukj.cn

[S29] C：变参函数
来源：http://xr.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lj.wgjwhj.cn

[S30] C：头文件保护
来源：http://ai.szsharing.cn

#ifndef X_H
来源：http://vn.huanxung.cn

#define X_H
来源：http://bl.huixiangedu.cn

#endif
来源：http://vp.hahajie.cn

[S31] C++：Hello World
来源：http://lk.huixinmuqiang.cn

#include <iostream>
来源：http://iq.huixiangedu.cn

int main() { std::cout << "Hello\n"; }
来源：http://yp.huixiangedu.cn

[S32] C++：字符串
来源：http://ja.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://sh.yuexingan06.cn

[S33] C++：vector 增删
来源：http://hz.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yv.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://gt.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://cd.huixinmuqiang.cn

[S35] C++：map
来源：http://wd.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ow.jctech888.com.cn

[S36] C++：unordered_map
来源：http://kk.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sn.newstarts.cn

[S37] C++：set
来源：http://hf.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ki.huixiangedu.cn

[S38] C++：排序
来源：http://jk.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://vm.521024.cn

[S39] C++：自定义比较器排序
来源：http://cg.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fz.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://xv.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tt.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://yn.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xz.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://sx.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://dr.shxzukj.cn

[S43] C++：智能指针
来源：http://jd.521024.cn

auto p = std::make_unique<int>(5);
来源：http://kz.hnjuh.cn

[S44] C++：引用传参
来源：http://jf.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://af.gzmigu.cn

[S45] C++：lambda
来源：http://wy.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dd.colortex.cn

[S46] C++：函数模板
来源：http://yz.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ln.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://rb.huanxung.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://et.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://jx.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wd.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://ko.hahajie.cn

[S49] C++：写文件
来源：http://dx.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oz.wgjwhj.cn

[S50] C++：格式化数字
来源：http://hj.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kp.gzmigu.cn

[S51] C++：显式类型转换
来源：http://qz.521024.cn

static_cast<double>(a) / b
来源：http://lp.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://ik.asd995.cn

int size() const noexcept { return n_; }
来源：http://eo.chemitech.net.cn

[S53] C++：移动语义
来源：http://yt.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://br.bjjhwx.cn

[S54] C++：异常处理
来源：http://ds.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jw.shxzukj.cn

[S55] C++：结构化绑定
来源：http://lm.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cj.chemitech.net.cn

[S56] C++：optional
来源：http://ag.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gi.colortex.cn

[S57] C++：编译期常量
来源：http://oo.9csxet.cn

constexpr int N = 10;
来源：http://js.hnjuh.cn

[S58] C++：命名空间
来源：http://xj.haigaiapp.cn

namespace ns { int f() { return 1; } }
来源：http://ht.yuntaijiaju.cn

[S59] C++：静态断言
来源：http://kt.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uh.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://pq.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eq.muxihuayi.cn

================================================================================
来源：http://ot.jctech888.com.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://db.yuexingan06.cn

================================================================================
来源：http://pu.newstarts.cn

[T01] Kotlin：Hello World
来源：http://lr.hahajie.cn

println("Hello")
来源：http://ct.haigaiapp.cn

[T02] Kotlin：变量
来源：http://jl.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gi.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://wa.yuexingan06.cn

"值: $b"
来源：http://ge.newstarts.cn

[T04] Kotlin：空安全
来源：http://nz.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://ri.yuexingan06.cn


<!-- 参考信息 -->