代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wf.haigaiapp.cn

[Q90] 生成序号列
来源：http://xz.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ux.shxzukj.cn

================================================================================
来源：http://vj.hnjuh.cn

R. Bash 专题
来源：http://ha.asd995.cn

================================================================================
来源：http://iv.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://ve.521024.cn

#!/usr/bin/env bash
来源：http://qp.yuntaijiaju.cn

set -euo pipefail
来源：http://nd.huanxung.cn

[R02] 变量赋值与使用
来源：http://cu.bjjhwx.cn

name="Tom"; echo "$name"
来源：http://au.huanxung.cn

[R03] 只读变量
来源：http://pg.wgjwhj.cn

readonly PI=3.14
来源：http://rf.gzmigu.cn

[R04] 位置参数
来源：http://pu.521024.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kh.nicolike.cn

[R05] 参数默认值
来源：http://gi.muxihuayi.cn

name="${1:-default}"
来源：http://yd.panjiajie.cn

[R06] 判断命令是否存在
来源：http://pu.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://te.huixiangedu.cn

[R07] if 判断文件
来源：http://mb.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vs.shxzukj.cn

[R08] 数值比较
来源：http://mw.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qp.yuntaijiaju.cn

[R09] 字符串比较
来源：http://ki.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wt.panjiajie.cn

[R10] 正则匹配
来源：http://bs.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kp.chemitech.net.cn

[R11] case 多分支
来源：http://qh.521024.cn

case "$1" in
来源：http://ne.szsharing.cn

start) echo "启动" ;;
来源：http://cm.hahajie.cn

stop)  echo "停止" ;;
来源：http://qz.9csxet.cn

*)     echo "未知命令" ;;
来源：http://qw.hahajie.cn

esac
来源：http://ih.shtwfgs.cn

[R12] for 遍历文件
来源：http://nx.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://jf.shtwfgs.cn

[R13] for 计数循环
来源：http://mp.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://pf.asd995.cn

[R14] C 风格 for
来源：http://hp.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nd.colortex.cn

[R15] while 逐行读文件
来源：http://st.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nh.asd995.cn

[R16] until 等待条件
来源：http://lg.newstarts.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fb.newstarts.cn

[R17] 数组定义与取值
来源：http://pc.9csxet.cn

arr=(a b c); echo "${arr[0]}"
来源：http://di.huixinmuqiang.cn

[R18] 遍历数组
来源：http://ln.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zj.521024.cn

[R19] 数组长度
来源：http://zc.huixiangedu.cn

echo "${#arr[@]}"
来源：http://eh.gzmigu.cn

[R20] 关联数组（字典）
来源：http://km.bookmarksfly.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uh.9csxet.cn

[R21] 字符串长度
来源：http://tv.bookmarksfly.cn

echo "${#s}"
来源：http://yl.yuntaijiaju.cn

[R22] 截取子串
来源：http://zn.chemitech.net.cn

echo "${s:0:5}"
来源：http://xu.huixinmuqiang.cn

[R23] 字符串替换
来源：http://az.shtwfgs.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tn.yuexingan06.cn

[R24] 大小写转换
来源：http://aw.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xi.shtwfgs.cn

[R25] 去后缀 / 去前缀
来源：http://bh.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pk.colortex.cn

[R26] 命令替换
来源：http://yj.asd995.cn

now=$(date +%F); echo "$now"
来源：http://ip.bookmarksfly.cn

[R27] 算术展开
来源：http://he.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://tf.bookmarksfly.cn

[R28] 浮点运算
来源：http://nh.521024.cn

echo "scale=2; 10/3" | bc
来源：http://qh.colortex.cn

[R29] 定义函数
来源：http://xm.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nv.muxihuayi.cn

[R30] 函数返回状态码
来源：http://gn.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://oe.huixiangedu.cn

[R31] 局部变量
来源：http://wd.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://gh.szsharing.cn

[R32] 参数个数校验
来源：http://bb.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ih.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://hz.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oa.jianghongdianzi.cn

[R34] 退出时清理
来源：http://yh.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dx.gzmigu.cn

[R35] 后台执行并等待
来源：http://we.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sc.huanxung.cn

[R36] 并发执行多个任务
来源：http://ks.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oy.huixinmuqiang.cn

[R37] 把输出赋给变量
来源：http://xu.asd995.cn

files=$(ls -1)
来源：http://el.jctech888.com.cn

[R38] 管道串联
来源：http://vd.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://xu.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://ur.haigaiapp.cn

cmd > out.log 2>&1
来源：http://wc.hnjuh.cn

[R40] 追加写日志
来源：http://lg.newstarts.cn

echo "log" >> out.log
来源：http://rv.panjiajie.cn

[R41] 丢弃输出
来源：http://ms.shxzskj.cn

cmd >/dev/null 2>&1
来源：http://nf.nicolike.cn

[R42] 输入重定向
来源：http://oa.nszjky.cn

