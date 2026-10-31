代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://bw.9csxet.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rp.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cm.szsharing.cn

[Q89] 判断表是否存在
来源：http://ju.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qi.lnxyls.cn

[Q90] 生成序号列
来源：http://tv.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://av.hnjuh.cn

================================================================================
来源：http://kq.szsharing.cn

R. Bash 专题
来源：http://rm.hnjuh.cn

================================================================================
来源：http://ih.colortex.cn

[R01] shebang 与严格模式
来源：http://pe.gzmigu.cn

#!/usr/bin/env bash
来源：http://gk.asd995.cn

set -euo pipefail
来源：http://uj.muxihuayi.cn

[R02] 变量赋值与使用
来源：http://cm.9csxet.cn

name="Tom"; echo "$name"
来源：http://no.521024.cn

[R03] 只读变量
来源：http://dq.yuntaijiaju.cn

readonly PI=3.14
来源：http://ee.huixinmuqiang.cn

[R04] 位置参数
来源：http://vd.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ki.521024.cn

[R05] 参数默认值
来源：http://cy.huanxung.cn

name="${1:-default}"
来源：http://xl.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://gy.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rb.shxzskj.cn

[R07] if 判断文件
来源：http://ze.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yk.chemitech.net.cn

[R08] 数值比较
来源：http://xj.gzmigu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lz.muxihuayi.cn

[R09] 字符串比较
来源：http://vt.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ih.asd995.cn

[R10] 正则匹配
来源：http://pb.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dx.521024.cn

[R11] case 多分支
来源：http://ei.hnjuh.cn

case "$1" in
来源：http://ew.huixiangedu.cn

start) echo "启动" ;;
来源：http://fr.shxzskj.cn

stop)  echo "停止" ;;
来源：http://bp.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://pd.gzmigu.cn

esac
来源：http://mv.hnjuh.cn

[R12] for 遍历文件
来源：http://nc.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://lm.yuexingan06.cn

[R13] for 计数循环
来源：http://vb.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://jp.wgjwhj.cn

[R14] C 风格 for
来源：http://qm.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nt.huanxung.cn

[R15] while 逐行读文件
来源：http://ez.jctech888.com.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ak.hahajie.cn

[R16] until 等待条件
来源：http://mb.yuexingan06.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zn.asd995.cn

[R17] 数组定义与取值
来源：http://fw.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hn.colortex.cn

[R18] 遍历数组
来源：http://xb.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vw.gzmigu.cn

[R19] 数组长度
来源：http://fd.nszjky.cn

echo "${#arr[@]}"
来源：http://ej.shxzukj.cn

[R20] 关联数组（字典）
来源：http://ju.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://le.wgjwhj.cn

[R21] 字符串长度
来源：http://pb.haigaiapp.cn

echo "${#s}"
来源：http://lt.shxzukj.cn

[R22] 截取子串
来源：http://ck.huanxung.cn

echo "${s:0:5}"
来源：http://ua.huixiangedu.cn

[R23] 字符串替换
来源：http://xz.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://au.shxzukj.cn

[R24] 大小写转换
来源：http://vy.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://im.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://th.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cr.szxytkj.cn

[R26] 命令替换
来源：http://ti.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://oa.wgjwhj.cn

[R27] 算术展开
来源：http://ne.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://qf.lnxyls.cn

[R28] 浮点运算
来源：http://ig.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://pn.jianghongdianzi.cn

[R29] 定义函数
来源：http://xb.yuexingan06.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ro.shxzskj.cn

[R30] 函数返回状态码
来源：http://hg.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://da.jctech888.com.cn

[R31] 局部变量
来源：http://vm.huanxung.cn

f() { local x=1; echo "$x"; }
来源：http://dc.panjiajie.cn

[R32] 参数个数校验
来源：http://bm.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kb.panjiajie.cn

[R33] 捕获错误并提示行号
来源：http://jz.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zn.lnxyls.cn

[R34] 退出时清理
来源：http://nn.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yr.chemitech.net.cn

[R35] 后台执行并等待
来源：http://bt.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://on.nszjky.cn

[R36] 并发执行多个任务
来源：http://jr.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ua.szsharing.cn

[R37] 把输出赋给变量
来源：http://vy.bookmarksfly.cn

files=$(ls -1)
来源：http://iu.shxzukj.cn

[R38] 管道串联
来源：http://sd.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://aq.panjiajie.cn

[R39] 重定向标准输出与错误
来源：http://al.wgjwhj.cn

cmd > out.log 2>&1
来源：http://jw.newstarts.cn

[R40] 追加写日志
来源：http://ls.521024.cn

echo "log" >> out.log
来源：http://se.chemitech.net.cn

[R41] 丢弃输出
来源：http://ik.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://wc.yuntaijiaju.cn

[R42] 输入重定向
来源：http://lm.bookmarksfly.cn

wc -l < a.txt
来源：http://kh.gzmigu.cn

