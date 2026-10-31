代发 wailian999

readonly PI=3.14
来源：http://hs.9csxet.cn

[R04] 位置参数
来源：http://dq.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nr.shxzskj.cn

[R05] 参数默认值
来源：http://id.huixiangedu.cn

name="${1:-default}"
来源：http://gi.shxzukj.cn

[R06] 判断命令是否存在
来源：http://fc.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dq.colortex.cn

[R07] if 判断文件
来源：http://iz.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kf.hahajie.cn

[R08] 数值比较
来源：http://xa.nszjky.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tx.yuexingan06.cn

[R09] 字符串比较
来源：http://iu.bookmarksfly.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xa.yuexingan06.cn

[R10] 正则匹配
来源：http://ye.muxihuayi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ts.yuntaijiaju.cn

[R11] case 多分支
来源：http://gl.newstarts.cn

case "$1" in
来源：http://np.asd995.cn

start) echo "启动" ;;
来源：http://sn.hnjuh.cn

stop)  echo "停止" ;;
来源：http://vi.521024.cn

*)     echo "未知命令" ;;
来源：http://ih.nszjky.cn

esac
来源：http://lm.lnxyls.cn

[R12] for 遍历文件
来源：http://hm.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://nl.colortex.cn

[R13] for 计数循环
来源：http://hz.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://mq.yuntaijiaju.cn

[R14] C 风格 for
来源：http://ty.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vn.panjiajie.cn

[R15] while 逐行读文件
来源：http://zm.hahajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://db.chemitech.net.cn

[R16] until 等待条件
来源：http://bs.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qc.chemitech.net.cn

[R17] 数组定义与取值
来源：http://gs.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yo.szsharing.cn

[R18] 遍历数组
来源：http://ec.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ir.9csxet.cn

[R19] 数组长度
来源：http://ph.hnjuh.cn

echo "${#arr[@]}"
来源：http://uo.9csxet.cn

[R20] 关联数组（字典）
来源：http://vj.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ow.hnjuh.cn

[R21] 字符串长度
来源：http://vu.shxzukj.cn

echo "${#s}"
来源：http://td.chemitech.net.cn

[R22] 截取子串
来源：http://oe.szsharing.cn

echo "${s:0:5}"
来源：http://hc.huixiangedu.cn

[R23] 字符串替换
来源：http://kj.huixinmuqiang.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tn.gzmigu.cn

[R24] 大小写转换
来源：http://bm.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rb.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://np.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rg.colortex.cn

[R26] 命令替换
来源：http://yr.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://dp.wgjwhj.cn

[R27] 算术展开
来源：http://tz.huanxung.cn

echo $((1 + 2 * 3))
来源：http://yc.hahajie.cn

[R28] 浮点运算
来源：http://wo.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://ut.hahajie.cn

[R29] 定义函数
来源：http://jd.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wz.yuntaijiaju.cn

[R30] 函数返回状态码
来源：http://ab.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://cg.shxzskj.cn

[R31] 局部变量
来源：http://xz.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://mq.bookmarksfly.cn

[R32] 参数个数校验
来源：http://kk.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wm.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://ix.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://aw.shxzukj.cn

[R34] 退出时清理
来源：http://xl.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cb.shxzukj.cn

[R35] 后台执行并等待
来源：http://fa.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ql.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://op.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ud.gzmigu.cn

[R37] 把输出赋给变量
来源：http://dj.521024.cn

files=$(ls -1)
来源：http://ey.szsharing.cn

[R38] 管道串联
来源：http://ci.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://vj.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://ke.muxihuayi.cn

cmd > out.log 2>&1
来源：http://pv.panjiajie.cn

[R40] 追加写日志
来源：http://yx.chemitech.net.cn

echo "log" >> out.log
来源：http://ik.chemitech.net.cn

[R41] 丢弃输出
来源：http://ym.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://xz.bookmarksfly.cn

[R42] 输入重定向
来源：http://jd.521024.cn

wc -l < a.txt
来源：http://ah.lnxyls.cn

[R43] 按名字查找文件
来源：http://jz.lnxyls.cn

find . -name "*.log" -type f
来源：http://to.bjjhwx.cn

[R44] 按修改时间查找
来源：http://hp.haigaiapp.cn

find . -mtime -7 -type f
来源：http://hh.chemitech.net.cn

[R45] 批量删除
来源：http://ig.asd995.cn

