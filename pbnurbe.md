代发 wailian999

R. Bash 专题
来源：http://pa.haigaiapp.cn

================================================================================
来源：http://aj.9csxet.cn

[R01] shebang 与严格模式
来源：http://vq.nicolike.cn

#!/usr/bin/env bash
来源：http://ms.colortex.cn

set -euo pipefail
来源：http://ze.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://od.szxytkj.cn

name="Tom"; echo "$name"
来源：http://fi.haigaiapp.cn

[R03] 只读变量
来源：http://yy.shxzskj.cn

readonly PI=3.14
来源：http://pu.wgjwhj.cn

[R04] 位置参数
来源：http://ow.panjiajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://te.lnxyls.cn

[R05] 参数默认值
来源：http://kv.gzmigu.cn

name="${1:-default}"
来源：http://rl.hnjuh.cn

[R06] 判断命令是否存在
来源：http://tu.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qv.huixiangedu.cn

[R07] if 判断文件
来源：http://to.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lw.haigaiapp.cn

[R08] 数值比较
来源：http://bp.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kh.bjjhwx.cn

[R09] 字符串比较
来源：http://ck.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ns.shxzukj.cn

[R10] 正则匹配
来源：http://xj.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ws.haigaiapp.cn

[R11] case 多分支
来源：http://bl.yuntaijiaju.cn

case "$1" in
来源：http://hq.muxihuayi.cn

start) echo "启动" ;;
来源：http://mo.szxytkj.cn

stop)  echo "停止" ;;
来源：http://jp.hnjuh.cn

*)     echo "未知命令" ;;
来源：http://ha.yuntaijiaju.cn

esac
来源：http://pa.chemitech.net.cn

[R12] for 遍历文件
来源：http://ni.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://cr.newstarts.cn

[R13] for 计数循环
来源：http://vn.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://se.shtwfgs.cn

[R14] C 风格 for
来源：http://hq.lnxyls.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nh.9csxet.cn

[R15] while 逐行读文件
来源：http://kj.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://st.yuexingan06.cn

[R16] until 等待条件
来源：http://ph.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://aq.hahajie.cn

[R17] 数组定义与取值
来源：http://ru.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rd.jianghongdianzi.cn

[R18] 遍历数组
来源：http://sz.huixiangedu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vv.szsharing.cn

[R19] 数组长度
来源：http://tu.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://ys.521024.cn

[R20] 关联数组（字典）
来源：http://fb.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vo.huanxung.cn

[R21] 字符串长度
来源：http://hu.gzmigu.cn

echo "${#s}"
来源：http://zx.colortex.cn

[R22] 截取子串
来源：http://cn.newstarts.cn

echo "${s:0:5}"
来源：http://hu.hahajie.cn

[R23] 字符串替换
来源：http://tb.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gc.szsharing.cn

[R24] 大小写转换
来源：http://qp.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lr.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://jk.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jp.jianghongdianzi.cn

[R26] 命令替换
来源：http://lo.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://zz.gzmigu.cn

[R27] 算术展开
来源：http://tz.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://ej.muxihuayi.cn

[R28] 浮点运算
来源：http://or.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://bg.shxzskj.cn

[R29] 定义函数
来源：http://ih.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ko.szsharing.cn

[R30] 函数返回状态码
来源：http://aa.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://ss.yuexingan06.cn

[R31] 局部变量
来源：http://mk.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://uk.szxytkj.cn

[R32] 参数个数校验
来源：http://ai.huixinmuqiang.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ab.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://lu.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mc.huixiangedu.cn

[R34] 退出时清理
来源：http://tt.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qy.gzmigu.cn

[R35] 后台执行并等待
来源：http://sy.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lt.szxytkj.cn

[R36] 并发执行多个任务
来源：http://ex.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ly.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://yk.muxihuayi.cn

files=$(ls -1)
来源：http://mb.hahajie.cn

[R38] 管道串联
来源：http://mf.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://xd.hahajie.cn

[R39] 重定向标准输出与错误
来源：http://dz.nszjky.cn

cmd > out.log 2>&1
来源：http://wm.lnxyls.cn

[R40] 追加写日志
来源：http://hf.shxzskj.cn

echo "log" >> out.log
来源：http://gh.shxzukj.cn

[R41] 丢弃输出
来源：http://wc.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://iz.hahajie.cn

[R42] 输入重定向
来源：http://yw.colortex.cn

wc -l < a.txt
来源：http://zx.asd995.cn

[R43] 按名字查找文件
来源：http://tv.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://hr.shxzukj.cn

[R44] 按修改时间查找
来源：http://hb.wgjwhj.cn

find . -mtime -7 -type f
来源：http://xl.jctech888.com.cn

