代发 wailian999

[Q86] 读取 JSON 字段
来源：http://ke.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://el.huanxung.cn

[Q87] JSON 字段做条件
来源：http://cf.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fe.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://dq.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ro.hnjuh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jm.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://ij.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fq.nszjky.cn

[Q90] 生成序号列
来源：http://tr.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fe.asd995.cn

================================================================================
来源：http://ox.newstarts.cn

R. Bash 专题
来源：http://bo.jianghongdianzi.cn

================================================================================
来源：http://vp.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://ux.huixinmuqiang.cn

#!/usr/bin/env bash
来源：http://yq.nszjky.cn

set -euo pipefail
来源：http://ym.asd995.cn

[R02] 变量赋值与使用
来源：http://kq.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://jc.haigaiapp.cn

[R03] 只读变量
来源：http://ag.muxihuayi.cn

readonly PI=3.14
来源：http://lo.gzmigu.cn

[R04] 位置参数
来源：http://fz.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kn.yuntaijiaju.cn

[R05] 参数默认值
来源：http://by.colortex.cn

name="${1:-default}"
来源：http://gx.szxytkj.cn

[R06] 判断命令是否存在
来源：http://df.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cr.muxihuayi.cn

[R07] if 判断文件
来源：http://oz.jianghongdianzi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ug.muxihuayi.cn

[R08] 数值比较
来源：http://tt.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lm.szsharing.cn

[R09] 字符串比较
来源：http://fk.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ge.szxytkj.cn

[R10] 正则匹配
来源：http://tq.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pe.gzmigu.cn

[R11] case 多分支
来源：http://xr.colortex.cn

case "$1" in
来源：http://uo.huixinmuqiang.cn

start) echo "启动" ;;
来源：http://fe.shxzskj.cn

stop)  echo "停止" ;;
来源：http://dc.gzmigu.cn

*)     echo "未知命令" ;;
来源：http://wt.colortex.cn

esac
来源：http://we.yuexingan06.cn

[R12] for 遍历文件
来源：http://sq.shtwfgs.cn

for f in *.txt; do echo "$f"; done
来源：http://jz.asd995.cn

[R13] for 计数循环
来源：http://zx.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://uj.panjiajie.cn

[R14] C 风格 for
来源：http://wh.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jn.shtwfgs.cn

[R15] while 逐行读文件
来源：http://ll.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qd.9csxet.cn

[R16] until 等待条件
来源：http://hl.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xb.yuntaijiaju.cn

[R17] 数组定义与取值
来源：http://fw.hahajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gi.bjjhwx.cn

[R18] 遍历数组
来源：http://rl.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aj.yuexingan06.cn

[R19] 数组长度
来源：http://ae.asd995.cn

echo "${#arr[@]}"
来源：http://vh.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://mw.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qf.shxzskj.cn

[R21] 字符串长度
来源：http://kv.nicolike.cn

echo "${#s}"
来源：http://yx.panjiajie.cn

[R22] 截取子串
来源：http://il.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://xd.szsharing.cn

[R23] 字符串替换
来源：http://qb.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eb.colortex.cn

[R24] 大小写转换
来源：http://aj.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xe.9csxet.cn

[R25] 去后缀 / 去前缀
来源：http://co.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fq.gzmigu.cn

[R26] 命令替换
来源：http://hp.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://kp.bjjhwx.cn

[R27] 算术展开
来源：http://cd.9csxet.cn

echo $((1 + 2 * 3))
来源：http://ak.colortex.cn

[R28] 浮点运算
来源：http://vm.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://vu.lnxyls.cn

[R29] 定义函数
来源：http://ks.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jj.hahajie.cn

[R30] 函数返回状态码
来源：http://zx.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://oz.wgjwhj.cn

[R31] 局部变量
来源：http://kq.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://vc.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://uy.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vl.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://ta.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hq.jianghongdianzi.cn

[R34] 退出时清理
来源：http://qy.yuexingan06.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vt.huanxung.cn

[R35] 后台执行并等待
来源：http://bl.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ao.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://zl.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ls.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://jk.wgjwhj.cn

files=$(ls -1)
来源：http://tj.hnjuh.cn

[R38] 管道串联
来源：http://jp.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://xd.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://qp.hnjuh.cn

cmd > out.log 2>&1
来源：http://ou.gzmigu.cn

[R40] 追加写日志
来源：http://xd.hahajie.cn

echo "log" >> out.log
来源：http://eh.shxzukj.cn

