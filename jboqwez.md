代发 wailian999

set -euo pipefail
来源：http://ov.shxzukj.cn

[R02] 变量赋值与使用
来源：http://vo.shtwfgs.cn

name="Tom"; echo "$name"
来源：http://uj.nicolike.cn

[R03] 只读变量
来源：http://mn.hnjuh.cn

readonly PI=3.14
来源：http://vv.colortex.cn

[R04] 位置参数
来源：http://oz.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ct.521024.cn

[R05] 参数默认值
来源：http://px.9csxet.cn

name="${1:-default}"
来源：http://bz.9csxet.cn

[R06] 判断命令是否存在
来源：http://tp.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qb.nszjky.cn

[R07] if 判断文件
来源：http://fk.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eg.huixiangedu.cn

[R08] 数值比较
来源：http://te.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://va.huixiangedu.cn

[R09] 字符串比较
来源：http://gw.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pq.muxihuayi.cn

[R10] 正则匹配
来源：http://au.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ks.wgjwhj.cn

[R11] case 多分支
来源：http://ob.yuexingan06.cn

case "$1" in
来源：http://bv.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://jl.shxzukj.cn

stop)  echo "停止" ;;
来源：http://ya.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://li.gzmigu.cn

esac
来源：http://sw.haigaiapp.cn

[R12] for 遍历文件
来源：http://fs.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://gd.nszjky.cn

[R13] for 计数循环
来源：http://ke.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://up.yuntaijiaju.cn

[R14] C 风格 for
来源：http://wn.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ku.hnjuh.cn

[R15] while 逐行读文件
来源：http://fg.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ug.shxzskj.cn

[R16] until 等待条件
来源：http://ug.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tb.huixinmuqiang.cn

[R17] 数组定义与取值
来源：http://pu.521024.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mv.panjiajie.cn

[R18] 遍历数组
来源：http://xs.huixiangedu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vj.jctech888.com.cn

[R19] 数组长度
来源：http://os.huixiangedu.cn

echo "${#arr[@]}"
来源：http://wx.lnxyls.cn

[R20] 关联数组（字典）
来源：http://rk.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qq.hnjuh.cn

[R21] 字符串长度
来源：http://jr.9csxet.cn

echo "${#s}"
来源：http://ow.jctech888.com.cn

[R22] 截取子串
来源：http://mv.9csxet.cn

echo "${s:0:5}"
来源：http://ji.chemitech.net.cn

[R23] 字符串替换
来源：http://yh.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gx.bjjhwx.cn

[R24] 大小写转换
来源：http://sg.szxytkj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ff.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://nt.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qq.panjiajie.cn

[R26] 命令替换
来源：http://uw.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://yt.panjiajie.cn

[R27] 算术展开
来源：http://hg.asd995.cn

echo $((1 + 2 * 3))
来源：http://mo.colortex.cn

[R28] 浮点运算
来源：http://hn.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://un.huixiangedu.cn

[R29] 定义函数
来源：http://eh.haigaiapp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nq.shxzukj.cn

[R30] 函数返回状态码
来源：http://kn.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://gf.jctech888.com.cn

[R31] 局部变量
来源：http://uh.hnjuh.cn

f() { local x=1; echo "$x"; }
来源：http://fp.asd995.cn

[R32] 参数个数校验
来源：http://mw.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pi.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://zb.gzmigu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fh.bjjhwx.cn

[R34] 退出时清理
来源：http://tz.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zb.shxzskj.cn

[R35] 后台执行并等待
来源：http://rr.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lb.szxytkj.cn

[R36] 并发执行多个任务
来源：http://fk.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://us.szsharing.cn

[R37] 把输出赋给变量
来源：http://kc.huixiangedu.cn

files=$(ls -1)
来源：http://if.colortex.cn

[R38] 管道串联
来源：http://cy.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://vw.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://zb.9csxet.cn

cmd > out.log 2>&1
来源：http://kn.haigaiapp.cn

[R40] 追加写日志
来源：http://rb.szsharing.cn

echo "log" >> out.log
来源：http://ca.wgjwhj.cn

[R41] 丢弃输出
来源：http://um.newstarts.cn

cmd >/dev/null 2>&1
来源：http://cc.yuexingan06.cn

[R42] 输入重定向
来源：http://jf.haigaiapp.cn

wc -l < a.txt
来源：http://vp.szxytkj.cn

[R43] 按名字查找文件
来源：http://yj.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://bc.asd995.cn

[R44] 按修改时间查找
来源：http://or.chemitech.net.cn

find . -mtime -7 -type f
来源：http://nx.521024.cn

[R45] 批量删除
来源：http://cr.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://nj.newstarts.cn

[R46] 递归替换文件内容
来源：http://ov.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xg.shxzskj.cn

