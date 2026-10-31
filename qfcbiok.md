代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://rt.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kz.nszjky.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bf.lnxyls.cn

[Q89] 判断表是否存在
来源：http://xl.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pn.shxzukj.cn

[Q90] 生成序号列
来源：http://me.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ln.yuntaijiaju.cn

================================================================================
来源：http://pt.nszjky.cn

R. Bash 专题
来源：http://qg.gzmigu.cn

================================================================================
来源：http://bo.shxzukj.cn

[R01] shebang 与严格模式
来源：http://ra.szsharing.cn

#!/usr/bin/env bash
来源：http://cp.huixiangedu.cn

set -euo pipefail
来源：http://cy.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://jv.asd995.cn

name="Tom"; echo "$name"
来源：http://fv.chemitech.net.cn

[R03] 只读变量
来源：http://mo.9csxet.cn

readonly PI=3.14
来源：http://fh.bjjhwx.cn

[R04] 位置参数
来源：http://el.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yf.szxytkj.cn

[R05] 参数默认值
来源：http://ya.shxzukj.cn

name="${1:-default}"
来源：http://gv.521024.cn

[R06] 判断命令是否存在
来源：http://io.asd995.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ed.shtwfgs.cn

[R07] if 判断文件
来源：http://mv.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://di.szxytkj.cn

[R08] 数值比较
来源：http://an.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tv.haigaiapp.cn

[R09] 字符串比较
来源：http://ju.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qs.huixinmuqiang.cn

[R10] 正则匹配
来源：http://wa.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fx.jctech888.com.cn

[R11] case 多分支
来源：http://va.colortex.cn

case "$1" in
来源：http://wa.newstarts.cn

start) echo "启动" ;;
来源：http://kn.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://hc.colortex.cn

*)     echo "未知命令" ;;
来源：http://ta.wgjwhj.cn

esac
来源：http://cj.yuexingan06.cn

[R12] for 遍历文件
来源：http://mq.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://dx.szxytkj.cn

[R13] for 计数循环
来源：http://xq.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://ux.9csxet.cn

[R14] C 风格 for
来源：http://su.hahajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zj.newstarts.cn

[R15] while 逐行读文件
来源：http://nb.hahajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nc.bjjhwx.cn

[R16] until 等待条件
来源：http://ab.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eq.huixiangedu.cn

[R17] 数组定义与取值
来源：http://sl.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uy.szxytkj.cn

[R18] 遍历数组
来源：http://wi.szxytkj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xo.szxytkj.cn

[R19] 数组长度
来源：http://nh.huanxung.cn

echo "${#arr[@]}"
来源：http://dq.521024.cn

[R20] 关联数组（字典）
来源：http://we.9csxet.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ct.shxzskj.cn

[R21] 字符串长度
来源：http://jt.nicolike.cn

echo "${#s}"
来源：http://ps.haigaiapp.cn

[R22] 截取子串
来源：http://ny.bjjhwx.cn

echo "${s:0:5}"
来源：http://qe.9csxet.cn

[R23] 字符串替换
来源：http://an.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hy.asd995.cn

[R24] 大小写转换
来源：http://ks.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xt.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://mg.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lg.muxihuayi.cn

[R26] 命令替换
来源：http://mu.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://vw.asd995.cn

[R27] 算术展开
来源：http://sl.hahajie.cn

echo $((1 + 2 * 3))
来源：http://rm.chemitech.net.cn

[R28] 浮点运算
来源：http://vm.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://ji.521024.cn

[R29] 定义函数
来源：http://br.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ly.panjiajie.cn

[R30] 函数返回状态码
来源：http://ey.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://np.lnxyls.cn

[R31] 局部变量
来源：http://jb.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://vm.szxytkj.cn

[R32] 参数个数校验
来源：http://oo.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rt.muxihuayi.cn

[R33] 捕获错误并提示行号
来源：http://ba.hnjuh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yw.huixinmuqiang.cn

[R34] 退出时清理
来源：http://fi.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ca.lnxyls.cn

[R35] 后台执行并等待
来源：http://zm.jianghongdianzi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tb.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://qc.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tt.panjiajie.cn

[R37] 把输出赋给变量
来源：http://be.newstarts.cn

files=$(ls -1)
来源：http://ml.shxzskj.cn

[R38] 管道串联
来源：http://lr.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://pn.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://lx.nicolike.cn

cmd > out.log 2>&1
来源：http://ai.colortex.cn

[R40] 追加写日志
来源：http://dk.asd995.cn

echo "log" >> out.log
来源：http://sd.asd995.cn

[R41] 丢弃输出
来源：http://gh.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://kl.panjiajie.cn

[R42] 输入重定向
来源：http://pb.shtwfgs.cn

