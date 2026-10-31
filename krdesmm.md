代发 wailian999

name="${1:-default}"
来源：http://nm.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://oo.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bh.hahajie.cn

[R07] if 判断文件
来源：http://op.bjjhwx.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rl.shxzukj.cn

[R08] 数值比较
来源：http://sl.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wl.haigaiapp.cn

[R09] 字符串比较
来源：http://nl.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yu.jianghongdianzi.cn

[R10] 正则匹配
来源：http://zf.muxihuayi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bn.huanxung.cn

[R11] case 多分支
来源：http://lm.nicolike.cn

case "$1" in
来源：http://fl.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://dj.gzmigu.cn

stop)  echo "停止" ;;
来源：http://ee.asd995.cn

*)     echo "未知命令" ;;
来源：http://va.bjjhwx.cn

esac
来源：http://ut.szxytkj.cn

[R12] for 遍历文件
来源：http://pp.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://rj.haigaiapp.cn

[R13] for 计数循环
来源：http://xi.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://ke.szsharing.cn

[R14] C 风格 for
来源：http://nv.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vm.asd995.cn

[R15] while 逐行读文件
来源：http://eq.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zw.lnxyls.cn

[R16] until 等待条件
来源：http://ao.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://me.shxzskj.cn

[R17] 数组定义与取值
来源：http://xj.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hu.haigaiapp.cn

[R18] 遍历数组
来源：http://ay.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hs.szxytkj.cn

[R19] 数组长度
来源：http://xx.haigaiapp.cn

echo "${#arr[@]}"
来源：http://ek.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://rp.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dy.yuntaijiaju.cn

[R21] 字符串长度
来源：http://jl.yuntaijiaju.cn

echo "${#s}"
来源：http://nq.shxzukj.cn

[R22] 截取子串
来源：http://ks.hahajie.cn

echo "${s:0:5}"
来源：http://ts.huanxung.cn

[R23] 字符串替换
来源：http://yy.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fb.gzmigu.cn

[R24] 大小写转换
来源：http://ng.newstarts.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ye.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://oh.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cw.gzmigu.cn

[R26] 命令替换
来源：http://bu.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://sp.szsharing.cn

[R27] 算术展开
来源：http://df.asd995.cn

echo $((1 + 2 * 3))
来源：http://at.shxzskj.cn

[R28] 浮点运算
来源：http://xh.newstarts.cn

echo "scale=2; 10/3" | bc
来源：http://yc.huanxung.cn

[R29] 定义函数
来源：http://up.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nj.bjjhwx.cn

[R30] 函数返回状态码
来源：http://xs.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://pl.muxihuayi.cn

[R31] 局部变量
来源：http://mp.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://qi.newstarts.cn

[R32] 参数个数校验
来源：http://fw.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ji.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://ke.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iq.szxytkj.cn

[R34] 退出时清理
来源：http://ky.yuntaijiaju.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ox.huanxung.cn

[R35] 后台执行并等待
来源：http://uy.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ji.lnxyls.cn

[R36] 并发执行多个任务
来源：http://be.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tn.shxzskj.cn

[R37] 把输出赋给变量
来源：http://km.nszjky.cn

files=$(ls -1)
来源：http://om.newstarts.cn

[R38] 管道串联
来源：http://kj.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://dr.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://br.gzmigu.cn

cmd > out.log 2>&1
来源：http://mn.newstarts.cn

[R40] 追加写日志
来源：http://rz.521024.cn

echo "log" >> out.log
来源：http://sg.chemitech.net.cn

[R41] 丢弃输出
来源：http://qa.asd995.cn

cmd >/dev/null 2>&1
来源：http://gh.huixinmuqiang.cn

[R42] 输入重定向
来源：http://zm.bookmarksfly.cn

wc -l < a.txt
来源：http://kz.nicolike.cn

[R43] 按名字查找文件
来源：http://jw.huanxung.cn

find . -name "*.log" -type f
来源：http://hb.shxzskj.cn

[R44] 按修改时间查找
来源：http://tn.huanxung.cn

find . -mtime -7 -type f
来源：http://yw.asd995.cn

[R45] 批量删除
来源：http://gc.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://sg.panjiajie.cn

[R46] 递归替换文件内容
来源：http://hq.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eo.huanxung.cn

[R47] sed 单行替换
来源：http://qu.shxzskj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ju.panjiajie.cn

[R48] awk 取指定列
来源：http://xc.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://lu.huixiangedu.cn

[R49] awk 带条件
来源：http://dw.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wx.asd995.cn

[R50] awk 求和
来源：http://cq.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rg.chemitech.net.cn

