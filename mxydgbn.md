代发 wailian999

[Q84] 去除首尾空格
来源：http://pl.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://xs.jianghongdianzi.cn

[Q85] 数值取整
来源：http://ma.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gt.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://rf.haigaiapp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ji.colortex.cn

[Q87] JSON 字段做条件
来源：http://sq.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gw.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://ow.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jo.lnxyls.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rz.szxytkj.cn

[Q89] 判断表是否存在
来源：http://pd.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yr.521024.cn

[Q90] 生成序号列
来源：http://wy.jctech888.com.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sn.colortex.cn

================================================================================
来源：http://no.hahajie.cn

R. Bash 专题
来源：http://kd.shtwfgs.cn

================================================================================
来源：http://bl.panjiajie.cn

[R01] shebang 与严格模式
来源：http://an.muxihuayi.cn

#!/usr/bin/env bash
来源：http://ce.yuexingan06.cn

set -euo pipefail
来源：http://pb.bjjhwx.cn

[R02] 变量赋值与使用
来源：http://kv.hnjuh.cn

name="Tom"; echo "$name"
来源：http://iw.521024.cn

[R03] 只读变量
来源：http://hw.hnjuh.cn

readonly PI=3.14
来源：http://fm.bookmarksfly.cn

[R04] 位置参数
来源：http://cy.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ov.muxihuayi.cn

[R05] 参数默认值
来源：http://jn.yuexingan06.cn

name="${1:-default}"
来源：http://tq.hnjuh.cn

[R06] 判断命令是否存在
来源：http://bl.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wc.wgjwhj.cn

[R07] if 判断文件
来源：http://co.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pw.colortex.cn

[R08] 数值比较
来源：http://sk.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qh.newstarts.cn

[R09] 字符串比较
来源：http://fx.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zm.nicolike.cn

[R10] 正则匹配
来源：http://ly.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yz.9csxet.cn

[R11] case 多分支
来源：http://nd.jctech888.com.cn

case "$1" in
来源：http://cu.shxzukj.cn

start) echo "启动" ;;
来源：http://br.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://nc.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://ob.panjiajie.cn

esac
来源：http://rs.bjjhwx.cn

[R12] for 遍历文件
来源：http://cp.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://jm.newstarts.cn

[R13] for 计数循环
来源：http://sn.yuntaijiaju.cn

for i in {1..10}; do echo "$i"; done
来源：http://wk.haigaiapp.cn

[R14] C 风格 for
来源：http://rf.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pn.bjjhwx.cn

[R15] while 逐行读文件
来源：http://vo.huanxung.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jx.huixiangedu.cn

[R16] until 等待条件
来源：http://op.bjjhwx.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jf.asd995.cn

[R17] 数组定义与取值
来源：http://ye.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ua.huixiangedu.cn

[R18] 遍历数组
来源：http://ko.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bf.szxytkj.cn

[R19] 数组长度
来源：http://ma.hahajie.cn

echo "${#arr[@]}"
来源：http://dh.shtwfgs.cn

[R20] 关联数组（字典）
来源：http://rl.hnjuh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wv.nszjky.cn

[R21] 字符串长度
来源：http://bd.jianghongdianzi.cn

echo "${#s}"
来源：http://go.yuntaijiaju.cn

[R22] 截取子串
来源：http://ki.nszjky.cn

echo "${s:0:5}"
来源：http://kg.szxytkj.cn

[R23] 字符串替换
来源：http://sb.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oo.wgjwhj.cn

[R24] 大小写转换
来源：http://lt.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vm.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://ib.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uw.521024.cn

[R26] 命令替换
来源：http://ti.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://gt.9csxet.cn

[R27] 算术展开
来源：http://ov.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://fj.521024.cn

[R28] 浮点运算
来源：http://fu.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://ye.wgjwhj.cn

[R29] 定义函数
来源：http://wt.jctech888.com.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uk.huixiangedu.cn

[R30] 函数返回状态码
来源：http://pm.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://dd.haigaiapp.cn

[R31] 局部变量
来源：http://ij.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://pp.shxzukj.cn

[R32] 参数个数校验
来源：http://ao.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fx.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://ju.gzmigu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ri.huixiangedu.cn

[R34] 退出时清理
来源：http://os.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ce.shtwfgs.cn

[R35] 后台执行并等待
来源：http://qk.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tb.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://sv.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yb.hahajie.cn

[R37] 把输出赋给变量
来源：http://lw.szxytkj.cn

files=$(ls -1)
来源：http://el.huixinmuqiang.cn

