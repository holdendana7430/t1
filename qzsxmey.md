代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kd.shxzukj.cn

[R10] 正则匹配
来源：http://co.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mf.huixiangedu.cn

[R11] case 多分支
来源：http://ku.nszjky.cn

case "$1" in
来源：http://ph.shxzskj.cn

start) echo "启动" ;;
来源：http://ue.panjiajie.cn

stop)  echo "停止" ;;
来源：http://pv.nicolike.cn

*)     echo "未知命令" ;;
来源：http://dq.521024.cn

esac
来源：http://ue.panjiajie.cn

[R12] for 遍历文件
来源：http://vn.shxzskj.cn

for f in *.txt; do echo "$f"; done
来源：http://nv.newstarts.cn

[R13] for 计数循环
来源：http://te.jianghongdianzi.cn

for i in {1..10}; do echo "$i"; done
来源：http://ss.jianghongdianzi.cn

[R14] C 风格 for
来源：http://nk.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jp.szsharing.cn

[R15] while 逐行读文件
来源：http://pn.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ta.yuntaijiaju.cn

[R16] until 等待条件
来源：http://vz.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://or.hahajie.cn

[R17] 数组定义与取值
来源：http://is.bookmarksfly.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mm.szxytkj.cn

[R18] 遍历数组
来源：http://hm.colortex.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xx.yuntaijiaju.cn

[R19] 数组长度
来源：http://rv.jianghongdianzi.cn

echo "${#arr[@]}"
来源：http://ug.hnjuh.cn

[R20] 关联数组（字典）
来源：http://at.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bs.shxzukj.cn

[R21] 字符串长度
来源：http://ki.szxytkj.cn

echo "${#s}"
来源：http://cn.bjjhwx.cn

[R22] 截取子串
来源：http://fo.szxytkj.cn

echo "${s:0:5}"
来源：http://mj.shtwfgs.cn

[R23] 字符串替换
来源：http://nt.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gg.szsharing.cn

[R24] 大小写转换
来源：http://gk.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ve.huixinmuqiang.cn

[R25] 去后缀 / 去前缀
来源：http://op.wgjwhj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://oi.bookmarksfly.cn

[R26] 命令替换
来源：http://sd.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://ra.asd995.cn

[R27] 算术展开
来源：http://nr.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://bn.bjjhwx.cn

[R28] 浮点运算
来源：http://in.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://xl.szsharing.cn

[R29] 定义函数
来源：http://ao.yuntaijiaju.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gw.yuntaijiaju.cn

[R30] 函数返回状态码
来源：http://vn.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://ov.shxzukj.cn

[R31] 局部变量
来源：http://xl.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://qq.yuexingan06.cn

[R32] 参数个数校验
来源：http://yg.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gc.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://zb.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kf.huanxung.cn

[R34] 退出时清理
来源：http://za.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gx.nszjky.cn

[R35] 后台执行并等待
来源：http://ms.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wa.huanxung.cn

[R36] 并发执行多个任务
来源：http://ke.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bv.nszjky.cn

[R37] 把输出赋给变量
来源：http://yf.chemitech.net.cn

files=$(ls -1)
来源：http://nr.lnxyls.cn

[R38] 管道串联
来源：http://il.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://xv.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://rk.szsharing.cn

cmd > out.log 2>&1
来源：http://ce.9csxet.cn

[R40] 追加写日志
来源：http://ss.huixiangedu.cn

echo "log" >> out.log
来源：http://cq.yuexingan06.cn

[R41] 丢弃输出
来源：http://bi.shxzskj.cn

cmd >/dev/null 2>&1
来源：http://sk.muxihuayi.cn

[R42] 输入重定向
来源：http://gi.chemitech.net.cn

wc -l < a.txt
来源：http://wj.gzmigu.cn

[R43] 按名字查找文件
来源：http://ex.bjjhwx.cn

find . -name "*.log" -type f
来源：http://qm.nicolike.cn

[R44] 按修改时间查找
来源：http://ov.nicolike.cn

find . -mtime -7 -type f
来源：http://xf.hnjuh.cn

[R45] 批量删除
来源：http://ma.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://ll.huixiangedu.cn

[R46] 递归替换文件内容
来源：http://mh.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ha.gzmigu.cn

[R47] sed 单行替换
来源：http://id.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ht.newstarts.cn

[R48] awk 取指定列
来源：http://um.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://th.wgjwhj.cn

[R49] awk 带条件
来源：http://zm.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kj.shxzskj.cn

[R50] awk 求和
来源：http://oi.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xs.chemitech.net.cn

[R51] 排序去重取前几
来源：http://sn.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xz.yuntaijiaju.cn

[R52] 统计行数
来源：http://iy.huanxung.cn

