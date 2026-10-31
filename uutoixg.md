代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hq.lnxyls.cn

[Q90] 生成序号列
来源：http://sb.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ns.huixinmuqiang.cn

================================================================================
来源：http://ji.shxzukj.cn

R. Bash 专题
来源：http://xn.gzmigu.cn

================================================================================
来源：http://fg.szsharing.cn

[R01] shebang 与严格模式
来源：http://hz.asd995.cn

#!/usr/bin/env bash
来源：http://bn.wgjwhj.cn

set -euo pipefail
来源：http://qm.szsharing.cn

[R02] 变量赋值与使用
来源：http://pm.shtwfgs.cn

name="Tom"; echo "$name"
来源：http://nm.jianghongdianzi.cn

[R03] 只读变量
来源：http://rq.wgjwhj.cn

readonly PI=3.14
来源：http://lx.chemitech.net.cn

[R04] 位置参数
来源：http://fv.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mo.huixiangedu.cn

[R05] 参数默认值
来源：http://bd.chemitech.net.cn

name="${1:-default}"
来源：http://wv.521024.cn

[R06] 判断命令是否存在
来源：http://jo.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mm.shtwfgs.cn

[R07] if 判断文件
来源：http://rz.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oq.huixiangedu.cn

[R08] 数值比较
来源：http://ya.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fn.muxihuayi.cn

[R09] 字符串比较
来源：http://nx.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fo.wgjwhj.cn

[R10] 正则匹配
来源：http://gr.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fq.szxytkj.cn

[R11] case 多分支
来源：http://ag.bjjhwx.cn

case "$1" in
来源：http://gu.asd995.cn

start) echo "启动" ;;
来源：http://oy.huixiangedu.cn

stop)  echo "停止" ;;
来源：http://ex.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://fe.shtwfgs.cn

esac
来源：http://rc.muxihuayi.cn

[R12] for 遍历文件
来源：http://vv.bjjhwx.cn

for f in *.txt; do echo "$f"; done
来源：http://vt.huanxung.cn

[R13] for 计数循环
来源：http://jg.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://vl.jctech888.com.cn

[R14] C 风格 for
来源：http://xj.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gh.haigaiapp.cn

[R15] while 逐行读文件
来源：http://re.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cg.huixinmuqiang.cn

[R16] until 等待条件
来源：http://sy.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uk.yuexingan06.cn

[R17] 数组定义与取值
来源：http://nf.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://eb.chemitech.net.cn

[R18] 遍历数组
来源：http://ns.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cl.jctech888.com.cn

[R19] 数组长度
来源：http://fb.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://ug.shtwfgs.cn

[R20] 关联数组（字典）
来源：http://jd.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lm.muxihuayi.cn

[R21] 字符串长度
来源：http://xf.shxzukj.cn

echo "${#s}"
来源：http://iw.huixiangedu.cn

[R22] 截取子串
来源：http://zo.hahajie.cn

echo "${s:0:5}"
来源：http://ck.nicolike.cn

[R23] 字符串替换
来源：http://jz.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uv.huixinmuqiang.cn

[R24] 大小写转换
来源：http://ff.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ce.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://aw.szsharing.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sw.jctech888.com.cn

[R26] 命令替换
来源：http://pk.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://me.yuntaijiaju.cn

[R27] 算术展开
来源：http://oe.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://ag.jctech888.com.cn

[R28] 浮点运算
来源：http://dg.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://nq.jctech888.com.cn

[R29] 定义函数
来源：http://jq.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vw.lnxyls.cn

[R30] 函数返回状态码
来源：http://br.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://et.shxzukj.cn

[R31] 局部变量
来源：http://iv.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://vg.shxzukj.cn

[R32] 参数个数校验
来源：http://ys.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hl.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://ib.huanxung.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ib.asd995.cn

[R34] 退出时清理
来源：http://ft.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jr.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://yc.hahajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ay.nicolike.cn

[R36] 并发执行多个任务
来源：http://iv.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bz.521024.cn

[R37] 把输出赋给变量
来源：http://fu.9csxet.cn

files=$(ls -1)
来源：http://tr.chemitech.net.cn

[R38] 管道串联
来源：http://ia.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://kx.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://di.shxzukj.cn

cmd > out.log 2>&1
来源：http://xe.colortex.cn

[R40] 追加写日志
来源：http://sp.huixinmuqiang.cn

echo "log" >> out.log
来源：http://ro.newstarts.cn

[R41] 丢弃输出
来源：http://ez.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://xw.jianghongdianzi.cn

[R42] 输入重定向
来源：http://nx.huixinmuqiang.cn

wc -l < a.txt
来源：http://oi.muxihuayi.cn

