代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zj.muxihuayi.cn

[Q90] 生成序号列
来源：http://ko.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://of.colortex.cn

================================================================================
来源：http://pl.huanxung.cn

R. Bash 专题
来源：http://lc.haigaiapp.cn

================================================================================
来源：http://xj.asd995.cn

[R01] shebang 与严格模式
来源：http://vt.colortex.cn

#!/usr/bin/env bash
来源：http://ct.shxzukj.cn

set -euo pipefail
来源：http://ak.szsharing.cn

[R02] 变量赋值与使用
来源：http://xe.newstarts.cn

name="Tom"; echo "$name"
来源：http://xj.nicolike.cn

[R03] 只读变量
来源：http://mc.9csxet.cn

readonly PI=3.14
来源：http://rz.hahajie.cn

[R04] 位置参数
来源：http://ya.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eo.jctech888.com.cn

[R05] 参数默认值
来源：http://ay.jianghongdianzi.cn

name="${1:-default}"
来源：http://jw.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://mv.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gv.shxzukj.cn

[R07] if 判断文件
来源：http://fr.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ft.gzmigu.cn

[R08] 数值比较
来源：http://yu.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nc.gzmigu.cn

[R09] 字符串比较
来源：http://yl.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jv.bjjhwx.cn

[R10] 正则匹配
来源：http://wb.newstarts.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dj.nicolike.cn

[R11] case 多分支
来源：http://xw.nszjky.cn

case "$1" in
来源：http://zj.hahajie.cn

start) echo "启动" ;;
来源：http://tt.nicolike.cn

stop)  echo "停止" ;;
来源：http://iy.szsharing.cn

*)     echo "未知命令" ;;
来源：http://pg.bookmarksfly.cn

esac
来源：http://mq.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://wm.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://hi.muxihuayi.cn

[R13] for 计数循环
来源：http://bq.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://la.muxihuayi.cn

[R14] C 风格 for
来源：http://mq.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kb.shxzukj.cn

[R15] while 逐行读文件
来源：http://ui.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gw.shtwfgs.cn

[R16] until 等待条件
来源：http://ww.muxihuayi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wk.szxytkj.cn

[R17] 数组定义与取值
来源：http://tz.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://im.asd995.cn

[R18] 遍历数组
来源：http://ig.9csxet.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sr.nicolike.cn

[R19] 数组长度
来源：http://fy.shtwfgs.cn

echo "${#arr[@]}"
来源：http://xw.hnjuh.cn

[R20] 关联数组（字典）
来源：http://pp.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zl.lnxyls.cn

[R21] 字符串长度
来源：http://vt.huixinmuqiang.cn

echo "${#s}"
来源：http://ss.bookmarksfly.cn

[R22] 截取子串
来源：http://bv.hnjuh.cn

echo "${s:0:5}"
来源：http://oy.newstarts.cn

[R23] 字符串替换
来源：http://rs.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pu.9csxet.cn

[R24] 大小写转换
来源：http://yu.521024.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zg.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://xk.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zd.muxihuayi.cn

[R26] 命令替换
来源：http://de.haigaiapp.cn

now=$(date +%F); echo "$now"
来源：http://et.asd995.cn

[R27] 算术展开
来源：http://kf.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://zb.nicolike.cn

[R28] 浮点运算
来源：http://tg.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://sz.nicolike.cn

[R29] 定义函数
来源：http://bc.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kc.hnjuh.cn

[R30] 函数返回状态码
来源：http://va.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://kz.9csxet.cn

[R31] 局部变量
来源：http://on.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://gr.521024.cn

[R32] 参数个数校验
来源：http://rt.haigaiapp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kn.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://nz.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sl.huixinmuqiang.cn

[R34] 退出时清理
来源：http://iy.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://km.gzmigu.cn

[R35] 后台执行并等待
来源：http://rm.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dl.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://uk.shxzukj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fj.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://ca.huixinmuqiang.cn

files=$(ls -1)
来源：http://xn.muxihuayi.cn

[R38] 管道串联
来源：http://gw.nicolike.cn

cat a.txt | grep -i error | wc -l
来源：http://lp.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://vd.shxzukj.cn

cmd > out.log 2>&1
来源：http://xc.panjiajie.cn

[R40] 追加写日志
来源：http://ua.huanxung.cn

echo "log" >> out.log
来源：http://fn.nicolike.cn

[R41] 丢弃输出
来源：http://ep.lnxyls.cn

cmd >/dev/null 2>&1
来源：http://ht.shxzskj.cn

[R42] 输入重定向
来源：http://sn.newstarts.cn

wc -l < a.txt
来源：http://ul.wgjwhj.cn