[R51] 排序去重取前几
来源：http://rg.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hl.yuexingan06.cn

[R52] 统计行数
来源：http://ol.gzmigu.cn

wc -l a.txt
来源：http://uk.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://bx.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yi.lnxyls.cn

[R54] 比较两个文件
来源：http://bf.huixinmuqiang.cn

diff a.txt b.txt
来源：http://ad.jianghongdianzi.cn

[R55] 压缩与解压
来源：http://bt.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://io.szsharing.cn

[R56] 远程拷贝
来源：http://dn.nicolike.cn

scp file user@host:/path/
来源：http://az.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://kt.colortex.cn

ssh user@host 'uptime'
来源：http://pe.nszjky.cn

[R58] 下载文件
来源：http://ef.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://av.yuexingan06.cn

[R59] 发 POST JSON
来源：http://di.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nq.wgjwhj.cn

[R60] 只看 HTTP 状态码
来源：http://pd.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hk.szsharing.cn

[R61] 磁盘占用
来源：http://za.gzmigu.cn

df -h;  du -sh *
来源：http://db.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://lg.chemitech.net.cn

du -ah . | sort -rh | head -10
来源：http://fz.shxzskj.cn

[R63] 内存与进程
来源：http://yn.521024.cn

free -h;  ps aux | grep nginx
来源：http://tc.wgjwhj.cn

[R64] 结束进程
来源：http://jf.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://zc.huanxung.cn

[R65] 查看端口占用
来源：http://dq.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://se.521024.cn

[R66] 定时任务
来源：http://qh.muxihuayi.cn

crontab -e;  crontab -l
来源：http://sl.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://nu.lnxyls.cn

openssl rand -hex 16
来源：http://dl.9csxet.cn

[R68] 计算文件校验值
来源：http://fm.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vr.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://vp.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://ob.chemitech.net.cn

[R70] 时间戳与互转
来源：http://sn.colortex.cn

date +%s;  date -d @1700000000
来源：http://qe.hahajie.cn

[R71] 日期格式化
来源：http://ei.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mb.bjjhwx.cn

[R72] 等待端口就绪
来源：http://vj.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pi.wgjwhj.cn

[R73] 分割大日志
来源：http://gq.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://zc.shtwfgs.cn

[R74] 批量重命名
来源：http://ny.jctech888.com.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ws.shxzukj.cn

[R75] 导出环境变量
来源：http://bo.szsharing.cn

export PATH="$HOME/bin:$PATH"
来源：http://cr.haigaiapp.cn

[R76] 使用临时文件
来源：http://ai.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wx.szxytkj.cn

[R77] 读取用户输入
来源：http://uy.asd995.cn

read -rp "请输入: " ans
来源：http://io.yuexingan06.cn

[R78] 交互式菜单
来源：http://ad.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gb.shxzskj.cn

[R79] 解析命令行选项
来源：http://bl.9csxet.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gx.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://hy.huixiangedu.cn

time ./run.sh
来源：http://rn.nicolike.cn

================================================================================
来源：http://sl.shxzskj.cn

S. C / C++ 专题
来源：http://ik.yuntaijiaju.cn

================================================================================
来源：http://oq.9csxet.cn

[S01] C：Hello World
来源：http://wr.jianghongdianzi.cn

#include <stdio.h>
来源：http://dc.panjiajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hq.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://le.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://if.nicolike.cn

[S03] C：读入整数
来源：http://fb.521024.cn

int x; scanf("%d", &x);
来源：http://tc.yuexingan06.cn

[S04] C：字符串复制
来源：http://wi.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dp.wgjwhj.cn

[S05] C：字符串长度
来源：http://en.nszjky.cn

strlen(s)
来源：http://kb.shxzukj.cn

[S06] C：字符串比较
来源：http://lv.wgjwhj.cn

strcmp(a, b) == 0
来源：http://dr.asd995.cn

[S07] C：数组遍历求和
来源：http://fe.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nb.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://do.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gu.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://kb.hnjuh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ic.bjjhwx.cn

[S10] C：指针与解引用
来源：http://bq.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://dg.nicolike.cn

[S11] C：逐行读文件
来源：http://ia.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://sk.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ml.521024.cn

fclose(f);
来源：http://nv.shxzskj.cn

[S12] C：写文件
来源：http://bw.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gi.wgjwhj.cn

[S13] C：宏定义
来源：http://uu.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zr.bookmarksfly.cn

[S14] C：枚举
来源：http://cq.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://ly.hnjuh.cn

[S15] C：类型转换
来源：http://bf.jianghongdianzi.cn

(double) a / b
来源：http://ky.huanxung.cn

[S16] C：位操作置位
来源：http://lg.haigaiapp.cn

