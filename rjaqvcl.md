代发 wailian999

R. Bash 专题
来源：http://qb.haigaiapp.cn

================================================================================
来源：http://vt.newstarts.cn

[R01] shebang 与严格模式
来源：http://rq.asd995.cn

#!/usr/bin/env bash
来源：http://fs.szsharing.cn

set -euo pipefail
来源：http://zs.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://eq.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://df.huanxung.cn

[R03] 只读变量
来源：http://ay.szsharing.cn

readonly PI=3.14
来源：http://bw.chemitech.net.cn

[R04] 位置参数
来源：http://ss.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vs.bjjhwx.cn

[R05] 参数默认值
来源：http://wp.bookmarksfly.cn

name="${1:-default}"
来源：http://qi.panjiajie.cn

[R06] 判断命令是否存在
来源：http://vr.yuexingan06.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eq.szsharing.cn

[R07] if 判断文件
来源：http://fk.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rh.muxihuayi.cn

[R08] 数值比较
来源：http://yu.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sw.huixiangedu.cn

[R09] 字符串比较
来源：http://zo.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fm.9csxet.cn

[R10] 正则匹配
来源：http://qq.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ur.chemitech.net.cn

[R11] case 多分支
来源：http://yf.yuntaijiaju.cn

case "$1" in
来源：http://ty.9csxet.cn

start) echo "启动" ;;
来源：http://tz.hnjuh.cn

stop)  echo "停止" ;;
来源：http://wc.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://tl.bjjhwx.cn

esac
来源：http://jb.wgjwhj.cn

[R12] for 遍历文件
来源：http://tt.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://mp.hnjuh.cn

[R13] for 计数循环
来源：http://wm.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://gw.jctech888.com.cn

[R14] C 风格 for
来源：http://kd.9csxet.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ye.nicolike.cn

[R15] while 逐行读文件
来源：http://gw.bjjhwx.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cj.szxytkj.cn

[R16] until 等待条件
来源：http://ov.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xt.jianghongdianzi.cn

[R17] 数组定义与取值
来源：http://ze.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://to.huixiangedu.cn

[R18] 遍历数组
来源：http://cf.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bp.asd995.cn

[R19] 数组长度
来源：http://bj.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://pn.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://qc.bookmarksfly.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://py.panjiajie.cn

[R21] 字符串长度
来源：http://ae.yuexingan06.cn

echo "${#s}"
来源：http://vo.nszjky.cn

[R22] 截取子串
来源：http://ke.shtwfgs.cn

echo "${s:0:5}"
来源：http://jv.521024.cn

[R23] 字符串替换
来源：http://qb.newstarts.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://am.nicolike.cn

[R24] 大小写转换
来源：http://af.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bx.521024.cn

[R25] 去后缀 / 去前缀
来源：http://bg.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jd.nszjky.cn

[R26] 命令替换
来源：http://tf.huixiangedu.cn

now=$(date +%F); echo "$now"
来源：http://lz.haigaiapp.cn

[R27] 算术展开
来源：http://vu.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://fa.hahajie.cn

[R28] 浮点运算
来源：http://bf.huixiangedu.cn

echo "scale=2; 10/3" | bc
来源：http://ui.panjiajie.cn

[R29] 定义函数
来源：http://ao.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://to.colortex.cn

[R30] 函数返回状态码
来源：http://yw.lnxyls.cn

f() { return 0; }; f || echo "失败了"
来源：http://jj.muxihuayi.cn

[R31] 局部变量
来源：http://lh.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://cn.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://lo.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://de.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://ee.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qx.wgjwhj.cn

[R34] 退出时清理
来源：http://uk.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rc.9csxet.cn

[R35] 后台执行并等待
来源：http://wr.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ae.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://tf.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kz.szxytkj.cn

[R37] 把输出赋给变量
来源：http://yn.huanxung.cn

files=$(ls -1)
来源：http://ky.gzmigu.cn

[R38] 管道串联
来源：http://iw.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://ry.panjiajie.cn

[R39] 重定向标准输出与错误
来源：http://md.wgjwhj.cn

cmd > out.log 2>&1
来源：http://xx.asd995.cn

[R40] 追加写日志
来源：http://xz.asd995.cn

echo "log" >> out.log
来源：http://vd.9csxet.cn

[R41] 丢弃输出
来源：http://ot.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://hu.nszjky.cn

[R42] 输入重定向
来源：http://fp.jianghongdianzi.cn

wc -l < a.txt
来源：http://ro.9csxet.cn

[R43] 按名字查找文件
来源：http://ly.9csxet.cn

find . -name "*.log" -type f
来源：http://jn.9csxet.cn

