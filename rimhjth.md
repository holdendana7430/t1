代发 wailian999

set -euo pipefail
来源：http://oq.jianghongdianzi.cn

[R02] 变量赋值与使用
来源：http://dk.bjjhwx.cn

name="Tom"; echo "$name"
来源：http://dr.gzmigu.cn

[R03] 只读变量
来源：http://fg.haigaiapp.cn

readonly PI=3.14
来源：http://dc.panjiajie.cn

[R04] 位置参数
来源：http://mp.chemitech.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rr.yuntaijiaju.cn

[R05] 参数默认值
来源：http://vp.huanxung.cn

name="${1:-default}"
来源：http://br.asd995.cn

[R06] 判断命令是否存在
来源：http://gj.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ir.521024.cn

[R07] if 判断文件
来源：http://ck.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vj.szsharing.cn

[R08] 数值比较
来源：http://ps.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ba.nszjky.cn

[R09] 字符串比较
来源：http://gj.lnxyls.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sp.szxytkj.cn

[R10] 正则匹配
来源：http://ra.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://on.jianghongdianzi.cn

[R11] case 多分支
来源：http://mn.bookmarksfly.cn

case "$1" in
来源：http://cf.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://jv.shxzskj.cn

stop)  echo "停止" ;;
来源：http://vr.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://si.huanxung.cn

esac
来源：http://eo.bookmarksfly.cn

[R12] for 遍历文件
来源：http://pd.newstarts.cn

for f in *.txt; do echo "$f"; done
来源：http://tr.jctech888.com.cn

[R13] for 计数循环
来源：http://kh.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://gi.shxzskj.cn

[R14] C 风格 for
来源：http://gt.huanxung.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mf.shtwfgs.cn

[R15] while 逐行读文件
来源：http://nd.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bc.szsharing.cn

[R16] until 等待条件
来源：http://ef.521024.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://un.9csxet.cn

[R17] 数组定义与取值
来源：http://lg.shtwfgs.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zx.gzmigu.cn

[R18] 遍历数组
来源：http://qj.huixiangedu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hg.yuexingan06.cn

[R19] 数组长度
来源：http://wx.shxzukj.cn

echo "${#arr[@]}"
来源：http://jw.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://px.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ng.hnjuh.cn

[R21] 字符串长度
来源：http://kg.jctech888.com.cn

echo "${#s}"
来源：http://hk.szsharing.cn

[R22] 截取子串
来源：http://gh.521024.cn

echo "${s:0:5}"
来源：http://wd.shxzukj.cn

[R23] 字符串替换
来源：http://xw.chemitech.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mf.newstarts.cn

[R24] 大小写转换
来源：http://rj.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sh.bjjhwx.cn

[R25] 去后缀 / 去前缀
来源：http://ff.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ta.shtwfgs.cn

[R26] 命令替换
来源：http://ib.yuntaijiaju.cn

now=$(date +%F); echo "$now"
来源：http://pk.jctech888.com.cn

[R27] 算术展开
来源：http://dw.yuntaijiaju.cn

echo $((1 + 2 * 3))
来源：http://ih.muxihuayi.cn

[R28] 浮点运算
来源：http://mz.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://ny.panjiajie.cn

[R29] 定义函数
来源：http://oh.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vi.chemitech.net.cn

[R30] 函数返回状态码
来源：http://dk.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://mj.shtwfgs.cn

[R31] 局部变量
来源：http://kp.shxzukj.cn

f() { local x=1; echo "$x"; }
来源：http://sl.hnjuh.cn

[R32] 参数个数校验
来源：http://nm.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yf.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://hd.gzmigu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kl.gzmigu.cn

[R34] 退出时清理
来源：http://mz.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zx.9csxet.cn

[R35] 后台执行并等待
来源：http://bl.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fg.nszjky.cn

[R36] 并发执行多个任务
来源：http://aj.shxzukj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://em.9csxet.cn

[R37] 把输出赋给变量
来源：http://ei.shtwfgs.cn

files=$(ls -1)
来源：http://go.huixinmuqiang.cn

[R38] 管道串联
来源：http://re.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://wh.panjiajie.cn

[R39] 重定向标准输出与错误
来源：http://ji.asd995.cn

cmd > out.log 2>&1
来源：http://sk.521024.cn

[R40] 追加写日志
来源：http://rk.nszjky.cn

echo "log" >> out.log
来源：http://vj.shtwfgs.cn

[R41] 丢弃输出
来源：http://ru.9csxet.cn

cmd >/dev/null 2>&1
来源：http://pd.shxzskj.cn

[R42] 输入重定向
来源：http://qi.nszjky.cn

wc -l < a.txt
来源：http://wq.shxzukj.cn

[R43] 按名字查找文件
来源：http://yt.hahajie.cn

find . -name "*.log" -type f
来源：http://bc.nicolike.cn

[R44] 按修改时间查找
来源：http://jv.huanxung.cn

