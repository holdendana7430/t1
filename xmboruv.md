代发 wailian999

set -euo pipefail
来源：http://wf.shxzskj.cn

[R02] 变量赋值与使用
来源：http://qa.521024.cn

name="Tom"; echo "$name"
来源：http://sq.shtwfgs.cn

[R03] 只读变量
来源：http://kf.panjiajie.cn

readonly PI=3.14
来源：http://la.panjiajie.cn

[R04] 位置参数
来源：http://xo.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://et.szsharing.cn

[R05] 参数默认值
来源：http://lf.newstarts.cn

name="${1:-default}"
来源：http://vf.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://nt.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xx.wgjwhj.cn

[R07] if 判断文件
来源：http://oy.521024.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yq.chemitech.net.cn

[R08] 数值比较
来源：http://mq.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tn.wgjwhj.cn

[R09] 字符串比较
来源：http://lk.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jr.huixiangedu.cn

[R10] 正则匹配
来源：http://py.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kk.jianghongdianzi.cn

[R11] case 多分支
来源：http://lx.bookmarksfly.cn

case "$1" in
来源：http://rw.bjjhwx.cn

start) echo "启动" ;;
来源：http://ut.szsharing.cn

stop)  echo "停止" ;;
来源：http://jq.521024.cn

*)     echo "未知命令" ;;
来源：http://gn.colortex.cn

esac
来源：http://pz.shxzukj.cn

[R12] for 遍历文件
来源：http://kq.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://om.muxihuayi.cn

[R13] for 计数循环
来源：http://tc.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://lv.panjiajie.cn

[R14] C 风格 for
来源：http://kh.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ir.bjjhwx.cn

[R15] while 逐行读文件
来源：http://rf.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://na.chemitech.net.cn

[R16] until 等待条件
来源：http://rn.muxihuayi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xv.shxzskj.cn

[R17] 数组定义与取值
来源：http://zj.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ik.huixiangedu.cn

[R18] 遍历数组
来源：http://sp.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://br.huixinmuqiang.cn

[R19] 数组长度
来源：http://jm.lnxyls.cn

echo "${#arr[@]}"
来源：http://mo.wgjwhj.cn

[R20] 关联数组（字典）
来源：http://wc.hnjuh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bn.shxzskj.cn

[R21] 字符串长度
来源：http://wq.shxzskj.cn

echo "${#s}"
来源：http://cl.yuntaijiaju.cn

[R22] 截取子串
来源：http://rp.muxihuayi.cn

echo "${s:0:5}"
来源：http://nq.yuntaijiaju.cn

[R23] 字符串替换
来源：http://ea.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ww.jianghongdianzi.cn

[R24] 大小写转换
来源：http://hl.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ka.521024.cn

[R25] 去后缀 / 去前缀
来源：http://hs.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gr.panjiajie.cn

[R26] 命令替换
来源：http://ix.521024.cn

now=$(date +%F); echo "$now"
来源：http://oq.shtwfgs.cn

[R27] 算术展开
来源：http://ni.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://kb.521024.cn

[R28] 浮点运算
来源：http://ee.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://bm.haigaiapp.cn

[R29] 定义函数
来源：http://cf.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kw.szsharing.cn

[R30] 函数返回状态码
来源：http://lu.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://bl.haigaiapp.cn

[R31] 局部变量
来源：http://tf.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://gh.panjiajie.cn

[R32] 参数个数校验
来源：http://hx.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xc.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://di.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bw.colortex.cn

[R34] 退出时清理
来源：http://wr.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hs.shxzukj.cn

[R35] 后台执行并等待
来源：http://iz.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lv.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://pk.shxzukj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xz.bjjhwx.cn

[R37] 把输出赋给变量
来源：http://xr.hnjuh.cn

files=$(ls -1)
来源：http://jj.yuntaijiaju.cn

[R38] 管道串联
来源：http://ks.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://bm.hahajie.cn

[R39] 重定向标准输出与错误
来源：http://pc.nszjky.cn

cmd > out.log 2>&1
来源：http://lj.huanxung.cn

[R40] 追加写日志
来源：http://on.huixiangedu.cn

echo "log" >> out.log
来源：http://nx.szxytkj.cn

[R41] 丢弃输出
来源：http://fn.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://km.yuexingan06.cn

[R42] 输入重定向
来源：http://gt.asd995.cn

wc -l < a.txt
来源：http://ji.nszjky.cn

[R43] 按名字查找文件
来源：http://be.hahajie.cn

find . -name "*.log" -type f
来源：http://gs.521024.cn

[R44] 按修改时间查找
来源：http://wc.521024.cn