find . -name "*.tmp" -delete
来源：http://ol.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://gq.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ru.panjiajie.cn

[R47] sed 单行替换
来源：http://ie.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ah.colortex.cn

[R48] awk 取指定列
来源：http://rx.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://rq.hahajie.cn

[R49] awk 带条件
来源：http://zl.shxzskj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gu.lnxyls.cn

[R50] awk 求和
来源：http://rv.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://oq.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://yl.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://st.nszjky.cn

[R52] 统计行数
来源：http://ik.muxihuayi.cn

wc -l a.txt
来源：http://in.nszjky.cn

[R53] 查看文件头与实时尾
来源：http://ds.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aq.bjjhwx.cn

[R54] 比较两个文件
来源：http://wu.jctech888.com.cn

diff a.txt b.txt
来源：http://sf.szxytkj.cn

[R55] 压缩与解压
来源：http://me.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jq.newstarts.cn

[R56] 远程拷贝
来源：http://pw.panjiajie.cn

scp file user@host:/path/
来源：http://we.hahajie.cn

[R57] 远程执行命令
来源：http://wq.huanxung.cn

ssh user@host 'uptime'
来源：http://xd.yuntaijiaju.cn

[R58] 下载文件
来源：http://iz.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bl.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://yo.szxytkj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://da.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://tx.muxihuayi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fh.bookmarksfly.cn

[R61] 磁盘占用
来源：http://xm.jianghongdianzi.cn

df -h;  du -sh *
来源：http://ol.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://ex.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://kn.jctech888.com.cn

[R63] 内存与进程
来源：http://pn.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://qh.jctech888.com.cn

[R64] 结束进程
来源：http://fx.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://eh.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://ac.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ge.yuntaijiaju.cn

[R66] 定时任务
来源：http://qb.shtwfgs.cn

crontab -e;  crontab -l
来源：http://cv.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://dt.huixiangedu.cn

openssl rand -hex 16
来源：http://gi.yuntaijiaju.cn

[R68] 计算文件校验值
来源：http://fw.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kc.lnxyls.cn

[R69] 生成随机密码
来源：http://hd.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://kr.huanxung.cn

[R70] 时间戳与互转
来源：http://qx.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://xd.chemitech.net.cn

[R71] 日期格式化
来源：http://ux.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://oq.hnjuh.cn

[R72] 等待端口就绪
来源：http://cu.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yn.521024.cn

[R73] 分割大日志
来源：http://lj.gzmigu.cn

split -l 1000 big.log part_
来源：http://qy.yuntaijiaju.cn

[R74] 批量重命名
来源：http://bp.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ws.shxzskj.cn

[R75] 导出环境变量
来源：http://iz.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://aq.szxytkj.cn

[R76] 使用临时文件
来源：http://qi.hahajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sr.haigaiapp.cn

[R77] 读取用户输入
来源：http://ia.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://bv.haigaiapp.cn

[R78] 交互式菜单
来源：http://bz.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cv.yuexingan06.cn

[R79] 解析命令行选项
来源：http://hd.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ig.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://cx.nicolike.cn

time ./run.sh
来源：http://dj.wgjwhj.cn

================================================================================
来源：http://tv.nicolike.cn

S. C / C++ 专题
来源：http://zo.jctech888.com.cn

================================================================================
来源：http://xa.colortex.cn

[S01] C：Hello World
来源：http://uo.jctech888.com.cn

#include <stdio.h>
来源：http://xq.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mj.szxytkj.cn

[S02] C：变量与格式化输出
来源：http://uw.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://uw.asd995.cn

[S03] C：读入整数
来源：http://pt.shxzskj.cn

int x; scanf("%d", &x);
来源：http://aq.szsharing.cn

[S04] C：字符串复制
来源：http://bl.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pe.shtwfgs.cn

[S05] C：字符串长度
来源：http://gx.bjjhwx.cn

strlen(s)
来源：http://qj.521024.cn

[S06] C：字符串比较
来源：http://ix.nszjky.cn

strcmp(a, b) == 0
来源：http://tj.szsharing.cn

[S07] C：数组遍历求和
来源：http://yn.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zh.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://ee.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rv.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://zh.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hd.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://xg.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://ww.9csxet.cn

[S11] C：逐行读文件
来源：http://ne.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://ei.nicolike.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gw.jctech888.com.cn

fclose(f);
来源：http://aa.asd995.cn

[S12] C：写文件
来源：http://oi.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hk.hahajie.cn

