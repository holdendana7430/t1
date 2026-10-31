代发 wailian999

set -euo pipefail
来源：http://cz.9csxet.cn

[R02] 变量赋值与使用
来源：http://dh.9csxet.cn

name="Tom"; echo "$name"
来源：http://vr.shxzskj.cn

[R03] 只读变量
来源：http://dd.newstarts.cn

readonly PI=3.14
来源：http://ii.jianghongdianzi.cn

[R04] 位置参数
来源：http://ec.shxzukj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gz.521024.cn

[R05] 参数默认值
来源：http://pi.yuntaijiaju.cn

name="${1:-default}"
来源：http://as.haigaiapp.cn

[R06] 判断命令是否存在
来源：http://ct.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zq.yuntaijiaju.cn

[R07] if 判断文件
来源：http://ik.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ye.hnjuh.cn

[R08] 数值比较
来源：http://vg.nszjky.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://at.9csxet.cn

[R09] 字符串比较
来源：http://hf.jctech888.com.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lh.asd995.cn

[R10] 正则匹配
来源：http://ul.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dp.521024.cn

[R11] case 多分支
来源：http://tl.huixiangedu.cn

case "$1" in
来源：http://hg.gzmigu.cn

start) echo "启动" ;;
来源：http://gu.gzmigu.cn

stop)  echo "停止" ;;
来源：http://id.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://vi.wgjwhj.cn

esac
来源：http://xp.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://kk.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://ft.jianghongdianzi.cn

[R13] for 计数循环
来源：http://gc.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://rz.nicolike.cn

[R14] C 风格 for
来源：http://cn.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dy.gzmigu.cn

[R15] while 逐行读文件
来源：http://gl.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ae.lnxyls.cn

[R16] until 等待条件
来源：http://es.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lb.newstarts.cn

[R17] 数组定义与取值
来源：http://dg.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ek.521024.cn

[R18] 遍历数组
来源：http://tt.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yu.shxzukj.cn

[R19] 数组长度
来源：http://lr.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://io.521024.cn

[R20] 关联数组（字典）
来源：http://it.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lz.szxytkj.cn

[R21] 字符串长度
来源：http://ew.jctech888.com.cn

echo "${#s}"
来源：http://kk.9csxet.cn

[R22] 截取子串
来源：http://nl.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://ii.yuntaijiaju.cn

[R23] 字符串替换
来源：http://ia.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dp.shtwfgs.cn

[R24] 大小写转换
来源：http://qp.hnjuh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cr.bjjhwx.cn

[R25] 去后缀 / 去前缀
来源：http://vk.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://za.chemitech.net.cn

[R26] 命令替换
来源：http://iv.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://va.shtwfgs.cn

[R27] 算术展开
来源：http://dc.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://fz.9csxet.cn

[R28] 浮点运算
来源：http://qm.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://wy.hnjuh.cn

[R29] 定义函数
来源：http://um.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://db.hnjuh.cn

[R30] 函数返回状态码
来源：http://po.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://jj.yuexingan06.cn

[R31] 局部变量
来源：http://zl.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://rv.jctech888.com.cn

[R32] 参数个数校验
来源：http://jq.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pz.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://pq.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vi.muxihuayi.cn

[R34] 退出时清理
来源：http://ph.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fo.wgjwhj.cn

[R35] 后台执行并等待
来源：http://zh.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kr.hnjuh.cn

[R36] 并发执行多个任务
来源：http://ik.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lh.shxzskj.cn

[R37] 把输出赋给变量
来源：http://gi.wgjwhj.cn

files=$(ls -1)
来源：http://vi.chemitech.net.cn

[R38] 管道串联
来源：http://tb.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://rq.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://xu.jctech888.com.cn

cmd > out.log 2>&1
来源：http://ca.nszjky.cn

[R40] 追加写日志
来源：http://ty.szsharing.cn

echo "log" >> out.log
来源：http://as.9csxet.cn

[R41] 丢弃输出
来源：http://nc.szsharing.cn

cmd >/dev/null 2>&1
来源：http://zg.jctech888.com.cn

[R42] 输入重定向
来源：http://fm.szxytkj.cn

wc -l < a.txt
来源：http://kv.haigaiapp.cn

[R43] 按名字查找文件
来源：http://kw.colortex.cn

find . -name "*.log" -type f
来源：http://ib.hnjuh.cn

[R44] 按修改时间查找
来源：http://xm.bjjhwx.cn

find . -mtime -7 -type f
来源：http://xc.yuntaijiaju.cn

[R45] 批量删除
来源：http://yb.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://hm.nicolike.cn