[R41] 丢弃输出
来源：http://ip.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://tf.huanxung.cn

[R42] 输入重定向
来源：http://rp.panjiajie.cn

wc -l < a.txt
来源：http://pj.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://gu.asd995.cn

find . -name "*.log" -type f
来源：http://yy.asd995.cn

[R44] 按修改时间查找
来源：http://py.gzmigu.cn

find . -mtime -7 -type f
来源：http://on.huixiangedu.cn

[R45] 批量删除
来源：http://hn.hahajie.cn

find . -name "*.tmp" -delete
来源：http://ya.hahajie.cn

[R46] 递归替换文件内容
来源：http://ra.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://me.jctech888.com.cn

[R47] sed 单行替换
来源：http://cg.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zw.panjiajie.cn

[R48] awk 取指定列
来源：http://lt.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://bq.huanxung.cn

[R49] awk 带条件
来源：http://qv.jianghongdianzi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://me.yuexingan06.cn

[R50] awk 求和
来源：http://ge.bjjhwx.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qv.panjiajie.cn

[R51] 排序去重取前几
来源：http://wg.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kc.shxzukj.cn

[R52] 统计行数
来源：http://pn.haigaiapp.cn

wc -l a.txt
来源：http://xm.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://du.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vy.huanxung.cn

[R54] 比较两个文件
来源：http://hn.szsharing.cn

diff a.txt b.txt
来源：http://kh.huixiangedu.cn

[R55] 压缩与解压
来源：http://bh.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lm.jctech888.com.cn

[R56] 远程拷贝
来源：http://rn.asd995.cn

scp file user@host:/path/
来源：http://ve.gzmigu.cn

[R57] 远程执行命令
来源：http://oc.shtwfgs.cn

ssh user@host 'uptime'
来源：http://lw.panjiajie.cn

[R58] 下载文件
来源：http://ya.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jz.lnxyls.cn

[R59] 发 POST JSON
来源：http://zu.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jb.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://ca.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rd.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://ux.muxihuayi.cn

df -h;  du -sh *
来源：http://ic.hnjuh.cn

[R62] 找最占空间的文件
来源：http://ak.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://xq.yuntaijiaju.cn

[R63] 内存与进程
来源：http://rz.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://py.nszjky.cn

[R64] 结束进程
来源：http://bl.lnxyls.cn

kill -9 $(pgrep -f app.py)
来源：http://id.bjjhwx.cn

[R65] 查看端口占用
来源：http://na.szxytkj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mk.yuntaijiaju.cn

[R66] 定时任务
来源：http://mr.muxihuayi.cn

crontab -e;  crontab -l
来源：http://nj.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://zh.huixinmuqiang.cn

openssl rand -hex 16
来源：http://sj.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://he.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://je.gzmigu.cn

[R69] 生成随机密码
来源：http://kc.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://ga.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://dk.panjiajie.cn

date +%s;  date -d @1700000000
来源：http://aa.szsharing.cn

[R71] 日期格式化
来源：http://va.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dc.chemitech.net.cn

[R72] 等待端口就绪
来源：http://ew.newstarts.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://aq.wgjwhj.cn

[R73] 分割大日志
来源：http://xd.asd995.cn

split -l 1000 big.log part_
来源：http://ku.hahajie.cn

[R74] 批量重命名
来源：http://hj.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uf.newstarts.cn

[R75] 导出环境变量
来源：http://zd.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://yq.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://rh.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qo.lnxyls.cn

[R77] 读取用户输入
来源：http://dw.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://tj.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://op.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ms.bjjhwx.cn

[R79] 解析命令行选项
来源：http://mk.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://um.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://et.9csxet.cn

time ./run.sh
来源：http://rs.huixiangedu.cn

================================================================================
来源：http://ai.asd995.cn

S. C / C++ 专题
来源：http://rf.521024.cn

================================================================================
来源：http://av.jctech888.com.cn

[S01] C：Hello World
来源：http://pm.gzmigu.cn

#include <stdio.h>
来源：http://du.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rl.521024.cn

[S02] C：变量与格式化输出
来源：http://rp.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://pb.colortex.cn

[S03] C：读入整数
来源：http://cy.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://uq.szsharing.cn

[S04] C：字符串复制
来源：http://en.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kd.panjiajie.cn

[S05] C：字符串长度
来源：http://jt.nszjky.cn

strlen(s)
来源：http://ka.haigaiapp.cn

[S06] C：字符串比较
来源：http://lc.panjiajie.cn