find . -mtime -7 -type f
来源：http://eh.shxzskj.cn

[R45] 批量删除
来源：http://bk.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://gc.shxzskj.cn

[R46] 递归替换文件内容
来源：http://ox.shxzukj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sh.huanxung.cn

[R47] sed 单行替换
来源：http://vh.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fk.panjiajie.cn

[R48] awk 取指定列
来源：http://qc.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://pu.yuntaijiaju.cn

[R49] awk 带条件
来源：http://rl.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yi.jianghongdianzi.cn

[R50] awk 求和
来源：http://qw.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ou.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://nj.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sr.lnxyls.cn

[R52] 统计行数
来源：http://cx.gzmigu.cn

wc -l a.txt
来源：http://ko.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://ei.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xe.bookmarksfly.cn

[R54] 比较两个文件
来源：http://vl.nicolike.cn

diff a.txt b.txt
来源：http://eo.9csxet.cn

[R55] 压缩与解压
来源：http://qb.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uf.jctech888.com.cn

[R56] 远程拷贝
来源：http://in.asd995.cn

scp file user@host:/path/
来源：http://si.szxytkj.cn

[R57] 远程执行命令
来源：http://oj.gzmigu.cn

ssh user@host 'uptime'
来源：http://jb.jianghongdianzi.cn

[R58] 下载文件
来源：http://aa.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mt.wgjwhj.cn

[R59] 发 POST JSON
来源：http://tx.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ya.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://lg.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uf.bjjhwx.cn

[R61] 磁盘占用
来源：http://mi.yuntaijiaju.cn

df -h;  du -sh *
来源：http://no.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://sg.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://wy.haigaiapp.cn

[R63] 内存与进程
来源：http://pf.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://ov.bookmarksfly.cn

[R64] 结束进程
来源：http://ag.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://am.9csxet.cn

[R65] 查看端口占用
来源：http://ty.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://px.jctech888.com.cn

[R66] 定时任务
来源：http://ji.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://su.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://jq.asd995.cn

openssl rand -hex 16
来源：http://eq.nszjky.cn

[R68] 计算文件校验值
来源：http://pj.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ni.nicolike.cn

[R69] 生成随机密码
来源：http://ed.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://dl.muxihuayi.cn

[R70] 时间戳与互转
来源：http://qq.asd995.cn

date +%s;  date -d @1700000000
来源：http://yz.jctech888.com.cn

[R71] 日期格式化
来源：http://ri.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://io.colortex.cn

[R72] 等待端口就绪
来源：http://oj.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fi.nszjky.cn

[R73] 分割大日志
来源：http://tr.shxzukj.cn

split -l 1000 big.log part_
来源：http://ei.muxihuayi.cn

[R74] 批量重命名
来源：http://vw.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fv.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://mn.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://jy.nicolike.cn

[R76] 使用临时文件
来源：http://nj.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wt.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://dp.lnxyls.cn

read -rp "请输入: " ans
来源：http://ok.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://yc.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://it.yuexingan06.cn

[R79] 解析命令行选项
来源：http://hd.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tg.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://bd.shxzskj.cn

time ./run.sh
来源：http://wc.huixiangedu.cn

================================================================================
来源：http://ft.jianghongdianzi.cn

S. C / C++ 专题
来源：http://hb.lnxyls.cn

================================================================================
来源：http://rx.szxytkj.cn

[S01] C：Hello World
来源：http://qi.panjiajie.cn

#include <stdio.h>
来源：http://pb.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dl.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://ns.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://hw.huixiangedu.cn

[S03] C：读入整数
来源：http://eh.jianghongdianzi.cn

int x; scanf("%d", &x);
来源：http://hw.shxzskj.cn

[S04] C：字符串复制
来源：http://pn.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jb.lnxyls.cn

[S05] C：字符串长度
来源：http://is.bookmarksfly.cn

strlen(s)
来源：http://dm.muxihuayi.cn

[S06] C：字符串比较
来源：http://ff.9csxet.cn

strcmp(a, b) == 0
来源：http://kn.jctech888.com.cn

[S07] C：数组遍历求和
来源：http://qk.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dk.huixinmuqiang.cn

[S08] C：动态内存分配与释放
来源：http://bd.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kt.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://us.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://up.chemitech.net.cn

[S10] C：指针与解引用
来源：http://qo.newstarts.cn

int *p = &a;  *p = 5;
来源：http://nq.shxzskj.cn

[S11] C：逐行读文件
来源：http://ja.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://of.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vr.jianghongdianzi.cn

fclose(f);
来源：http://fj.jianghongdianzi.cn

