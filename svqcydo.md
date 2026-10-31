代发 wailian999

set -euo pipefail
来源：http://va.shxzskj.cn

[R02] 变量赋值与使用
来源：http://yh.bjjhwx.cn

name="Tom"; echo "$name"
来源：http://on.huanxung.cn

[R03] 只读变量
来源：http://sw.hahajie.cn

readonly PI=3.14
来源：http://yc.shxzskj.cn

[R04] 位置参数
来源：http://ub.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ck.gzmigu.cn

[R05] 参数默认值
来源：http://vy.521024.cn

name="${1:-default}"
来源：http://vx.shtwfgs.cn

[R06] 判断命令是否存在
来源：http://nc.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ib.newstarts.cn

[R07] if 判断文件
来源：http://rm.shxzukj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zx.yuntaijiaju.cn

[R08] 数值比较
来源：http://pv.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nj.jctech888.com.cn

[R09] 字符串比较
来源：http://jg.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wv.hnjuh.cn

[R10] 正则匹配
来源：http://ph.yuexingan06.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ay.huanxung.cn

[R11] case 多分支
来源：http://ym.jctech888.com.cn

case "$1" in
来源：http://cj.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://tr.lnxyls.cn

stop)  echo "停止" ;;
来源：http://zs.hnjuh.cn

*)     echo "未知命令" ;;
来源：http://am.haigaiapp.cn

esac
来源：http://tv.colortex.cn

[R12] for 遍历文件
来源：http://jr.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://ua.newstarts.cn

[R13] for 计数循环
来源：http://dv.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://tc.szxytkj.cn

[R14] C 风格 for
来源：http://am.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ig.wgjwhj.cn

[R15] while 逐行读文件
来源：http://gg.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nl.521024.cn

[R16] until 等待条件
来源：http://ve.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xm.gzmigu.cn

[R17] 数组定义与取值
来源：http://sd.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://np.haigaiapp.cn

[R18] 遍历数组
来源：http://kn.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.chemitech.net.cn

[R19] 数组长度
来源：http://sv.lnxyls.cn

echo "${#arr[@]}"
来源：http://xw.colortex.cn

[R20] 关联数组（字典）
来源：http://ul.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://le.huixiangedu.cn

[R21] 字符串长度
来源：http://sw.wgjwhj.cn

echo "${#s}"
来源：http://du.szsharing.cn

[R22] 截取子串
来源：http://zs.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://sg.shxzskj.cn

[R23] 字符串替换
来源：http://ut.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cl.muxihuayi.cn

[R24] 大小写转换
来源：http://kv.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lj.szxytkj.cn

[R25] 去后缀 / 去前缀
来源：http://ob.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dv.shxzukj.cn

[R26] 命令替换
来源：http://um.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://ry.huanxung.cn

[R27] 算术展开
来源：http://ip.shxzukj.cn

echo $((1 + 2 * 3))
来源：http://te.panjiajie.cn

[R28] 浮点运算
来源：http://xi.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://fd.jctech888.com.cn

[R29] 定义函数
来源：http://od.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vb.szxytkj.cn

[R30] 函数返回状态码
来源：http://st.521024.cn

f() { return 0; }; f || echo "失败了"
来源：http://if.bjjhwx.cn

[R31] 局部变量
来源：http://ny.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://rc.szxytkj.cn

[R32] 参数个数校验
来源：http://ch.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vl.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://ym.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://it.shtwfgs.cn

[R34] 退出时清理
来源：http://pk.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ta.shtwfgs.cn

[R35] 后台执行并等待
来源：http://ex.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lu.gzmigu.cn

[R36] 并发执行多个任务
来源：http://lt.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ei.9csxet.cn

[R37] 把输出赋给变量
来源：http://bn.panjiajie.cn

files=$(ls -1)
来源：http://fz.yuexingan06.cn

[R38] 管道串联
来源：http://kj.shxzukj.cn

cat a.txt | grep -i error | wc -l
来源：http://bs.yuexingan06.cn

[R39] 重定向标准输出与错误
来源：http://yt.haigaiapp.cn

cmd > out.log 2>&1
来源：http://ui.jianghongdianzi.cn

[R40] 追加写日志
来源：http://jp.chemitech.net.cn

echo "log" >> out.log
来源：http://um.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://ol.yuntaijiaju.cn

cmd >/dev/null 2>&1
来源：http://ui.bookmarksfly.cn

[R42] 输入重定向
来源：http://zc.hnjuh.cn

wc -l < a.txt
来源：http://di.szxytkj.cn

[R43] 按名字查找文件
来源：http://ex.muxihuayi.cn

find . -name "*.log" -type f
来源：http://ar.szxytkj.cn

