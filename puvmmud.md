代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mk.panjiajie.cn

[Q90] 生成序号列
来源：http://lq.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hx.huanxung.cn

================================================================================
来源：http://jq.huixinmuqiang.cn

R. Bash 专题
来源：http://xn.szxytkj.cn

================================================================================
来源：http://nn.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://bs.wgjwhj.cn

#!/usr/bin/env bash
来源：http://ud.bookmarksfly.cn

set -euo pipefail
来源：http://lm.szsharing.cn

[R02] 变量赋值与使用
来源：http://dv.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://sv.9csxet.cn

[R03] 只读变量
来源：http://ti.szxytkj.cn

readonly PI=3.14
来源：http://rb.yuexingan06.cn

[R04] 位置参数
来源：http://xk.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ja.jianghongdianzi.cn

[R05] 参数默认值
来源：http://um.shxzukj.cn

name="${1:-default}"
来源：http://ar.gzmigu.cn

[R06] 判断命令是否存在
来源：http://hx.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ne.panjiajie.cn

[R07] if 判断文件
来源：http://dr.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ct.hahajie.cn

[R08] 数值比较
来源：http://gq.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gn.huixiangedu.cn

[R09] 字符串比较
来源：http://qf.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sl.gzmigu.cn

[R10] 正则匹配
来源：http://jg.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ae.hnjuh.cn

[R11] case 多分支
来源：http://bi.colortex.cn

case "$1" in
来源：http://qh.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://py.shtwfgs.cn

stop)  echo "停止" ;;
来源：http://kq.newstarts.cn

*)     echo "未知命令" ;;
来源：http://im.jctech888.com.cn

esac
来源：http://hw.521024.cn

[R12] for 遍历文件
来源：http://sp.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://in.gzmigu.cn

[R13] for 计数循环
来源：http://dy.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://mz.bjjhwx.cn

[R14] C 风格 for
来源：http://vy.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lr.521024.cn

[R15] while 逐行读文件
来源：http://aj.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ip.9csxet.cn

[R16] until 等待条件
来源：http://pl.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://se.chemitech.net.cn

[R17] 数组定义与取值
来源：http://vg.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qt.jianghongdianzi.cn

[R18] 遍历数组
来源：http://gg.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dp.hnjuh.cn

[R19] 数组长度
来源：http://wg.szsharing.cn

echo "${#arr[@]}"
来源：http://at.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://rh.panjiajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cz.szsharing.cn

[R21] 字符串长度
来源：http://vq.shxzskj.cn

echo "${#s}"
来源：http://oa.shxzukj.cn

[R22] 截取子串
来源：http://rz.asd995.cn

echo "${s:0:5}"
来源：http://mv.panjiajie.cn

[R23] 字符串替换
来源：http://le.bjjhwx.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://km.wgjwhj.cn

[R24] 大小写转换
来源：http://ue.szxytkj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yg.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://gv.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zs.bookmarksfly.cn

[R26] 命令替换
来源：http://gq.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://bf.jctech888.com.cn

[R27] 算术展开
来源：http://in.asd995.cn

echo $((1 + 2 * 3))
来源：http://ry.szsharing.cn

[R28] 浮点运算
来源：http://qh.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://ax.huixiangedu.cn

[R29] 定义函数
来源：http://po.bjjhwx.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ex.nszjky.cn

[R30] 函数返回状态码
来源：http://wz.lnxyls.cn

f() { return 0; }; f || echo "失败了"
来源：http://os.9csxet.cn

[R31] 局部变量
来源：http://jy.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://md.muxihuayi.cn

[R32] 参数个数校验
来源：http://qf.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ms.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://qk.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hs.yuexingan06.cn

[R34] 退出时清理
来源：http://po.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gv.521024.cn

[R35] 后台执行并等待
来源：http://ow.hahajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ip.521024.cn

[R36] 并发执行多个任务
来源：http://dz.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cy.521024.cn

[R37] 把输出赋给变量
来源：http://gx.521024.cn

files=$(ls -1)
来源：http://ei.muxihuayi.cn

[R38] 管道串联
来源：http://ik.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://aq.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://yu.haigaiapp.cn

cmd > out.log 2>&1
来源：http://xt.nicolike.cn

[R40] 追加写日志
来源：http://bf.huixiangedu.cn

echo "log" >> out.log
来源：http://oo.bjjhwx.cn

[R41] 丢弃输出
来源：http://kt.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://fa.nszjky.cn

[R42] 输入重定向
来源：http://kp.shtwfgs.cn

wc -l < a.txt
来源：http://jv.haigaiapp.cn

[R43] 按名字查找文件
来源：http://cb.lnxyls.cn

