代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gl.521024.cn

[R08] 数值比较
来源：http://fl.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ua.hahajie.cn

[R09] 字符串比较
来源：http://ll.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oh.shxzukj.cn

[R10] 正则匹配
来源：http://qh.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ys.bookmarksfly.cn

[R11] case 多分支
来源：http://lk.newstarts.cn

case "$1" in
来源：http://vt.9csxet.cn

start) echo "启动" ;;
来源：http://bc.hnjuh.cn

stop)  echo "停止" ;;
来源：http://jb.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://hs.szsharing.cn

esac
来源：http://rv.haigaiapp.cn

[R12] for 遍历文件
来源：http://ph.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://eo.newstarts.cn

[R13] for 计数循环
来源：http://xo.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://aa.nicolike.cn

[R14] C 风格 for
来源：http://cc.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ht.nicolike.cn

[R15] while 逐行读文件
来源：http://tg.yuexingan06.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://co.jctech888.com.cn

[R16] until 等待条件
来源：http://ta.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://or.newstarts.cn

[R17] 数组定义与取值
来源：http://fp.hahajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yh.newstarts.cn

[R18] 遍历数组
来源：http://gq.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rq.huixinmuqiang.cn

[R19] 数组长度
来源：http://py.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://xr.newstarts.cn

[R20] 关联数组（字典）
来源：http://uu.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://br.hnjuh.cn

[R21] 字符串长度
来源：http://dq.muxihuayi.cn

echo "${#s}"
来源：http://qs.bookmarksfly.cn

[R22] 截取子串
来源：http://ro.shtwfgs.cn

echo "${s:0:5}"
来源：http://gr.panjiajie.cn

[R23] 字符串替换
来源：http://uk.chemitech.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kv.nicolike.cn

[R24] 大小写转换
来源：http://xr.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wc.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://ic.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sb.shxzskj.cn

[R26] 命令替换
来源：http://cm.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://rg.colortex.cn

[R27] 算术展开
来源：http://dy.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://ae.bookmarksfly.cn

[R28] 浮点运算
来源：http://ol.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://hy.bookmarksfly.cn

[R29] 定义函数
来源：http://sg.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zj.hnjuh.cn

[R30] 函数返回状态码
来源：http://qo.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://vs.bookmarksfly.cn

[R31] 局部变量
来源：http://kz.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://pr.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://ov.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tv.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://mx.hnjuh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cp.huixinmuqiang.cn

[R34] 退出时清理
来源：http://sw.chemitech.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zq.bookmarksfly.cn

[R35] 后台执行并等待
来源：http://xo.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cw.asd995.cn

[R36] 并发执行多个任务
来源：http://cq.muxihuayi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mb.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://ei.gzmigu.cn

files=$(ls -1)
来源：http://ya.chemitech.net.cn

[R38] 管道串联
来源：http://bb.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://pw.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://sy.chemitech.net.cn

cmd > out.log 2>&1
来源：http://iz.chemitech.net.cn

[R40] 追加写日志
来源：http://jr.colortex.cn

echo "log" >> out.log
来源：http://pr.colortex.cn

[R41] 丢弃输出
来源：http://qj.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://ck.muxihuayi.cn

[R42] 输入重定向
来源：http://zd.gzmigu.cn

wc -l < a.txt
来源：http://fh.colortex.cn

[R43] 按名字查找文件
来源：http://sm.wgjwhj.cn

find . -name "*.log" -type f
来源：http://vg.gzmigu.cn

[R44] 按修改时间查找
来源：http://bl.9csxet.cn

find . -mtime -7 -type f
来源：http://ob.jctech888.com.cn

[R45] 批量删除
来源：http://pa.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://tx.shxzskj.cn

[R46] 递归替换文件内容
来源：http://ir.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zr.gzmigu.cn

[R47] sed 单行替换
来源：http://or.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sq.gzmigu.cn

[R48] awk 取指定列
来源：http://zc.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://jj.wgjwhj.cn

[R49] awk 带条件
来源：http://vj.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kv.huixiangedu.cn

[R50] awk 求和
来源：http://ys.colortex.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jr.chemitech.net.cn

[R51] 排序去重取前几
来源：http://hx.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gf.yuntaijiaju.cn

[R52] 统计行数
来源：http://vf.huanxung.cn

wc -l a.txt
来源：http://vx.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://qj.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gr.shtwfgs.cn

[R54] 比较两个文件
来源：http://kk.lnxyls.cn