[R43] 按名字查找文件
来源：http://ah.lnxyls.cn

find . -name "*.log" -type f
来源：http://kd.shxzskj.cn

[R44] 按修改时间查找
来源：http://nv.wgjwhj.cn

find . -mtime -7 -type f
来源：http://tu.nszjky.cn

[R45] 批量删除
来源：http://co.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://ny.nicolike.cn

[R46] 递归替换文件内容
来源：http://zs.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xx.shxzskj.cn

[R47] sed 单行替换
来源：http://fd.panjiajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wi.colortex.cn

[R48] awk 取指定列
来源：http://vj.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://mp.9csxet.cn

[R49] awk 带条件
来源：http://ct.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tv.szxytkj.cn

[R50] awk 求和
来源：http://ni.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xs.colortex.cn

[R51] 排序去重取前几
来源：http://zu.jianghongdianzi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mr.newstarts.cn

[R52] 统计行数
来源：http://ed.muxihuayi.cn

wc -l a.txt
来源：http://re.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://ox.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gy.huixiangedu.cn

[R54] 比较两个文件
来源：http://rx.chemitech.net.cn

diff a.txt b.txt
来源：http://zf.szxytkj.cn

[R55] 压缩与解压
来源：http://ht.shxzukj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ad.colortex.cn

[R56] 远程拷贝
来源：http://cm.huixiangedu.cn

scp file user@host:/path/
来源：http://qm.521024.cn

[R57] 远程执行命令
来源：http://xm.newstarts.cn

ssh user@host 'uptime'
来源：http://xh.hahajie.cn

[R58] 下载文件
来源：http://ye.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ce.shxzskj.cn

[R59] 发 POST JSON
来源：http://ok.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wt.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://bs.yuntaijiaju.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kw.jctech888.com.cn

[R61] 磁盘占用
来源：http://qt.huanxung.cn

df -h;  du -sh *
来源：http://lg.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://as.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://mk.shxzskj.cn

[R63] 内存与进程
来源：http://bf.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://nx.9csxet.cn

[R64] 结束进程
来源：http://uj.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://iz.szsharing.cn

[R65] 查看端口占用
来源：http://ur.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dg.bookmarksfly.cn

[R66] 定时任务
来源：http://os.muxihuayi.cn

crontab -e;  crontab -l
来源：http://xd.asd995.cn

[R67] 生成随机十六进制串
来源：http://xq.muxihuayi.cn

openssl rand -hex 16
来源：http://by.shtwfgs.cn

[R68] 计算文件校验值
来源：http://dx.gzmigu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gd.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://px.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://rj.huanxung.cn

[R70] 时间戳与互转
来源：http://ae.521024.cn

date +%s;  date -d @1700000000
来源：http://uy.bookmarksfly.cn

[R71] 日期格式化
来源：http://pc.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gm.jctech888.com.cn

[R72] 等待端口就绪
来源：http://tq.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zk.bookmarksfly.cn

[R73] 分割大日志
来源：http://yh.szxytkj.cn

split -l 1000 big.log part_
来源：http://iu.shxzskj.cn

[R74] 批量重命名
来源：http://vf.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://np.huanxung.cn

[R75] 导出环境变量
来源：http://sx.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://ug.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://sf.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bm.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://yd.muxihuayi.cn

read -rp "请输入: " ans
来源：http://cl.nicolike.cn

[R78] 交互式菜单
来源：http://gj.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://iq.huanxung.cn

[R79] 解析命令行选项
来源：http://fl.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gh.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://gz.colortex.cn

time ./run.sh
来源：http://dd.yuntaijiaju.cn

================================================================================
来源：http://th.hahajie.cn

S. C / C++ 专题
来源：http://qm.asd995.cn

================================================================================
来源：http://qf.jianghongdianzi.cn

[S01] C：Hello World
来源：http://nh.shtwfgs.cn

#include <stdio.h>
来源：http://et.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://iv.asd995.cn

[S02] C：变量与格式化输出
来源：http://ms.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://se.colortex.cn

[S03] C：读入整数
来源：http://qh.colortex.cn

int x; scanf("%d", &x);
来源：http://yp.hahajie.cn

[S04] C：字符串复制
来源：http://rl.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sx.nicolike.cn

[S05] C：字符串长度
来源：http://qf.nicolike.cn

strlen(s)
来源：http://ey.gzmigu.cn

[S06] C：字符串比较
来源：http://uw.9csxet.cn

strcmp(a, b) == 0
来源：http://it.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://qu.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xy.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://az.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mn.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://av.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lr.521024.cn