[R45] 批量删除
来源：http://dw.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://te.muxihuayi.cn

[R46] 递归替换文件内容
来源：http://np.yuntaijiaju.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://di.shxzskj.cn

[R47] sed 单行替换
来源：http://ti.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hp.bookmarksfly.cn

[R48] awk 取指定列
来源：http://mk.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://wd.yuntaijiaju.cn

[R49] awk 带条件
来源：http://ce.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oz.wgjwhj.cn

[R50] awk 求和
来源：http://zb.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qh.9csxet.cn

[R51] 排序去重取前几
来源：http://vy.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lq.9csxet.cn

[R52] 统计行数
来源：http://hq.muxihuayi.cn

wc -l a.txt
来源：http://wi.colortex.cn

[R53] 查看文件头与实时尾
来源：http://rm.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wh.hnjuh.cn

[R54] 比较两个文件
来源：http://iy.wgjwhj.cn

diff a.txt b.txt
来源：http://vf.huanxung.cn

[R55] 压缩与解压
来源：http://uq.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yj.colortex.cn

[R56] 远程拷贝
来源：http://xl.huixinmuqiang.cn

scp file user@host:/path/
来源：http://ae.bookmarksfly.cn

[R57] 远程执行命令
来源：http://lj.gzmigu.cn

ssh user@host 'uptime'
来源：http://dq.szsharing.cn

[R58] 下载文件
来源：http://ow.colortex.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://my.jctech888.com.cn

[R59] 发 POST JSON
来源：http://go.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qn.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://hd.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tu.muxihuayi.cn

[R61] 磁盘占用
来源：http://bm.panjiajie.cn

df -h;  du -sh *
来源：http://dx.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://oq.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://kd.chemitech.net.cn

[R63] 内存与进程
来源：http://gu.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://qj.bookmarksfly.cn

[R64] 结束进程
来源：http://mr.hnjuh.cn

kill -9 $(pgrep -f app.py)
来源：http://xv.szxytkj.cn

[R65] 查看端口占用
来源：http://bl.jctech888.com.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ag.shxzskj.cn

[R66] 定时任务
来源：http://xr.szsharing.cn

crontab -e;  crontab -l
来源：http://ca.colortex.cn

[R67] 生成随机十六进制串
来源：http://vd.hahajie.cn

openssl rand -hex 16
来源：http://wy.gzmigu.cn

[R68] 计算文件校验值
来源：http://ko.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://az.huixiangedu.cn

[R69] 生成随机密码
来源：http://ev.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://xm.jianghongdianzi.cn

[R70] 时间戳与互转
来源：http://bv.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://bc.lnxyls.cn

[R71] 日期格式化
来源：http://rp.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kg.szsharing.cn

[R72] 等待端口就绪
来源：http://bp.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pf.lnxyls.cn

[R73] 分割大日志
来源：http://wy.521024.cn

split -l 1000 big.log part_
来源：http://za.nszjky.cn

[R74] 批量重命名
来源：http://pv.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oa.shtwfgs.cn

[R75] 导出环境变量
来源：http://pp.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://jz.newstarts.cn

[R76] 使用临时文件
来源：http://no.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wl.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://ti.hahajie.cn

read -rp "请输入: " ans
来源：http://qk.shxzskj.cn

[R78] 交互式菜单
来源：http://zo.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yw.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://oi.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nt.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://lf.bjjhwx.cn

time ./run.sh
来源：http://lr.lnxyls.cn

================================================================================
来源：http://jx.chemitech.net.cn

S. C / C++ 专题
来源：http://wg.szsharing.cn

================================================================================
来源：http://mk.szxytkj.cn

[S01] C：Hello World
来源：http://nu.shtwfgs.cn

#include <stdio.h>
来源：http://yr.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fz.521024.cn

[S02] C：变量与格式化输出
来源：http://de.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://qh.shxzskj.cn

[S03] C：读入整数
来源：http://un.szxytkj.cn

int x; scanf("%d", &x);
来源：http://ju.asd995.cn

[S04] C：字符串复制
来源：http://ao.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fm.jctech888.com.cn

[S05] C：字符串长度
来源：http://tk.newstarts.cn

strlen(s)
来源：http://pj.shxzskj.cn

[S06] C：字符串比较
来源：http://pc.muxihuayi.cn

strcmp(a, b) == 0
来源：http://ds.panjiajie.cn

[S07] C：数组遍历求和
来源：http://mu.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://de.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://ia.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jv.panjiajie.cn

[S09] C：结构体定义与初始化
来源：http://na.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hd.chemitech.net.cn

[S10] C：指针与解引用
来源：http://lf.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://oa.shtwfgs.cn

[S11] C：逐行读文件
来源：http://an.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://ab.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://if.colortex.cn

