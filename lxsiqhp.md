代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ee.szsharing.cn

[R10] 正则匹配
来源：http://yd.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zq.yuexingan06.cn

[R11] case 多分支
来源：http://ah.jianghongdianzi.cn

case "$1" in
来源：http://nf.bjjhwx.cn

start) echo "启动" ;;
来源：http://we.gzmigu.cn

stop)  echo "停止" ;;
来源：http://mh.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://pw.shxzskj.cn

esac
来源：http://mu.nicolike.cn

[R12] for 遍历文件
来源：http://os.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://rs.yuntaijiaju.cn

[R13] for 计数循环
来源：http://lr.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://qa.wgjwhj.cn

[R14] C 风格 for
来源：http://lb.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uv.nicolike.cn

[R15] while 逐行读文件
来源：http://lh.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sf.gzmigu.cn

[R16] until 等待条件
来源：http://py.jctech888.com.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zf.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://cb.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://op.jctech888.com.cn

[R18] 遍历数组
来源：http://vh.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ek.nicolike.cn

[R19] 数组长度
来源：http://cp.asd995.cn

echo "${#arr[@]}"
来源：http://zd.asd995.cn

[R20] 关联数组（字典）
来源：http://sn.nszjky.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xg.yuntaijiaju.cn

[R21] 字符串长度
来源：http://vp.yuntaijiaju.cn

echo "${#s}"
来源：http://yj.szxytkj.cn

[R22] 截取子串
来源：http://ms.wgjwhj.cn

echo "${s:0:5}"
来源：http://un.huixiangedu.cn

[R23] 字符串替换
来源：http://au.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jo.shxzskj.cn

[R24] 大小写转换
来源：http://wk.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vn.9csxet.cn

[R25] 去后缀 / 去前缀
来源：http://wv.colortex.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vi.hnjuh.cn

[R26] 命令替换
来源：http://nt.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://ed.lnxyls.cn

[R27] 算术展开
来源：http://nm.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://qz.panjiajie.cn

[R28] 浮点运算
来源：http://iv.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://ue.newstarts.cn

[R29] 定义函数
来源：http://sz.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vk.szsharing.cn

[R30] 函数返回状态码
来源：http://lv.szxytkj.cn

f() { return 0; }; f || echo "失败了"
来源：http://nn.newstarts.cn

[R31] 局部变量
来源：http://id.hnjuh.cn

f() { local x=1; echo "$x"; }
来源：http://qt.521024.cn

[R32] 参数个数校验
来源：http://ho.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sq.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://ua.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fl.szxytkj.cn

[R34] 退出时清理
来源：http://sn.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nj.gzmigu.cn

[R35] 后台执行并等待
来源：http://cl.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gk.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://aw.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mj.hnjuh.cn

[R37] 把输出赋给变量
来源：http://yk.521024.cn

files=$(ls -1)
来源：http://lp.colortex.cn

[R38] 管道串联
来源：http://wk.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://jm.lnxyls.cn

[R39] 重定向标准输出与错误
来源：http://tq.9csxet.cn

cmd > out.log 2>&1
来源：http://vk.panjiajie.cn

[R40] 追加写日志
来源：http://qt.bookmarksfly.cn

echo "log" >> out.log
来源：http://mf.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://gw.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://qx.gzmigu.cn

[R42] 输入重定向
来源：http://zn.shxzukj.cn

wc -l < a.txt
来源：http://wt.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://cu.gzmigu.cn

find . -name "*.log" -type f
来源：http://he.shxzskj.cn

[R44] 按修改时间查找
来源：http://dp.shxzskj.cn

find . -mtime -7 -type f
来源：http://le.huixiangedu.cn

[R45] 批量删除
来源：http://qi.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://mx.colortex.cn

[R46] 递归替换文件内容
来源：http://aa.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rx.shtwfgs.cn

[R47] sed 单行替换
来源：http://en.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://uz.szxytkj.cn

[R48] awk 取指定列
来源：http://wn.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://yj.jianghongdianzi.cn

[R49] awk 带条件
来源：http://li.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ol.shxzskj.cn

[R50] awk 求和
来源：http://na.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xw.nszjky.cn

[R51] 排序去重取前几
来源：http://zm.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ta.chemitech.net.cn

[R52] 统计行数
来源：http://fi.bookmarksfly.cn

wc -l a.txt
来源：http://sg.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://te.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nn.shxzukj.cn

[R54] 比较两个文件
来源：http://ck.chemitech.net.cn