[S10] C：指针与解引用
来源：http://pc.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://mk.panjiajie.cn

[S11] C：逐行读文件
来源：http://sn.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://dt.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bi.bookmarksfly.cn

fclose(f);
来源：http://zb.chemitech.net.cn

[S12] C：写文件
来源：http://fd.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bl.panjiajie.cn

[S13] C：宏定义
来源：http://sk.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jn.asd995.cn

[S14] C：枚举
来源：http://cu.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://pi.521024.cn

[S15] C：类型转换
来源：http://mo.bjjhwx.cn

(double) a / b
来源：http://dn.shtwfgs.cn

[S16] C：位操作置位
来源：http://wf.szxytkj.cn

x |= (1 << 3);
来源：http://my.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://ze.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ji.nszjky.cn

[S18] C：命令行参数
来源：http://jm.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://fv.lnxyls.cn

[S19] C：快速排序
来源：http://rq.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qx.yuntaijiaju.cn

[S20] C：二分查找
来源：http://sp.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xo.newstarts.cn

[S21] C：字符类别判断
来源：http://ud.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://te.hnjuh.cn

[S22] C：字符串转数字
来源：http://ij.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://um.9csxet.cn

[S23] C：随机数
来源：http://kv.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://el.szxytkj.cn

[S24] C：获取本地时间
来源：http://vp.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ko.521024.cn

[S25] C：内存拷贝
来源：http://br.hnjuh.cn

memcpy(dst, src, n);
来源：http://pm.bookmarksfly.cn

[S26] C：内存清零
来源：http://oh.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://zu.yuexingan06.cn

[S27] C：定义常量
来源：http://fs.shxzukj.cn

const double PI = 3.14159;
来源：http://bl.haigaiapp.cn

[S28] C：静态变量
来源：http://af.panjiajie.cn

static int counter = 0;
来源：http://wg.szxytkj.cn

[S29] C：变参函数
来源：http://xy.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nd.huixiangedu.cn

[S30] C：头文件保护
来源：http://hf.shtwfgs.cn

#ifndef X_H
来源：http://cm.gzmigu.cn

#define X_H
来源：http://yz.huixinmuqiang.cn

#endif
来源：http://jf.huixiangedu.cn

[S31] C++：Hello World
来源：http://dv.nicolike.cn

#include <iostream>
来源：http://bq.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://kt.521024.cn

[S32] C++：字符串
来源：http://qn.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://tq.jctech888.com.cn

[S33] C++：vector 增删
来源：http://hi.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fs.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://za.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://xd.newstarts.cn

[S35] C++：map
来源：http://ky.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jv.szxytkj.cn

[S36] C++：unordered_map
来源：http://mz.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mb.shxzskj.cn

[S37] C++：set
来源：http://wo.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dw.gzmigu.cn

[S38] C++：排序
来源：http://ma.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://hv.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://vu.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pf.9csxet.cn

[S40] C++：查找元素
来源：http://ai.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ru.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://we.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zf.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://zb.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://jn.nszjky.cn

[S43] C++：智能指针
来源：http://aj.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://sp.muxihuayi.cn

[S44] C++：引用传参
来源：http://ck.asd995.cn

void inc(int &x) { ++x; }
来源：http://us.bjjhwx.cn

[S45] C++：lambda
来源：http://xu.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lj.jctech888.com.cn

[S46] C++：函数模板
来源：http://gf.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gp.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://lc.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yc.huanxung.cn

[S48] C++：逐行读文件
来源：http://os.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oq.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://ef.bookmarksfly.cn

[S49] C++：写文件
来源：http://iu.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://md.jctech888.com.cn

[S50] C++：格式化数字
来源：http://pf.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://no.chemitech.net.cn

[S51] C++：显式类型转换
来源：http://qq.szxytkj.cn

static_cast<double>(a) / b
来源：http://vu.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://aj.newstarts.cn

int size() const noexcept { return n_; }
来源：http://qo.huixiangedu.cn

[S53] C++：移动语义
来源：http://wn.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://vf.yuexingan06.cn

[S54] C++：异常处理
来源：http://ya.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oz.nszjky.cn

[S55] C++：结构化绑定
来源：http://dl.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hd.newstarts.cn

[S56] C++：optional
来源：http://ng.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vn.huixinmuqiang.cn

[S57] C++：编译期常量
来源：http://zi.nszjky.cn

constexpr int N = 10;
来源：http://ch.yuexingan06.cn

[S58] C++：命名空间
来源：http://xt.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://uw.gzmigu.cn

[S59] C++：静态断言
来源：http://ho.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://li.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://bd.shtwfgs.cn


<!-- 参考信息 -->