[R43] 按名字查找文件
来源：http://xd.asd995.cn

find . -name "*.log" -type f
来源：http://xt.9csxet.cn

[R44] 按修改时间查找
来源：http://te.hahajie.cn

find . -mtime -7 -type f
来源：http://aa.wgjwhj.cn

[R45] 批量删除
来源：http://ko.nszjky.cn

find . -name "*.tmp" -delete
来源：http://uo.shxzskj.cn

[R46] 递归替换文件内容
来源：http://hg.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mf.muxihuayi.cn

[R47] sed 单行替换
来源：http://vp.nszjky.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ev.colortex.cn

[R48] awk 取指定列
来源：http://kh.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://bz.szxytkj.cn

[R49] awk 带条件
来源：http://mo.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ir.nszjky.cn

[R50] awk 求和
来源：http://yq.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://na.szxytkj.cn

[R51] 排序去重取前几
来源：http://pa.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yn.bjjhwx.cn

[R52] 统计行数
来源：http://wz.colortex.cn

wc -l a.txt
来源：http://ks.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://iu.shxzskj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hv.yuexingan06.cn

[R54] 比较两个文件
来源：http://yk.shtwfgs.cn

diff a.txt b.txt
来源：http://fq.colortex.cn

[R55] 压缩与解压
来源：http://kc.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pe.chemitech.net.cn

[R56] 远程拷贝
来源：http://nh.521024.cn

scp file user@host:/path/
来源：http://mh.nszjky.cn

[R57] 远程执行命令
来源：http://bt.yuexingan06.cn

ssh user@host 'uptime'
来源：http://jr.huanxung.cn

[R58] 下载文件
来源：http://fb.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nt.huanxung.cn

[R59] 发 POST JSON
来源：http://fn.521024.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kz.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://jf.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qx.9csxet.cn

[R61] 磁盘占用
来源：http://fm.nszjky.cn

df -h;  du -sh *
来源：http://ch.huanxung.cn

[R62] 找最占空间的文件
来源：http://uz.lnxyls.cn

du -ah . | sort -rh | head -10
来源：http://st.szxytkj.cn

[R63] 内存与进程
来源：http://eo.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://me.bjjhwx.cn

[R64] 结束进程
来源：http://zc.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://ex.521024.cn

[R65] 查看端口占用
来源：http://xq.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kp.huixiangedu.cn

[R66] 定时任务
来源：http://ui.panjiajie.cn

crontab -e;  crontab -l
来源：http://rg.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://ag.jianghongdianzi.cn

openssl rand -hex 16
来源：http://fu.szsharing.cn

[R68] 计算文件校验值
来源：http://pp.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gi.jctech888.com.cn

[R69] 生成随机密码
来源：http://kv.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://in.bjjhwx.cn

[R70] 时间戳与互转
来源：http://cl.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://io.jianghongdianzi.cn

[R71] 日期格式化
来源：http://me.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tr.nszjky.cn

[R72] 等待端口就绪
来源：http://by.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vy.newstarts.cn

[R73] 分割大日志
来源：http://sq.haigaiapp.cn

split -l 1000 big.log part_
来源：http://jf.bjjhwx.cn

[R74] 批量重命名
来源：http://ik.9csxet.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ea.huixinmuqiang.cn

[R75] 导出环境变量
来源：http://lo.bjjhwx.cn

export PATH="$HOME/bin:$PATH"
来源：http://en.shxzukj.cn

[R76] 使用临时文件
来源：http://ed.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vu.bookmarksfly.cn

[R77] 读取用户输入
来源：http://yp.hnjuh.cn

read -rp "请输入: " ans
来源：http://rp.lnxyls.cn

[R78] 交互式菜单
来源：http://eq.panjiajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rr.huanxung.cn

[R79] 解析命令行选项
来源：http://cy.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ym.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://xu.jctech888.com.cn

time ./run.sh
来源：http://zi.szsharing.cn

================================================================================
来源：http://cr.shtwfgs.cn

S. C / C++ 专题
来源：http://vz.bookmarksfly.cn

================================================================================
来源：http://nx.nszjky.cn

[S01] C：Hello World
来源：http://jv.gzmigu.cn

#include <stdio.h>
来源：http://yh.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gd.9csxet.cn

[S02] C：变量与格式化输出
来源：http://ds.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://zh.huixinmuqiang.cn

[S03] C：读入整数
来源：http://ys.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://ja.bookmarksfly.cn

[S04] C：字符串复制
来源：http://av.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://eb.9csxet.cn

[S05] C：字符串长度
来源：http://di.asd995.cn

strlen(s)
来源：http://vj.bookmarksfly.cn

[S06] C：字符串比较
来源：http://ge.shxzukj.cn

strcmp(a, b) == 0
来源：http://uv.gzmigu.cn

[S07] C：数组遍历求和
来源：http://ly.521024.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gv.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://bq.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mk.panjiajie.cn

