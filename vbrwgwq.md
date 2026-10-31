代发 wailian999

[Q86] 读取 JSON 字段
来源：http://lf.haigaiapp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yn.huanxung.cn

[Q87] JSON 字段做条件
来源：http://or.shxzukj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oj.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://pt.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cn.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ou.hahajie.cn

[Q89] 判断表是否存在
来源：http://pk.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ds.huanxung.cn

[Q90] 生成序号列
来源：http://er.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ge.bookmarksfly.cn

================================================================================
来源：http://ob.yuntaijiaju.cn

R. Bash 专题
来源：http://sq.szxytkj.cn

================================================================================
来源：http://op.521024.cn

[R01] shebang 与严格模式
来源：http://ru.wgjwhj.cn

#!/usr/bin/env bash
来源：http://hs.shtwfgs.cn

set -euo pipefail
来源：http://jf.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://ev.shxzukj.cn

name="Tom"; echo "$name"
来源：http://pg.jctech888.com.cn

[R03] 只读变量
来源：http://bx.nicolike.cn

readonly PI=3.14
来源：http://zl.szsharing.cn

[R04] 位置参数
来源：http://dj.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://aq.huanxung.cn

[R05] 参数默认值
来源：http://yy.colortex.cn

name="${1:-default}"
来源：http://km.lnxyls.cn

[R06] 判断命令是否存在
来源：http://qw.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dd.szxytkj.cn

[R07] if 判断文件
来源：http://uc.9csxet.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qa.bookmarksfly.cn

[R08] 数值比较
来源：http://ig.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://on.jianghongdianzi.cn

[R09] 字符串比较
来源：http://zn.nszjky.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zy.bjjhwx.cn

[R10] 正则匹配
来源：http://ot.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vo.huixinmuqiang.cn

[R11] case 多分支
来源：http://vw.huanxung.cn

case "$1" in
来源：http://wz.nicolike.cn

start) echo "启动" ;;
来源：http://no.gzmigu.cn

stop)  echo "停止" ;;
来源：http://wk.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://wo.nicolike.cn

esac
来源：http://az.szsharing.cn

[R12] for 遍历文件
来源：http://bd.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://bc.bjjhwx.cn

[R13] for 计数循环
来源：http://bf.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://yl.huixiangedu.cn

[R14] C 风格 for
来源：http://ki.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wk.newstarts.cn

[R15] while 逐行读文件
来源：http://mg.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wy.hnjuh.cn

[R16] until 等待条件
来源：http://or.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qg.newstarts.cn

[R17] 数组定义与取值
来源：http://sb.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oi.lnxyls.cn

[R18] 遍历数组
来源：http://zi.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sl.shxzukj.cn

[R19] 数组长度
来源：http://ni.chemitech.net.cn

echo "${#arr[@]}"
来源：http://of.nszjky.cn

[R20] 关联数组（字典）
来源：http://sf.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fx.nicolike.cn

[R21] 字符串长度
来源：http://el.9csxet.cn

echo "${#s}"
来源：http://ra.shxzskj.cn

[R22] 截取子串
来源：http://cp.nszjky.cn

echo "${s:0:5}"
来源：http://si.shtwfgs.cn

[R23] 字符串替换
来源：http://vi.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bo.jianghongdianzi.cn

[R24] 大小写转换
来源：http://lj.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hf.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://dv.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wn.nicolike.cn

[R26] 命令替换
来源：http://pf.yuntaijiaju.cn

now=$(date +%F); echo "$now"
来源：http://yd.szxytkj.cn

[R27] 算术展开
来源：http://hh.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://jm.9csxet.cn

[R28] 浮点运算
来源：http://ng.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://cf.shxzukj.cn

[R29] 定义函数
来源：http://qi.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zd.szxytkj.cn

[R30] 函数返回状态码
来源：http://bz.9csxet.cn

f() { return 0; }; f || echo "失败了"
来源：http://mo.yuexingan06.cn

[R31] 局部变量
来源：http://lh.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://tw.nszjky.cn

[R32] 参数个数校验
来源：http://zs.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ug.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://dl.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jb.huixiangedu.cn

[R34] 退出时清理
来源：http://hr.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sj.asd995.cn

[R35] 后台执行并等待
来源：http://ee.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://po.hnjuh.cn

[R36] 并发执行多个任务
来源：http://bb.muxihuayi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kb.9csxet.cn

[R37] 把输出赋给变量
来源：http://tu.bjjhwx.cn

files=$(ls -1)
来源：http://ux.nicolike.cn

[R38] 管道串联
来源：http://fm.huixiangedu.cn

cat a.txt | grep -i error | wc -l
来源：http://mo.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://sw.panjiajie.cn