strcmp(a, b) == 0
来源：http://xl.newstarts.cn

[S07] C：数组遍历求和
来源：http://uy.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rm.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://li.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vl.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://rf.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kt.huixiangedu.cn

[S10] C：指针与解引用
来源：http://lm.newstarts.cn

int *p = &a;  *p = 5;
来源：http://fu.bjjhwx.cn

[S11] C：逐行读文件
来源：http://ly.muxihuayi.cn

FILE *f = fopen("a.txt", "r");
来源：http://wa.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ep.jctech888.com.cn

fclose(f);
来源：http://at.haigaiapp.cn

[S12] C：写文件
来源：http://ff.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://of.bookmarksfly.cn

[S13] C：宏定义
来源：http://fe.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zz.gzmigu.cn

[S14] C：枚举
来源：http://ub.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://dm.szsharing.cn

[S15] C：类型转换
来源：http://du.huixinmuqiang.cn

(double) a / b
来源：http://cu.muxihuayi.cn

[S16] C：位操作置位
来源：http://yc.bjjhwx.cn

x |= (1 << 3);
来源：http://go.colortex.cn

[S17] C：安全拼接字符串
来源：http://bq.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rz.haigaiapp.cn

[S18] C：命令行参数
来源：http://xz.haigaiapp.cn

int main(int argc, char **argv)
来源：http://os.szxytkj.cn

[S19] C：快速排序
来源：http://ec.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://em.yuntaijiaju.cn

[S20] C：二分查找
来源：http://my.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ti.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://nu.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ad.521024.cn

[S22] C：字符串转数字
来源：http://ep.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ro.gzmigu.cn

[S23] C：随机数
来源：http://gv.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mn.hnjuh.cn

[S24] C：获取本地时间
来源：http://ox.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ap.huixiangedu.cn

[S25] C：内存拷贝
来源：http://nb.colortex.cn

memcpy(dst, src, n);
来源：http://jh.hahajie.cn

[S26] C：内存清零
来源：http://mc.colortex.cn

memset(a, 0, sizeof a);
来源：http://ze.jianghongdianzi.cn

[S27] C：定义常量
来源：http://tt.wgjwhj.cn

const double PI = 3.14159;
来源：http://ro.newstarts.cn

[S28] C：静态变量
来源：http://wh.yuntaijiaju.cn

static int counter = 0;
来源：http://cm.nszjky.cn

[S29] C：变参函数
来源：http://my.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wd.hahajie.cn

[S30] C：头文件保护
来源：http://gi.wgjwhj.cn

#ifndef X_H
来源：http://rw.wgjwhj.cn

#define X_H
来源：http://dy.jctech888.com.cn

#endif
来源：http://pq.bjjhwx.cn

[S31] C++：Hello World
来源：http://gk.haigaiapp.cn

#include <iostream>
来源：http://af.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://oi.wgjwhj.cn

[S32] C++：字符串
来源：http://iy.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://sl.shtwfgs.cn

[S33] C++：vector 增删
来源：http://yo.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nb.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://ho.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://ow.panjiajie.cn

[S35] C++：map
来源：http://ab.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bq.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://ed.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eh.yuexingan06.cn

[S37] C++：set
来源：http://yq.jctech888.com.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xe.nicolike.cn

[S38] C++：排序
来源：http://lg.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://gd.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://md.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wt.521024.cn

[S40] C++：查找元素
来源：http://fq.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zy.shxzskj.cn

[S41] C++：类与构造函数
来源：http://fh.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nn.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://xk.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://bf.shxzskj.cn

[S43] C++：智能指针
来源：http://mx.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://jv.shxzukj.cn

[S44] C++：引用传参
来源：http://mh.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://mw.nszjky.cn

[S45] C++：lambda
来源：http://ee.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wj.gzmigu.cn

[S46] C++：函数模板
来源：http://ao.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://go.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://eh.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jg.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://zf.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nn.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://sa.gzmigu.cn

[S49] C++：写文件
来源：http://st.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dr.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://nu.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ld.9csxet.cn

[S51] C++：显式类型转换
来源：http://an.9csxet.cn

static_cast<double>(a) / b
来源：http://vl.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://li.nszjky.cn

int size() const noexcept { return n_; }
来源：http://ct.bookmarksfly.cn

[S53] C++：移动语义
来源：http://qu.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://zq.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://eu.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gx.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://ld.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kr.jianghongdianzi.cn

[S56] C++：optional
来源：http://qw.hnjuh.cn


<!-- 参考信息 -->