[R43] 按名字查找文件
来源：http://qr.panjiajie.cn

find . -name "*.log" -type f
来源：http://xc.hahajie.cn

[R44] 按修改时间查找
来源：http://xl.bjjhwx.cn

find . -mtime -7 -type f
来源：http://kl.panjiajie.cn

[R45] 批量删除
来源：http://cr.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://sn.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://ku.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ox.huixiangedu.cn

[R47] sed 单行替换
来源：http://ap.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nw.huanxung.cn

[R48] awk 取指定列
来源：http://sq.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://ea.huixiangedu.cn

[R49] awk 带条件
来源：http://gz.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yr.shxzukj.cn

[R50] awk 求和
来源：http://ak.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ld.huixiangedu.cn

[R51] 排序去重取前几
来源：http://fw.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fr.colortex.cn

[R52] 统计行数
来源：http://oz.bjjhwx.cn

wc -l a.txt
来源：http://zl.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://xt.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lo.huanxung.cn

[R54] 比较两个文件
来源：http://yg.jctech888.com.cn

diff a.txt b.txt
来源：http://ho.panjiajie.cn

[R55] 压缩与解压
来源：http://qk.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uo.panjiajie.cn

[R56] 远程拷贝
来源：http://zq.asd995.cn

scp file user@host:/path/
来源：http://xz.colortex.cn

[R57] 远程执行命令
来源：http://xz.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://dm.521024.cn

[R58] 下载文件
来源：http://ki.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xx.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://vo.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ub.yuexingan06.cn

[R60] 只看 HTTP 状态码
来源：http://qg.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ba.shtwfgs.cn

[R61] 磁盘占用
来源：http://vp.yuexingan06.cn

df -h;  du -sh *
来源：http://ce.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://vh.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://an.panjiajie.cn

[R63] 内存与进程
来源：http://rc.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://ke.shtwfgs.cn

[R64] 结束进程
来源：http://xe.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://xj.hnjuh.cn

[R65] 查看端口占用
来源：http://od.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bb.hnjuh.cn

[R66] 定时任务
来源：http://qn.muxihuayi.cn

crontab -e;  crontab -l
来源：http://fr.colortex.cn

[R67] 生成随机十六进制串
来源：http://tn.jctech888.com.cn

openssl rand -hex 16
来源：http://ua.huanxung.cn

[R68] 计算文件校验值
来源：http://vw.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lj.521024.cn

[R69] 生成随机密码
来源：http://xy.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://nk.asd995.cn

[R70] 时间戳与互转
来源：http://kh.nszjky.cn

date +%s;  date -d @1700000000
来源：http://hb.hnjuh.cn

[R71] 日期格式化
来源：http://zv.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://co.yuexingan06.cn

[R72] 等待端口就绪
来源：http://fw.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qc.panjiajie.cn

[R73] 分割大日志
来源：http://jw.haigaiapp.cn

split -l 1000 big.log part_
来源：http://ek.shxzskj.cn

[R74] 批量重命名
来源：http://fo.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yc.huanxung.cn

[R75] 导出环境变量
来源：http://sf.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://er.521024.cn

[R76] 使用临时文件
来源：http://sn.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://co.lnxyls.cn

[R77] 读取用户输入
来源：http://dh.panjiajie.cn

read -rp "请输入: " ans
来源：http://of.asd995.cn

[R78] 交互式菜单
来源：http://po.jctech888.com.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nr.gzmigu.cn

[R79] 解析命令行选项
来源：http://ew.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://se.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://rl.shxzukj.cn

time ./run.sh
来源：http://jf.chemitech.net.cn

================================================================================
来源：http://uq.nszjky.cn

S. C / C++ 专题
来源：http://oq.bookmarksfly.cn

================================================================================
来源：http://un.hahajie.cn

[S01] C：Hello World
来源：http://gr.nszjky.cn

#include <stdio.h>
来源：http://qg.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://oi.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://tb.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://ye.hnjuh.cn

[S03] C：读入整数
来源：http://ze.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://uf.bjjhwx.cn

[S04] C：字符串复制
来源：http://qd.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ec.wgjwhj.cn

[S05] C：字符串长度
来源：http://hu.muxihuayi.cn

strlen(s)
来源：http://ee.newstarts.cn

[S06] C：字符串比较
来源：http://es.chemitech.net.cn

strcmp(a, b) == 0
来源：http://xh.lnxyls.cn

[S07] C：数组遍历求和
来源：http://ot.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://be.521024.cn

[S08] C：动态内存分配与释放
来源：http://vf.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pc.colortex.cn

[S09] C：结构体定义与初始化
来源：http://uz.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lt.hahajie.cn

[S10] C：指针与解引用
来源：http://na.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://ap.hnjuh.cn

