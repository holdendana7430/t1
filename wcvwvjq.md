代发 wailian999

[Q86] 读取 JSON 字段
来源：http://mv.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://on.colortex.cn

[Q87] JSON 字段做条件
来源：http://rt.newstarts.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bc.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://pk.jctech888.com.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fh.newstarts.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uj.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://be.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://il.haigaiapp.cn

[Q90] 生成序号列
来源：http://gn.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kp.muxihuayi.cn

================================================================================
来源：http://uo.shtwfgs.cn

R. Bash 专题
来源：http://nq.szxytkj.cn

================================================================================
来源：http://au.yuexingan06.cn

[R01] shebang 与严格模式
来源：http://zq.shxzukj.cn

#!/usr/bin/env bash
来源：http://ji.hahajie.cn

set -euo pipefail
来源：http://lt.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://hv.szxytkj.cn

name="Tom"; echo "$name"
来源：http://dg.huanxung.cn

[R03] 只读变量
来源：http://ux.jctech888.com.cn

readonly PI=3.14
来源：http://nl.bjjhwx.cn

[R04] 位置参数
来源：http://ir.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xk.lnxyls.cn

[R05] 参数默认值
来源：http://jx.gzmigu.cn

name="${1:-default}"
来源：http://oq.newstarts.cn

[R06] 判断命令是否存在
来源：http://eg.bjjhwx.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dr.huixinmuqiang.cn

[R07] if 判断文件
来源：http://zv.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yj.shxzskj.cn

[R08] 数值比较
来源：http://wo.panjiajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yw.jianghongdianzi.cn

[R09] 字符串比较
来源：http://qj.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://za.huanxung.cn

[R10] 正则匹配
来源：http://tm.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bd.shxzukj.cn

[R11] case 多分支
来源：http://xm.jianghongdianzi.cn

case "$1" in
来源：http://zp.yuexingan06.cn

start) echo "启动" ;;
来源：http://bu.asd995.cn

stop)  echo "停止" ;;
来源：http://jl.shtwfgs.cn

*)     echo "未知命令" ;;
来源：http://wb.9csxet.cn

esac
来源：http://dy.bookmarksfly.cn

[R12] for 遍历文件
来源：http://fi.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://gb.chemitech.net.cn

[R13] for 计数循环
来源：http://xe.haigaiapp.cn

for i in {1..10}; do echo "$i"; done
来源：http://db.bjjhwx.cn

[R14] C 风格 for
来源：http://ct.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uu.nszjky.cn

[R15] while 逐行读文件
来源：http://ng.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zm.huixinmuqiang.cn

[R16] until 等待条件
来源：http://rt.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ah.shxzukj.cn

[R17] 数组定义与取值
来源：http://cv.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hj.jctech888.com.cn

[R18] 遍历数组
来源：http://pf.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.huixinmuqiang.cn

[R19] 数组长度
来源：http://jc.9csxet.cn

echo "${#arr[@]}"
来源：http://xv.nszjky.cn

[R20] 关联数组（字典）
来源：http://iz.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dh.lnxyls.cn

[R21] 字符串长度
来源：http://zi.huanxung.cn

echo "${#s}"
来源：http://nh.9csxet.cn

[R22] 截取子串
来源：http://es.huixiangedu.cn

echo "${s:0:5}"
来源：http://ay.panjiajie.cn

[R23] 字符串替换
来源：http://kj.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gp.gzmigu.cn

[R24] 大小写转换
来源：http://ob.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nb.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://vu.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kh.newstarts.cn

[R26] 命令替换
来源：http://qk.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://pp.colortex.cn

[R27] 算术展开
来源：http://zl.huanxung.cn

echo $((1 + 2 * 3))
来源：http://ne.shtwfgs.cn

[R28] 浮点运算
来源：http://yk.nszjky.cn

echo "scale=2; 10/3" | bc
来源：http://gp.huanxung.cn

[R29] 定义函数
来源：http://iv.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vd.hahajie.cn

[R30] 函数返回状态码
来源：http://hp.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://qx.chemitech.net.cn

[R31] 局部变量
来源：http://yg.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://bv.panjiajie.cn

[R32] 参数个数校验
来源：http://hu.haigaiapp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tl.521024.cn

[R33] 捕获错误并提示行号
来源：http://ez.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xz.shtwfgs.cn

[R34] 退出时清理
来源：http://yz.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jm.wgjwhj.cn

[R35] 后台执行并等待
来源：http://ik.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ur.newstarts.cn

[R36] 并发执行多个任务
来源：http://oy.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yu.asd995.cn

[R37] 把输出赋给变量
来源：http://tm.hnjuh.cn

files=$(ls -1)
来源：http://jz.colortex.cn

[R38] 管道串联
来源：http://rs.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://ho.haigaiapp.cn