find . -mtime -7 -type f
来源：http://ue.huanxung.cn

[R45] 批量删除
来源：http://tp.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://hg.shxzukj.cn

[R46] 递归替换文件内容
来源：http://jn.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dq.lnxyls.cn

[R47] sed 单行替换
来源：http://wp.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yu.bookmarksfly.cn

[R48] awk 取指定列
来源：http://cw.hahajie.cn

awk '{print $1, $3}' a.txt
来源：http://dh.haigaiapp.cn

[R49] awk 带条件
来源：http://ad.shxzskj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ll.huixinmuqiang.cn

[R50] awk 求和
来源：http://ke.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cc.lnxyls.cn

[R51] 排序去重取前几
来源：http://ue.yuexingan06.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jn.nszjky.cn

[R52] 统计行数
来源：http://jx.muxihuayi.cn

wc -l a.txt
来源：http://zc.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://vb.shxzskj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fw.huanxung.cn

[R54] 比较两个文件
来源：http://ac.haigaiapp.cn

diff a.txt b.txt
来源：http://jh.chemitech.net.cn

[R55] 压缩与解压
来源：http://oq.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tp.bookmarksfly.cn

[R56] 远程拷贝
来源：http://yf.shtwfgs.cn

scp file user@host:/path/
来源：http://mb.lnxyls.cn

[R57] 远程执行命令
来源：http://tn.yuntaijiaju.cn

ssh user@host 'uptime'
来源：http://ps.nszjky.cn

[R58] 下载文件
来源：http://jk.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://we.yuexingan06.cn

[R59] 发 POST JSON
来源：http://vh.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qg.jianghongdianzi.cn

[R60] 只看 HTTP 状态码
来源：http://gr.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sz.hnjuh.cn

[R61] 磁盘占用
来源：http://dh.asd995.cn

df -h;  du -sh *
来源：http://kt.shxzukj.cn

[R62] 找最占空间的文件
来源：http://hg.521024.cn

du -ah . | sort -rh | head -10
来源：http://rl.szxytkj.cn

[R63] 内存与进程
来源：http://aw.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://ju.colortex.cn

[R64] 结束进程
来源：http://ih.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://qi.haigaiapp.cn

[R65] 查看端口占用
来源：http://jr.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tr.bjjhwx.cn

[R66] 定时任务
来源：http://st.hahajie.cn

crontab -e;  crontab -l
来源：http://zv.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://hp.wgjwhj.cn

openssl rand -hex 16
来源：http://qv.muxihuayi.cn

[R68] 计算文件校验值
来源：http://ij.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jt.hahajie.cn

[R69] 生成随机密码
来源：http://mx.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://ze.muxihuayi.cn

[R70] 时间戳与互转
来源：http://iu.colortex.cn

date +%s;  date -d @1700000000
来源：http://sz.yuexingan06.cn

[R71] 日期格式化
来源：http://gq.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bz.haigaiapp.cn

[R72] 等待端口就绪
来源：http://me.yuexingan06.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ao.nicolike.cn

[R73] 分割大日志
来源：http://fy.newstarts.cn

split -l 1000 big.log part_
来源：http://dr.wgjwhj.cn

[R74] 批量重命名
来源：http://ma.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pf.huanxung.cn

[R75] 导出环境变量
来源：http://lf.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://sx.shxzskj.cn

[R76] 使用临时文件
来源：http://fj.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nf.haigaiapp.cn

[R77] 读取用户输入
来源：http://mw.bjjhwx.cn

read -rp "请输入: " ans
来源：http://nt.jctech888.com.cn

[R78] 交互式菜单
来源：http://ry.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ii.9csxet.cn

[R79] 解析命令行选项
来源：http://xx.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qe.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://dr.colortex.cn

time ./run.sh
来源：http://ih.9csxet.cn

================================================================================
来源：http://sc.chemitech.net.cn

S. C / C++ 专题
来源：http://aw.yuntaijiaju.cn

================================================================================
来源：http://ys.jianghongdianzi.cn

[S01] C：Hello World
来源：http://ax.wgjwhj.cn

#include <stdio.h>
来源：http://wb.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hx.asd995.cn

[S02] C：变量与格式化输出
来源：http://fg.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://vr.jianghongdianzi.cn

[S03] C：读入整数
来源：http://ok.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://sg.lnxyls.cn

[S04] C：字符串复制
来源：http://bv.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cm.huanxung.cn

[S05] C：字符串长度
来源：http://pk.hahajie.cn

strlen(s)
来源：http://vk.huixiangedu.cn

[S06] C：字符串比较
来源：http://lx.shxzskj.cn

strcmp(a, b) == 0
来源：http://dc.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://il.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://es.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://tx.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ua.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://ku.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gh.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://ux.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://qt.haigaiapp.cn

[S11] C：逐行读文件
来源：http://cm.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://yt.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qi.szsharing.cn

