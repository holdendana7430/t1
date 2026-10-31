代发 wailian999

readonly PI=3.14
来源：http://sr.shxzukj.cn

[R04] 位置参数
来源：http://au.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ox.shxzskj.cn

[R05] 参数默认值
来源：http://uu.9csxet.cn

name="${1:-default}"
来源：http://jh.asd995.cn

[R06] 判断命令是否存在
来源：http://px.bjjhwx.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://et.lnxyls.cn

[R07] if 判断文件
来源：http://yg.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eu.huixiangedu.cn

[R08] 数值比较
来源：http://bc.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zt.hnjuh.cn

[R09] 字符串比较
来源：http://ia.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zt.hahajie.cn

[R10] 正则匹配
来源：http://zo.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kf.hahajie.cn

[R11] case 多分支
来源：http://fl.colortex.cn

case "$1" in
来源：http://nc.colortex.cn

start) echo "启动" ;;
来源：http://ks.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://yn.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://oc.nicolike.cn

esac
来源：http://hz.shtwfgs.cn

[R12] for 遍历文件
来源：http://kj.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://qc.9csxet.cn

[R13] for 计数循环
来源：http://br.szsharing.cn

for i in {1..10}; do echo "$i"; done
来源：http://ex.asd995.cn

[R14] C 风格 for
来源：http://gd.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://od.huanxung.cn

[R15] while 逐行读文件
来源：http://rc.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fw.shtwfgs.cn

[R16] until 等待条件
来源：http://ig.newstarts.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fo.lnxyls.cn

[R17] 数组定义与取值
来源：http://pi.muxihuayi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qi.newstarts.cn

[R18] 遍历数组
来源：http://ok.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mz.gzmigu.cn

[R19] 数组长度
来源：http://il.nicolike.cn

echo "${#arr[@]}"
来源：http://mw.newstarts.cn

[R20] 关联数组（字典）
来源：http://pw.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://up.szxytkj.cn

[R21] 字符串长度
来源：http://tj.huixinmuqiang.cn

echo "${#s}"
来源：http://xz.asd995.cn

[R22] 截取子串
来源：http://nt.colortex.cn

echo "${s:0:5}"
来源：http://na.jianghongdianzi.cn

[R23] 字符串替换
来源：http://pi.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yf.panjiajie.cn

[R24] 大小写转换
来源：http://vv.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://so.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://bw.lnxyls.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mg.chemitech.net.cn

[R26] 命令替换
来源：http://fn.nicolike.cn

now=$(date +%F); echo "$now"
来源：http://sh.lnxyls.cn

[R27] 算术展开
来源：http://ch.asd995.cn

echo $((1 + 2 * 3))
来源：http://cu.lnxyls.cn

[R28] 浮点运算
来源：http://kq.521024.cn

echo "scale=2; 10/3" | bc
来源：http://ua.lnxyls.cn

[R29] 定义函数
来源：http://cf.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fd.colortex.cn

[R30] 函数返回状态码
来源：http://ix.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://qj.yuntaijiaju.cn

[R31] 局部变量
来源：http://oq.gzmigu.cn

f() { local x=1; echo "$x"; }
来源：http://bd.chemitech.net.cn

[R32] 参数个数校验
来源：http://hy.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xl.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://sc.asd995.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fj.colortex.cn

[R34] 退出时清理
来源：http://tw.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ek.haigaiapp.cn

[R35] 后台执行并等待
来源：http://mh.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wk.jianghongdianzi.cn

[R36] 并发执行多个任务
来源：http://ff.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pi.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://fy.wgjwhj.cn

files=$(ls -1)
来源：http://pf.chemitech.net.cn

[R38] 管道串联
来源：http://vo.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://ha.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://we.yuexingan06.cn

cmd > out.log 2>&1
来源：http://fe.newstarts.cn

[R40] 追加写日志
来源：http://pi.szsharing.cn

echo "log" >> out.log
来源：http://vu.huanxung.cn

[R41] 丢弃输出
来源：http://re.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://ub.hnjuh.cn

[R42] 输入重定向
来源：http://zm.asd995.cn

wc -l < a.txt
来源：http://jy.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://gr.wgjwhj.cn

find . -name "*.log" -type f
来源：http://pn.nszjky.cn

[R44] 按修改时间查找
来源：http://up.gzmigu.cn

find . -mtime -7 -type f
来源：http://it.hnjuh.cn

[R45] 批量删除
来源：http://sr.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://nr.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://an.asd995.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jk.szxytkj.cn

[R47] sed 单行替换
来源：http://dk.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pu.bjjhwx.cn

[R48] awk 取指定列
来源：http://lh.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://an.9csxet.cn