[R39] 重定向标准输出与错误
来源：http://ok.chemitech.net.cn

cmd > out.log 2>&1
来源：http://og.szsharing.cn

[R40] 追加写日志
来源：http://ti.panjiajie.cn

echo "log" >> out.log
来源：http://uz.jctech888.com.cn

[R41] 丢弃输出
来源：http://ju.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://rb.haigaiapp.cn

[R42] 输入重定向
来源：http://jo.colortex.cn

wc -l < a.txt
来源：http://dv.panjiajie.cn

[R43] 按名字查找文件
来源：http://vd.colortex.cn

find . -name "*.log" -type f
来源：http://lp.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://fs.shxzukj.cn

find . -mtime -7 -type f
来源：http://lu.newstarts.cn

[R45] 批量删除
来源：http://pb.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://gv.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://pj.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zy.asd995.cn

[R47] sed 单行替换
来源：http://qx.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fo.chemitech.net.cn

[R48] awk 取指定列
来源：http://az.hahajie.cn

awk '{print $1, $3}' a.txt
来源：http://zn.bjjhwx.cn

[R49] awk 带条件
来源：http://ow.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ea.huixiangedu.cn

[R50] awk 求和
来源：http://xs.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zv.panjiajie.cn

[R51] 排序去重取前几
来源：http://ki.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yc.muxihuayi.cn

[R52] 统计行数
来源：http://tf.nszjky.cn

wc -l a.txt
来源：http://fn.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://ol.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wa.newstarts.cn

[R54] 比较两个文件
来源：http://iv.lnxyls.cn

diff a.txt b.txt
来源：http://le.521024.cn

[R55] 压缩与解压
来源：http://ik.shxzukj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yv.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://em.huanxung.cn

scp file user@host:/path/
来源：http://xd.nszjky.cn

[R57] 远程执行命令
来源：http://xo.gzmigu.cn

ssh user@host 'uptime'
来源：http://cs.colortex.cn

[R58] 下载文件
来源：http://kx.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sn.521024.cn

[R59] 发 POST JSON
来源：http://gh.521024.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oj.nicolike.cn

[R60] 只看 HTTP 状态码
来源：http://su.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://of.panjiajie.cn

[R61] 磁盘占用
来源：http://kq.wgjwhj.cn

df -h;  du -sh *
来源：http://wa.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://hd.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://lo.szsharing.cn

[R63] 内存与进程
来源：http://qr.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://fr.newstarts.cn

[R64] 结束进程
来源：http://wn.lnxyls.cn

kill -9 $(pgrep -f app.py)
来源：http://mj.hnjuh.cn

[R65] 查看端口占用
来源：http://wk.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vu.muxihuayi.cn

[R66] 定时任务
来源：http://kz.szsharing.cn

crontab -e;  crontab -l
来源：http://yz.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://dp.colortex.cn

openssl rand -hex 16
来源：http://lg.szsharing.cn

[R68] 计算文件校验值
来源：http://gm.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jq.521024.cn

[R69] 生成随机密码
来源：http://mi.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://np.nicolike.cn

[R70] 时间戳与互转
来源：http://hp.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://sg.521024.cn

[R71] 日期格式化
来源：http://nr.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://no.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://pf.yuexingan06.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fv.bjjhwx.cn

[R73] 分割大日志
来源：http://kz.jctech888.com.cn

split -l 1000 big.log part_
来源：http://zm.jctech888.com.cn

[R74] 批量重命名
来源：http://pn.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wg.szxytkj.cn

[R75] 导出环境变量
来源：http://ty.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://ux.shxzukj.cn

[R76] 使用临时文件
来源：http://hu.shxzskj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uz.jctech888.com.cn

[R77] 读取用户输入
来源：http://zi.newstarts.cn

read -rp "请输入: " ans
来源：http://jj.chemitech.net.cn

[R78] 交互式菜单
来源：http://zu.9csxet.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sp.szsharing.cn

[R79] 解析命令行选项
来源：http://qt.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tq.521024.cn

[R80] 查看脚本执行耗时
来源：http://sk.muxihuayi.cn

time ./run.sh
来源：http://fi.chemitech.net.cn

================================================================================
来源：http://ti.panjiajie.cn

S. C / C++ 专题
来源：http://ie.9csxet.cn

================================================================================
来源：http://fo.bjjhwx.cn

[S01] C：Hello World
来源：http://qj.lnxyls.cn

#include <stdio.h>
来源：http://uj.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xn.521024.cn

[S02] C：变量与格式化输出
来源：http://bb.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://ve.huixiangedu.cn

[S03] C：读入整数
来源：http://mt.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://du.nicolike.cn

[S04] C：字符串复制
来源：http://ke.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qn.szsharing.cn

[S05] C：字符串长度
来源：http://ud.shtwfgs.cn

