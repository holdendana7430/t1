代发 wailian999

[Q86] 读取 JSON 字段
来源：http://or.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xg.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://wk.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://li.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://xz.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xj.nszjky.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cp.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://kr.yuntaijiaju.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yg.521024.cn

[Q90] 生成序号列
来源：http://cp.muxihuayi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://me.huanxung.cn

================================================================================
来源：http://cj.jianghongdianzi.cn

R. Bash 专题
来源：http://gx.9csxet.cn

================================================================================
来源：http://vu.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://jb.shxzukj.cn

#!/usr/bin/env bash
来源：http://kb.gzmigu.cn

set -euo pipefail
来源：http://ux.jianghongdianzi.cn

[R02] 变量赋值与使用
来源：http://ai.newstarts.cn

name="Tom"; echo "$name"
来源：http://dv.nszjky.cn

[R03] 只读变量
来源：http://qv.newstarts.cn

readonly PI=3.14
来源：http://qo.huanxung.cn

[R04] 位置参数
来源：http://tm.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bo.nszjky.cn

[R05] 参数默认值
来源：http://lh.shtwfgs.cn

name="${1:-default}"
来源：http://qz.haigaiapp.cn

[R06] 判断命令是否存在
来源：http://ai.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sw.lnxyls.cn

[R07] if 判断文件
来源：http://fx.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ra.9csxet.cn

[R08] 数值比较
来源：http://yj.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nw.huixiangedu.cn

[R09] 字符串比较
来源：http://dw.huanxung.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://na.haigaiapp.cn

[R10] 正则匹配
来源：http://id.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oy.wgjwhj.cn

[R11] case 多分支
来源：http://yg.panjiajie.cn

case "$1" in
来源：http://iy.9csxet.cn

start) echo "启动" ;;
来源：http://ka.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://vq.9csxet.cn

*)     echo "未知命令" ;;
来源：http://hh.bookmarksfly.cn

esac
来源：http://bj.newstarts.cn

[R12] for 遍历文件
来源：http://kt.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://lb.shxzukj.cn

[R13] for 计数循环
来源：http://yy.asd995.cn

for i in {1..10}; do echo "$i"; done
来源：http://ne.szxytkj.cn

[R14] C 风格 for
来源：http://yu.lnxyls.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://td.chemitech.net.cn

[R15] while 逐行读文件
来源：http://wc.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kc.jianghongdianzi.cn

[R16] until 等待条件
来源：http://xr.nszjky.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://od.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://yr.bjjhwx.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fd.yuexingan06.cn

[R18] 遍历数组
来源：http://mo.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mb.bjjhwx.cn

[R19] 数组长度
来源：http://gt.muxihuayi.cn

echo "${#arr[@]}"
来源：http://vf.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://xa.9csxet.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pw.lnxyls.cn

[R21] 字符串长度
来源：http://ow.huixiangedu.cn

echo "${#s}"
来源：http://pb.szxytkj.cn

[R22] 截取子串
来源：http://mq.shxzukj.cn

echo "${s:0:5}"
来源：http://js.shtwfgs.cn

[R23] 字符串替换
来源：http://kt.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zw.asd995.cn

[R24] 大小写转换
来源：http://yk.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tv.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://mb.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bv.9csxet.cn

[R26] 命令替换
来源：http://dm.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://ax.chemitech.net.cn

[R27] 算术展开
来源：http://tf.hahajie.cn

echo $((1 + 2 * 3))
来源：http://hn.shxzskj.cn

[R28] 浮点运算
来源：http://ou.huixiangedu.cn

echo "scale=2; 10/3" | bc
来源：http://sl.shtwfgs.cn

[R29] 定义函数
来源：http://yw.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://on.huanxung.cn

[R30] 函数返回状态码
来源：http://wp.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://mo.lnxyls.cn

[R31] 局部变量
来源：http://dx.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://cv.huixiangedu.cn

[R32] 参数个数校验
来源：http://na.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oi.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://ck.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://in.yuexingan06.cn

[R34] 退出时清理
来源：http://sj.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ri.huixiangedu.cn

[R35] 后台执行并等待
来源：http://an.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ga.huixinmuqiang.cn

[R36] 并发执行多个任务
来源：http://sa.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ms.shxzskj.cn

[R37] 把输出赋给变量
来源：http://yf.huixiangedu.cn

files=$(ls -1)
来源：http://uq.jianghongdianzi.cn

[R38] 管道串联
来源：http://hm.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://xh.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://ap.chemitech.net.cn

cmd > out.log 2>&1
来源：http://kl.asd995.cn

[R40] 追加写日志
来源：http://ql.gzmigu.cn

echo "log" >> out.log
来源：http://ka.shxzskj.cn