x |= (1 << 3);
来源：http://fg.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://qc.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://db.bjjhwx.cn

[S18] C：命令行参数
来源：http://sp.yuexingan06.cn

int main(int argc, char **argv)
来源：http://fq.bjjhwx.cn

[S19] C：快速排序
来源：http://it.9csxet.cn

qsort(a, n, sizeof(int), cmp);
来源：http://go.shxzskj.cn

[S20] C：二分查找
来源：http://dd.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zn.bjjhwx.cn

[S21] C：字符类别判断
来源：http://zv.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rg.shxzukj.cn

[S22] C：字符串转数字
来源：http://rf.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zj.521024.cn

[S23] C：随机数
来源：http://ng.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://us.gzmigu.cn

[S24] C：获取本地时间
来源：http://kv.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kv.jctech888.com.cn

[S25] C：内存拷贝
来源：http://el.shxzukj.cn

memcpy(dst, src, n);
来源：http://td.huixinmuqiang.cn

[S26] C：内存清零
来源：http://ms.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://rj.chemitech.net.cn

[S27] C：定义常量
来源：http://ri.chemitech.net.cn

const double PI = 3.14159;
来源：http://gx.asd995.cn

[S28] C：静态变量
来源：http://vd.jctech888.com.cn

static int counter = 0;
来源：http://jq.jianghongdianzi.cn

[S29] C：变参函数
来源：http://pk.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://th.jctech888.com.cn

[S30] C：头文件保护
来源：http://am.panjiajie.cn

#ifndef X_H
来源：http://gw.muxihuayi.cn

#define X_H
来源：http://jx.hahajie.cn

#endif
来源：http://af.521024.cn

[S31] C++：Hello World
来源：http://hh.wgjwhj.cn

#include <iostream>
来源：http://ae.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://rm.yuexingan06.cn

[S32] C++：字符串
来源：http://sd.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://gv.newstarts.cn

[S33] C++：vector 增删
来源：http://ya.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ac.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://dq.szxytkj.cn

for (auto &x : v) { std::cout << x; }
来源：http://gf.lnxyls.cn

[S35] C++：map
来源：http://pv.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wc.hahajie.cn

[S36] C++：unordered_map
来源：http://ht.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.szxytkj.cn

[S37] C++：set
来源：http://nu.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dx.szxytkj.cn

[S38] C++：排序
来源：http://yo.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://yw.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://no.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gf.gzmigu.cn

[S40] C++：查找元素
来源：http://cr.jianghongdianzi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ez.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://sw.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jx.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://cj.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://wx.huanxung.cn

[S43] C++：智能指针
来源：http://uk.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://kd.bjjhwx.cn

[S44] C++：引用传参
来源：http://xs.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://bb.colortex.cn

[S45] C++：lambda
来源：http://ba.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://er.hahajie.cn

[S46] C++：函数模板
来源：http://ky.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fm.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://xp.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xb.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://np.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kz.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://lz.chemitech.net.cn

[S49] C++：写文件
来源：http://oq.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ry.newstarts.cn

[S50] C++：格式化数字
来源：http://sy.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ti.nicolike.cn

[S51] C++：显式类型转换
来源：http://nm.nszjky.cn

static_cast<double>(a) / b
来源：http://ls.huixinmuqiang.cn

[S52] C++：const 与 noexcept
来源：http://mf.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://ch.bjjhwx.cn

[S53] C++：移动语义
来源：http://ck.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://aw.hnjuh.cn

[S54] C++：异常处理
来源：http://wf.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fc.521024.cn

[S55] C++：结构化绑定
来源：http://xo.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oo.hnjuh.cn

[S56] C++：optional
来源：http://ih.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zq.colortex.cn

[S57] C++：编译期常量
来源：http://zq.nicolike.cn

constexpr int N = 10;
来源：http://ns.huixiangedu.cn

[S58] C++：命名空间
来源：http://po.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://hu.yuexingan06.cn

[S59] C++：静态断言
来源：http://nx.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://se.521024.cn

[S60] C++：遍历并删除元素
来源：http://sn.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vd.newstarts.cn

================================================================================
来源：http://nm.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fx.panjiajie.cn

================================================================================
来源：http://bx.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://vm.jctech888.com.cn

println("Hello")
来源：http://dn.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://uk.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nv.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://xj.haigaiapp.cn

"值: $b"
来源：http://dy.panjiajie.cn

[T04] Kotlin：空安全
来源：http://bg.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://hy.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://sx.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://et.521024.cn

[T06] Kotlin：集合映射
来源：http://db.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tn.521024.cn


<!-- 参考信息 -->