[R38] 管道串联
来源：http://za.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://ml.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://tb.newstarts.cn

cmd > out.log 2>&1
来源：http://qe.muxihuayi.cn

[R40] 追加写日志
来源：http://vj.521024.cn

echo "log" >> out.log
来源：http://yy.wgjwhj.cn

[R41] 丢弃输出
来源：http://tq.nszjky.cn

cmd >/dev/null 2>&1
来源：http://yz.colortex.cn

[R42] 输入重定向
来源：http://ky.wgjwhj.cn

wc -l < a.txt
来源：http://rh.haigaiapp.cn

[R43] 按名字查找文件
来源：http://is.colortex.cn

find . -name "*.log" -type f
来源：http://zg.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://id.yuexingan06.cn

find . -mtime -7 -type f
来源：http://rt.yuexingan06.cn

[R45] 批量删除
来源：http://tw.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://ub.newstarts.cn

[R46] 递归替换文件内容
来源：http://xx.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zw.shxzukj.cn

[R47] sed 单行替换
来源：http://gk.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://uy.bjjhwx.cn

[R48] awk 取指定列
来源：http://cm.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://wd.hnjuh.cn

[R49] awk 带条件
来源：http://xv.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xf.asd995.cn

[R50] awk 求和
来源：http://sa.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qp.gzmigu.cn

[R51] 排序去重取前几
来源：http://jr.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://eb.521024.cn

[R52] 统计行数
来源：http://hi.shxzukj.cn

wc -l a.txt
来源：http://vc.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://vw.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tj.nszjky.cn

[R54] 比较两个文件
来源：http://ug.szxytkj.cn

diff a.txt b.txt
来源：http://xl.huixiangedu.cn

[R55] 压缩与解压
来源：http://jz.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://af.nszjky.cn

[R56] 远程拷贝
来源：http://df.nszjky.cn

scp file user@host:/path/
来源：http://ma.szxytkj.cn

[R57] 远程执行命令
来源：http://fg.9csxet.cn

ssh user@host 'uptime'
来源：http://fq.yuntaijiaju.cn

[R58] 下载文件
来源：http://sy.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ns.yuntaijiaju.cn

[R59] 发 POST JSON
来源：http://lk.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fr.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://bt.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ge.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://iz.wgjwhj.cn

df -h;  du -sh *
来源：http://kg.panjiajie.cn

[R62] 找最占空间的文件
来源：http://te.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://lr.nicolike.cn

[R63] 内存与进程
来源：http://pi.9csxet.cn

free -h;  ps aux | grep nginx
来源：http://go.shxzukj.cn

[R64] 结束进程
来源：http://ff.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://mu.gzmigu.cn

[R65] 查看端口占用
来源：http://mt.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nv.shxzskj.cn

[R66] 定时任务
来源：http://ma.newstarts.cn

crontab -e;  crontab -l
来源：http://sk.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://wr.colortex.cn

openssl rand -hex 16
来源：http://ov.jctech888.com.cn

[R68] 计算文件校验值
来源：http://oh.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ai.yuexingan06.cn

[R69] 生成随机密码
来源：http://mv.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://cc.panjiajie.cn

[R70] 时间戳与互转
来源：http://pe.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://fv.huixinmuqiang.cn

[R71] 日期格式化
来源：http://kx.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ma.colortex.cn

[R72] 等待端口就绪
来源：http://wz.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nm.shxzukj.cn

[R73] 分割大日志
来源：http://pt.nszjky.cn

split -l 1000 big.log part_
来源：http://sv.bookmarksfly.cn

[R74] 批量重命名
来源：http://fl.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://va.jianghongdianzi.cn

[R75] 导出环境变量
来源：http://qw.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://kk.gzmigu.cn

[R76] 使用临时文件
来源：http://wa.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fh.huixiangedu.cn

[R77] 读取用户输入
来源：http://nb.shxzskj.cn

read -rp "请输入: " ans
来源：http://wo.hnjuh.cn

[R78] 交互式菜单
来源：http://fy.9csxet.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vc.muxihuayi.cn

[R79] 解析命令行选项
来源：http://pz.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sf.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://xk.haigaiapp.cn

time ./run.sh
来源：http://zh.shxzskj.cn

================================================================================
来源：http://vs.nicolike.cn

S. C / C++ 专题
来源：http://qm.gzmigu.cn

================================================================================
来源：http://jc.521024.cn

[S01] C：Hello World
来源：http://kf.wgjwhj.cn

