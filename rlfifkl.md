代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fh.jctech888.com.cn

[Q90] 生成序号列
来源：http://rr.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fy.hnjuh.cn

================================================================================
来源：http://rc.asd995.cn

R. Bash 专题
来源：http://oz.hnjuh.cn

================================================================================
来源：http://es.shxzukj.cn

[R01] shebang 与严格模式
来源：http://oc.szsharing.cn

#!/usr/bin/env bash
来源：http://es.szsharing.cn

set -euo pipefail
来源：http://qm.bjjhwx.cn

[R02] 变量赋值与使用
来源：http://dp.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://mo.shtwfgs.cn

[R03] 只读变量
来源：http://qq.jianghongdianzi.cn

readonly PI=3.14
来源：http://he.shxzskj.cn

[R04] 位置参数
来源：http://pk.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bb.huixiangedu.cn

[R05] 参数默认值
来源：http://ns.jianghongdianzi.cn

name="${1:-default}"
来源：http://ll.asd995.cn

[R06] 判断命令是否存在
来源：http://qt.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zc.colortex.cn

[R07] if 判断文件
来源：http://to.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nb.nicolike.cn

[R08] 数值比较
来源：http://oi.szxytkj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yl.muxihuayi.cn

[R09] 字符串比较
来源：http://dt.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vy.nicolike.cn

[R10] 正则匹配
来源：http://md.shtwfgs.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://op.haigaiapp.cn

[R11] case 多分支
来源：http://mb.9csxet.cn

case "$1" in
来源：http://nf.gzmigu.cn

start) echo "启动" ;;
来源：http://fk.shxzukj.cn

stop)  echo "停止" ;;
来源：http://th.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://ll.chemitech.net.cn

esac
来源：http://jx.asd995.cn

[R12] for 遍历文件
来源：http://om.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://dn.jctech888.com.cn

[R13] for 计数循环
来源：http://gc.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://ht.szxytkj.cn

[R14] C 风格 for
来源：http://ey.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yj.wgjwhj.cn

[R15] while 逐行读文件
来源：http://io.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mt.huixiangedu.cn

[R16] until 等待条件
来源：http://wl.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xp.panjiajie.cn

[R17] 数组定义与取值
来源：http://hn.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wu.jianghongdianzi.cn

[R18] 遍历数组
来源：http://az.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ak.jctech888.com.cn

[R19] 数组长度
来源：http://od.szxytkj.cn

echo "${#arr[@]}"
来源：http://pz.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://oi.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zy.shxzskj.cn

[R21] 字符串长度
来源：http://sz.muxihuayi.cn

echo "${#s}"
来源：http://vf.jctech888.com.cn

[R22] 截取子串
来源：http://sb.shxzukj.cn

echo "${s:0:5}"
来源：http://tt.yuntaijiaju.cn

[R23] 字符串替换
来源：http://uy.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qy.nicolike.cn

[R24] 大小写转换
来源：http://sk.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://re.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://rv.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pl.shxzukj.cn

[R26] 命令替换
来源：http://ci.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://zb.muxihuayi.cn

[R27] 算术展开
来源：http://zx.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://ue.huixiangedu.cn

[R28] 浮点运算
来源：http://pc.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://vy.yuntaijiaju.cn

[R29] 定义函数
来源：http://mq.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ew.huanxung.cn

[R30] 函数返回状态码
来源：http://zs.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://do.yuexingan06.cn

[R31] 局部变量
来源：http://or.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://xf.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://ie.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hx.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://ro.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://en.9csxet.cn

[R34] 退出时清理
来源：http://av.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dk.muxihuayi.cn

[R35] 后台执行并等待
来源：http://du.gzmigu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xl.hnjuh.cn

[R36] 并发执行多个任务
来源：http://vk.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fj.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://pt.hnjuh.cn

files=$(ls -1)
来源：http://sc.newstarts.cn

[R38] 管道串联
来源：http://sx.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://if.panjiajie.cn

[R39] 重定向标准输出与错误
来源：http://wa.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://pz.newstarts.cn

[R40] 追加写日志
来源：http://ay.shxzskj.cn

echo "log" >> out.log
来源：http://dl.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://cg.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://mq.lnxyls.cn

[R42] 输入重定向
来源：http://gg.shxzskj.cn

wc -l < a.txt
来源：http://ws.newstarts.cn