[R49] awk 带条件
来源：http://jv.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wo.521024.cn

[R50] awk 求和
来源：http://cv.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yt.shxzskj.cn

[R51] 排序去重取前几
来源：http://ct.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xh.asd995.cn

[R52] 统计行数
来源：http://cu.huixiangedu.cn

wc -l a.txt
来源：http://ah.yuntaijiaju.cn

[R53] 查看文件头与实时尾
来源：http://oh.lnxyls.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yb.panjiajie.cn

[R54] 比较两个文件
来源：http://sy.szsharing.cn

diff a.txt b.txt
来源：http://qu.shxzukj.cn

[R55] 压缩与解压
来源：http://mc.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://la.wgjwhj.cn

[R56] 远程拷贝
来源：http://ow.huanxung.cn

scp file user@host:/path/
来源：http://jc.muxihuayi.cn

[R57] 远程执行命令
来源：http://dh.nicolike.cn

ssh user@host 'uptime'
来源：http://kn.shtwfgs.cn

[R58] 下载文件
来源：http://cf.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uf.shxzukj.cn

[R59] 发 POST JSON
来源：http://zb.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wv.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://kb.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ou.huixiangedu.cn

[R61] 磁盘占用
来源：http://ql.jctech888.com.cn

df -h;  du -sh *
来源：http://ym.szxytkj.cn

[R62] 找最占空间的文件
来源：http://xg.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://qg.yuntaijiaju.cn

[R63] 内存与进程
来源：http://gh.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://fz.jianghongdianzi.cn

[R64] 结束进程
来源：http://pg.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://pv.shxzskj.cn

[R65] 查看端口占用
来源：http://yj.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bz.shxzukj.cn

[R66] 定时任务
来源：http://xs.hahajie.cn

crontab -e;  crontab -l
来源：http://io.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://fw.colortex.cn

openssl rand -hex 16
来源：http://ge.newstarts.cn

[R68] 计算文件校验值
来源：http://ok.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dj.huanxung.cn

[R69] 生成随机密码
来源：http://yc.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://ds.haigaiapp.cn

[R70] 时间戳与互转
来源：http://dl.szsharing.cn

date +%s;  date -d @1700000000
来源：http://tl.huixiangedu.cn

[R71] 日期格式化
来源：http://tg.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hm.huanxung.cn

[R72] 等待端口就绪
来源：http://jc.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yh.shxzukj.cn

[R73] 分割大日志
来源：http://pp.gzmigu.cn

split -l 1000 big.log part_
来源：http://ua.nicolike.cn

[R74] 批量重命名
来源：http://gv.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vf.haigaiapp.cn

[R75] 导出环境变量
来源：http://uj.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://ib.huixiangedu.cn

[R76] 使用临时文件
来源：http://ae.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kg.panjiajie.cn

[R77] 读取用户输入
来源：http://py.chemitech.net.cn

read -rp "请输入: " ans
来源：http://yw.szxytkj.cn

[R78] 交互式菜单
来源：http://jd.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ol.hahajie.cn

[R79] 解析命令行选项
来源：http://bq.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xs.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://bf.yuntaijiaju.cn

time ./run.sh
来源：http://wz.chemitech.net.cn

================================================================================
来源：http://sk.huanxung.cn

S. C / C++ 专题
来源：http://vv.szxytkj.cn

================================================================================
来源：http://rd.yuexingan06.cn

[S01] C：Hello World
来源：http://er.nszjky.cn

#include <stdio.h>
来源：http://co.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://km.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://yg.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://rw.huixiangedu.cn

[S03] C：读入整数
来源：http://uj.nicolike.cn

int x; scanf("%d", &x);
来源：http://ip.yuexingan06.cn

[S04] C：字符串复制
来源：http://ht.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pi.szxytkj.cn

[S05] C：字符串长度
来源：http://jv.lnxyls.cn

strlen(s)
来源：http://ip.huanxung.cn

[S06] C：字符串比较
来源：http://ob.hahajie.cn

strcmp(a, b) == 0
来源：http://ao.colortex.cn

[S07] C：数组遍历求和
来源：http://et.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gy.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://zt.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gy.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://rj.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uw.nszjky.cn

[S10] C：指针与解引用
来源：http://cx.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://uy.chemitech.net.cn

[S11] C：逐行读文件
来源：http://jd.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://bi.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gc.jianghongdianzi.cn

fclose(f);
来源：http://vz.jianghongdianzi.cn

[S12] C：写文件
来源：http://lw.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ec.hahajie.cn

[S13] C：宏定义
来源：http://oy.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wv.jctech888.com.cn

[S14] C：枚举
来源：http://lq.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://ge.huixinmuqiang.cn