#include <stdio.h>
来源：http://df.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vo.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://yh.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://gv.huixinmuqiang.cn

[S03] C：读入整数
来源：http://vg.colortex.cn

int x; scanf("%d", &x);
来源：http://rh.shxzskj.cn

[S04] C：字符串复制
来源：http://sz.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qd.jianghongdianzi.cn

[S05] C：字符串长度
来源：http://vc.nszjky.cn

strlen(s)
来源：http://pt.shtwfgs.cn

[S06] C：字符串比较
来源：http://gm.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://ku.asd995.cn

[S07] C：数组遍历求和
来源：http://oz.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ei.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://ew.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lg.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://eq.hnjuh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qh.bjjhwx.cn

[S10] C：指针与解引用
来源：http://jh.shxzukj.cn

int *p = &a;  *p = 5;
来源：http://he.nszjky.cn

[S11] C：逐行读文件
来源：http://be.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://cv.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gl.huanxung.cn

fclose(f);
来源：http://qs.lnxyls.cn

[S12] C：写文件
来源：http://ei.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rb.yuntaijiaju.cn

[S13] C：宏定义
来源：http://vv.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ya.nszjky.cn

[S14] C：枚举
来源：http://ta.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://lx.521024.cn

[S15] C：类型转换
来源：http://qw.huanxung.cn

(double) a / b
来源：http://kb.haigaiapp.cn

[S16] C：位操作置位
来源：http://uu.chemitech.net.cn

x |= (1 << 3);
来源：http://ih.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://pr.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ng.haigaiapp.cn

[S18] C：命令行参数
来源：http://em.haigaiapp.cn

int main(int argc, char **argv)
来源：http://bo.nszjky.cn

[S19] C：快速排序
来源：http://uf.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://by.colortex.cn

[S20] C：二分查找
来源：http://ap.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fm.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://sj.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yl.nicolike.cn

[S22] C：字符串转数字
来源：http://uh.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ac.wgjwhj.cn

[S23] C：随机数
来源：http://xt.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wj.panjiajie.cn

[S24] C：获取本地时间
来源：http://lb.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nj.hahajie.cn

[S25] C：内存拷贝
来源：http://vb.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://hr.shxzukj.cn

[S26] C：内存清零
来源：http://pu.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://iv.9csxet.cn

[S27] C：定义常量
来源：http://ki.huanxung.cn

const double PI = 3.14159;
来源：http://bx.asd995.cn

[S28] C：静态变量
来源：http://yx.jctech888.com.cn

static int counter = 0;
来源：http://wz.9csxet.cn

[S29] C：变参函数
来源：http://tz.huanxung.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://so.lnxyls.cn

[S30] C：头文件保护
来源：http://ef.yuntaijiaju.cn

#ifndef X_H
来源：http://tb.shxzukj.cn

#define X_H
来源：http://vg.haigaiapp.cn

#endif
来源：http://pb.hnjuh.cn

[S31] C++：Hello World
来源：http://sg.shtwfgs.cn

#include <iostream>
来源：http://ju.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://ln.asd995.cn

[S32] C++：字符串
来源：http://eg.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://yp.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://ll.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cw.nszjky.cn

[S34] C++：遍历 vector
来源：http://hp.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://qh.9csxet.cn

[S35] C++：map
来源：http://rt.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cp.muxihuayi.cn

[S36] C++：unordered_map
来源：http://yp.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sb.chemitech.net.cn

[S37] C++：set
来源：http://su.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vw.huixiangedu.cn

[S38] C++：排序
来源：http://nv.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://zl.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://nt.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bt.bookmarksfly.cn

[S40] C++：查找元素
来源：http://rh.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fb.lnxyls.cn

[S41] C++：类与构造函数
来源：http://uy.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://os.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://ak.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://cn.hahajie.cn

[S43] C++：智能指针
来源：http://dk.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://ef.yuexingan06.cn

[S44] C++：引用传参
来源：http://di.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://xo.asd995.cn

[S45] C++：lambda
来源：http://os.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ts.jctech888.com.cn

[S46] C++：函数模板
来源：http://qw.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xi.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://gc.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://td.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://df.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ow.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://zr.bjjhwx.cn

[S49] C++：写文件
来源：http://uz.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hq.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://fa.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hy.huanxung.cn

[S51] C++：显式类型转换
来源：http://pu.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://dx.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://pp.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://bg.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://zn.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://ko.panjiajie.cn

[S54] C++：异常处理
来源：http://xu.gzmigu.cn


<!-- 参考信息 -->