[S12] C：写文件
来源：http://up.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rx.jianghongdianzi.cn

[S13] C：宏定义
来源：http://of.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ik.hahajie.cn

[S14] C：枚举
来源：http://fc.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://vx.jctech888.com.cn

[S15] C：类型转换
来源：http://jx.haigaiapp.cn

(double) a / b
来源：http://jl.shxzskj.cn

[S16] C：位操作置位
来源：http://se.szsharing.cn

x |= (1 << 3);
来源：http://fd.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://zc.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wr.panjiajie.cn

[S18] C：命令行参数
来源：http://cq.shxzskj.cn

int main(int argc, char **argv)
来源：http://sf.yuntaijiaju.cn

[S19] C：快速排序
来源：http://ew.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yuntaijiaju.cn

[S20] C：二分查找
来源：http://fk.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fw.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://va.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vt.huanxung.cn

[S22] C：字符串转数字
来源：http://eb.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gc.hahajie.cn

[S23] C：随机数
来源：http://lp.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rn.yuexingan06.cn

[S24] C：获取本地时间
来源：http://kv.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wd.szsharing.cn

[S25] C：内存拷贝
来源：http://gv.lnxyls.cn

memcpy(dst, src, n);
来源：http://zd.lnxyls.cn

[S26] C：内存清零
来源：http://zl.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://zr.colortex.cn

[S27] C：定义常量
来源：http://ke.hnjuh.cn

const double PI = 3.14159;
来源：http://re.shxzukj.cn

[S28] C：静态变量
来源：http://yg.huixiangedu.cn

static int counter = 0;
来源：http://ok.gzmigu.cn

[S29] C：变参函数
来源：http://xw.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ku.bookmarksfly.cn

[S30] C：头文件保护
来源：http://ap.huixinmuqiang.cn

#ifndef X_H
来源：http://cz.wgjwhj.cn

#define X_H
来源：http://cs.szxytkj.cn

#endif
来源：http://xt.szxytkj.cn

[S31] C++：Hello World
来源：http://of.hnjuh.cn

#include <iostream>
来源：http://sw.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://bb.nicolike.cn

[S32] C++：字符串
来源：http://bg.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://ji.hahajie.cn

[S33] C++：vector 增删
来源：http://bl.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ue.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://ph.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://xy.panjiajie.cn

[S35] C++：map
来源：http://ij.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gt.shtwfgs.cn

[S36] C++：unordered_map
来源：http://qi.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fs.gzmigu.cn

[S37] C++：set
来源：http://pv.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xn.gzmigu.cn

[S38] C++：排序
来源：http://iy.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://ni.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://fb.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ml.9csxet.cn

[S40] C++：查找元素
来源：http://oh.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ez.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://mb.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cc.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://bl.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://fs.bookmarksfly.cn

[S43] C++：智能指针
来源：http://mr.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://lw.haigaiapp.cn

[S44] C++：引用传参
来源：http://ij.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://bw.jctech888.com.cn

[S45] C++：lambda
来源：http://si.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wb.nicolike.cn

[S46] C++：函数模板
来源：http://co.szxytkj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ss.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://lf.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rp.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://rr.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lj.asd995.cn

while (std::getline(in, line)) { }
来源：http://za.panjiajie.cn

[S49] C++：写文件
来源：http://uc.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yl.jctech888.com.cn

[S50] C++：格式化数字
来源：http://ep.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jn.gzmigu.cn

[S51] C++：显式类型转换
来源：http://ye.huixiangedu.cn

static_cast<double>(a) / b
来源：http://ni.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://xi.nicolike.cn

int size() const noexcept { return n_; }
来源：http://eq.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://dn.colortex.cn

std::vector<int> w = std::move(v);
来源：http://ur.9csxet.cn

[S54] C++：异常处理
来源：http://sz.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uz.hnjuh.cn

[S55] C++：结构化绑定
来源：http://zl.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rh.newstarts.cn

[S56] C++：optional
来源：http://vm.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://an.hahajie.cn

[S57] C++：编译期常量
来源：http://pf.huixiangedu.cn

constexpr int N = 10;
来源：http://ly.521024.cn

[S58] C++：命名空间
来源：http://hy.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://jy.huixiangedu.cn

[S59] C++：静态断言
来源：http://dj.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hl.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://ti.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uo.bjjhwx.cn

================================================================================
来源：http://zx.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ga.haigaiapp.cn

================================================================================
来源：http://et.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://xh.wgjwhj.cn

println("Hello")
来源：http://bd.huanxung.cn

[T02] Kotlin：变量
来源：http://cj.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zs.shtwfgs.cn


<!-- 参考信息 -->