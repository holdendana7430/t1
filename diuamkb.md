代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://vj.asd995.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bm.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ab.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://be.521024.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cx.hnjuh.cn

[Q90] 生成序号列
来源：http://oj.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yo.szsharing.cn

================================================================================
来源：http://fe.hahajie.cn

R. Bash 专题
来源：http://ib.huixiangedu.cn

================================================================================
来源：http://xa.hahajie.cn

[R01] shebang 与严格模式
来源：http://fw.newstarts.cn

#!/usr/bin/env bash
来源：http://fm.shtwfgs.cn

set -euo pipefail
来源：http://nc.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://ab.haigaiapp.cn

name="Tom"; echo "$name"
来源：http://it.szsharing.cn

[R03] 只读变量
来源：http://it.yuntaijiaju.cn

readonly PI=3.14
来源：http://og.521024.cn

[R04] 位置参数
来源：http://nd.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zm.szsharing.cn

[R05] 参数默认值
来源：http://id.bookmarksfly.cn

name="${1:-default}"
来源：http://ea.gzmigu.cn

[R06] 判断命令是否存在
来源：http://sx.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://da.jianghongdianzi.cn

[R07] if 判断文件
来源：http://wn.yuntaijiaju.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uh.yuntaijiaju.cn

[R08] 数值比较
来源：http://kc.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tt.asd995.cn

[R09] 字符串比较
来源：http://sj.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ax.bjjhwx.cn

[R10] 正则匹配
来源：http://ym.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jq.huanxung.cn

[R11] case 多分支
来源：http://od.hahajie.cn

case "$1" in
来源：http://jo.hahajie.cn

start) echo "启动" ;;
来源：http://pd.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://rg.hahajie.cn

*)     echo "未知命令" ;;
来源：http://of.asd995.cn

esac
来源：http://cl.lnxyls.cn

[R12] for 遍历文件
来源：http://ho.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://ex.hahajie.cn

[R13] for 计数循环
来源：http://dp.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://mq.521024.cn

[R14] C 风格 for
来源：http://an.shxzskj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xq.jctech888.com.cn

[R15] while 逐行读文件
来源：http://mt.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zk.haigaiapp.cn

[R16] until 等待条件
来源：http://wo.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ej.szsharing.cn

[R17] 数组定义与取值
来源：http://ru.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ht.huixiangedu.cn

[R18] 遍历数组
来源：http://rs.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://na.shxzukj.cn

[R19] 数组长度
来源：http://ew.gzmigu.cn

echo "${#arr[@]}"
来源：http://hk.shxzukj.cn

[R20] 关联数组（字典）
来源：http://ze.yuntaijiaju.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://np.9csxet.cn

[R21] 字符串长度
来源：http://jf.muxihuayi.cn

echo "${#s}"
来源：http://fd.nszjky.cn

[R22] 截取子串
来源：http://bk.jctech888.com.cn

echo "${s:0:5}"
来源：http://br.colortex.cn

[R23] 字符串替换
来源：http://pt.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vy.nicolike.cn

[R24] 大小写转换
来源：http://nu.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vr.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://mk.wgjwhj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uw.521024.cn

[R26] 命令替换
来源：http://ds.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://ng.szxytkj.cn

[R27] 算术展开
来源：http://xc.hnjuh.cn

echo $((1 + 2 * 3))
来源：http://gq.huixiangedu.cn

[R28] 浮点运算
来源：http://ha.muxihuayi.cn

echo "scale=2; 10/3" | bc
来源：http://vl.shxzukj.cn

[R29] 定义函数
来源：http://fc.szxytkj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dm.szxytkj.cn

[R30] 函数返回状态码
来源：http://ld.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://dv.colortex.cn

[R31] 局部变量
来源：http://xs.haigaiapp.cn

f() { local x=1; echo "$x"; }
来源：http://zn.hahajie.cn

[R32] 参数个数校验
来源：http://cp.nszjky.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ma.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://tc.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wf.gzmigu.cn

[R34] 退出时清理
来源：http://rr.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vs.colortex.cn

[R35] 后台执行并等待
来源：http://xt.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rq.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://gw.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lo.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://tu.szxytkj.cn

files=$(ls -1)
来源：http://ww.szsharing.cn

[R38] 管道串联
来源：http://bl.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://al.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://xn.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://ig.shxzukj.cn

[R40] 追加写日志
来源：http://cl.shxzskj.cn

echo "log" >> out.log
来源：http://xl.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://qe.jctech888.com.cn

cmd >/dev/null 2>&1
来源：http://ds.chemitech.net.cn

[R42] 输入重定向
来源：http://fs.colortex.cn