[R44] 按修改时间查找
来源：http://gh.szsharing.cn

find . -mtime -7 -type f
来源：http://tv.jianghongdianzi.cn

[R45] 批量删除
来源：http://fs.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://vz.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://xh.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dy.huanxung.cn

[R47] sed 单行替换
来源：http://di.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bp.shxzukj.cn

[R48] awk 取指定列
来源：http://rr.huixiangedu.cn

awk '{print $1, $3}' a.txt
来源：http://qw.newstarts.cn

[R49] awk 带条件
来源：http://zb.muxihuayi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ap.panjiajie.cn

[R50] awk 求和
来源：http://cp.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ms.panjiajie.cn

[R51] 排序去重取前几
来源：http://jq.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bd.newstarts.cn

[R52] 统计行数
来源：http://lf.nicolike.cn

wc -l a.txt
来源：http://nf.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://vy.gzmigu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oj.hahajie.cn

[R54] 比较两个文件
来源：http://be.yuntaijiaju.cn

diff a.txt b.txt
来源：http://qv.szsharing.cn

[R55] 压缩与解压
来源：http://zd.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mb.hnjuh.cn

[R56] 远程拷贝
来源：http://sd.yuexingan06.cn

scp file user@host:/path/
来源：http://bn.9csxet.cn

[R57] 远程执行命令
来源：http://hq.jctech888.com.cn

ssh user@host 'uptime'
来源：http://kw.szsharing.cn

[R58] 下载文件
来源：http://tu.hnjuh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ik.panjiajie.cn

[R59] 发 POST JSON
来源：http://kc.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sf.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://ad.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oa.szxytkj.cn

[R61] 磁盘占用
来源：http://uo.huixinmuqiang.cn

df -h;  du -sh *
来源：http://nm.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://wy.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://eu.nicolike.cn

[R63] 内存与进程
来源：http://lv.panjiajie.cn

free -h;  ps aux | grep nginx
来源：http://mk.521024.cn

[R64] 结束进程
来源：http://gq.haigaiapp.cn

kill -9 $(pgrep -f app.py)
来源：http://wo.panjiajie.cn

[R65] 查看端口占用
来源：http://bu.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://el.szsharing.cn

[R66] 定时任务
来源：http://hv.shxzukj.cn

crontab -e;  crontab -l
来源：http://nf.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://jn.shxzskj.cn

openssl rand -hex 16
来源：http://xm.nicolike.cn

[R68] 计算文件校验值
来源：http://ol.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ao.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://fw.hahajie.cn

head -c 16 /dev/urandom | base64
来源：http://cl.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://ir.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://yp.9csxet.cn

[R71] 日期格式化
来源：http://zi.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dh.chemitech.net.cn

[R72] 等待端口就绪
来源：http://gm.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xt.colortex.cn

[R73] 分割大日志
来源：http://wj.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://eg.9csxet.cn

[R74] 批量重命名
来源：http://su.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xl.szxytkj.cn

[R75] 导出环境变量
来源：http://nd.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://so.szxytkj.cn

[R76] 使用临时文件
来源：http://ua.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cm.bookmarksfly.cn

[R77] 读取用户输入
来源：http://ob.shtwfgs.cn

read -rp "请输入: " ans
来源：http://ff.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://nh.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ia.nszjky.cn

[R79] 解析命令行选项
来源：http://vf.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yv.asd995.cn

[R80] 查看脚本执行耗时
来源：http://pg.panjiajie.cn

time ./run.sh
来源：http://hu.huixinmuqiang.cn

================================================================================
来源：http://lb.jctech888.com.cn

S. C / C++ 专题
来源：http://dh.szxytkj.cn

================================================================================
来源：http://og.huixinmuqiang.cn

[S01] C：Hello World
来源：http://un.colortex.cn

#include <stdio.h>
来源：http://rx.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://im.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://zt.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://cn.nicolike.cn

[S03] C：读入整数
来源：http://mt.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://uq.asd995.cn

[S04] C：字符串复制
来源：http://ri.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ls.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://jh.nszjky.cn

strlen(s)
来源：http://jx.bjjhwx.cn

[S06] C：字符串比较
来源：http://mz.9csxet.cn

strcmp(a, b) == 0
来源：http://av.nszjky.cn

[S07] C：数组遍历求和
来源：http://ht.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ny.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://rd.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zx.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://uj.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yf.lnxyls.cn

[S10] C：指针与解引用
来源：http://ap.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://jh.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://bx.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://re.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://eg.9csxet.cn

fclose(f);
来源：http://yg.yuntaijiaju.cn

[S12] C：写文件
来源：http://nl.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ed.jctech888.com.cn