diff a.txt b.txt
来源：http://kk.nszjky.cn

[R55] 压缩与解压
来源：http://rx.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fk.shxzukj.cn

[R56] 远程拷贝
来源：http://co.lnxyls.cn

scp file user@host:/path/
来源：http://df.szsharing.cn

[R57] 远程执行命令
来源：http://zc.chemitech.net.cn

ssh user@host 'uptime'
来源：http://oa.huixiangedu.cn

[R58] 下载文件
来源：http://jq.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oh.haigaiapp.cn

[R59] 发 POST JSON
来源：http://cx.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sp.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://cx.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ep.panjiajie.cn

[R61] 磁盘占用
来源：http://so.hnjuh.cn

df -h;  du -sh *
来源：http://ir.shxzskj.cn

[R62] 找最占空间的文件
来源：http://is.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://fk.nszjky.cn

[R63] 内存与进程
来源：http://tx.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://vl.jianghongdianzi.cn

[R64] 结束进程
来源：http://bu.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://no.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://iv.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qt.huanxung.cn

[R66] 定时任务
来源：http://qj.nszjky.cn

crontab -e;  crontab -l
来源：http://kt.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://fj.shtwfgs.cn

openssl rand -hex 16
来源：http://uk.bjjhwx.cn

[R68] 计算文件校验值
来源：http://hv.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xw.jctech888.com.cn

[R69] 生成随机密码
来源：http://lb.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://ne.huixiangedu.cn

[R70] 时间戳与互转
来源：http://ir.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://ef.huanxung.cn

[R71] 日期格式化
来源：http://ah.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tz.chemitech.net.cn

[R72] 等待端口就绪
来源：http://uq.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jz.shxzukj.cn

[R73] 分割大日志
来源：http://fl.lnxyls.cn

split -l 1000 big.log part_
来源：http://nn.hnjuh.cn

[R74] 批量重命名
来源：http://bt.shxzskj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yz.shtwfgs.cn

[R75] 导出环境变量
来源：http://dh.bjjhwx.cn

export PATH="$HOME/bin:$PATH"
来源：http://ce.9csxet.cn

[R76] 使用临时文件
来源：http://du.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wn.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://hb.colortex.cn

read -rp "请输入: " ans
来源：http://of.yuexingan06.cn

[R78] 交互式菜单
来源：http://hj.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pe.jctech888.com.cn

[R79] 解析命令行选项
来源：http://yt.521024.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yq.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://co.nszjky.cn

time ./run.sh
来源：http://to.muxihuayi.cn

================================================================================
来源：http://le.jianghongdianzi.cn

S. C / C++ 专题
来源：http://fe.9csxet.cn

================================================================================
来源：http://qo.bookmarksfly.cn

[S01] C：Hello World
来源：http://dt.hahajie.cn

#include <stdio.h>
来源：http://xc.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bc.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://xi.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://hp.shxzukj.cn

[S03] C：读入整数
来源：http://sb.colortex.cn

int x; scanf("%d", &x);
来源：http://mt.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://kj.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pw.hahajie.cn

[S05] C：字符串长度
来源：http://gv.bookmarksfly.cn

strlen(s)
来源：http://ix.newstarts.cn

[S06] C：字符串比较
来源：http://kb.szxytkj.cn

strcmp(a, b) == 0
来源：http://vb.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://db.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sg.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://ka.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vs.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://nf.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kb.yuexingan06.cn

[S10] C：指针与解引用
来源：http://sk.huanxung.cn

int *p = &a;  *p = 5;
来源：http://ym.szsharing.cn

[S11] C：逐行读文件
来源：http://cv.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://ab.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tt.hahajie.cn

fclose(f);
来源：http://xt.szxytkj.cn

[S12] C：写文件
来源：http://xn.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dl.jianghongdianzi.cn

[S13] C：宏定义
来源：http://on.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fp.lnxyls.cn

[S14] C：枚举
来源：http://kz.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://za.szsharing.cn

[S15] C：类型转换
来源：http://sl.9csxet.cn

(double) a / b
来源：http://ew.shxzskj.cn

[S16] C：位操作置位
来源：http://ys.gzmigu.cn

x |= (1 << 3);
来源：http://wk.nicolike.cn

[S17] C：安全拼接字符串
来源：http://wu.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kg.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://bi.szsharing.cn

int main(int argc, char **argv)
来源：http://ki.szsharing.cn

[S19] C：快速排序
来源：http://rh.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ov.bookmarksfly.cn