[R46] 递归替换文件内容
来源：http://dy.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ma.jianghongdianzi.cn

[R47] sed 单行替换
来源：http://qh.shxzukj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gn.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://zg.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://kp.nszjky.cn

[R49] awk 带条件
来源：http://ff.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wt.jctech888.com.cn

[R50] awk 求和
来源：http://mi.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yc.chemitech.net.cn

[R51] 排序去重取前几
来源：http://mg.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lb.hnjuh.cn

[R52] 统计行数
来源：http://ws.asd995.cn

wc -l a.txt
来源：http://dj.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://je.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tt.szxytkj.cn

[R54] 比较两个文件
来源：http://fz.jianghongdianzi.cn

diff a.txt b.txt
来源：http://cs.shtwfgs.cn

[R55] 压缩与解压
来源：http://vq.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bh.panjiajie.cn

[R56] 远程拷贝
来源：http://gc.shxzskj.cn

scp file user@host:/path/
来源：http://oh.huixinmuqiang.cn

[R57] 远程执行命令
来源：http://hl.nszjky.cn

ssh user@host 'uptime'
来源：http://iu.haigaiapp.cn

[R58] 下载文件
来源：http://pk.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wj.shtwfgs.cn

[R59] 发 POST JSON
来源：http://rw.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yp.521024.cn

[R60] 只看 HTTP 状态码
来源：http://il.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ve.shxzukj.cn

[R61] 磁盘占用
来源：http://ej.gzmigu.cn

df -h;  du -sh *
来源：http://ht.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://ry.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://gx.huixinmuqiang.cn

[R63] 内存与进程
来源：http://py.colortex.cn

free -h;  ps aux | grep nginx
来源：http://wn.shxzskj.cn

[R64] 结束进程
来源：http://eo.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://nn.szsharing.cn

[R65] 查看端口占用
来源：http://gj.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oj.szxytkj.cn

[R66] 定时任务
来源：http://wv.yuexingan06.cn

crontab -e;  crontab -l
来源：http://by.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://ym.asd995.cn

openssl rand -hex 16
来源：http://zj.nicolike.cn

[R68] 计算文件校验值
来源：http://cm.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cu.szsharing.cn

[R69] 生成随机密码
来源：http://zh.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://cg.hahajie.cn

[R70] 时间戳与互转
来源：http://wb.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://za.huixiangedu.cn

[R71] 日期格式化
来源：http://jt.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zy.colortex.cn

[R72] 等待端口就绪
来源：http://pq.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ma.gzmigu.cn

[R73] 分割大日志
来源：http://xf.shtwfgs.cn

split -l 1000 big.log part_
来源：http://cl.hahajie.cn

[R74] 批量重命名
来源：http://ku.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ec.huixiangedu.cn

[R75] 导出环境变量
来源：http://me.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://eq.521024.cn

[R76] 使用临时文件
来源：http://vg.jianghongdianzi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qt.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://pb.shxzskj.cn

read -rp "请输入: " ans
来源：http://yr.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://uk.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mo.wgjwhj.cn

[R79] 解析命令行选项
来源：http://ei.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uj.9csxet.cn

[R80] 查看脚本执行耗时
来源：http://rg.gzmigu.cn

time ./run.sh
来源：http://kw.panjiajie.cn

================================================================================
来源：http://aq.huanxung.cn

S. C / C++ 专题
来源：http://vu.jianghongdianzi.cn

================================================================================
来源：http://pd.521024.cn

[S01] C：Hello World
来源：http://ys.hahajie.cn

#include <stdio.h>
来源：http://rw.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wd.hahajie.cn

[S02] C：变量与格式化输出
来源：http://qv.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://qg.chemitech.net.cn

[S03] C：读入整数
来源：http://ij.colortex.cn

int x; scanf("%d", &x);
来源：http://lm.jctech888.com.cn

[S04] C：字符串复制
来源：http://mi.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wx.shxzukj.cn

[S05] C：字符串长度
来源：http://js.hahajie.cn

strlen(s)
来源：http://pm.asd995.cn

[S06] C：字符串比较
来源：http://qm.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://bv.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://dq.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tp.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://fg.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cm.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://gg.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iv.panjiajie.cn

[S10] C：指针与解引用
来源：http://eq.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://lo.haigaiapp.cn

[S11] C：逐行读文件
来源：http://ec.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://bp.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fz.jctech888.com.cn

fclose(f);
来源：http://jg.521024.cn

[S12] C：写文件
来源：http://se.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vw.wgjwhj.cn

[S13] C：宏定义
来源：http://dj.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qm.szsharing.cn