[R47] sed 单行替换
来源：http://dg.shxzskj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fz.nszjky.cn

[R48] awk 取指定列
来源：http://wd.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://hp.yuntaijiaju.cn

[R49] awk 带条件
来源：http://bt.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rn.asd995.cn

[R50] awk 求和
来源：http://mt.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gh.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://gb.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bs.521024.cn

[R52] 统计行数
来源：http://tb.huixinmuqiang.cn

wc -l a.txt
来源：http://mw.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://jv.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gy.chemitech.net.cn

[R54] 比较两个文件
来源：http://fc.shtwfgs.cn

diff a.txt b.txt
来源：http://ur.wgjwhj.cn

[R55] 压缩与解压
来源：http://mp.shxzukj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tp.521024.cn

[R56] 远程拷贝
来源：http://lh.bookmarksfly.cn

scp file user@host:/path/
来源：http://eg.muxihuayi.cn

[R57] 远程执行命令
来源：http://jf.lnxyls.cn

ssh user@host 'uptime'
来源：http://zu.shxzukj.cn

[R58] 下载文件
来源：http://lz.jianghongdianzi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wq.asd995.cn

[R59] 发 POST JSON
来源：http://jr.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://or.jianghongdianzi.cn

[R60] 只看 HTTP 状态码
来源：http://vy.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wa.bookmarksfly.cn

[R61] 磁盘占用
来源：http://op.newstarts.cn

df -h;  du -sh *
来源：http://xx.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://mu.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://cx.yuntaijiaju.cn

[R63] 内存与进程
来源：http://xf.yuntaijiaju.cn

free -h;  ps aux | grep nginx
来源：http://jl.yuexingan06.cn

[R64] 结束进程
来源：http://ev.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://oi.shxzskj.cn

[R65] 查看端口占用
来源：http://iq.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fw.szxytkj.cn

[R66] 定时任务
来源：http://nm.muxihuayi.cn

crontab -e;  crontab -l
来源：http://hh.huanxung.cn

[R67] 生成随机十六进制串
来源：http://hn.asd995.cn

openssl rand -hex 16
来源：http://zr.szsharing.cn

[R68] 计算文件校验值
来源：http://vu.lnxyls.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zy.bjjhwx.cn

[R69] 生成随机密码
来源：http://ro.jctech888.com.cn

head -c 16 /dev/urandom | base64
来源：http://ti.hnjuh.cn

[R70] 时间戳与互转
来源：http://fa.9csxet.cn

date +%s;  date -d @1700000000
来源：http://se.huixiangedu.cn

[R71] 日期格式化
来源：http://re.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wa.yuexingan06.cn

[R72] 等待端口就绪
来源：http://xh.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mw.panjiajie.cn

[R73] 分割大日志
来源：http://bz.nszjky.cn

split -l 1000 big.log part_
来源：http://yk.shxzskj.cn

[R74] 批量重命名
来源：http://xz.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mb.wgjwhj.cn

[R75] 导出环境变量
来源：http://hw.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://sk.szxytkj.cn

[R76] 使用临时文件
来源：http://sx.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ja.haigaiapp.cn

[R77] 读取用户输入
来源：http://pi.nicolike.cn

read -rp "请输入: " ans
来源：http://ye.9csxet.cn

[R78] 交互式菜单
来源：http://nn.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://aa.shxzskj.cn

[R79] 解析命令行选项
来源：http://qx.521024.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ze.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://vb.bjjhwx.cn

time ./run.sh
来源：http://ac.9csxet.cn

================================================================================
来源：http://qb.bookmarksfly.cn

S. C / C++ 专题
来源：http://wo.szxytkj.cn

================================================================================
来源：http://cs.shxzskj.cn

[S01] C：Hello World
来源：http://hg.wgjwhj.cn

#include <stdio.h>
来源：http://ox.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ej.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://fl.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://ii.yuntaijiaju.cn

[S03] C：读入整数
来源：http://ej.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://ei.chemitech.net.cn

[S04] C：字符串复制
来源：http://wv.nicolike.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ml.szxytkj.cn

[S05] C：字符串长度
来源：http://lu.huixinmuqiang.cn

strlen(s)
来源：http://ra.hnjuh.cn

[S06] C：字符串比较
来源：http://hu.shxzukj.cn

strcmp(a, b) == 0
来源：http://ek.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://pk.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ks.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://ix.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xa.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://my.lnxyls.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vs.asd995.cn

[S10] C：指针与解引用
来源：http://vk.hahajie.cn

int *p = &a;  *p = 5;
来源：http://hz.chemitech.net.cn

[S11] C：逐行读文件
来源：http://oo.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://qd.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fu.gzmigu.cn

fclose(f);
来源：http://rz.szsharing.cn

[S12] C：写文件
来源：http://yl.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gv.lnxyls.cn