diff a.txt b.txt
来源：http://tf.nicolike.cn

[R55] 压缩与解压
来源：http://by.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qo.shtwfgs.cn

[R56] 远程拷贝
来源：http://sm.521024.cn

scp file user@host:/path/
来源：http://ey.haigaiapp.cn

[R57] 远程执行命令
来源：http://bx.shxzskj.cn

ssh user@host 'uptime'
来源：http://ca.521024.cn

[R58] 下载文件
来源：http://mq.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qc.hahajie.cn

[R59] 发 POST JSON
来源：http://ou.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ms.nicolike.cn

[R60] 只看 HTTP 状态码
来源：http://eo.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ah.szxytkj.cn

[R61] 磁盘占用
来源：http://es.jctech888.com.cn

df -h;  du -sh *
来源：http://bf.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://bc.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://vg.hnjuh.cn

[R63] 内存与进程
来源：http://ds.colortex.cn

free -h;  ps aux | grep nginx
来源：http://os.hnjuh.cn

[R64] 结束进程
来源：http://hv.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://xs.colortex.cn

[R65] 查看端口占用
来源：http://rk.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qa.gzmigu.cn

[R66] 定时任务
来源：http://zm.chemitech.net.cn

crontab -e;  crontab -l
来源：http://xe.jctech888.com.cn

[R67] 生成随机十六进制串
来源：http://ge.gzmigu.cn

openssl rand -hex 16
来源：http://mi.asd995.cn

[R68] 计算文件校验值
来源：http://ja.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vk.nicolike.cn

[R69] 生成随机密码
来源：http://ia.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://qz.haigaiapp.cn

[R70] 时间戳与互转
来源：http://kf.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://rg.shtwfgs.cn

[R71] 日期格式化
来源：http://cn.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kn.shxzukj.cn

[R72] 等待端口就绪
来源：http://xj.newstarts.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jy.szsharing.cn

[R73] 分割大日志
来源：http://ye.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://us.jctech888.com.cn

[R74] 批量重命名
来源：http://ww.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yy.hnjuh.cn

[R75] 导出环境变量
来源：http://ra.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://zh.hahajie.cn

[R76] 使用临时文件
来源：http://fm.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kk.hnjuh.cn

[R77] 读取用户输入
来源：http://gs.huanxung.cn

read -rp "请输入: " ans
来源：http://cw.hnjuh.cn

[R78] 交互式菜单
来源：http://co.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://un.gzmigu.cn

[R79] 解析命令行选项
来源：http://rx.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gh.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://wn.nszjky.cn

time ./run.sh
来源：http://fa.bjjhwx.cn

================================================================================
来源：http://qd.hahajie.cn

S. C / C++ 专题
来源：http://tb.lnxyls.cn

================================================================================
来源：http://yf.huixinmuqiang.cn

[S01] C：Hello World
来源：http://pd.colortex.cn

#include <stdio.h>
来源：http://jg.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wv.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://fl.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://cz.lnxyls.cn

[S03] C：读入整数
来源：http://po.shxzukj.cn

int x; scanf("%d", &x);
来源：http://vs.hahajie.cn

[S04] C：字符串复制
来源：http://yk.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xf.hahajie.cn

[S05] C：字符串长度
来源：http://ww.9csxet.cn

strlen(s)
来源：http://pq.szsharing.cn

[S06] C：字符串比较
来源：http://pi.colortex.cn

strcmp(a, b) == 0
来源：http://br.hahajie.cn

[S07] C：数组遍历求和
来源：http://og.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hy.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://ms.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wl.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://ff.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ub.bjjhwx.cn

[S10] C：指针与解引用
来源：http://or.hahajie.cn

int *p = &a;  *p = 5;
来源：http://jx.nicolike.cn

[S11] C：逐行读文件
来源：http://ag.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://mf.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wy.jianghongdianzi.cn

fclose(f);
来源：http://ic.haigaiapp.cn

[S12] C：写文件
来源：http://bj.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qf.panjiajie.cn

[S13] C：宏定义
来源：http://fb.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yv.shxzukj.cn

[S14] C：枚举
来源：http://kj.szsharing.cn

enum Color { RED, GREEN, BLUE };
来源：http://kn.asd995.cn

[S15] C：类型转换
来源：http://ef.9csxet.cn

(double) a / b
来源：http://dl.nicolike.cn

[S16] C：位操作置位
来源：http://qg.huixinmuqiang.cn