[R44] 按修改时间查找
来源：http://fk.haigaiapp.cn

find . -mtime -7 -type f
来源：http://ie.panjiajie.cn

[R45] 批量删除
来源：http://ur.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://qh.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://qt.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xv.muxihuayi.cn

[R47] sed 单行替换
来源：http://wr.panjiajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vc.wgjwhj.cn

[R48] awk 取指定列
来源：http://zo.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://lz.521024.cn

[R49] awk 带条件
来源：http://yc.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://do.newstarts.cn

[R50] awk 求和
来源：http://df.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ca.gzmigu.cn

[R51] 排序去重取前几
来源：http://wl.jianghongdianzi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://au.huixiangedu.cn

[R52] 统计行数
来源：http://ku.lnxyls.cn

wc -l a.txt
来源：http://vd.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://gv.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://es.hnjuh.cn

[R54] 比较两个文件
来源：http://sg.jianghongdianzi.cn

diff a.txt b.txt
来源：http://zh.bookmarksfly.cn

[R55] 压缩与解压
来源：http://fr.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bf.asd995.cn

[R56] 远程拷贝
来源：http://pa.hnjuh.cn

scp file user@host:/path/
来源：http://iq.yuexingan06.cn

[R57] 远程执行命令
来源：http://sh.shxzukj.cn

ssh user@host 'uptime'
来源：http://ux.shxzukj.cn

[R58] 下载文件
来源：http://zt.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hx.jctech888.com.cn

[R59] 发 POST JSON
来源：http://ti.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qm.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://bo.huanxung.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tt.jctech888.com.cn

[R61] 磁盘占用
来源：http://ck.shtwfgs.cn

df -h;  du -sh *
来源：http://sz.lnxyls.cn

[R62] 找最占空间的文件
来源：http://sz.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://wh.lnxyls.cn

[R63] 内存与进程
来源：http://le.newstarts.cn

free -h;  ps aux | grep nginx
来源：http://ka.shxzskj.cn

[R64] 结束进程
来源：http://nj.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://lt.szsharing.cn

[R65] 查看端口占用
来源：http://mv.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wb.9csxet.cn

[R66] 定时任务
来源：http://ls.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://uw.huanxung.cn

[R67] 生成随机十六进制串
来源：http://bv.hahajie.cn

openssl rand -hex 16
来源：http://ny.wgjwhj.cn

[R68] 计算文件校验值
来源：http://oo.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://op.chemitech.net.cn

[R69] 生成随机密码
来源：http://pe.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://vr.hnjuh.cn

[R70] 时间戳与互转
来源：http://sp.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://ac.shxzukj.cn

[R71] 日期格式化
来源：http://bz.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nd.hnjuh.cn

[R72] 等待端口就绪
来源：http://je.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bp.bookmarksfly.cn

[R73] 分割大日志
来源：http://ko.hnjuh.cn

split -l 1000 big.log part_
来源：http://pw.yuexingan06.cn

[R74] 批量重命名
来源：http://dp.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zl.asd995.cn

[R75] 导出环境变量
来源：http://eh.bjjhwx.cn

export PATH="$HOME/bin:$PATH"
来源：http://do.szsharing.cn

[R76] 使用临时文件
来源：http://dx.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uh.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://mc.yuexingan06.cn

read -rp "请输入: " ans
来源：http://hx.bookmarksfly.cn

[R78] 交互式菜单
来源：http://ct.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xh.yuexingan06.cn

[R79] 解析命令行选项
来源：http://ba.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://le.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://wn.asd995.cn

time ./run.sh
来源：http://nz.muxihuayi.cn

================================================================================
来源：http://lr.521024.cn

S. C / C++ 专题
来源：http://fy.nszjky.cn

================================================================================
来源：http://nh.lnxyls.cn

[S01] C：Hello World
来源：http://pg.hahajie.cn

#include <stdio.h>
来源：http://ip.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ym.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://no.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://nb.chemitech.net.cn

[S03] C：读入整数
来源：http://if.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://yr.panjiajie.cn

[S04] C：字符串复制
来源：http://ih.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zh.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://qj.haigaiapp.cn

strlen(s)
来源：http://ba.jctech888.com.cn

[S06] C：字符串比较
来源：http://da.shtwfgs.cn

strcmp(a, b) == 0
来源：http://gm.shxzukj.cn

[S07] C：数组遍历求和
来源：http://tl.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ff.asd995.cn

[S08] C：动态内存分配与释放
来源：http://ud.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://he.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://xh.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://up.yuexingan06.cn

[S10] C：指针与解引用
来源：http://rj.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://dm.nicolike.cn

[S11] C：逐行读文件
来源：http://ay.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://rv.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rl.szxytkj.cn