[S13] C：宏定义
来源：http://sa.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nr.huixiangedu.cn

[S14] C：枚举
来源：http://dn.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://ep.9csxet.cn

[S15] C：类型转换
来源：http://qc.huanxung.cn

(double) a / b
来源：http://os.chemitech.net.cn

[S16] C：位操作置位
来源：http://ha.nszjky.cn

x |= (1 << 3);
来源：http://qn.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://tk.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hm.jctech888.com.cn

[S18] C：命令行参数
来源：http://rx.gzmigu.cn

int main(int argc, char **argv)
来源：http://jc.panjiajie.cn

[S19] C：快速排序
来源：http://an.newstarts.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wy.panjiajie.cn

[S20] C：二分查找
来源：http://jf.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ns.nicolike.cn

[S21] C：字符类别判断
来源：http://dr.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ht.yuexingan06.cn

[S22] C：字符串转数字
来源：http://zk.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ct.newstarts.cn

[S23] C：随机数
来源：http://dr.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jc.shxzskj.cn

[S24] C：获取本地时间
来源：http://dr.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hm.wgjwhj.cn

[S25] C：内存拷贝
来源：http://oo.nicolike.cn

memcpy(dst, src, n);
来源：http://lw.521024.cn

[S26] C：内存清零
来源：http://ec.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://wn.521024.cn

[S27] C：定义常量
来源：http://dl.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://ct.hnjuh.cn

[S28] C：静态变量
来源：http://cx.hahajie.cn

static int counter = 0;
来源：http://ky.yuntaijiaju.cn

[S29] C：变参函数
来源：http://yk.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qk.panjiajie.cn

[S30] C：头文件保护
来源：http://tr.bookmarksfly.cn

#ifndef X_H
来源：http://fi.lnxyls.cn

#define X_H
来源：http://he.huanxung.cn

#endif
来源：http://hp.hahajie.cn

[S31] C++：Hello World
来源：http://gt.shxzskj.cn

#include <iostream>
来源：http://kn.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://fy.huixinmuqiang.cn

[S32] C++：字符串
来源：http://xn.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://uf.nszjky.cn

[S33] C++：vector 增删
来源：http://ic.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rj.huanxung.cn

[S34] C++：遍历 vector
来源：http://ps.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://it.shxzukj.cn

[S35] C++：map
来源：http://yy.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://id.colortex.cn

[S36] C++：unordered_map
来源：http://ww.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zw.huanxung.cn

[S37] C++：set
来源：http://if.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hb.shxzukj.cn

[S38] C++：排序
来源：http://fn.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://dz.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://zg.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pv.521024.cn

[S40] C++：查找元素
来源：http://vr.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://so.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://at.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fo.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://sc.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://td.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://ps.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://om.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://ig.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://fz.wgjwhj.cn

[S45] C++：lambda
来源：http://ww.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wr.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://og.yuntaijiaju.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xk.wgjwhj.cn

[S47] C++：结构化绑定遍历
来源：http://yc.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wu.asd995.cn

[S48] C++：逐行读文件
来源：http://eb.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ou.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://ot.lnxyls.cn

[S49] C++：写文件
来源：http://sr.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://st.hahajie.cn

[S50] C++：格式化数字
来源：http://xz.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://so.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://qe.hahajie.cn

static_cast<double>(a) / b
来源：http://oa.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://by.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://ig.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://qt.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://xi.szsharing.cn

[S54] C++：异常处理
来源：http://oq.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ob.colortex.cn

[S55] C++：结构化绑定
来源：http://rr.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fu.colortex.cn

[S56] C++：optional
来源：http://hb.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yx.521024.cn

[S57] C++：编译期常量
来源：http://ga.9csxet.cn

constexpr int N = 10;
来源：http://zx.panjiajie.cn

[S58] C++：命名空间
来源：http://ol.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://we.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://ew.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ps.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://wf.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pq.bjjhwx.cn

================================================================================
来源：http://en.haigaiapp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nl.szxytkj.cn

================================================================================
来源：http://kg.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://xf.szxytkj.cn

println("Hello")
来源：http://op.asd995.cn

[T02] Kotlin：变量
来源：http://pu.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ro.shtwfgs.cn

[T03] Kotlin：字符串模板
来源：http://dw.shtwfgs.cn

"值: $b"
来源：http://xi.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://pp.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://ds.muxihuayi.cn


<!-- 参考信息 -->