[R41] 丢弃输出
来源：http://zi.nicolike.cn

cmd >/dev/null 2>&1
来源：http://fj.hahajie.cn

[R42] 输入重定向
来源：http://vx.hahajie.cn

wc -l < a.txt
来源：http://or.jctech888.com.cn

[R43] 按名字查找文件
来源：http://lg.newstarts.cn

find . -name "*.log" -type f
来源：http://wg.nicolike.cn

[R44] 按修改时间查找
来源：http://yw.shxzukj.cn

find . -mtime -7 -type f
来源：http://fw.huanxung.cn

[R45] 批量删除
来源：http://cx.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://sp.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://gj.hnjuh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ld.9csxet.cn

[R47] sed 单行替换
来源：http://fy.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bi.gzmigu.cn

[R48] awk 取指定列
来源：http://wj.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://ku.huixiangedu.cn

[R49] awk 带条件
来源：http://dp.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wo.colortex.cn

[R50] awk 求和
来源：http://rw.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lq.nszjky.cn

[R51] 排序去重取前几
来源：http://yk.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nf.gzmigu.cn

[R52] 统计行数
来源：http://wg.jianghongdianzi.cn

wc -l a.txt
来源：http://gr.shxzskj.cn

[R53] 查看文件头与实时尾
来源：http://xm.lnxyls.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gx.panjiajie.cn

[R54] 比较两个文件
来源：http://hu.nszjky.cn

diff a.txt b.txt
来源：http://di.wgjwhj.cn

[R55] 压缩与解压
来源：http://ou.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ze.asd995.cn

[R56] 远程拷贝
来源：http://gu.shxzukj.cn

scp file user@host:/path/
来源：http://xf.newstarts.cn

[R57] 远程执行命令
来源：http://um.muxihuayi.cn

ssh user@host 'uptime'
来源：http://yr.huixiangedu.cn

[R58] 下载文件
来源：http://vj.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xl.colortex.cn

[R59] 发 POST JSON
来源：http://ju.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vb.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://lw.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ha.521024.cn

[R61] 磁盘占用
来源：http://ob.huanxung.cn

df -h;  du -sh *
来源：http://jc.shxzukj.cn

[R62] 找最占空间的文件
来源：http://ah.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://lq.bjjhwx.cn

[R63] 内存与进程
来源：http://op.wgjwhj.cn

free -h;  ps aux | grep nginx
来源：http://so.shtwfgs.cn

[R64] 结束进程
来源：http://mo.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://vx.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://ca.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ww.lnxyls.cn

[R66] 定时任务
来源：http://ki.bookmarksfly.cn

crontab -e;  crontab -l
来源：http://lu.szsharing.cn

[R67] 生成随机十六进制串
来源：http://le.jctech888.com.cn

openssl rand -hex 16
来源：http://bk.haigaiapp.cn

[R68] 计算文件校验值
来源：http://dj.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vc.bjjhwx.cn

[R69] 生成随机密码
来源：http://mf.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://sa.nicolike.cn

[R70] 时间戳与互转
来源：http://ss.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://vz.panjiajie.cn

[R71] 日期格式化
来源：http://en.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qo.gzmigu.cn

[R72] 等待端口就绪
来源：http://nm.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dv.asd995.cn

[R73] 分割大日志
来源：http://xd.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://je.nszjky.cn

[R74] 批量重命名
来源：http://gp.haigaiapp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ua.gzmigu.cn

[R75] 导出环境变量
来源：http://dx.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://ko.huixiangedu.cn

[R76] 使用临时文件
来源：http://zp.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zf.hahajie.cn

[R77] 读取用户输入
来源：http://ew.szxytkj.cn

read -rp "请输入: " ans
来源：http://ah.chemitech.net.cn

[R78] 交互式菜单
来源：http://vi.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bd.szxytkj.cn

[R79] 解析命令行选项
来源：http://wz.wgjwhj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jr.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://sv.chemitech.net.cn

time ./run.sh
来源：http://qr.nicolike.cn

================================================================================
来源：http://jp.shxzskj.cn

S. C / C++ 专题
来源：http://ul.newstarts.cn

================================================================================
来源：http://li.hnjuh.cn

[S01] C：Hello World
来源：http://by.nicolike.cn

#include <stdio.h>
来源：http://au.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sm.nszjky.cn

[S02] C：变量与格式化输出
来源：http://my.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://cw.huixiangedu.cn

[S03] C：读入整数
来源：http://aw.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://ua.hnjuh.cn

[S04] C：字符串复制
来源：http://nl.nicolike.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ou.jctech888.com.cn

[S05] C：字符串长度
来源：http://ks.huanxung.cn

strlen(s)
来源：http://pz.yuexingan06.cn

[S06] C：字符串比较
来源：http://sl.haigaiapp.cn