wc -l < a.txt
来源：http://ip.chemitech.net.cn

[R43] 按名字查找文件
来源：http://oh.haigaiapp.cn

find . -name "*.log" -type f
来源：http://ix.wgjwhj.cn

[R44] 按修改时间查找
来源：http://jm.shxzskj.cn

find . -mtime -7 -type f
来源：http://bx.yuexingan06.cn

[R45] 批量删除
来源：http://os.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://gu.nicolike.cn

[R46] 递归替换文件内容
来源：http://kk.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ph.bjjhwx.cn

[R47] sed 单行替换
来源：http://hk.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://td.panjiajie.cn

[R48] awk 取指定列
来源：http://zn.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://st.wgjwhj.cn

[R49] awk 带条件
来源：http://ma.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vm.jctech888.com.cn

[R50] awk 求和
来源：http://nq.jctech888.com.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lm.9csxet.cn

[R51] 排序去重取前几
来源：http://ku.huixiangedu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gm.lnxyls.cn

[R52] 统计行数
来源：http://be.newstarts.cn

wc -l a.txt
来源：http://cg.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://yi.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mc.szsharing.cn

[R54] 比较两个文件
来源：http://cn.asd995.cn

diff a.txt b.txt
来源：http://ag.szsharing.cn

[R55] 压缩与解压
来源：http://vt.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gb.szsharing.cn

[R56] 远程拷贝
来源：http://zt.bookmarksfly.cn

scp file user@host:/path/
来源：http://hj.szsharing.cn

[R57] 远程执行命令
来源：http://oa.szsharing.cn

ssh user@host 'uptime'
来源：http://aa.gzmigu.cn

[R58] 下载文件
来源：http://kj.jianghongdianzi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sk.haigaiapp.cn

[R59] 发 POST JSON
来源：http://lq.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ac.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://xq.hnjuh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hx.bjjhwx.cn

[R61] 磁盘占用
来源：http://fx.huixiangedu.cn

df -h;  du -sh *
来源：http://ts.9csxet.cn

[R62] 找最占空间的文件
来源：http://qe.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://wg.shxzskj.cn

[R63] 内存与进程
来源：http://nm.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://mz.haigaiapp.cn

[R64] 结束进程
来源：http://gq.hnjuh.cn

kill -9 $(pgrep -f app.py)
来源：http://ox.bjjhwx.cn

[R65] 查看端口占用
来源：http://sl.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qc.yuntaijiaju.cn

[R66] 定时任务
来源：http://zc.muxihuayi.cn

crontab -e;  crontab -l
来源：http://ch.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://va.jianghongdianzi.cn

openssl rand -hex 16
来源：http://og.nszjky.cn

[R68] 计算文件校验值
来源：http://vb.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vq.gzmigu.cn

[R69] 生成随机密码
来源：http://pc.hahajie.cn

head -c 16 /dev/urandom | base64
来源：http://ik.gzmigu.cn

[R70] 时间戳与互转
来源：http://uh.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://sw.nszjky.cn

[R71] 日期格式化
来源：http://pp.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cn.shxzukj.cn

[R72] 等待端口就绪
来源：http://yi.jianghongdianzi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bd.wgjwhj.cn

[R73] 分割大日志
来源：http://mw.9csxet.cn

split -l 1000 big.log part_
来源：http://dy.muxihuayi.cn

[R74] 批量重命名
来源：http://dq.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ci.lnxyls.cn

[R75] 导出环境变量
来源：http://ul.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://cv.bjjhwx.cn

[R76] 使用临时文件
来源：http://sm.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cl.colortex.cn

[R77] 读取用户输入
来源：http://sx.521024.cn

read -rp "请输入: " ans
来源：http://ro.521024.cn

[R78] 交互式菜单
来源：http://ci.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://at.gzmigu.cn

[R79] 解析命令行选项
来源：http://iv.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ye.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://ew.hahajie.cn

time ./run.sh
来源：http://qi.521024.cn

================================================================================
来源：http://qt.shxzskj.cn

S. C / C++ 专题
来源：http://bo.521024.cn

================================================================================
来源：http://re.shtwfgs.cn

[S01] C：Hello World
来源：http://ql.jctech888.com.cn

#include <stdio.h>
来源：http://nc.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ms.gzmigu.cn

[S02] C：变量与格式化输出
来源：http://ll.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://vq.muxihuayi.cn

[S03] C：读入整数
来源：http://kg.jianghongdianzi.cn

int x; scanf("%d", &x);
来源：http://of.wgjwhj.cn

[S04] C：字符串复制
来源：http://hy.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fv.hahajie.cn

[S05] C：字符串长度
来源：http://dh.muxihuayi.cn

strlen(s)
来源：http://nk.shtwfgs.cn

[S06] C：字符串比较
来源：http://sj.nszjky.cn

strcmp(a, b) == 0
来源：http://bv.shxzskj.cn