wc -l < a.txt
来源：http://pf.shxzskj.cn

[R43] 按名字查找文件
来源：http://eu.hahajie.cn

find . -name "*.log" -type f
来源：http://et.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://sl.gzmigu.cn

find . -mtime -7 -type f
来源：http://an.9csxet.cn

[R45] 批量删除
来源：http://fp.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://ee.huixiangedu.cn

[R46] 递归替换文件内容
来源：http://yd.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fb.nicolike.cn

[R47] sed 单行替换
来源：http://js.shxzskj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ma.panjiajie.cn

[R48] awk 取指定列
来源：http://nw.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://wh.newstarts.cn

[R49] awk 带条件
来源：http://cs.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ii.yuntaijiaju.cn

[R50] awk 求和
来源：http://lg.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rv.jctech888.com.cn

[R51] 排序去重取前几
来源：http://kc.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://id.shtwfgs.cn

[R52] 统计行数
来源：http://xc.521024.cn

wc -l a.txt
来源：http://mf.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://ns.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hx.haigaiapp.cn

[R54] 比较两个文件
来源：http://cm.wgjwhj.cn

diff a.txt b.txt
来源：http://mn.nicolike.cn

[R55] 压缩与解压
来源：http://rm.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gw.hahajie.cn

[R56] 远程拷贝
来源：http://cp.huixiangedu.cn

scp file user@host:/path/
来源：http://gn.szxytkj.cn

[R57] 远程执行命令
来源：http://gr.chemitech.net.cn

ssh user@host 'uptime'
来源：http://ln.hnjuh.cn

[R58] 下载文件
来源：http://ez.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mz.panjiajie.cn

[R59] 发 POST JSON
来源：http://lc.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://az.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://yd.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xs.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://fq.huixiangedu.cn

df -h;  du -sh *
来源：http://vw.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://pl.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://rf.asd995.cn

[R63] 内存与进程
来源：http://qd.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://ag.yuntaijiaju.cn

[R64] 结束进程
来源：http://gu.hnjuh.cn

kill -9 $(pgrep -f app.py)
来源：http://ff.muxihuayi.cn

[R65] 查看端口占用
来源：http://zj.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sl.lnxyls.cn

[R66] 定时任务
来源：http://db.gzmigu.cn

crontab -e;  crontab -l
来源：http://dm.asd995.cn

[R67] 生成随机十六进制串
来源：http://wo.lnxyls.cn

openssl rand -hex 16
来源：http://jq.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://gs.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hg.wgjwhj.cn

[R69] 生成随机密码
来源：http://ri.huixinmuqiang.cn

head -c 16 /dev/urandom | base64
来源：http://sx.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://jy.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://sb.hahajie.cn

[R71] 日期格式化
来源：http://qe.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xk.szxytkj.cn

[R72] 等待端口就绪
来源：http://da.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ch.asd995.cn

[R73] 分割大日志
来源：http://vo.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://kq.huixiangedu.cn

[R74] 批量重命名
来源：http://oh.nszjky.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gp.hnjuh.cn

[R75] 导出环境变量
来源：http://fa.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://df.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://cg.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jp.chemitech.net.cn

[R77] 读取用户输入
来源：http://al.nicolike.cn

read -rp "请输入: " ans
来源：http://sf.gzmigu.cn

[R78] 交互式菜单
来源：http://am.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ii.newstarts.cn

[R79] 解析命令行选项
来源：http://wk.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uj.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://hg.bookmarksfly.cn

time ./run.sh
来源：http://rr.521024.cn

================================================================================
来源：http://ol.nszjky.cn

S. C / C++ 专题
来源：http://lx.huixinmuqiang.cn

================================================================================
来源：http://dy.shxzskj.cn

[S01] C：Hello World
来源：http://qz.nicolike.cn

#include <stdio.h>
来源：http://mn.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nq.szxytkj.cn

[S02] C：变量与格式化输出
来源：http://qp.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://xg.szsharing.cn

[S03] C：读入整数
来源：http://hk.shxzukj.cn

int x; scanf("%d", &x);
来源：http://cz.newstarts.cn

[S04] C：字符串复制
来源：http://bx.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ra.hnjuh.cn

[S05] C：字符串长度
来源：http://xm.gzmigu.cn

strlen(s)
来源：http://ny.bjjhwx.cn

[S06] C：字符串比较
来源：http://ee.gzmigu.cn

strcmp(a, b) == 0
来源：http://wb.colortex.cn

[S07] C：数组遍历求和
来源：http://md.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gm.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://dh.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hf.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://yz.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zv.wgjwhj.cn