[R43] 按名字查找文件
来源：http://vy.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://yo.panjiajie.cn

[R44] 按修改时间查找
来源：http://rv.shxzskj.cn

find . -mtime -7 -type f
来源：http://ud.lnxyls.cn

[R45] 批量删除
来源：http://wk.szxytkj.cn

find . -name "*.tmp" -delete
来源：http://yw.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://em.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oc.szxytkj.cn

[R47] sed 单行替换
来源：http://jg.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ju.wgjwhj.cn

[R48] awk 取指定列
来源：http://lm.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://mw.shxzskj.cn

[R49] awk 带条件
来源：http://au.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gu.gzmigu.cn

[R50] awk 求和
来源：http://mb.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gq.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://xx.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ab.nicolike.cn

[R52] 统计行数
来源：http://ku.huixinmuqiang.cn

wc -l a.txt
来源：http://fe.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://qo.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://eb.newstarts.cn

[R54] 比较两个文件
来源：http://er.wgjwhj.cn

diff a.txt b.txt
来源：http://ob.colortex.cn

[R55] 压缩与解压
来源：http://ad.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rn.hnjuh.cn

[R56] 远程拷贝
来源：http://ai.huanxung.cn

scp file user@host:/path/
来源：http://mb.haigaiapp.cn

[R57] 远程执行命令
来源：http://ia.9csxet.cn

ssh user@host 'uptime'
来源：http://dq.yuexingan06.cn

[R58] 下载文件
来源：http://md.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dp.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://xq.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ty.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://pj.muxihuayi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xh.yuexingan06.cn

[R61] 磁盘占用
来源：http://js.521024.cn

df -h;  du -sh *
来源：http://od.newstarts.cn

[R62] 找最占空间的文件
来源：http://tg.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://zr.huixinmuqiang.cn

[R63] 内存与进程
来源：http://ir.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://bq.huixiangedu.cn

[R64] 结束进程
来源：http://tj.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://uh.shtwfgs.cn

[R65] 查看端口占用
来源：http://df.szxytkj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zn.szsharing.cn

[R66] 定时任务
来源：http://ta.gzmigu.cn

crontab -e;  crontab -l
来源：http://qq.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://gm.521024.cn

openssl rand -hex 16
来源：http://sc.yuexingan06.cn

[R68] 计算文件校验值
来源：http://qp.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ve.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://jg.colortex.cn

head -c 16 /dev/urandom | base64
来源：http://ak.nicolike.cn

[R70] 时间戳与互转
来源：http://jm.521024.cn

date +%s;  date -d @1700000000
来源：http://bu.huanxung.cn

[R71] 日期格式化
来源：http://bn.newstarts.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cc.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://fq.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zv.chemitech.net.cn

[R73] 分割大日志
来源：http://um.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://cq.bookmarksfly.cn

[R74] 批量重命名
来源：http://xf.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://na.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://up.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://pj.nicolike.cn

[R76] 使用临时文件
来源：http://wb.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://su.szxytkj.cn

[R77] 读取用户输入
来源：http://zr.521024.cn

read -rp "请输入: " ans
来源：http://qb.lnxyls.cn

[R78] 交互式菜单
来源：http://qs.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cl.muxihuayi.cn

[R79] 解析命令行选项
来源：http://ek.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lc.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://ih.asd995.cn

time ./run.sh
来源：http://aa.bjjhwx.cn

================================================================================
来源：http://ei.shxzskj.cn

S. C / C++ 专题
来源：http://nc.nicolike.cn

================================================================================
来源：http://eb.jctech888.com.cn

[S01] C：Hello World
来源：http://mz.haigaiapp.cn

#include <stdio.h>
来源：http://ll.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ow.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://ak.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://xb.chemitech.net.cn

[S03] C：读入整数
来源：http://al.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://dc.shxzskj.cn

[S04] C：字符串复制
来源：http://es.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fm.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://dc.9csxet.cn

strlen(s)
来源：http://pv.nszjky.cn

[S06] C：字符串比较
来源：http://cd.asd995.cn

strcmp(a, b) == 0
来源：http://pn.colortex.cn

[S07] C：数组遍历求和
来源：http://jn.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ga.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://gl.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://er.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://hi.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dz.newstarts.cn

[S10] C：指针与解引用
来源：http://lk.huixinmuqiang.cn