[S07] C：数组遍历求和
来源：http://rn.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rc.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://vm.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fw.huixinmuqiang.cn

[S09] C：结构体定义与初始化
来源：http://dl.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cx.szxytkj.cn

[S10] C：指针与解引用
来源：http://ct.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://wh.9csxet.cn

[S11] C：逐行读文件
来源：http://hs.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://lo.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cu.hnjuh.cn

fclose(f);
来源：http://bh.hnjuh.cn

[S12] C：写文件
来源：http://jh.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kp.yuntaijiaju.cn

[S13] C：宏定义
来源：http://jf.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zd.hnjuh.cn

[S14] C：枚举
来源：http://ug.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://tb.huixinmuqiang.cn

[S15] C：类型转换
来源：http://ba.hahajie.cn

(double) a / b
来源：http://am.huanxung.cn

[S16] C：位操作置位
来源：http://qm.huixinmuqiang.cn

x |= (1 << 3);
来源：http://ft.szsharing.cn

[S17] C：安全拼接字符串
来源：http://wq.bjjhwx.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yj.hahajie.cn

[S18] C：命令行参数
来源：http://qz.haigaiapp.cn

int main(int argc, char **argv)
来源：http://nb.chemitech.net.cn

[S19] C：快速排序
来源：http://df.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fv.jctech888.com.cn

[S20] C：二分查找
来源：http://ah.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qa.szxytkj.cn

[S21] C：字符类别判断
来源：http://an.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rd.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://zu.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ol.lnxyls.cn

[S23] C：随机数
来源：http://bp.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://aw.panjiajie.cn

[S24] C：获取本地时间
来源：http://cu.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tb.jctech888.com.cn

[S25] C：内存拷贝
来源：http://cw.nszjky.cn

memcpy(dst, src, n);
来源：http://ev.jctech888.com.cn

[S26] C：内存清零
来源：http://sb.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://il.yuntaijiaju.cn

[S27] C：定义常量
来源：http://oj.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://vr.lnxyls.cn

[S28] C：静态变量
来源：http://ur.wgjwhj.cn

static int counter = 0;
来源：http://vk.huixinmuqiang.cn

[S29] C：变参函数
来源：http://qr.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rd.huanxung.cn

[S30] C：头文件保护
来源：http://cm.shxzukj.cn

#ifndef X_H
来源：http://em.huanxung.cn

#define X_H
来源：http://uo.shxzukj.cn

#endif
来源：http://wo.hahajie.cn

[S31] C++：Hello World
来源：http://ua.bookmarksfly.cn

#include <iostream>
来源：http://rf.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://qn.huanxung.cn

[S32] C++：字符串
来源：http://fl.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://xj.szxytkj.cn

[S33] C++：vector 增删
来源：http://er.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iw.huanxung.cn

[S34] C++：遍历 vector
来源：http://cy.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://nm.huanxung.cn

[S35] C++：map
来源：http://hz.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kv.hahajie.cn

[S36] C++：unordered_map
来源：http://lw.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://me.521024.cn

[S37] C++：set
来源：http://gu.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vp.asd995.cn

[S38] C++：排序
来源：http://es.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://iu.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://sw.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sb.shtwfgs.cn

[S40] C++：查找元素
来源：http://ff.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dg.asd995.cn

[S41] C++：类与构造函数
来源：http://mw.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fl.colortex.cn

[S42] C++：继承与虚函数
来源：http://mu.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://yv.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://za.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://vt.shxzskj.cn

[S44] C++：引用传参
来源：http://mn.szsharing.cn

void inc(int &x) { ++x; }
来源：http://sx.521024.cn

[S45] C++：lambda
来源：http://oz.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ap.huanxung.cn

[S46] C++：函数模板
来源：http://tn.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kq.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://mh.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lf.haigaiapp.cn

[S48] C++：逐行读文件
来源：http://cm.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wq.jctech888.com.cn

while (std::getline(in, line)) { }
来源：http://cj.bookmarksfly.cn

[S49] C++：写文件
来源：http://cl.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sx.newstarts.cn

[S50] C++：格式化数字
来源：http://rr.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tl.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://io.nicolike.cn

static_cast<double>(a) / b
来源：http://ii.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://gq.nicolike.cn

int size() const noexcept { return n_; }
来源：http://hv.shxzukj.cn

[S53] C++：移动语义
来源：http://yu.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://vl.asd995.cn

[S54] C++：异常处理
来源：http://dk.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://na.521024.cn

[S55] C++：结构化绑定
来源：http://ho.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ry.nicolike.cn

[S56] C++：optional
来源：http://ip.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bo.hnjuh.cn

[S57] C++：编译期常量
来源：http://gj.huixinmuqiang.cn

constexpr int N = 10;
来源：http://wg.521024.cn

[S58] C++：命名空间
来源：http://jx.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://is.nszjky.cn

[S59] C++：静态断言
来源：http://uw.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yv.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://nr.nicolike.cn


<!-- 参考信息 -->