fclose(f);
来源：http://fn.wgjwhj.cn

[S12] C：写文件
来源：http://rc.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cp.jctech888.com.cn

[S13] C：宏定义
来源：http://qo.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pv.huixiangedu.cn

[S14] C：枚举
来源：http://sv.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://nh.shxzukj.cn

[S15] C：类型转换
来源：http://zu.huanxung.cn

(double) a / b
来源：http://zb.szxytkj.cn

[S16] C：位操作置位
来源：http://rd.chemitech.net.cn

x |= (1 << 3);
来源：http://oy.nicolike.cn

[S17] C：安全拼接字符串
来源：http://ub.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rd.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://zs.shxzukj.cn

int main(int argc, char **argv)
来源：http://bi.bjjhwx.cn

[S19] C：快速排序
来源：http://ia.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nr.9csxet.cn

[S20] C：二分查找
来源：http://cf.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ig.huanxung.cn

[S21] C：字符类别判断
来源：http://ng.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yg.hahajie.cn

[S22] C：字符串转数字
来源：http://sj.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ab.bookmarksfly.cn

[S23] C：随机数
来源：http://ci.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wy.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://hu.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mb.shtwfgs.cn

[S25] C：内存拷贝
来源：http://cg.colortex.cn

memcpy(dst, src, n);
来源：http://ls.bookmarksfly.cn

[S26] C：内存清零
来源：http://ku.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://vx.hnjuh.cn

[S27] C：定义常量
来源：http://tu.wgjwhj.cn

const double PI = 3.14159;
来源：http://ar.szxytkj.cn

[S28] C：静态变量
来源：http://tf.haigaiapp.cn

static int counter = 0;
来源：http://ts.jianghongdianzi.cn

[S29] C：变参函数
来源：http://nd.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ut.nicolike.cn

[S30] C：头文件保护
来源：http://mh.521024.cn

#ifndef X_H
来源：http://ac.bjjhwx.cn

#define X_H
来源：http://un.bookmarksfly.cn

#endif
来源：http://cj.szxytkj.cn

[S31] C++：Hello World
来源：http://eo.chemitech.net.cn

#include <iostream>
来源：http://cz.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://rd.panjiajie.cn

[S32] C++：字符串
来源：http://py.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://pd.bjjhwx.cn

[S33] C++：vector 增删
来源：http://ki.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://to.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://mu.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://kl.haigaiapp.cn

[S35] C++：map
来源：http://yh.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vs.haigaiapp.cn

[S36] C++：unordered_map
来源：http://mj.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://il.huixinmuqiang.cn

[S37] C++：set
来源：http://yb.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ui.jianghongdianzi.cn

[S38] C++：排序
来源：http://or.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://xs.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://ci.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jc.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://sy.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zw.shxzskj.cn

[S41] C++：类与构造函数
来源：http://xh.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xk.colortex.cn

[S42] C++：继承与虚函数
来源：http://vd.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://cq.521024.cn

[S43] C++：智能指针
来源：http://dp.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://zb.newstarts.cn

[S44] C++：引用传参
来源：http://is.newstarts.cn

void inc(int &x) { ++x; }
来源：http://ly.gzmigu.cn

[S45] C++：lambda
来源：http://jp.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gp.huixiangedu.cn

[S46] C++：函数模板
来源：http://zz.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mh.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://jy.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fh.9csxet.cn

[S48] C++：逐行读文件
来源：http://tq.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qr.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://ll.hahajie.cn

[S49] C++：写文件
来源：http://aw.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cw.shxzskj.cn

[S50] C++：格式化数字
来源：http://qi.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ci.nszjky.cn

[S51] C++：显式类型转换
来源：http://wj.gzmigu.cn

static_cast<double>(a) / b
来源：http://yx.newstarts.cn

[S52] C++：const 与 noexcept
来源：http://rr.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://fs.szxytkj.cn

[S53] C++：移动语义
来源：http://fw.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://rp.szsharing.cn

[S54] C++：异常处理
来源：http://vr.chemitech.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qg.9csxet.cn

[S55] C++：结构化绑定
来源：http://pc.muxihuayi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ng.nszjky.cn

[S56] C++：optional
来源：http://zo.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qe.huanxung.cn

[S57] C++：编译期常量
来源：http://cm.newstarts.cn

constexpr int N = 10;
来源：http://bn.newstarts.cn

[S58] C++：命名空间
来源：http://lh.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://se.chemitech.net.cn

[S59] C++：静态断言
来源：http://cn.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rs.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://bf.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nr.yuntaijiaju.cn

================================================================================
来源：http://hy.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://az.chemitech.net.cn

================================================================================
来源：http://um.nicolike.cn

[T01] Kotlin：Hello World
来源：http://ym.jianghongdianzi.cn

println("Hello")
来源：http://vw.nicolike.cn

[T02] Kotlin：变量
来源：http://kc.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ww.huanxung.cn


<!-- 参考信息 -->