[S11] C：逐行读文件
来源：http://dy.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://qw.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mw.colortex.cn

fclose(f);
来源：http://ya.wgjwhj.cn

[S12] C：写文件
来源：http://ij.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://np.yuexingan06.cn

[S13] C：宏定义
来源：http://pn.huanxung.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rk.bookmarksfly.cn

[S14] C：枚举
来源：http://wv.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://ps.huixinmuqiang.cn

[S15] C：类型转换
来源：http://mq.chemitech.net.cn

(double) a / b
来源：http://xw.bookmarksfly.cn

[S16] C：位操作置位
来源：http://lm.jianghongdianzi.cn

x |= (1 << 3);
来源：http://jg.9csxet.cn

[S17] C：安全拼接字符串
来源：http://jd.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hr.shxzukj.cn

[S18] C：命令行参数
来源：http://bs.newstarts.cn

int main(int argc, char **argv)
来源：http://lt.colortex.cn

[S19] C：快速排序
来源：http://cd.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qo.lnxyls.cn

[S20] C：二分查找
来源：http://lu.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ho.newstarts.cn

[S21] C：字符类别判断
来源：http://sw.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fd.yuexingan06.cn

[S22] C：字符串转数字
来源：http://dh.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rk.521024.cn

[S23] C：随机数
来源：http://cl.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hr.gzmigu.cn

[S24] C：获取本地时间
来源：http://al.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hd.bjjhwx.cn

[S25] C：内存拷贝
来源：http://mo.chemitech.net.cn

memcpy(dst, src, n);
来源：http://ed.lnxyls.cn

[S26] C：内存清零
来源：http://uw.521024.cn

memset(a, 0, sizeof a);
来源：http://qo.haigaiapp.cn

[S27] C：定义常量
来源：http://vv.asd995.cn

const double PI = 3.14159;
来源：http://ta.shtwfgs.cn

[S28] C：静态变量
来源：http://oe.yuntaijiaju.cn

static int counter = 0;
来源：http://co.bookmarksfly.cn

[S29] C：变参函数
来源：http://rz.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xe.hnjuh.cn

[S30] C：头文件保护
来源：http://wv.huixinmuqiang.cn

#ifndef X_H
来源：http://qv.huanxung.cn

#define X_H
来源：http://qq.shxzskj.cn

#endif
来源：http://cn.huixiangedu.cn

[S31] C++：Hello World
来源：http://fg.shtwfgs.cn

#include <iostream>
来源：http://gz.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://lq.lnxyls.cn

[S32] C++：字符串
来源：http://iv.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://zz.521024.cn

[S33] C++：vector 增删
来源：http://bd.jctech888.com.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gt.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://zo.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://oy.shxzukj.cn

[S35] C++：map
来源：http://fj.9csxet.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xf.huixiangedu.cn

[S36] C++：unordered_map
来源：http://bu.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pp.huanxung.cn

[S37] C++：set
来源：http://tl.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rd.jianghongdianzi.cn

[S38] C++：排序
来源：http://xd.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://kc.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://cv.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ry.chemitech.net.cn

[S40] C++：查找元素
来源：http://je.521024.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ey.panjiajie.cn

[S41] C++：类与构造函数
来源：http://hx.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dv.colortex.cn

[S42] C++：继承与虚函数
来源：http://mo.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://wr.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://qo.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://mk.yuexingan06.cn

[S44] C++：引用传参
来源：http://rd.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://wd.wgjwhj.cn

[S45] C++：lambda
来源：http://ic.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ys.huixiangedu.cn

[S46] C++：函数模板
来源：http://ig.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oc.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://gg.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pu.9csxet.cn

[S48] C++：逐行读文件
来源：http://hp.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vb.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://uv.gzmigu.cn

[S49] C++：写文件
来源：http://yd.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ce.hahajie.cn

[S50] C++：格式化数字
来源：http://sk.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yb.asd995.cn

[S51] C++：显式类型转换
来源：http://sj.nicolike.cn

static_cast<double>(a) / b
来源：http://cn.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://dc.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://tf.shtwfgs.cn

[S53] C++：移动语义
来源：http://lp.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://gv.bjjhwx.cn

[S54] C++：异常处理
来源：http://ed.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wl.nszjky.cn

[S55] C++：结构化绑定
来源：http://px.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oo.shxzukj.cn

[S56] C++：optional
来源：http://cy.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fp.lnxyls.cn

[S57] C++：编译期常量
来源：http://mz.bookmarksfly.cn

constexpr int N = 10;
来源：http://dd.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://gb.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://yn.huanxung.cn

[S59] C++：静态断言
来源：http://hr.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qi.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://xs.asd995.cn


<!-- 参考信息 -->