fclose(f);
来源：http://jl.shxzukj.cn

[S12] C：写文件
来源：http://zb.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zr.jianghongdianzi.cn

[S13] C：宏定义
来源：http://vo.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tj.chemitech.net.cn

[S14] C：枚举
来源：http://yd.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://px.muxihuayi.cn

[S15] C：类型转换
来源：http://no.nszjky.cn

(double) a / b
来源：http://lq.521024.cn

[S16] C：位操作置位
来源：http://iu.colortex.cn

x |= (1 << 3);
来源：http://nr.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://yt.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fz.szsharing.cn

[S18] C：命令行参数
来源：http://gq.haigaiapp.cn

int main(int argc, char **argv)
来源：http://sa.panjiajie.cn

[S19] C：快速排序
来源：http://ig.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pw.chemitech.net.cn

[S20] C：二分查找
来源：http://ry.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xu.521024.cn

[S21] C：字符类别判断
来源：http://ze.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yb.nicolike.cn

[S22] C：字符串转数字
来源：http://ks.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://aj.gzmigu.cn

[S23] C：随机数
来源：http://wt.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wv.shxzskj.cn

[S24] C：获取本地时间
来源：http://at.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cx.gzmigu.cn

[S25] C：内存拷贝
来源：http://ee.lnxyls.cn

memcpy(dst, src, n);
来源：http://zx.lnxyls.cn

[S26] C：内存清零
来源：http://ak.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://px.szsharing.cn

[S27] C：定义常量
来源：http://cb.521024.cn

const double PI = 3.14159;
来源：http://ur.jctech888.com.cn

[S28] C：静态变量
来源：http://lq.bjjhwx.cn

static int counter = 0;
来源：http://rf.jctech888.com.cn

[S29] C：变参函数
来源：http://il.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qg.9csxet.cn

[S30] C：头文件保护
来源：http://mn.huixinmuqiang.cn

#ifndef X_H
来源：http://fi.newstarts.cn

#define X_H
来源：http://wm.szxytkj.cn

#endif
来源：http://vd.huixiangedu.cn

[S31] C++：Hello World
来源：http://se.huixinmuqiang.cn

#include <iostream>
来源：http://mz.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://yc.hahajie.cn

[S32] C++：字符串
来源：http://hz.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://pr.nicolike.cn

[S33] C++：vector 增删
来源：http://pc.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://te.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://nz.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://hb.huixinmuqiang.cn

[S35] C++：map
来源：http://fr.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vh.yuexingan06.cn

[S36] C++：unordered_map
来源：http://ei.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tn.hnjuh.cn

[S37] C++：set
来源：http://ey.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jt.bookmarksfly.cn

[S38] C++：排序
来源：http://hz.shxzukj.cn

std::sort(v.begin(), v.end());
来源：http://lt.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://mg.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wt.shxzukj.cn

[S40] C++：查找元素
来源：http://kl.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bi.gzmigu.cn

[S41] C++：类与构造函数
来源：http://hp.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tx.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://kx.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://le.huixiangedu.cn

[S43] C++：智能指针
来源：http://nk.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://ck.asd995.cn

[S44] C++：引用传参
来源：http://ae.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://ie.bjjhwx.cn

[S45] C++：lambda
来源：http://nz.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yy.9csxet.cn

[S46] C++：函数模板
来源：http://ge.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xb.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://xu.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jq.hahajie.cn

[S48] C++：逐行读文件
来源：http://gu.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kf.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://pz.asd995.cn

[S49] C++：写文件
来源：http://ab.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ae.newstarts.cn

[S50] C++：格式化数字
来源：http://hn.shtwfgs.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mx.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://kv.colortex.cn

static_cast<double>(a) / b
来源：http://ul.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://la.huanxung.cn

int size() const noexcept { return n_; }
来源：http://ur.wgjwhj.cn

[S53] C++：移动语义
来源：http://hm.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://es.shtwfgs.cn

[S54] C++：异常处理
来源：http://fu.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wi.yuexingan06.cn

[S55] C++：结构化绑定
来源：http://pk.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xs.huanxung.cn

[S56] C++：optional
来源：http://ej.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ly.asd995.cn

[S57] C++：编译期常量
来源：http://cr.nicolike.cn

constexpr int N = 10;
来源：http://nc.szxytkj.cn

[S58] C++：命名空间
来源：http://hb.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://fw.521024.cn

[S59] C++：静态断言
来源：http://ee.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lj.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://zm.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dp.shxzskj.cn

================================================================================
来源：http://gb.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://so.szxytkj.cn

================================================================================
来源：http://co.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://uv.hahajie.cn

println("Hello")
来源：http://gx.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://dy.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lw.huanxung.cn


<!-- 参考信息 -->