[S10] C：指针与解引用
来源：http://ji.hahajie.cn

int *p = &a;  *p = 5;
来源：http://zr.newstarts.cn

[S11] C：逐行读文件
来源：http://ww.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://gf.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zj.yuntaijiaju.cn

fclose(f);
来源：http://lj.jctech888.com.cn

[S12] C：写文件
来源：http://hq.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xi.shxzukj.cn

[S13] C：宏定义
来源：http://yr.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hu.shxzukj.cn

[S14] C：枚举
来源：http://mf.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://ct.shxzskj.cn

[S15] C：类型转换
来源：http://cl.bookmarksfly.cn

(double) a / b
来源：http://eq.shtwfgs.cn

[S16] C：位操作置位
来源：http://im.gzmigu.cn

x |= (1 << 3);
来源：http://vo.huanxung.cn

[S17] C：安全拼接字符串
来源：http://sv.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pn.bjjhwx.cn

[S18] C：命令行参数
来源：http://vy.gzmigu.cn

int main(int argc, char **argv)
来源：http://sb.jianghongdianzi.cn

[S19] C：快速排序
来源：http://fv.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bj.szsharing.cn

[S20] C：二分查找
来源：http://bc.hahajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pz.panjiajie.cn

[S21] C：字符类别判断
来源：http://pf.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qe.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://fr.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ey.bookmarksfly.cn

[S23] C：随机数
来源：http://ex.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qo.huanxung.cn

[S24] C：获取本地时间
来源：http://qo.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://at.newstarts.cn

[S25] C：内存拷贝
来源：http://cg.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://gg.yuntaijiaju.cn

[S26] C：内存清零
来源：http://tu.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://an.yuexingan06.cn

[S27] C：定义常量
来源：http://xz.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://ds.yuexingan06.cn

[S28] C：静态变量
来源：http://ok.nicolike.cn

static int counter = 0;
来源：http://vc.9csxet.cn

[S29] C：变参函数
来源：http://xu.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tw.wgjwhj.cn

[S30] C：头文件保护
来源：http://sd.muxihuayi.cn

#ifndef X_H
来源：http://hq.hahajie.cn

#define X_H
来源：http://cb.gzmigu.cn

#endif
来源：http://vl.shtwfgs.cn

[S31] C++：Hello World
来源：http://lj.yuexingan06.cn

#include <iostream>
来源：http://jn.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://er.wgjwhj.cn

[S32] C++：字符串
来源：http://qc.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://jw.huanxung.cn

[S33] C++：vector 增删
来源：http://xz.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eg.szsharing.cn

[S34] C++：遍历 vector
来源：http://nw.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://yg.wgjwhj.cn

[S35] C++：map
来源：http://ss.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cs.9csxet.cn

[S36] C++：unordered_map
来源：http://kl.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fl.panjiajie.cn

[S37] C++：set
来源：http://ee.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kk.521024.cn

[S38] C++：排序
来源：http://nu.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://sf.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://an.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zv.szsharing.cn

[S40] C++：查找元素
来源：http://cd.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mb.huanxung.cn

[S41] C++：类与构造函数
来源：http://tc.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jf.nicolike.cn

[S42] C++：继承与虚函数
来源：http://pq.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://rx.colortex.cn

[S43] C++：智能指针
来源：http://ke.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://ye.jctech888.com.cn

[S44] C++：引用传参
来源：http://nd.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://ge.huixiangedu.cn

[S45] C++：lambda
来源：http://ib.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gv.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://vy.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ub.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://sm.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rw.panjiajie.cn

[S48] C++：逐行读文件
来源：http://qh.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tw.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://gl.bjjhwx.cn

[S49] C++：写文件
来源：http://wk.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qe.szsharing.cn

[S50] C++：格式化数字
来源：http://ql.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rl.asd995.cn

[S51] C++：显式类型转换
来源：http://wc.shxzukj.cn

static_cast<double>(a) / b
来源：http://br.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://rn.asd995.cn

int size() const noexcept { return n_; }
来源：http://ln.panjiajie.cn

[S53] C++：移动语义
来源：http://uq.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://pd.shxzskj.cn

[S54] C++：异常处理
来源：http://yk.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hr.nszjky.cn

[S55] C++：结构化绑定
来源：http://fy.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ur.wgjwhj.cn

[S56] C++：optional
来源：http://vk.jctech888.com.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cd.chemitech.net.cn

[S57] C++：编译期常量
来源：http://zw.gzmigu.cn

constexpr int N = 10;
来源：http://jw.panjiajie.cn

[S58] C++：命名空间
来源：http://np.chemitech.net.cn


<!-- 参考信息 -->