[S14] C：枚举
来源：http://hs.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://vb.huixiangedu.cn

[S15] C：类型转换
来源：http://fv.colortex.cn

(double) a / b
来源：http://zw.hahajie.cn

[S16] C：位操作置位
来源：http://tt.huanxung.cn

x |= (1 << 3);
来源：http://ca.nicolike.cn

[S17] C：安全拼接字符串
来源：http://mx.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://js.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://qa.yuexingan06.cn

int main(int argc, char **argv)
来源：http://yl.hnjuh.cn

[S19] C：快速排序
来源：http://ey.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mo.huixiangedu.cn

[S20] C：二分查找
来源：http://zb.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qa.521024.cn

[S21] C：字符类别判断
来源：http://gs.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://no.gzmigu.cn

[S22] C：字符串转数字
来源：http://xt.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bx.szsharing.cn

[S23] C：随机数
来源：http://gm.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jp.shxzukj.cn

[S24] C：获取本地时间
来源：http://eh.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://el.jctech888.com.cn

[S25] C：内存拷贝
来源：http://ni.szxytkj.cn

memcpy(dst, src, n);
来源：http://aq.shtwfgs.cn

[S26] C：内存清零
来源：http://nr.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://cq.gzmigu.cn

[S27] C：定义常量
来源：http://fa.nicolike.cn

const double PI = 3.14159;
来源：http://jo.yuexingan06.cn

[S28] C：静态变量
来源：http://iw.shxzskj.cn

static int counter = 0;
来源：http://be.hnjuh.cn

[S29] C：变参函数
来源：http://ot.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eb.9csxet.cn

[S30] C：头文件保护
来源：http://dr.shxzukj.cn

#ifndef X_H
来源：http://sf.9csxet.cn

#define X_H
来源：http://bw.hnjuh.cn

#endif
来源：http://kb.muxihuayi.cn

[S31] C++：Hello World
来源：http://mj.szxytkj.cn

#include <iostream>
来源：http://sg.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://sa.newstarts.cn

[S32] C++：字符串
来源：http://rv.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://hi.muxihuayi.cn

[S33] C++：vector 增删
来源：http://xy.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sq.panjiajie.cn

[S34] C++：遍历 vector
来源：http://mt.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://pt.9csxet.cn

[S35] C++：map
来源：http://al.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bo.huanxung.cn

[S36] C++：unordered_map
来源：http://ce.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ci.jianghongdianzi.cn

[S37] C++：set
来源：http://gb.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eu.shtwfgs.cn

[S38] C++：排序
来源：http://fr.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://mp.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://ck.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ti.szsharing.cn

[S40] C++：查找元素
来源：http://ej.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://as.szsharing.cn

[S41] C++：类与构造函数
来源：http://rh.bookmarksfly.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oj.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://fb.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://fn.nszjky.cn

[S43] C++：智能指针
来源：http://yc.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://iy.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://rm.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://wi.haigaiapp.cn

[S45] C++：lambda
来源：http://ld.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zy.asd995.cn

[S46] C++：函数模板
来源：http://sx.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cy.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://ta.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://br.nicolike.cn

[S48] C++：逐行读文件
来源：http://jn.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gr.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://da.9csxet.cn

[S49] C++：写文件
来源：http://kt.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ed.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://xk.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wp.nszjky.cn

[S51] C++：显式类型转换
来源：http://xn.chemitech.net.cn

static_cast<double>(a) / b
来源：http://vx.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://jb.nicolike.cn

int size() const noexcept { return n_; }
来源：http://lr.panjiajie.cn

[S53] C++：移动语义
来源：http://sr.wgjwhj.cn

std::vector<int> w = std::move(v);
来源：http://zw.asd995.cn

[S54] C++：异常处理
来源：http://nl.muxihuayi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zr.9csxet.cn

[S55] C++：结构化绑定
来源：http://fq.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kw.shxzukj.cn

[S56] C++：optional
来源：http://xf.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iq.wgjwhj.cn

[S57] C++：编译期常量
来源：http://fn.yuexingan06.cn

constexpr int N = 10;
来源：http://kf.yuexingan06.cn

[S58] C++：命名空间
来源：http://ks.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://ry.colortex.cn

[S59] C++：静态断言
来源：http://hk.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gr.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://xl.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yi.jianghongdianzi.cn

================================================================================
来源：http://lj.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://po.yuntaijiaju.cn

================================================================================
来源：http://lq.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://jr.colortex.cn

println("Hello")
来源：http://ah.gzmigu.cn

[T02] Kotlin：变量
来源：http://zi.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uq.jctech888.com.cn


<!-- 参考信息 -->