[S13] C：宏定义
来源：http://kc.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zb.bookmarksfly.cn

[S14] C：枚举
来源：http://dx.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://zx.yuntaijiaju.cn

[S15] C：类型转换
来源：http://yt.bookmarksfly.cn

(double) a / b
来源：http://fa.hahajie.cn

[S16] C：位操作置位
来源：http://nb.asd995.cn

x |= (1 << 3);
来源：http://wa.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://fu.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xp.panjiajie.cn

[S18] C：命令行参数
来源：http://oj.newstarts.cn

int main(int argc, char **argv)
来源：http://sm.nszjky.cn

[S19] C：快速排序
来源：http://lz.newstarts.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rk.szxytkj.cn

[S20] C：二分查找
来源：http://fw.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hs.hahajie.cn

[S21] C：字符类别判断
来源：http://xa.shxzskj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uv.lnxyls.cn

[S22] C：字符串转数字
来源：http://fu.nszjky.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ev.lnxyls.cn

[S23] C：随机数
来源：http://aa.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ot.nicolike.cn

[S24] C：获取本地时间
来源：http://we.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ol.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://qj.shxzskj.cn

memcpy(dst, src, n);
来源：http://tr.wgjwhj.cn

[S26] C：内存清零
来源：http://sl.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://wa.9csxet.cn

[S27] C：定义常量
来源：http://mc.hahajie.cn

const double PI = 3.14159;
来源：http://mk.lnxyls.cn

[S28] C：静态变量
来源：http://ns.jctech888.com.cn

static int counter = 0;
来源：http://wj.yuexingan06.cn

[S29] C：变参函数
来源：http://zw.panjiajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://og.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://cj.szxytkj.cn

#ifndef X_H
来源：http://bg.szsharing.cn

#define X_H
来源：http://pc.muxihuayi.cn

#endif
来源：http://om.9csxet.cn

[S31] C++：Hello World
来源：http://vf.panjiajie.cn

#include <iostream>
来源：http://im.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://sl.shtwfgs.cn

[S32] C++：字符串
来源：http://xj.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://dh.nicolike.cn

[S33] C++：vector 增删
来源：http://ag.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sq.muxihuayi.cn

[S34] C++：遍历 vector
来源：http://nd.szsharing.cn

for (auto &x : v) { std::cout << x; }
来源：http://oe.muxihuayi.cn

[S35] C++：map
来源：http://uq.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eu.gzmigu.cn

[S36] C++：unordered_map
来源：http://vf.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pm.bookmarksfly.cn

[S37] C++：set
来源：http://kp.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vv.colortex.cn

[S38] C++：排序
来源：http://xa.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://kl.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://sp.huixinmuqiang.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ol.asd995.cn

[S40] C++：查找元素
来源：http://dw.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ox.asd995.cn

[S41] C++：类与构造函数
来源：http://nz.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zr.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://ew.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://ld.shtwfgs.cn

[S43] C++：智能指针
来源：http://at.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://an.muxihuayi.cn

[S44] C++：引用传参
来源：http://rj.521024.cn

void inc(int &x) { ++x; }
来源：http://on.haigaiapp.cn

[S45] C++：lambda
来源：http://yw.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oc.chemitech.net.cn

[S46] C++：函数模板
来源：http://bf.szxytkj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pq.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://jc.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mx.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://yu.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zr.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://ub.shxzukj.cn

[S49] C++：写文件
来源：http://bo.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wo.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://ma.huanxung.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lh.nszjky.cn

[S51] C++：显式类型转换
来源：http://nt.muxihuayi.cn

static_cast<double>(a) / b
来源：http://uv.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://nt.szsharing.cn

int size() const noexcept { return n_; }
来源：http://gs.panjiajie.cn

[S53] C++：移动语义
来源：http://ax.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://ti.chemitech.net.cn

[S54] C++：异常处理
来源：http://eg.yuntaijiaju.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dj.huanxung.cn

[S55] C++：结构化绑定
来源：http://dc.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uw.jianghongdianzi.cn

[S56] C++：optional
来源：http://vt.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jr.nicolike.cn

[S57] C++：编译期常量
来源：http://dy.panjiajie.cn

constexpr int N = 10;
来源：http://fo.haigaiapp.cn

[S58] C++：命名空间
来源：http://mw.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://lc.gzmigu.cn

[S59] C++：静态断言
来源：http://zr.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uv.huixinmuqiang.cn

[S60] C++：遍历并删除元素
来源：http://jb.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nb.asd995.cn

================================================================================
来源：http://gz.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vu.9csxet.cn

================================================================================
来源：http://kq.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://ol.szxytkj.cn

println("Hello")
来源：http://et.bjjhwx.cn

[T02] Kotlin：变量
来源：http://dq.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cs.hnjuh.cn


<!-- 参考信息 -->