cmd > out.log 2>&1
来源：http://dw.gzmigu.cn

[R40] 追加写日志
来源：http://su.bjjhwx.cn

echo "log" >> out.log
来源：http://mi.nicolike.cn

[R41] 丢弃输出
来源：http://ad.jctech888.com.cn

cmd >/dev/null 2>&1
来源：http://qd.chemitech.net.cn

[R42] 输入重定向
来源：http://ie.huanxung.cn

wc -l < a.txt
来源：http://hw.nicolike.cn

[R43] 按名字查找文件
来源：http://iw.shtwfgs.cn

find . -name "*.log" -type f
来源：http://wa.szxytkj.cn

[R44] 按修改时间查找
来源：http://cq.haigaiapp.cn

find . -mtime -7 -type f
来源：http://gd.szsharing.cn

[R45] 批量删除
来源：http://bz.huanxung.cn

find . -name "*.tmp" -delete
来源：http://vf.521024.cn

[R46] 递归替换文件内容
来源：http://we.chemitech.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wq.huanxung.cn

[R47] sed 单行替换
来源：http://qb.bjjhwx.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yf.szxytkj.cn

[R48] awk 取指定列
来源：http://zq.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://ic.nszjky.cn

[R49] awk 带条件
来源：http://zb.lnxyls.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yw.szsharing.cn

[R50] awk 求和
来源：http://yg.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://aq.hnjuh.cn

[R51] 排序去重取前几
来源：http://lq.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ef.yuntaijiaju.cn

[R52] 统计行数
来源：http://xj.nszjky.cn

wc -l a.txt
来源：http://wu.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://gq.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iv.hnjuh.cn

[R54] 比较两个文件
来源：http://ut.9csxet.cn

diff a.txt b.txt
来源：http://vp.shxzskj.cn

[R55] 压缩与解压
来源：http://gt.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ug.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://pw.szxytkj.cn

scp file user@host:/path/
来源：http://xr.chemitech.net.cn

[R57] 远程执行命令
来源：http://np.chemitech.net.cn

ssh user@host 'uptime'
来源：http://qj.lnxyls.cn

[R58] 下载文件
来源：http://xn.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gw.gzmigu.cn

[R59] 发 POST JSON
来源：http://wv.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xu.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://nr.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ya.bookmarksfly.cn

[R61] 磁盘占用
来源：http://nq.gzmigu.cn

df -h;  du -sh *
来源：http://vv.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://ub.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://jj.szsharing.cn

[R63] 内存与进程
来源：http://id.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://bl.jianghongdianzi.cn

[R64] 结束进程
来源：http://cd.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://xz.asd995.cn

[R65] 查看端口占用
来源：http://fh.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xq.szsharing.cn

[R66] 定时任务
来源：http://zh.newstarts.cn

crontab -e;  crontab -l
来源：http://cr.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://wg.521024.cn

openssl rand -hex 16
来源：http://wk.shxzskj.cn

[R68] 计算文件校验值
来源：http://hr.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cl.shtwfgs.cn

[R69] 生成随机密码
来源：http://lv.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://tk.haigaiapp.cn

[R70] 时间戳与互转
来源：http://ko.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://lo.panjiajie.cn

[R71] 日期格式化
来源：http://mf.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xp.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://nr.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://um.huixinmuqiang.cn

[R73] 分割大日志
来源：http://gs.szsharing.cn

split -l 1000 big.log part_
来源：http://qh.muxihuayi.cn

[R74] 批量重命名
来源：http://wf.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tt.hahajie.cn

[R75] 导出环境变量
来源：http://rf.hnjuh.cn

export PATH="$HOME/bin:$PATH"
来源：http://me.huixiangedu.cn

[R76] 使用临时文件
来源：http://zc.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vn.chemitech.net.cn

[R77] 读取用户输入
来源：http://ev.shtwfgs.cn

read -rp "请输入: " ans
来源：http://or.newstarts.cn

[R78] 交互式菜单
来源：http://wn.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fn.haigaiapp.cn

[R79] 解析命令行选项
来源：http://pz.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bd.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://lm.521024.cn

time ./run.sh
来源：http://vg.bookmarksfly.cn

================================================================================
来源：http://nd.shxzukj.cn

S. C / C++ 专题
来源：http://az.szsharing.cn

================================================================================
来源：http://tg.huanxung.cn

[S01] C：Hello World
来源：http://si.shxzukj.cn

#include <stdio.h>
来源：http://gn.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ab.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://ok.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://kd.yuexingan06.cn

[S03] C：读入整数
来源：http://ny.colortex.cn

int x; scanf("%d", &x);
来源：http://zw.colortex.cn

[S04] C：字符串复制
来源：http://xm.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oj.wgjwhj.cn