[S15] C：类型转换
来源：http://nn.shxzukj.cn

(double) a / b
来源：http://si.szsharing.cn

[S16] C：位操作置位
来源：http://kh.521024.cn

x |= (1 << 3);
来源：http://tr.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://gg.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pq.shxzukj.cn

[S18] C：命令行参数
来源：http://vt.asd995.cn

int main(int argc, char **argv)
来源：http://ed.haigaiapp.cn

[S19] C：快速排序
来源：http://ga.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://er.huixiangedu.cn

[S20] C：二分查找
来源：http://wg.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uo.newstarts.cn

[S21] C：字符类别判断
来源：http://ni.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pr.hahajie.cn

[S22] C：字符串转数字
来源：http://kn.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gf.bjjhwx.cn

[S23] C：随机数
来源：http://ha.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lj.jctech888.com.cn

[S24] C：获取本地时间
来源：http://dn.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gh.asd995.cn

[S25] C：内存拷贝
来源：http://rc.wgjwhj.cn

memcpy(dst, src, n);
来源：http://sc.yuntaijiaju.cn

[S26] C：内存清零
来源：http://fo.colortex.cn

memset(a, 0, sizeof a);
来源：http://db.nicolike.cn

[S27] C：定义常量
来源：http://es.szxytkj.cn

const double PI = 3.14159;
来源：http://pq.panjiajie.cn

[S28] C：静态变量
来源：http://kd.asd995.cn

static int counter = 0;
来源：http://ms.9csxet.cn

[S29] C：变参函数
来源：http://rj.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qv.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://zt.shxzskj.cn

#ifndef X_H
来源：http://zy.nicolike.cn

#define X_H
来源：http://ef.521024.cn

#endif
来源：http://yh.szxytkj.cn

[S31] C++：Hello World
来源：http://tl.9csxet.cn

#include <iostream>
来源：http://in.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://ze.wgjwhj.cn

[S32] C++：字符串
来源：http://ri.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://bo.muxihuayi.cn

[S33] C++：vector 增删
来源：http://xy.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zj.szxytkj.cn

[S34] C++：遍历 vector
来源：http://pj.szxytkj.cn

for (auto &x : v) { std::cout << x; }
来源：http://ca.szxytkj.cn

[S35] C++：map
来源：http://qp.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mn.lnxyls.cn

[S36] C++：unordered_map
来源：http://ll.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yy.bookmarksfly.cn

[S37] C++：set
来源：http://xg.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oh.colortex.cn

[S38] C++：排序
来源：http://ku.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://lv.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://ua.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uj.newstarts.cn

[S40] C++：查找元素
来源：http://ou.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lx.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://iz.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hj.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://dc.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://pl.haigaiapp.cn

[S43] C++：智能指针
来源：http://fk.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://sn.muxihuayi.cn

[S44] C++：引用传参
来源：http://hz.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://lt.huixiangedu.cn

[S45] C++：lambda
来源：http://oq.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qu.colortex.cn

[S46] C++：函数模板
来源：http://gv.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rn.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://rd.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kq.hnjuh.cn

[S48] C++：逐行读文件
来源：http://tg.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://de.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://gd.shtwfgs.cn

[S49] C++：写文件
来源：http://qt.chemitech.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rb.lnxyls.cn

[S50] C++：格式化数字
来源：http://ua.shtwfgs.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gh.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://bs.yuntaijiaju.cn

static_cast<double>(a) / b
来源：http://vd.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://go.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://wh.nicolike.cn

[S53] C++：移动语义
来源：http://kn.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://tl.szsharing.cn

[S54] C++：异常处理
来源：http://cs.chemitech.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ju.huixiangedu.cn

[S55] C++：结构化绑定
来源：http://az.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mj.colortex.cn

[S56] C++：optional
来源：http://ms.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ng.bjjhwx.cn

[S57] C++：编译期常量
来源：http://vr.bookmarksfly.cn

constexpr int N = 10;
来源：http://iy.wgjwhj.cn

[S58] C++：命名空间
来源：http://xq.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://is.9csxet.cn

[S59] C++：静态断言
来源：http://mu.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cr.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://ws.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qt.asd995.cn

================================================================================
来源：http://wx.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://im.muxihuayi.cn

================================================================================
来源：http://mx.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://fa.huixiangedu.cn

println("Hello")
来源：http://hz.colortex.cn

[T02] Kotlin：变量
来源：http://ws.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wp.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://lz.wgjwhj.cn

"值: $b"
来源：http://xb.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://oy.lnxyls.cn

val n: String? = null;  n?.length
来源：http://px.nicolike.cn


<!-- 参考信息 -->