x |= (1 << 3);
来源：http://ks.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://pw.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wp.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://fb.chemitech.net.cn

int main(int argc, char **argv)
来源：http://se.hahajie.cn

[S19] C：快速排序
来源：http://tp.gzmigu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fe.newstarts.cn

[S20] C：二分查找
来源：http://br.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xp.panjiajie.cn

[S21] C：字符类别判断
来源：http://sd.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iu.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://jh.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://in.muxihuayi.cn

[S23] C：随机数
来源：http://gr.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ly.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://iu.521024.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ii.nszjky.cn

[S25] C：内存拷贝
来源：http://xh.lnxyls.cn

memcpy(dst, src, n);
来源：http://ke.newstarts.cn

[S26] C：内存清零
来源：http://hk.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://ms.muxihuayi.cn

[S27] C：定义常量
来源：http://da.chemitech.net.cn

const double PI = 3.14159;
来源：http://tc.jianghongdianzi.cn

[S28] C：静态变量
来源：http://du.huixinmuqiang.cn

static int counter = 0;
来源：http://bd.lnxyls.cn

[S29] C：变参函数
来源：http://mq.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gr.colortex.cn

[S30] C：头文件保护
来源：http://zr.bjjhwx.cn

#ifndef X_H
来源：http://rd.yuexingan06.cn

#define X_H
来源：http://hv.szsharing.cn

#endif
来源：http://xj.shtwfgs.cn

[S31] C++：Hello World
来源：http://nz.bjjhwx.cn

#include <iostream>
来源：http://nq.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://ih.bjjhwx.cn

[S32] C++：字符串
来源：http://bv.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://sd.nszjky.cn

[S33] C++：vector 增删
来源：http://sh.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jb.shxzukj.cn

[S34] C++：遍历 vector
来源：http://np.shxzskj.cn

for (auto &x : v) { std::cout << x; }
来源：http://qn.chemitech.net.cn

[S35] C++：map
来源：http://sj.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lt.521024.cn

[S36] C++：unordered_map
来源：http://qv.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ls.muxihuayi.cn

[S37] C++：set
来源：http://pa.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ef.haigaiapp.cn

[S38] C++：排序
来源：http://vt.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://wb.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://rw.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lz.hnjuh.cn

[S40] C++：查找元素
来源：http://bg.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yz.gzmigu.cn

[S41] C++：类与构造函数
来源：http://am.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ih.huanxung.cn

[S42] C++：继承与虚函数
来源：http://ug.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://wd.bjjhwx.cn

[S43] C++：智能指针
来源：http://ec.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://gg.nicolike.cn

[S44] C++：引用传参
来源：http://an.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://nl.shxzukj.cn

[S45] C++：lambda
来源：http://oi.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ne.huanxung.cn

[S46] C++：函数模板
来源：http://nr.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wt.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://aj.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fh.huanxung.cn

[S48] C++：逐行读文件
来源：http://zx.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zu.szsharing.cn

while (std::getline(in, line)) { }
来源：http://gi.nszjky.cn

[S49] C++：写文件
来源：http://ia.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dj.nszjky.cn

[S50] C++：格式化数字
来源：http://nt.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aa.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://ku.yuntaijiaju.cn

static_cast<double>(a) / b
来源：http://bi.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://gu.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://am.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://xa.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://hb.shxzukj.cn

[S54] C++：异常处理
来源：http://on.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dr.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://ei.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mh.gzmigu.cn

[S56] C++：optional
来源：http://fb.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zi.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://uw.newstarts.cn

constexpr int N = 10;
来源：http://nm.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://gc.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://ej.szxytkj.cn

[S59] C++：静态断言
来源：http://ig.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mc.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://qv.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zz.colortex.cn

================================================================================
来源：http://so.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vl.shxzskj.cn

================================================================================
来源：http://kk.szxytkj.cn

[T01] Kotlin：Hello World
来源：http://kv.bookmarksfly.cn

println("Hello")
来源：http://ae.szxytkj.cn

[T02] Kotlin：变量
来源：http://ym.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vq.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://el.bjjhwx.cn

"值: $b"
来源：http://ox.hnjuh.cn

[T04] Kotlin：空安全
来源：http://sm.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://lk.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://ak.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jw.521024.cn

[T06] Kotlin：集合映射
来源：http://qs.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nx.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://er.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nx.colortex.cn

[T08] Kotlin：数据类
来源：http://mu.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://me.huixinmuqiang.cn


<!-- 参考信息 -->