find . -name "*.log" -type f
来源：http://ko.shxzukj.cn

[R44] 按修改时间查找
来源：http://fi.haigaiapp.cn

find . -mtime -7 -type f
来源：http://tg.szxytkj.cn

[R45] 批量删除
来源：http://qs.szsharing.cn

find . -name "*.tmp" -delete
来源：http://dn.nszjky.cn

[R46] 递归替换文件内容
来源：http://dd.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ws.huanxung.cn

[R47] sed 单行替换
来源：http://bt.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://io.newstarts.cn

[R48] awk 取指定列
来源：http://um.gzmigu.cn

awk '{print $1, $3}' a.txt
来源：http://dj.chemitech.net.cn

[R49] awk 带条件
来源：http://un.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vd.gzmigu.cn

[R50] awk 求和
来源：http://fp.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ge.szsharing.cn

[R51] 排序去重取前几
来源：http://uh.yuexingan06.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://uv.yuexingan06.cn

[R52] 统计行数
来源：http://sf.shxzskj.cn

wc -l a.txt
来源：http://ys.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://za.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zj.wgjwhj.cn

[R54] 比较两个文件
来源：http://ha.chemitech.net.cn

diff a.txt b.txt
来源：http://hr.newstarts.cn

[R55] 压缩与解压
来源：http://du.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zq.lnxyls.cn

[R56] 远程拷贝
来源：http://dw.nszjky.cn

scp file user@host:/path/
来源：http://pm.gzmigu.cn

[R57] 远程执行命令
来源：http://lr.newstarts.cn

ssh user@host 'uptime'
来源：http://zv.huixinmuqiang.cn

[R58] 下载文件
来源：http://oy.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zy.newstarts.cn

[R59] 发 POST JSON
来源：http://lv.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wp.jianghongdianzi.cn

[R60] 只看 HTTP 状态码
来源：http://yf.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fe.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://gz.chemitech.net.cn

df -h;  du -sh *
来源：http://oq.shxzukj.cn

[R62] 找最占空间的文件
来源：http://zi.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://hb.gzmigu.cn

[R63] 内存与进程
来源：http://ec.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://cp.bjjhwx.cn

[R64] 结束进程
来源：http://ju.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://st.gzmigu.cn

[R65] 查看端口占用
来源：http://vb.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://na.huixinmuqiang.cn

[R66] 定时任务
来源：http://gq.nszjky.cn

crontab -e;  crontab -l
来源：http://xa.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://fb.szxytkj.cn

openssl rand -hex 16
来源：http://wv.nszjky.cn

[R68] 计算文件校验值
来源：http://vr.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uj.521024.cn

[R69] 生成随机密码
来源：http://os.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://yf.521024.cn

[R70] 时间戳与互转
来源：http://hw.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://ei.hahajie.cn

[R71] 日期格式化
来源：http://id.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qx.asd995.cn

[R72] 等待端口就绪
来源：http://yo.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ky.newstarts.cn

[R73] 分割大日志
来源：http://ch.muxihuayi.cn

split -l 1000 big.log part_
来源：http://za.gzmigu.cn

[R74] 批量重命名
来源：http://fh.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ah.szxytkj.cn

[R75] 导出环境变量
来源：http://es.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://li.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://uy.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zu.hahajie.cn

[R77] 读取用户输入
来源：http://mq.nszjky.cn

read -rp "请输入: " ans
来源：http://ng.huanxung.cn

[R78] 交互式菜单
来源：http://sk.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kh.shxzskj.cn

[R79] 解析命令行选项
来源：http://rd.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xd.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://dx.szxytkj.cn

time ./run.sh
来源：http://oa.lnxyls.cn

================================================================================
来源：http://rh.huixinmuqiang.cn

S. C / C++ 专题
来源：http://ri.jctech888.com.cn

================================================================================
来源：http://ge.521024.cn

[S01] C：Hello World
来源：http://pp.haigaiapp.cn

#include <stdio.h>
来源：http://gv.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pb.szsharing.cn

[S02] C：变量与格式化输出
来源：http://jw.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://eh.panjiajie.cn

[S03] C：读入整数
来源：http://tl.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://pr.colortex.cn

[S04] C：字符串复制
来源：http://nv.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zw.huixiangedu.cn

[S05] C：字符串长度
来源：http://ev.shtwfgs.cn

strlen(s)
来源：http://gw.huanxung.cn

[S06] C：字符串比较
来源：http://qb.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://su.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://in.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iq.521024.cn

[S08] C：动态内存分配与释放
来源：http://el.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vx.panjiajie.cn

[S09] C：结构体定义与初始化
来源：http://ar.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lx.bjjhwx.cn