wc -l < a.txt
来源：http://ul.bjjhwx.cn

[R43] 按名字查找文件
来源：http://gb.colortex.cn

find . -name "*.log" -type f
来源：http://li.muxihuayi.cn

[R44] 按修改时间查找
来源：http://mg.haigaiapp.cn

find . -mtime -7 -type f
来源：http://hr.lnxyls.cn

[R45] 批量删除
来源：http://ob.521024.cn

find . -name "*.tmp" -delete
来源：http://sx.nicolike.cn

[R46] 递归替换文件内容
来源：http://gt.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zm.bjjhwx.cn

[R47] sed 单行替换
来源：http://pn.shxzskj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rz.huixiangedu.cn

[R48] awk 取指定列
来源：http://wz.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://mh.asd995.cn

[R49] awk 带条件
来源：http://jq.huixinmuqiang.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bw.asd995.cn

[R50] awk 求和
来源：http://rf.bjjhwx.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nu.wgjwhj.cn

[R51] 排序去重取前几
来源：http://ro.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ms.chemitech.net.cn

[R52] 统计行数
来源：http://hk.chemitech.net.cn

wc -l a.txt
来源：http://gc.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://kr.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://in.haigaiapp.cn

[R54] 比较两个文件
来源：http://ok.yuexingan06.cn

diff a.txt b.txt
来源：http://dj.521024.cn

[R55] 压缩与解压
来源：http://ww.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wf.colortex.cn

[R56] 远程拷贝
来源：http://qz.bjjhwx.cn

scp file user@host:/path/
来源：http://jl.asd995.cn

[R57] 远程执行命令
来源：http://xw.colortex.cn

ssh user@host 'uptime'
来源：http://tm.muxihuayi.cn

[R58] 下载文件
来源：http://fm.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hh.huixiangedu.cn

[R59] 发 POST JSON
来源：http://zj.haigaiapp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xc.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://iy.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bc.szsharing.cn

[R61] 磁盘占用
来源：http://rg.bookmarksfly.cn

df -h;  du -sh *
来源：http://ux.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://ho.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://ep.haigaiapp.cn

[R63] 内存与进程
来源：http://cf.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://td.asd995.cn

[R64] 结束进程
来源：http://ou.chemitech.net.cn

kill -9 $(pgrep -f app.py)
来源：http://xg.hahajie.cn

[R65] 查看端口占用
来源：http://ee.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vm.szxytkj.cn

[R66] 定时任务
来源：http://xj.lnxyls.cn

crontab -e;  crontab -l
来源：http://xi.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://nl.hnjuh.cn

openssl rand -hex 16
来源：http://al.yuexingan06.cn

[R68] 计算文件校验值
来源：http://uo.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ra.szxytkj.cn

[R69] 生成随机密码
来源：http://xa.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://wj.wgjwhj.cn

[R70] 时间戳与互转
来源：http://tj.huixinmuqiang.cn

date +%s;  date -d @1700000000
来源：http://bt.newstarts.cn

[R71] 日期格式化
来源：http://wq.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://iw.gzmigu.cn

[R72] 等待端口就绪
来源：http://zh.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jz.chemitech.net.cn

[R73] 分割大日志
来源：http://se.nicolike.cn

split -l 1000 big.log part_
来源：http://px.shxzskj.cn

[R74] 批量重命名
来源：http://zi.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oh.huixiangedu.cn

[R75] 导出环境变量
来源：http://se.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://hf.nicolike.cn

[R76] 使用临时文件
来源：http://ky.shxzskj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xh.newstarts.cn

[R77] 读取用户输入
来源：http://ia.yuexingan06.cn

read -rp "请输入: " ans
来源：http://pr.colortex.cn

[R78] 交互式菜单
来源：http://yg.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://da.jctech888.com.cn

[R79] 解析命令行选项
来源：http://sf.wgjwhj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://de.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://vl.jctech888.com.cn

time ./run.sh
来源：http://kg.yuexingan06.cn

================================================================================
来源：http://aj.shtwfgs.cn

S. C / C++ 专题
来源：http://qc.9csxet.cn

================================================================================
来源：http://rr.panjiajie.cn

[S01] C：Hello World
来源：http://ca.nszjky.cn

#include <stdio.h>
来源：http://mu.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tk.huanxung.cn

[S02] C：变量与格式化输出
来源：http://mu.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://du.521024.cn

[S03] C：读入整数
来源：http://xi.gzmigu.cn

int x; scanf("%d", &x);
来源：http://ew.hnjuh.cn

[S04] C：字符串复制
来源：http://hz.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://be.panjiajie.cn

[S05] C：字符串长度
来源：http://km.hahajie.cn