[S09] C：结构体定义与初始化
来源：http://ru.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nh.panjiajie.cn

[S10] C：指针与解引用
来源：http://mv.nicolike.cn

int *p = &a;  *p = 5;
来源：http://ao.hnjuh.cn

[S11] C：逐行读文件
来源：http://mg.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://bc.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://am.asd995.cn

fclose(f);
来源：http://qu.9csxet.cn

[S12] C：写文件
来源：http://yh.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cz.jianghongdianzi.cn

[S13] C：宏定义
来源：http://ms.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rr.asd995.cn

[S14] C：枚举
来源：http://av.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://kb.muxihuayi.cn

[S15] C：类型转换
来源：http://co.gzmigu.cn

(double) a / b
来源：http://ey.9csxet.cn

[S16] C：位操作置位
来源：http://np.panjiajie.cn

x |= (1 << 3);
来源：http://tr.szsharing.cn

[S17] C：安全拼接字符串
来源：http://yk.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tr.huanxung.cn

[S18] C：命令行参数
来源：http://dl.huixinmuqiang.cn

int main(int argc, char **argv)
来源：http://lm.9csxet.cn

[S19] C：快速排序
来源：http://ks.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://um.521024.cn

[S20] C：二分查找
来源：http://ub.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wg.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://dg.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fs.lnxyls.cn

[S22] C：字符串转数字
来源：http://pr.521024.cn

atoi("42");  strtod("3.14", NULL);
来源：http://we.wgjwhj.cn

[S23] C：随机数
来源：http://hu.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bd.hahajie.cn

[S24] C：获取本地时间
来源：http://lk.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bw.shxzukj.cn

[S25] C：内存拷贝
来源：http://fc.yuexingan06.cn

memcpy(dst, src, n);
来源：http://ll.asd995.cn

[S26] C：内存清零
来源：http://ch.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://ue.lnxyls.cn

[S27] C：定义常量
来源：http://we.shtwfgs.cn

const double PI = 3.14159;
来源：http://sg.szxytkj.cn

[S28] C：静态变量
来源：http://ud.panjiajie.cn

static int counter = 0;
来源：http://wf.hnjuh.cn

[S29] C：变参函数
来源：http://vv.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eh.szxytkj.cn

[S30] C：头文件保护
来源：http://pz.521024.cn

#ifndef X_H
来源：http://kz.hnjuh.cn

#define X_H
来源：http://jq.szsharing.cn

#endif
来源：http://nd.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://wi.newstarts.cn

#include <iostream>
来源：http://uf.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://wu.szxytkj.cn

[S32] C++：字符串
来源：http://lf.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://xm.shxzukj.cn

[S33] C++：vector 增删
来源：http://jq.wgjwhj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uq.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://ni.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://bc.chemitech.net.cn

[S35] C++：map
来源：http://ba.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sy.huanxung.cn

[S36] C++：unordered_map
来源：http://te.gzmigu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xl.colortex.cn

[S37] C++：set
来源：http://an.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://am.muxihuayi.cn

[S38] C++：排序
来源：http://is.colortex.cn

std::sort(v.begin(), v.end());
来源：http://tf.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://nx.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ki.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://wh.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://on.hnjuh.cn

[S41] C++：类与构造函数
来源：http://xp.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iu.asd995.cn

[S42] C++：继承与虚函数
来源：http://xy.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://gp.shtwfgs.cn

[S43] C++：智能指针
来源：http://gk.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://ou.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://ik.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://hv.huixiangedu.cn

[S45] C++：lambda
来源：http://gn.colortex.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mk.shtwfgs.cn

[S46] C++：函数模板
来源：http://sb.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ht.bjjhwx.cn

[S47] C++：结构化绑定遍历
来源：http://ib.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bz.hnjuh.cn

[S48] C++：逐行读文件
来源：http://rr.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pe.colortex.cn

while (std::getline(in, line)) { }
来源：http://ti.szsharing.cn

[S49] C++：写文件
来源：http://ei.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zy.nicolike.cn

[S50] C++：格式化数字
来源：http://oi.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xd.newstarts.cn

[S51] C++：显式类型转换
来源：http://zq.chemitech.net.cn

static_cast<double>(a) / b
来源：http://wb.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://at.huanxung.cn

int size() const noexcept { return n_; }
来源：http://zr.gzmigu.cn

[S53] C++：移动语义
来源：http://ky.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://it.bookmarksfly.cn

[S54] C++：异常处理
来源：http://xw.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bp.panjiajie.cn

[S55] C++：结构化绑定
来源：http://ot.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rq.huanxung.cn

[S56] C++：optional
来源：http://bs.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wj.9csxet.cn

[S57] C++：编译期常量
来源：http://ef.shxzskj.cn

constexpr int N = 10;
来源：http://mx.panjiajie.cn

[S58] C++：命名空间
来源：http://lf.asd995.cn


<!-- 参考信息 -->