strlen(s)
来源：http://rl.szsharing.cn

[S06] C：字符串比较
来源：http://nt.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://mm.szsharing.cn

[S07] C：数组遍历求和
来源：http://ra.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yi.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://ur.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ke.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://ak.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kt.wgjwhj.cn

[S10] C：指针与解引用
来源：http://cn.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://ck.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://jq.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://oz.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://en.shtwfgs.cn

fclose(f);
来源：http://qm.szsharing.cn

[S12] C：写文件
来源：http://id.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yp.panjiajie.cn

[S13] C：宏定义
来源：http://ux.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sv.shxzukj.cn

[S14] C：枚举
来源：http://ug.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://se.yuexingan06.cn

[S15] C：类型转换
来源：http://nq.asd995.cn

(double) a / b
来源：http://cs.szxytkj.cn

[S16] C：位操作置位
来源：http://sy.yuexingan06.cn

x |= (1 << 3);
来源：http://vv.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://mg.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jz.nszjky.cn

[S18] C：命令行参数
来源：http://ag.jctech888.com.cn

int main(int argc, char **argv)
来源：http://fu.9csxet.cn

[S19] C：快速排序
来源：http://pp.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://su.gzmigu.cn

[S20] C：二分查找
来源：http://sd.9csxet.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vg.nszjky.cn

[S21] C：字符类别判断
来源：http://nd.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gv.szsharing.cn

[S22] C：字符串转数字
来源：http://ee.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rc.panjiajie.cn

[S23] C：随机数
来源：http://ag.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://az.lnxyls.cn

[S24] C：获取本地时间
来源：http://md.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vc.hnjuh.cn

[S25] C：内存拷贝
来源：http://qi.muxihuayi.cn

memcpy(dst, src, n);
来源：http://ps.haigaiapp.cn

[S26] C：内存清零
来源：http://ct.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://le.shtwfgs.cn

[S27] C：定义常量
来源：http://mm.shxzskj.cn

const double PI = 3.14159;
来源：http://rb.haigaiapp.cn

[S28] C：静态变量
来源：http://yl.wgjwhj.cn

static int counter = 0;
来源：http://pi.chemitech.net.cn

[S29] C：变参函数
来源：http://hi.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ru.jctech888.com.cn

[S30] C：头文件保护
来源：http://jt.9csxet.cn

#ifndef X_H
来源：http://vj.hnjuh.cn

#define X_H
来源：http://ls.szsharing.cn

#endif
来源：http://eg.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://rk.yuntaijiaju.cn

#include <iostream>
来源：http://gc.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://ng.jctech888.com.cn

[S32] C++：字符串
来源：http://sc.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://sn.haigaiapp.cn

[S33] C++：vector 增删
来源：http://wa.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://so.nicolike.cn

[S34] C++：遍历 vector
来源：http://gk.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://rw.bjjhwx.cn

[S35] C++：map
来源：http://sr.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eo.yuexingan06.cn

[S36] C++：unordered_map
来源：http://fz.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://em.nicolike.cn

[S37] C++：set
来源：http://um.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vl.jianghongdianzi.cn

[S38] C++：排序
来源：http://bq.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://nn.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://ib.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bb.bookmarksfly.cn

[S40] C++：查找元素
来源：http://bm.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zj.gzmigu.cn

[S41] C++：类与构造函数
来源：http://vn.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pv.yuntaijiaju.cn

[S42] C++：继承与虚函数
来源：http://gw.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://le.shxzskj.cn

[S43] C++：智能指针
来源：http://pi.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://mr.lnxyls.cn

[S44] C++：引用传参
来源：http://st.newstarts.cn

void inc(int &x) { ++x; }
来源：http://pn.muxihuayi.cn

[S45] C++：lambda
来源：http://vg.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dr.gzmigu.cn

[S46] C++：函数模板
来源：http://ms.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ib.yuexingan06.cn

[S47] C++：结构化绑定遍历
来源：http://ig.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hq.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://hh.haigaiapp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://to.szsharing.cn

while (std::getline(in, line)) { }
来源：http://dp.wgjwhj.cn

[S49] C++：写文件
来源：http://fj.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bq.jctech888.com.cn

[S50] C++：格式化数字
来源：http://gi.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gf.gzmigu.cn

[S51] C++：显式类型转换
来源：http://xj.colortex.cn

static_cast<double>(a) / b
来源：http://sg.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://rj.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://zs.shxzukj.cn

[S53] C++：移动语义
来源：http://gp.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://tq.szsharing.cn

[S54] C++：异常处理
来源：http://lf.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://td.szsharing.cn

[S55] C++：结构化绑定
来源：http://sc.bjjhwx.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nx.muxihuayi.cn

[S56] C++：optional
来源：http://fn.521024.cn


<!-- 参考信息 -->