[S20] C：二分查找
来源：http://em.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://as.hahajie.cn

[S21] C：字符类别判断
来源：http://jv.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sz.huixiangedu.cn

[S22] C：字符串转数字
来源：http://eo.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ps.panjiajie.cn

[S23] C：随机数
来源：http://ey.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ay.bjjhwx.cn

[S24] C：获取本地时间
来源：http://rk.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rd.yuexingan06.cn

[S25] C：内存拷贝
来源：http://uj.shxzskj.cn

memcpy(dst, src, n);
来源：http://lu.shxzukj.cn

[S26] C：内存清零
来源：http://ip.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://bg.hahajie.cn

[S27] C：定义常量
来源：http://mx.9csxet.cn

const double PI = 3.14159;
来源：http://ul.huixiangedu.cn

[S28] C：静态变量
来源：http://re.haigaiapp.cn

static int counter = 0;
来源：http://pr.huanxung.cn

[S29] C：变参函数
来源：http://kt.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iw.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://cb.bjjhwx.cn

#ifndef X_H
来源：http://be.newstarts.cn

#define X_H
来源：http://vi.huixinmuqiang.cn

#endif
来源：http://go.chemitech.net.cn

[S31] C++：Hello World
来源：http://it.lnxyls.cn

#include <iostream>
来源：http://zo.yuexingan06.cn

int main() { std::cout << "Hello\n"; }
来源：http://tw.huixiangedu.cn

[S32] C++：字符串
来源：http://wa.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://bp.chemitech.net.cn

[S33] C++：vector 增删
来源：http://ax.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://an.szxytkj.cn

[S34] C++：遍历 vector
来源：http://eg.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://li.hnjuh.cn

[S35] C++：map
来源：http://pa.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nt.panjiajie.cn

[S36] C++：unordered_map
来源：http://rl.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ez.chemitech.net.cn

[S37] C++：set
来源：http://ny.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uh.asd995.cn

[S38] C++：排序
来源：http://gs.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://sj.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://df.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lq.haigaiapp.cn

[S40] C++：查找元素
来源：http://sk.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rj.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://kw.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qe.huanxung.cn

[S42] C++：继承与虚函数
来源：http://lp.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://jb.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://df.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://cg.asd995.cn

[S44] C++：引用传参
来源：http://hl.9csxet.cn

void inc(int &x) { ++x; }
来源：http://vr.gzmigu.cn

[S45] C++：lambda
来源：http://am.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hw.yuexingan06.cn

[S46] C++：函数模板
来源：http://ie.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cb.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://mk.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lp.szsharing.cn

[S48] C++：逐行读文件
来源：http://pp.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jb.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://uh.jianghongdianzi.cn

[S49] C++：写文件
来源：http://uv.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bl.panjiajie.cn

[S50] C++：格式化数字
来源：http://ep.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ip.szxytkj.cn

[S51] C++：显式类型转换
来源：http://cp.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://pb.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://fm.nszjky.cn

int size() const noexcept { return n_; }
来源：http://ea.huixiangedu.cn

[S53] C++：移动语义
来源：http://lx.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://eb.colortex.cn

[S54] C++：异常处理
来源：http://dw.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tl.521024.cn

[S55] C++：结构化绑定
来源：http://xh.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jo.gzmigu.cn

[S56] C++：optional
来源：http://ko.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ez.newstarts.cn

[S57] C++：编译期常量
来源：http://um.yuntaijiaju.cn

constexpr int N = 10;
来源：http://nd.colortex.cn

[S58] C++：命名空间
来源：http://hy.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://ep.szxytkj.cn

[S59] C++：静态断言
来源：http://ep.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ek.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://dt.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uz.lnxyls.cn

================================================================================
来源：http://hc.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oc.gzmigu.cn

================================================================================
来源：http://yz.bjjhwx.cn

[T01] Kotlin：Hello World
来源：http://sh.huixinmuqiang.cn

println("Hello")
来源：http://pn.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://lu.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mr.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://du.wgjwhj.cn

"值: $b"
来源：http://yw.szsharing.cn

[T04] Kotlin：空安全
来源：http://mu.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://rw.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://gd.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mc.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://yq.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oe.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://rg.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://am.szsharing.cn

[T08] Kotlin：数据类
来源：http://db.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://ul.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://gz.asd995.cn

fun String.exclaim() = this + "!"
来源：http://or.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://qo.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://iu.szsharing.cn


<!-- 参考信息 -->