strlen(s)
来源：http://ha.bookmarksfly.cn

[S06] C：字符串比较
来源：http://uu.lnxyls.cn

strcmp(a, b) == 0
来源：http://ok.hnjuh.cn

[S07] C：数组遍历求和
来源：http://hh.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ps.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://gb.huixinmuqiang.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dg.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://bi.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fp.shxzukj.cn

[S10] C：指针与解引用
来源：http://xs.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://dj.szsharing.cn

[S11] C：逐行读文件
来源：http://kw.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://yp.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qd.newstarts.cn

fclose(f);
来源：http://id.nszjky.cn

[S12] C：写文件
来源：http://fr.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ue.chemitech.net.cn

[S13] C：宏定义
来源：http://ef.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xf.huixinmuqiang.cn

[S14] C：枚举
来源：http://hw.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://sm.shxzskj.cn

[S15] C：类型转换
来源：http://ex.panjiajie.cn

(double) a / b
来源：http://pg.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://rd.shxzukj.cn

x |= (1 << 3);
来源：http://ow.hahajie.cn

[S17] C：安全拼接字符串
来源：http://sp.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kq.newstarts.cn

[S18] C：命令行参数
来源：http://yq.nszjky.cn

int main(int argc, char **argv)
来源：http://oc.521024.cn

[S19] C：快速排序
来源：http://zi.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zf.shxzukj.cn

[S20] C：二分查找
来源：http://nm.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dl.huanxung.cn

[S21] C：字符类别判断
来源：http://iw.wgjwhj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hq.colortex.cn

[S22] C：字符串转数字
来源：http://ye.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qp.yuexingan06.cn

[S23] C：随机数
来源：http://jl.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fb.colortex.cn

[S24] C：获取本地时间
来源：http://xg.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zk.9csxet.cn

[S25] C：内存拷贝
来源：http://ts.bjjhwx.cn

memcpy(dst, src, n);
来源：http://gs.haigaiapp.cn

[S26] C：内存清零
来源：http://ga.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://gr.shxzukj.cn

[S27] C：定义常量
来源：http://at.asd995.cn

const double PI = 3.14159;
来源：http://xl.lnxyls.cn

[S28] C：静态变量
来源：http://us.521024.cn

static int counter = 0;
来源：http://xe.shtwfgs.cn

[S29] C：变参函数
来源：http://ac.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ox.szxytkj.cn

[S30] C：头文件保护
来源：http://hv.lnxyls.cn

#ifndef X_H
来源：http://wf.colortex.cn

#define X_H
来源：http://lo.lnxyls.cn

#endif
来源：http://rk.huanxung.cn

[S31] C++：Hello World
来源：http://xo.yuntaijiaju.cn

#include <iostream>
来源：http://jz.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://xc.jctech888.com.cn

[S32] C++：字符串
来源：http://kv.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://sd.newstarts.cn

[S33] C++：vector 增删
来源：http://ps.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zf.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://da.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://py.colortex.cn

[S35] C++：map
来源：http://nz.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bq.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://xd.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zz.gzmigu.cn

[S37] C++：set
来源：http://zq.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jw.jctech888.com.cn

[S38] C++：排序
来源：http://tk.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://hr.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://hy.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bk.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://fw.lnxyls.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cs.shxzukj.cn

[S41] C++：类与构造函数
来源：http://bl.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://no.yuntaijiaju.cn

[S42] C++：继承与虚函数
来源：http://ef.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://pv.szxytkj.cn

[S43] C++：智能指针
来源：http://qe.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://md.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://ae.huanxung.cn

void inc(int &x) { ++x; }
来源：http://tx.lnxyls.cn

[S45] C++：lambda
来源：http://zk.colortex.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ae.haigaiapp.cn

[S46] C++：函数模板
来源：http://kl.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pt.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://ej.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ea.colortex.cn

[S48] C++：逐行读文件
来源：http://mv.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ba.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://vc.colortex.cn

[S49] C++：写文件
来源：http://wi.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bd.hahajie.cn

[S50] C++：格式化数字
来源：http://pu.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zy.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://bx.gzmigu.cn

static_cast<double>(a) / b
来源：http://tr.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://oo.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://hr.szxytkj.cn

[S53] C++：移动语义
来源：http://bq.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://vs.huixiangedu.cn

[S54] C++：异常处理
来源：http://fv.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oo.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://tu.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zy.muxihuayi.cn

[S56] C++：optional
来源：http://ay.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ch.521024.cn

[S57] C++：编译期常量
来源：http://fa.yuexingan06.cn

constexpr int N = 10;
来源：http://ii.shtwfgs.cn

[S58] C++：命名空间
来源：http://ux.huanxung.cn


<!-- 参考信息 -->