wc -l a.txt
来源：http://hf.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://lp.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ip.panjiajie.cn

[R54] 比较两个文件
来源：http://my.asd995.cn

diff a.txt b.txt
来源：http://ch.lnxyls.cn

[R55] 压缩与解压
来源：http://wh.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gr.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://rb.muxihuayi.cn

scp file user@host:/path/
来源：http://vo.bookmarksfly.cn

[R57] 远程执行命令
来源：http://lo.szsharing.cn

ssh user@host 'uptime'
来源：http://iw.asd995.cn

[R58] 下载文件
来源：http://xz.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ai.shtwfgs.cn

[R59] 发 POST JSON
来源：http://fk.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ld.wgjwhj.cn

[R60] 只看 HTTP 状态码
来源：http://jf.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qu.haigaiapp.cn

[R61] 磁盘占用
来源：http://kq.bjjhwx.cn

df -h;  du -sh *
来源：http://cl.asd995.cn

[R62] 找最占空间的文件
来源：http://ol.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://aa.nicolike.cn

[R63] 内存与进程
来源：http://hg.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://wo.newstarts.cn

[R64] 结束进程
来源：http://vx.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://re.lnxyls.cn

[R65] 查看端口占用
来源：http://rx.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uo.shxzukj.cn

[R66] 定时任务
来源：http://nr.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://ib.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://tl.huanxung.cn

openssl rand -hex 16
来源：http://pr.hnjuh.cn

[R68] 计算文件校验值
来源：http://am.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bm.bookmarksfly.cn

[R69] 生成随机密码
来源：http://mi.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://nw.newstarts.cn

[R70] 时间戳与互转
来源：http://kv.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://yg.hahajie.cn

[R71] 日期格式化
来源：http://sn.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uk.chemitech.net.cn

[R72] 等待端口就绪
来源：http://js.newstarts.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vq.lnxyls.cn

[R73] 分割大日志
来源：http://mh.bjjhwx.cn

split -l 1000 big.log part_
来源：http://zo.huixinmuqiang.cn

[R74] 批量重命名
来源：http://lm.haigaiapp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pg.shxzskj.cn

[R75] 导出环境变量
来源：http://ux.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://yi.szxytkj.cn

[R76] 使用临时文件
来源：http://fr.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jg.521024.cn

[R77] 读取用户输入
来源：http://ni.huanxung.cn

read -rp "请输入: " ans
来源：http://uv.lnxyls.cn

[R78] 交互式菜单
来源：http://vi.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mb.chemitech.net.cn

[R79] 解析命令行选项
来源：http://yz.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ga.shxzukj.cn

[R80] 查看脚本执行耗时
来源：http://qv.shtwfgs.cn

time ./run.sh
来源：http://gg.521024.cn

================================================================================
来源：http://jh.colortex.cn

S. C / C++ 专题
来源：http://ye.szxytkj.cn

================================================================================
来源：http://xe.lnxyls.cn

[S01] C：Hello World
来源：http://rm.shxzskj.cn

#include <stdio.h>
来源：http://bh.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qb.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://op.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://wd.haigaiapp.cn

[S03] C：读入整数
来源：http://nk.szxytkj.cn

int x; scanf("%d", &x);
来源：http://sk.nicolike.cn

[S04] C：字符串复制
来源：http://ma.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xu.chemitech.net.cn

[S05] C：字符串长度
来源：http://ro.9csxet.cn

strlen(s)
来源：http://kq.huanxung.cn

[S06] C：字符串比较
来源：http://qb.haigaiapp.cn

strcmp(a, b) == 0
来源：http://an.shxzskj.cn

[S07] C：数组遍历求和
来源：http://rx.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jt.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://ti.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sm.521024.cn

[S09] C：结构体定义与初始化
来源：http://ua.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ji.haigaiapp.cn

[S10] C：指针与解引用
来源：http://ff.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://fi.nicolike.cn

[S11] C：逐行读文件
来源：http://qs.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://xj.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jq.szsharing.cn

fclose(f);
来源：http://xh.hahajie.cn

[S12] C：写文件
来源：http://it.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jx.bookmarksfly.cn

[S13] C：宏定义
来源：http://vz.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pd.huanxung.cn

[S14] C：枚举
来源：http://sf.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://pi.yuexingan06.cn

[S15] C：类型转换
来源：http://px.szxytkj.cn

(double) a / b
来源：http://bm.9csxet.cn

[S16] C：位操作置位
来源：http://ze.hahajie.cn

x |= (1 << 3);
来源：http://iz.asd995.cn

[S17] C：安全拼接字符串
来源：http://ul.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sr.bjjhwx.cn

[S18] C：命令行参数
来源：http://qa.nszjky.cn

int main(int argc, char **argv)
来源：http://yt.huixinmuqiang.cn