[S13] C：宏定义
来源：http://ig.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ri.shxzukj.cn

[S14] C：枚举
来源：http://ez.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://wo.wgjwhj.cn

[S15] C：类型转换
来源：http://ix.hahajie.cn

(double) a / b
来源：http://zk.shxzukj.cn

[S16] C：位操作置位
来源：http://yb.jianghongdianzi.cn

x |= (1 << 3);
来源：http://yy.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://bs.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qx.wgjwhj.cn

[S18] C：命令行参数
来源：http://cz.shxzskj.cn

int main(int argc, char **argv)
来源：http://zu.gzmigu.cn

[S19] C：快速排序
来源：http://no.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tt.bjjhwx.cn

[S20] C：二分查找
来源：http://sr.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nv.shxzukj.cn

[S21] C：字符类别判断
来源：http://ar.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xy.chemitech.net.cn

[S22] C：字符串转数字
来源：http://iw.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tf.newstarts.cn

[S23] C：随机数
来源：http://wp.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hm.huanxung.cn

[S24] C：获取本地时间
来源：http://fl.chemitech.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aa.muxihuayi.cn

[S25] C：内存拷贝
来源：http://de.colortex.cn

memcpy(dst, src, n);
来源：http://gb.szxytkj.cn

[S26] C：内存清零
来源：http://pe.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://qo.chemitech.net.cn

[S27] C：定义常量
来源：http://tq.wgjwhj.cn

const double PI = 3.14159;
来源：http://ot.huixiangedu.cn

[S28] C：静态变量
来源：http://bt.lnxyls.cn

static int counter = 0;
来源：http://di.wgjwhj.cn

[S29] C：变参函数
来源：http://fh.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ha.muxihuayi.cn

[S30] C：头文件保护
来源：http://fj.hahajie.cn

#ifndef X_H
来源：http://te.hnjuh.cn

#define X_H
来源：http://tt.jctech888.com.cn

#endif
来源：http://tf.szxytkj.cn

[S31] C++：Hello World
来源：http://em.haigaiapp.cn

#include <iostream>
来源：http://ii.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://xb.bjjhwx.cn

[S32] C++：字符串
来源：http://cy.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://iw.huanxung.cn

[S33] C++：vector 增删
来源：http://pv.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dg.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://vv.shxzskj.cn

for (auto &x : v) { std::cout << x; }
来源：http://au.jctech888.com.cn

[S35] C++：map
来源：http://vo.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wv.lnxyls.cn

[S36] C++：unordered_map
来源：http://rg.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://go.huixiangedu.cn

[S37] C++：set
来源：http://yr.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wf.jctech888.com.cn

[S38] C++：排序
来源：http://ze.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://sv.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://jq.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jy.panjiajie.cn

[S40] C++：查找元素
来源：http://xx.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ek.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://hx.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ai.nicolike.cn

[S42] C++：继承与虚函数
来源：http://uw.521024.cn

class B : public Base { public: void f() override {} };
来源：http://ui.521024.cn

[S43] C++：智能指针
来源：http://nn.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://cq.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://kh.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://ua.panjiajie.cn

[S45] C++：lambda
来源：http://vr.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yc.nicolike.cn

[S46] C++：函数模板
来源：http://lv.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ci.yuexingan06.cn

[S47] C++：结构化绑定遍历
来源：http://dp.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ro.hahajie.cn

[S48] C++：逐行读文件
来源：http://zd.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zo.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://os.jctech888.com.cn

[S49] C++：写文件
来源：http://ay.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hh.asd995.cn

[S50] C++：格式化数字
来源：http://pz.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wb.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://ms.hnjuh.cn

static_cast<double>(a) / b
来源：http://bh.jianghongdianzi.cn

[S52] C++：const 与 noexcept
来源：http://cw.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://sy.bookmarksfly.cn

[S53] C++：移动语义
来源：http://ok.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://ge.panjiajie.cn

[S54] C++：异常处理
来源：http://hb.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mt.hnjuh.cn

[S55] C++：结构化绑定
来源：http://ih.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uu.huixiangedu.cn

[S56] C++：optional
来源：http://zs.shxzskj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uf.9csxet.cn

[S57] C++：编译期常量
来源：http://jw.szxytkj.cn

constexpr int N = 10;
来源：http://ic.szsharing.cn

[S58] C++：命名空间
来源：http://zs.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://ub.huanxung.cn

[S59] C++：静态断言
来源：http://qj.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wi.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://lk.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mi.panjiajie.cn

================================================================================
来源：http://ew.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mh.jianghongdianzi.cn

================================================================================
来源：http://pf.bookmarksfly.cn


<!-- 参考信息 -->