[S05] C：字符串长度
来源：http://lr.wgjwhj.cn

strlen(s)
来源：http://na.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://pl.yuexingan06.cn

strcmp(a, b) == 0
来源：http://rm.asd995.cn

[S07] C：数组遍历求和
来源：http://zt.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uc.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://ut.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fw.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://wx.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://in.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://pc.huixinmuqiang.cn

int *p = &a;  *p = 5;
来源：http://lo.shtwfgs.cn

[S11] C：逐行读文件
来源：http://of.lnxyls.cn

FILE *f = fopen("a.txt", "r");
来源：http://wp.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hf.yuexingan06.cn

fclose(f);
来源：http://xx.szsharing.cn

[S12] C：写文件
来源：http://pw.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cy.bjjhwx.cn

[S13] C：宏定义
来源：http://ul.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gr.wgjwhj.cn

[S14] C：枚举
来源：http://fm.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://wh.nicolike.cn

[S15] C：类型转换
来源：http://wn.asd995.cn

(double) a / b
来源：http://ro.huixiangedu.cn

[S16] C：位操作置位
来源：http://ws.nszjky.cn

x |= (1 << 3);
来源：http://li.9csxet.cn

[S17] C：安全拼接字符串
来源：http://yc.lnxyls.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pj.haigaiapp.cn

[S18] C：命令行参数
来源：http://in.jctech888.com.cn

int main(int argc, char **argv)
来源：http://ks.colortex.cn

[S19] C：快速排序
来源：http://lv.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pl.muxihuayi.cn

[S20] C：二分查找
来源：http://aw.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qb.shtwfgs.cn

[S21] C：字符类别判断
来源：http://vn.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sx.jctech888.com.cn

[S22] C：字符串转数字
来源：http://rh.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://st.nszjky.cn

[S23] C：随机数
来源：http://wi.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ec.9csxet.cn

[S24] C：获取本地时间
来源：http://ln.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bg.szxytkj.cn

[S25] C：内存拷贝
来源：http://rf.shxzskj.cn

memcpy(dst, src, n);
来源：http://pf.szsharing.cn

[S26] C：内存清零
来源：http://zg.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://hq.shxzskj.cn

[S27] C：定义常量
来源：http://kc.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://wo.lnxyls.cn

[S28] C：静态变量
来源：http://ui.yuntaijiaju.cn

static int counter = 0;
来源：http://ta.huanxung.cn

[S29] C：变参函数
来源：http://fb.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yj.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://ve.shxzukj.cn

#ifndef X_H
来源：http://wf.muxihuayi.cn

#define X_H
来源：http://pf.shxzukj.cn

#endif
来源：http://ke.wgjwhj.cn

[S31] C++：Hello World
来源：http://sc.huixinmuqiang.cn

#include <iostream>
来源：http://vm.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://pl.szxytkj.cn

[S32] C++：字符串
来源：http://hy.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://xw.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://vu.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hd.colortex.cn

[S34] C++：遍历 vector
来源：http://nk.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://nc.newstarts.cn

[S35] C++：map
来源：http://dk.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dp.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://ah.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vq.9csxet.cn

[S37] C++：set
来源：http://ho.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cq.yuntaijiaju.cn

[S38] C++：排序
来源：http://yj.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://tr.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://ec.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tk.bookmarksfly.cn

[S40] C++：查找元素
来源：http://iz.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pr.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://uy.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xw.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://bb.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://jt.shtwfgs.cn

[S43] C++：智能指针
来源：http://yk.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://xw.yuexingan06.cn

[S44] C++：引用传参
来源：http://dz.szsharing.cn

void inc(int &x) { ++x; }
来源：http://tc.nicolike.cn

[S45] C++：lambda
来源：http://nj.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wo.yuexingan06.cn

[S46] C++：函数模板
来源：http://an.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://en.panjiajie.cn

[S47] C++：结构化绑定遍历
来源：http://nl.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ce.haigaiapp.cn

[S48] C++：逐行读文件
来源：http://os.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ey.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://fs.jctech888.com.cn

[S49] C++：写文件
来源：http://lz.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ep.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://va.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ph.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://rk.bjjhwx.cn

static_cast<double>(a) / b
来源：http://ma.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://fq.newstarts.cn

int size() const noexcept { return n_; }
来源：http://gn.521024.cn

[S53] C++：移动语义
来源：http://hj.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://ju.shtwfgs.cn

[S54] C++：异常处理
来源：http://gz.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pj.szsharing.cn

[S55] C++：结构化绑定
来源：http://ja.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wj.shxzskj.cn

[S56] C++：optional
来源：http://hh.nszjky.cn


<!-- 参考信息 -->