[S19] C：快速排序
来源：http://fk.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ar.nicolike.cn

[S20] C：二分查找
来源：http://an.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nx.nicolike.cn

[S21] C：字符类别判断
来源：http://eq.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ut.chemitech.net.cn

[S22] C：字符串转数字
来源：http://ff.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ts.nicolike.cn

[S23] C：随机数
来源：http://ns.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://in.shxzukj.cn

[S24] C：获取本地时间
来源：http://mg.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rz.szsharing.cn

[S25] C：内存拷贝
来源：http://aj.yuexingan06.cn

memcpy(dst, src, n);
来源：http://ah.lnxyls.cn

[S26] C：内存清零
来源：http://lm.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://ug.jctech888.com.cn

[S27] C：定义常量
来源：http://by.jctech888.com.cn

const double PI = 3.14159;
来源：http://wr.shxzskj.cn

[S28] C：静态变量
来源：http://oe.shxzskj.cn

static int counter = 0;
来源：http://hr.shxzukj.cn

[S29] C：变参函数
来源：http://ie.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gr.newstarts.cn

[S30] C：头文件保护
来源：http://zn.521024.cn

#ifndef X_H
来源：http://bg.shtwfgs.cn

#define X_H
来源：http://oq.asd995.cn

#endif
来源：http://ok.hnjuh.cn

[S31] C++：Hello World
来源：http://sy.asd995.cn

#include <iostream>
来源：http://ut.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://do.shxzukj.cn

[S32] C++：字符串
来源：http://is.521024.cn

std::string s = "hi";  s += "!";
来源：http://ie.panjiajie.cn

[S33] C++：vector 增删
来源：http://ww.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bk.hahajie.cn

[S34] C++：遍历 vector
来源：http://il.szxytkj.cn

for (auto &x : v) { std::cout << x; }
来源：http://xg.szsharing.cn

[S35] C++：map
来源：http://ad.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sp.nicolike.cn

[S36] C++：unordered_map
来源：http://ma.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gw.shxzskj.cn

[S37] C++：set
来源：http://mb.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fr.9csxet.cn

[S38] C++：排序
来源：http://hh.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://za.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://ld.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sl.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://uu.nicolike.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://co.szsharing.cn

[S41] C++：类与构造函数
来源：http://xc.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gb.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://xz.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://je.huanxung.cn

[S43] C++：智能指针
来源：http://wg.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://gy.szxytkj.cn

[S44] C++：引用传参
来源：http://xu.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://xf.yuntaijiaju.cn

[S45] C++：lambda
来源：http://se.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nn.hahajie.cn

[S46] C++：函数模板
来源：http://vw.yuntaijiaju.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vk.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://fd.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://je.panjiajie.cn

[S48] C++：逐行读文件
来源：http://sc.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ne.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://jk.lnxyls.cn

[S49] C++：写文件
来源：http://li.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hd.gzmigu.cn

[S50] C++：格式化数字
来源：http://ii.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tl.colortex.cn

[S51] C++：显式类型转换
来源：http://cv.newstarts.cn

static_cast<double>(a) / b
来源：http://pu.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://fk.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://cn.muxihuayi.cn

[S53] C++：移动语义
来源：http://cg.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://wr.lnxyls.cn

[S54] C++：异常处理
来源：http://sv.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://af.shxzukj.cn

[S55] C++：结构化绑定
来源：http://oo.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://su.shxzukj.cn

[S56] C++：optional
来源：http://ii.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bo.nicolike.cn

[S57] C++：编译期常量
来源：http://ow.nszjky.cn

constexpr int N = 10;
来源：http://qv.shxzukj.cn

[S58] C++：命名空间
来源：http://tx.521024.cn

namespace ns { int f() { return 1; } }
来源：http://op.gzmigu.cn

[S59] C++：静态断言
来源：http://su.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zz.bjjhwx.cn

[S60] C++：遍历并删除元素
来源：http://ty.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gd.colortex.cn

================================================================================
来源：http://wa.gzmigu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xe.shtwfgs.cn

================================================================================
来源：http://wb.huanxung.cn

[T01] Kotlin：Hello World
来源：http://lo.huixiangedu.cn

println("Hello")
来源：http://kr.szxytkj.cn

[T02] Kotlin：变量
来源：http://dk.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://og.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://ts.asd995.cn

"值: $b"
来源：http://sy.shxzukj.cn

[T04] Kotlin：空安全
来源：http://ou.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://fj.9csxet.cn

[T05] Kotlin：when 表达式
来源：http://mc.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fs.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://ma.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://iq.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://tf.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ul.lnxyls.cn

[T08] Kotlin：数据类
来源：http://gd.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://re.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://ex.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://lj.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://ly.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tz.521024.cn


<!-- 参考信息 -->