int *p = &a;  *p = 5;
来源：http://np.newstarts.cn

[S11] C：逐行读文件
来源：http://id.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://fr.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sp.shxzukj.cn

fclose(f);
来源：http://jm.bookmarksfly.cn

[S12] C：写文件
来源：http://wh.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sf.szxytkj.cn

[S13] C：宏定义
来源：http://nc.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wr.asd995.cn

[S14] C：枚举
来源：http://ik.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://yw.hahajie.cn

[S15] C：类型转换
来源：http://xt.gzmigu.cn

(double) a / b
来源：http://ng.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://ab.shxzskj.cn

x |= (1 << 3);
来源：http://zk.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://ek.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ti.521024.cn

[S18] C：命令行参数
来源：http://di.szxytkj.cn

int main(int argc, char **argv)
来源：http://tt.huanxung.cn

[S19] C：快速排序
来源：http://tc.newstarts.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uc.wgjwhj.cn

[S20] C：二分查找
来源：http://zg.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hq.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://kk.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pv.shtwfgs.cn

[S22] C：字符串转数字
来源：http://im.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://za.yuntaijiaju.cn

[S23] C：随机数
来源：http://gx.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://du.nicolike.cn

[S24] C：获取本地时间
来源：http://pw.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oo.shxzukj.cn

[S25] C：内存拷贝
来源：http://mu.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://rv.9csxet.cn

[S26] C：内存清零
来源：http://he.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://ro.nicolike.cn

[S27] C：定义常量
来源：http://uv.bjjhwx.cn

const double PI = 3.14159;
来源：http://ri.newstarts.cn

[S28] C：静态变量
来源：http://sg.chemitech.net.cn

static int counter = 0;
来源：http://gl.panjiajie.cn

[S29] C：变参函数
来源：http://is.9csxet.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ul.9csxet.cn

[S30] C：头文件保护
来源：http://sb.521024.cn

#ifndef X_H
来源：http://wo.colortex.cn

#define X_H
来源：http://qb.shxzskj.cn

#endif
来源：http://lk.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://tn.panjiajie.cn

#include <iostream>
来源：http://xx.huanxung.cn

int main() { std::cout << "Hello\n"; }
来源：http://jp.huixiangedu.cn

[S32] C++：字符串
来源：http://lo.huixinmuqiang.cn

std::string s = "hi";  s += "!";
来源：http://gf.wgjwhj.cn

[S33] C++：vector 增删
来源：http://ve.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://py.lnxyls.cn

[S34] C++：遍历 vector
来源：http://lk.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://ak.gzmigu.cn

[S35] C++：map
来源：http://iv.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bm.9csxet.cn

[S36] C++：unordered_map
来源：http://kk.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sr.521024.cn

[S37] C++：set
来源：http://nm.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wa.521024.cn

[S38] C++：排序
来源：http://dr.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://mc.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://oi.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ti.nicolike.cn

[S40] C++：查找元素
来源：http://vn.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lr.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://va.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://as.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://sz.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://ra.bookmarksfly.cn

[S43] C++：智能指针
来源：http://hc.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://pp.newstarts.cn

[S44] C++：引用传参
来源：http://ag.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://bl.huixiangedu.cn

[S45] C++：lambda
来源：http://np.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xi.yuexingan06.cn

[S46] C++：函数模板
来源：http://nl.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gr.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://um.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mr.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://oj.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gj.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://df.haigaiapp.cn

[S49] C++：写文件
来源：http://lx.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rx.hnjuh.cn

[S50] C++：格式化数字
来源：http://sn.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xe.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://vx.shxzskj.cn

static_cast<double>(a) / b
来源：http://yh.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://bg.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://od.szxytkj.cn

[S53] C++：移动语义
来源：http://wj.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://jt.newstarts.cn

[S54] C++：异常处理
来源：http://gw.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lm.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://pn.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ad.panjiajie.cn

[S56] C++：optional
来源：http://gd.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eq.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://xp.huixinmuqiang.cn

constexpr int N = 10;
来源：http://nj.shxzukj.cn

[S58] C++：命名空间
来源：http://zh.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://xb.shxzskj.cn

[S59] C++：静态断言
来源：http://ez.yuntaijiaju.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tr.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://sj.colortex.cn


<!-- 参考信息 -->