strcmp(a, b) == 0
来源：http://hl.lnxyls.cn

[S07] C：数组遍历求和
来源：http://wa.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cu.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://jp.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gk.colortex.cn

[S09] C：结构体定义与初始化
来源：http://es.bookmarksfly.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jj.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://fr.huixinmuqiang.cn

int *p = &a;  *p = 5;
来源：http://ro.panjiajie.cn

[S11] C：逐行读文件
来源：http://xq.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://kf.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ba.bjjhwx.cn

fclose(f);
来源：http://ol.muxihuayi.cn

[S12] C：写文件
来源：http://oh.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xl.newstarts.cn

[S13] C：宏定义
来源：http://jw.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dg.asd995.cn

[S14] C：枚举
来源：http://qt.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://jd.hnjuh.cn

[S15] C：类型转换
来源：http://ui.nicolike.cn

(double) a / b
来源：http://kr.huanxung.cn

[S16] C：位操作置位
来源：http://sj.colortex.cn

x |= (1 << 3);
来源：http://hg.nszjky.cn

[S17] C：安全拼接字符串
来源：http://bg.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xh.jctech888.com.cn

[S18] C：命令行参数
来源：http://sd.bookmarksfly.cn

int main(int argc, char **argv)
来源：http://ql.wgjwhj.cn

[S19] C：快速排序
来源：http://to.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hb.shxzukj.cn

[S20] C：二分查找
来源：http://vl.9csxet.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://be.521024.cn

[S21] C：字符类别判断
来源：http://ok.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://py.muxihuayi.cn

[S22] C：字符串转数字
来源：http://sl.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sf.bjjhwx.cn

[S23] C：随机数
来源：http://fa.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mc.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://iz.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bv.yuexingan06.cn

[S25] C：内存拷贝
来源：http://id.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://uq.bjjhwx.cn

[S26] C：内存清零
来源：http://ln.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://im.shxzskj.cn

[S27] C：定义常量
来源：http://rn.colortex.cn

const double PI = 3.14159;
来源：http://bn.chemitech.net.cn

[S28] C：静态变量
来源：http://kw.nszjky.cn

static int counter = 0;
来源：http://wa.asd995.cn

[S29] C：变参函数
来源：http://dq.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rn.wgjwhj.cn

[S30] C：头文件保护
来源：http://rw.szxytkj.cn

#ifndef X_H
来源：http://id.szxytkj.cn

#define X_H
来源：http://bg.bjjhwx.cn

#endif
来源：http://hu.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://ac.wgjwhj.cn

#include <iostream>
来源：http://wi.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://wc.bookmarksfly.cn

[S32] C++：字符串
来源：http://ww.asd995.cn

std::string s = "hi";  s += "!";
来源：http://ki.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://vq.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fy.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://ux.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://im.jianghongdianzi.cn

[S35] C++：map
来源：http://ho.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://is.wgjwhj.cn

[S36] C++：unordered_map
来源：http://kx.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pf.gzmigu.cn

[S37] C++：set
来源：http://mz.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eg.bjjhwx.cn

[S38] C++：排序
来源：http://mb.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://ox.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://ml.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hh.wgjwhj.cn

[S40] C++：查找元素
来源：http://qf.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pw.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://ln.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://is.huanxung.cn

[S42] C++：继承与虚函数
来源：http://nx.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://hy.jctech888.com.cn

[S43] C++：智能指针
来源：http://zc.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://ez.shxzskj.cn

[S44] C++：引用传参
来源：http://vp.9csxet.cn

void inc(int &x) { ++x; }
来源：http://kv.bookmarksfly.cn

[S45] C++：lambda
来源：http://pq.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fn.yuexingan06.cn

[S46] C++：函数模板
来源：http://li.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xe.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://pb.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fs.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://rw.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://la.szsharing.cn

while (std::getline(in, line)) { }
来源：http://xs.hahajie.cn

[S49] C++：写文件
来源：http://ai.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xb.wgjwhj.cn

[S50] C++：格式化数字
来源：http://hy.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tn.panjiajie.cn

[S51] C++：显式类型转换
来源：http://fp.huanxung.cn

static_cast<double>(a) / b
来源：http://yf.newstarts.cn

[S52] C++：const 与 noexcept
来源：http://na.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://zp.yuexingan06.cn

[S53] C++：移动语义
来源：http://bg.521024.cn

std::vector<int> w = std::move(v);
来源：http://yi.bookmarksfly.cn

[S54] C++：异常处理
来源：http://wn.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hl.nicolike.cn

[S55] C++：结构化绑定
来源：http://rp.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://at.muxihuayi.cn

[S56] C++：optional
来源：http://jx.huixinmuqiang.cn


<!-- 参考信息 -->