fclose(f);
来源：http://nz.bookmarksfly.cn

[S12] C：写文件
来源：http://su.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ov.shtwfgs.cn

[S13] C：宏定义
来源：http://jm.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sk.muxihuayi.cn

[S14] C：枚举
来源：http://uo.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://jd.huixinmuqiang.cn

[S15] C：类型转换
来源：http://lc.lnxyls.cn

(double) a / b
来源：http://xx.haigaiapp.cn

[S16] C：位操作置位
来源：http://rs.nszjky.cn

x |= (1 << 3);
来源：http://gx.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://lw.huixiangedu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mw.nicolike.cn

[S18] C：命令行参数
来源：http://md.muxihuayi.cn

int main(int argc, char **argv)
来源：http://kf.nszjky.cn

[S19] C：快速排序
来源：http://br.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oj.9csxet.cn

[S20] C：二分查找
来源：http://qe.521024.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nj.shxzukj.cn

[S21] C：字符类别判断
来源：http://pp.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vy.huanxung.cn

[S22] C：字符串转数字
来源：http://hg.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ev.huanxung.cn

[S23] C：随机数
来源：http://xc.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tl.wgjwhj.cn

[S24] C：获取本地时间
来源：http://jc.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ct.9csxet.cn

[S25] C：内存拷贝
来源：http://zq.shxzskj.cn

memcpy(dst, src, n);
来源：http://fr.panjiajie.cn

[S26] C：内存清零
来源：http://zp.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://bd.gzmigu.cn

[S27] C：定义常量
来源：http://xu.521024.cn

const double PI = 3.14159;
来源：http://wn.newstarts.cn

[S28] C：静态变量
来源：http://mf.haigaiapp.cn

static int counter = 0;
来源：http://jg.asd995.cn

[S29] C：变参函数
来源：http://sr.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://el.hnjuh.cn

[S30] C：头文件保护
来源：http://et.newstarts.cn

#ifndef X_H
来源：http://cz.asd995.cn

#define X_H
来源：http://yx.lnxyls.cn

#endif
来源：http://yj.bookmarksfly.cn

[S31] C++：Hello World
来源：http://jh.shxzukj.cn

#include <iostream>
来源：http://hg.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://mf.bookmarksfly.cn

[S32] C++：字符串
来源：http://sr.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://od.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://sm.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ew.nicolike.cn

[S34] C++：遍历 vector
来源：http://fh.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://ss.huanxung.cn

[S35] C++：map
来源：http://fe.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lj.colortex.cn

[S36] C++：unordered_map
来源：http://fb.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ki.bookmarksfly.cn

[S37] C++：set
来源：http://xq.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ko.bjjhwx.cn

[S38] C++：排序
来源：http://xn.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://qm.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://xi.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nl.jctech888.com.cn

[S40] C++：查找元素
来源：http://zr.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kv.lnxyls.cn

[S41] C++：类与构造函数
来源：http://ok.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cl.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://ui.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://vo.szxytkj.cn

[S43] C++：智能指针
来源：http://ju.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://eq.shtwfgs.cn

[S44] C++：引用传参
来源：http://hq.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://ci.huanxung.cn

[S45] C++：lambda
来源：http://lm.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bg.nicolike.cn

[S46] C++：函数模板
来源：http://pk.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rv.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://rt.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gs.lnxyls.cn

[S48] C++：逐行读文件
来源：http://ss.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kc.asd995.cn

while (std::getline(in, line)) { }
来源：http://zk.jctech888.com.cn

[S49] C++：写文件
来源：http://cw.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ox.colortex.cn

[S50] C++：格式化数字
来源：http://py.huanxung.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gi.asd995.cn

[S51] C++：显式类型转换
来源：http://gj.hahajie.cn

static_cast<double>(a) / b
来源：http://ua.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://ie.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://as.lnxyls.cn

[S53] C++：移动语义
来源：http://pp.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://un.muxihuayi.cn

[S54] C++：异常处理
来源：http://vd.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ss.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://ew.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qr.jctech888.com.cn

[S56] C++：optional
来源：http://vx.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zv.panjiajie.cn

[S57] C++：编译期常量
来源：http://yp.chemitech.net.cn

constexpr int N = 10;
来源：http://my.gzmigu.cn

[S58] C++：命名空间
来源：http://ou.yuexingan06.cn

namespace ns { int f() { return 1; } }
来源：http://sf.colortex.cn

[S59] C++：静态断言
来源：http://je.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mm.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://mv.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sy.shxzskj.cn

================================================================================
来源：http://dl.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yh.huixinmuqiang.cn

================================================================================
来源：http://as.bjjhwx.cn


<!-- 参考信息 -->