[S10] C：指针与解引用
来源：http://ei.huixinmuqiang.cn

int *p = &a;  *p = 5;
来源：http://si.colortex.cn

[S11] C：逐行读文件
来源：http://fc.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://wc.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zy.szsharing.cn

fclose(f);
来源：http://bp.bookmarksfly.cn

[S12] C：写文件
来源：http://ua.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vp.huixiangedu.cn

[S13] C：宏定义
来源：http://xt.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pv.chemitech.net.cn

[S14] C：枚举
来源：http://br.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://xu.jctech888.com.cn

[S15] C：类型转换
来源：http://bs.521024.cn

(double) a / b
来源：http://ey.521024.cn

[S16] C：位操作置位
来源：http://hi.jctech888.com.cn

x |= (1 << 3);
来源：http://gf.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://wu.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tr.szxytkj.cn

[S18] C：命令行参数
来源：http://gk.szsharing.cn

int main(int argc, char **argv)
来源：http://ld.yuntaijiaju.cn

[S19] C：快速排序
来源：http://kh.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jp.bookmarksfly.cn

[S20] C：二分查找
来源：http://ps.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hq.nicolike.cn

[S21] C：字符类别判断
来源：http://qv.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mg.521024.cn

[S22] C：字符串转数字
来源：http://cs.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ah.haigaiapp.cn

[S23] C：随机数
来源：http://yn.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://na.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://fx.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sg.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://js.asd995.cn

memcpy(dst, src, n);
来源：http://yq.chemitech.net.cn

[S26] C：内存清零
来源：http://ns.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://ea.nicolike.cn

[S27] C：定义常量
来源：http://lv.shxzukj.cn

const double PI = 3.14159;
来源：http://sy.hnjuh.cn

[S28] C：静态变量
来源：http://cd.huixinmuqiang.cn

static int counter = 0;
来源：http://mx.huixinmuqiang.cn

[S29] C：变参函数
来源：http://vv.9csxet.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tr.newstarts.cn

[S30] C：头文件保护
来源：http://ha.jianghongdianzi.cn

#ifndef X_H
来源：http://iu.panjiajie.cn

#define X_H
来源：http://dn.huixinmuqiang.cn

#endif
来源：http://qb.bjjhwx.cn

[S31] C++：Hello World
来源：http://pt.9csxet.cn

#include <iostream>
来源：http://yp.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://lx.huanxung.cn

[S32] C++：字符串
来源：http://ic.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://hm.haigaiapp.cn

[S33] C++：vector 增删
来源：http://uv.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tg.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://pi.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://uv.gzmigu.cn

[S35] C++：map
来源：http://qk.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cs.hahajie.cn

[S36] C++：unordered_map
来源：http://su.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ai.jctech888.com.cn

[S37] C++：set
来源：http://di.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gy.huixiangedu.cn

[S38] C++：排序
来源：http://ey.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://rq.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://np.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zu.9csxet.cn

[S40] C++：查找元素
来源：http://pw.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oh.colortex.cn

[S41] C++：类与构造函数
来源：http://vy.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hi.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://qa.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://tx.jctech888.com.cn

[S43] C++：智能指针
来源：http://tv.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://qn.huixiangedu.cn

[S44] C++：引用传参
来源：http://hu.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://zq.shxzukj.cn

[S45] C++：lambda
来源：http://ey.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://te.szxytkj.cn

[S46] C++：函数模板
来源：http://lb.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://js.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://ih.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hs.szsharing.cn

[S48] C++：逐行读文件
来源：http://yt.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dr.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://hk.lnxyls.cn

[S49] C++：写文件
来源：http://kw.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ze.shtwfgs.cn

[S50] C++：格式化数字
来源：http://hd.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ok.nicolike.cn

[S51] C++：显式类型转换
来源：http://fk.9csxet.cn

static_cast<double>(a) / b
来源：http://cx.huixinmuqiang.cn

[S52] C++：const 与 noexcept
来源：http://pf.hahajie.cn

int size() const noexcept { return n_; }
来源：http://pc.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://dg.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://mz.gzmigu.cn

[S54] C++：异常处理
来源：http://tq.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gy.asd995.cn

[S55] C++：结构化绑定
来源：http://ra.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mo.muxihuayi.cn

[S56] C++：optional
来源：http://rt.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kt.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://zl.muxihuayi.cn

constexpr int N = 10;
来源：http://kb.huixiangedu.cn

[S58] C++：命名空间
来源：http://xi.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://kr.szxytkj.cn

[S59] C++：静态断言
来源：http://gf.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pp.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://ov.nicolike.cn


<!-- 参考信息 -->