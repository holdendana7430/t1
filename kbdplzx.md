代发 wailian999

[Q86] 读取 JSON 字段
来源：http://fp.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sh.hahajie.cn

[Q87] JSON 字段做条件
来源：http://ym.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eo.huanxung.cn

[Q88] 行转列（条件聚合）
来源：http://dy.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ir.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ag.shxzukj.cn

[Q89] 判断表是否存在
来源：http://yq.gzmigu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ko.jctech888.com.cn

[Q90] 生成序号列
来源：http://po.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ei.yuexingan06.cn

================================================================================
来源：http://nk.yuntaijiaju.cn

R. Bash 专题
来源：http://nd.haigaiapp.cn

================================================================================
来源：http://yr.9csxet.cn

[R01] shebang 与严格模式
来源：http://pk.szxytkj.cn

#!/usr/bin/env bash
来源：http://oo.hnjuh.cn

set -euo pipefail
来源：http://kg.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://ro.newstarts.cn

name="Tom"; echo "$name"
来源：http://qt.lnxyls.cn

[R03] 只读变量
来源：http://xz.shtwfgs.cn

readonly PI=3.14
来源：http://ck.shxzskj.cn

[R04] 位置参数
来源：http://yo.panjiajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rk.gzmigu.cn

[R05] 参数默认值
来源：http://sr.521024.cn

name="${1:-default}"
来源：http://yx.hahajie.cn

[R06] 判断命令是否存在
来源：http://ks.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jd.hahajie.cn

[R07] if 判断文件
来源：http://cd.jctech888.com.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ua.yuntaijiaju.cn

[R08] 数值比较
来源：http://ys.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fh.521024.cn

[R09] 字符串比较
来源：http://rn.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://og.bjjhwx.cn

[R10] 正则匹配
来源：http://yu.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ph.asd995.cn

[R11] case 多分支
来源：http://au.szsharing.cn

case "$1" in
来源：http://pe.shxzukj.cn

start) echo "启动" ;;
来源：http://hm.shtwfgs.cn

stop)  echo "停止" ;;
来源：http://af.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://dq.nszjky.cn

esac
来源：http://ak.nszjky.cn

[R12] for 遍历文件
来源：http://ju.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://ro.bjjhwx.cn

[R13] for 计数循环
来源：http://yc.huanxung.cn

for i in {1..10}; do echo "$i"; done
来源：http://mk.yuexingan06.cn

[R14] C 风格 for
来源：http://cf.haigaiapp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qn.haigaiapp.cn

[R15] while 逐行读文件
来源：http://mg.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bz.huanxung.cn

[R16] until 等待条件
来源：http://ho.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://af.newstarts.cn

[R17] 数组定义与取值
来源：http://xg.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ej.lnxyls.cn

[R18] 遍历数组
来源：http://vl.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yk.jctech888.com.cn

[R19] 数组长度
来源：http://nl.hnjuh.cn

echo "${#arr[@]}"
来源：http://te.nszjky.cn

[R20] 关联数组（字典）
来源：http://qx.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qc.colortex.cn

[R21] 字符串长度
来源：http://vg.haigaiapp.cn

echo "${#s}"
来源：http://ni.521024.cn

[R22] 截取子串
来源：http://gx.haigaiapp.cn

echo "${s:0:5}"
来源：http://hc.lnxyls.cn

[R23] 字符串替换
来源：http://qw.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hh.jianghongdianzi.cn

[R24] 大小写转换
来源：http://rl.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ap.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://yf.huixiangedu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ws.jctech888.com.cn

[R26] 命令替换
来源：http://pc.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://ef.jianghongdianzi.cn

[R27] 算术展开
来源：http://oy.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://zc.shtwfgs.cn

[R28] 浮点运算
来源：http://kd.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://sp.huixinmuqiang.cn

[R29] 定义函数
来源：http://om.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://er.gzmigu.cn

[R30] 函数返回状态码
来源：http://kf.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://hp.asd995.cn

[R31] 局部变量
来源：http://wf.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://my.9csxet.cn

[R32] 参数个数校验
来源：http://xl.shtwfgs.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pj.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://fp.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ny.huixiangedu.cn

[R34] 退出时清理
来源：http://uy.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mg.shxzskj.cn

[R35] 后台执行并等待
来源：http://gq.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tm.521024.cn

[R36] 并发执行多个任务
来源：http://mp.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qh.muxihuayi.cn

[R37] 把输出赋给变量
来源：http://ra.521024.cn

files=$(ls -1)
来源：http://ck.bjjhwx.cn

[R38] 管道串联
来源：http://vx.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://ok.bookmarksfly.cn

[R39] 重定向标准输出与错误
来源：http://qc.huanxung.cn

cmd > out.log 2>&1
来源：http://xq.bjjhwx.cn

[R40] 追加写日志
来源：http://hq.gzmigu.cn

echo "log" >> out.log
来源：http://yu.521024.cn

[R41] 丢弃输出
来源：http://dt.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://xl.bjjhwx.cn

[R42] 输入重定向
来源：http://zv.asd995.cn

wc -l < a.txt
来源：http://lw.shtwfgs.cn

[R43] 按名字查找文件
来源：http://im.hahajie.cn

find . -name "*.log" -type f
来源：http://ns.muxihuayi.cn

[R44] 按修改时间查找
来源：http://mx.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://pf.szsharing.cn

[R45] 批量删除
来源：http://ny.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://ez.shxzukj.cn

[R46] 递归替换文件内容
来源：http://hl.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dp.panjiajie.cn

[R47] sed 单行替换
来源：http://ur.nszjky.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ru.hnjuh.cn

[R48] awk 取指定列
来源：http://ho.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://pr.bjjhwx.cn

[R49] awk 带条件
来源：http://yk.muxihuayi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ru.lnxyls.cn

[R50] awk 求和
来源：http://fh.bjjhwx.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uk.hnjuh.cn

[R51] 排序去重取前几
来源：http://ap.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ky.hnjuh.cn

[R52] 统计行数
来源：http://po.bjjhwx.cn

wc -l a.txt
来源：http://ja.521024.cn

[R53] 查看文件头与实时尾
来源：http://fh.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://je.hahajie.cn

[R54] 比较两个文件
来源：http://nn.hahajie.cn

diff a.txt b.txt
来源：http://vw.gzmigu.cn

[R55] 压缩与解压
来源：http://ob.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kb.panjiajie.cn

[R56] 远程拷贝
来源：http://ms.yuexingan06.cn

scp file user@host:/path/
来源：http://ih.gzmigu.cn

[R57] 远程执行命令
来源：http://nd.jctech888.com.cn

ssh user@host 'uptime'
来源：http://lc.szxytkj.cn

[R58] 下载文件
来源：http://et.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://de.shxzskj.cn

[R59] 发 POST JSON
来源：http://es.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://va.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://bh.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oz.szxytkj.cn

[R61] 磁盘占用
来源：http://uh.yuexingan06.cn

df -h;  du -sh *
来源：http://rh.shxzukj.cn

[R62] 找最占空间的文件
来源：http://xp.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://di.bjjhwx.cn

[R63] 内存与进程
来源：http://el.newstarts.cn

free -h;  ps aux | grep nginx
来源：http://ee.haigaiapp.cn

[R64] 结束进程
来源：http://ra.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://pm.jctech888.com.cn

[R65] 查看端口占用
来源：http://ln.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ov.hahajie.cn

[R66] 定时任务
来源：http://rn.newstarts.cn

crontab -e;  crontab -l
来源：http://dc.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://qa.gzmigu.cn

openssl rand -hex 16
来源：http://fc.nszjky.cn

[R68] 计算文件校验值
来源：http://fa.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ae.newstarts.cn

[R69] 生成随机密码
来源：http://qq.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://jt.asd995.cn

[R70] 时间戳与互转
来源：http://vf.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://ja.nszjky.cn

[R71] 日期格式化
来源：http://es.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ar.jctech888.com.cn

[R72] 等待端口就绪
来源：http://ti.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://va.haigaiapp.cn

[R73] 分割大日志
来源：http://df.jctech888.com.cn

split -l 1000 big.log part_
来源：http://tw.jianghongdianzi.cn

[R74] 批量重命名
来源：http://gb.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bq.nszjky.cn

[R75] 导出环境变量
来源：http://ep.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://fj.szxytkj.cn

[R76] 使用临时文件
来源：http://do.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tn.nicolike.cn

[R77] 读取用户输入
来源：http://qn.shtwfgs.cn

read -rp "请输入: " ans
来源：http://sx.lnxyls.cn

[R78] 交互式菜单
来源：http://tb.jctech888.com.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xx.bjjhwx.cn

[R79] 解析命令行选项
来源：http://fz.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ui.9csxet.cn

[R80] 查看脚本执行耗时
来源：http://aq.521024.cn

time ./run.sh
来源：http://dv.shtwfgs.cn

================================================================================
来源：http://lw.shtwfgs.cn

S. C / C++ 专题
来源：http://pp.szsharing.cn

================================================================================
来源：http://eh.hahajie.cn

[S01] C：Hello World
来源：http://hr.521024.cn

#include <stdio.h>
来源：http://fs.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ch.hahajie.cn

[S02] C：变量与格式化输出
来源：http://fr.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://zl.shtwfgs.cn

[S03] C：读入整数
来源：http://vh.jianghongdianzi.cn

int x; scanf("%d", &x);
来源：http://gn.chemitech.net.cn

[S04] C：字符串复制
来源：http://wd.panjiajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pp.521024.cn

[S05] C：字符串长度
来源：http://mr.521024.cn

strlen(s)
来源：http://oc.jctech888.com.cn

[S06] C：字符串比较
来源：http://qt.chemitech.net.cn

strcmp(a, b) == 0
来源：http://ug.shxzukj.cn

[S07] C：数组遍历求和
来源：http://qo.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uz.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://cs.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://il.bjjhwx.cn

[S09] C：结构体定义与初始化
来源：http://gt.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dy.szxytkj.cn

[S10] C：指针与解引用
来源：http://pw.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://xq.nicolike.cn

[S11] C：逐行读文件
来源：http://ni.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://nr.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bp.haigaiapp.cn

fclose(f);
来源：http://yp.shxzskj.cn

[S12] C：写文件
来源：http://yk.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://al.chemitech.net.cn

[S13] C：宏定义
来源：http://ea.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lk.wgjwhj.cn

[S14] C：枚举
来源：http://wd.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://lk.haigaiapp.cn

[S15] C：类型转换
来源：http://ww.szsharing.cn

(double) a / b
来源：http://pg.szsharing.cn

[S16] C：位操作置位
来源：http://ij.hnjuh.cn

x |= (1 << 3);
来源：http://vi.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://pq.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fz.muxihuayi.cn

[S18] C：命令行参数
来源：http://ih.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://bv.shtwfgs.cn

[S19] C：快速排序
来源：http://wg.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qo.shtwfgs.cn

[S20] C：二分查找
来源：http://sx.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ch.hahajie.cn

[S21] C：字符类别判断
来源：http://mn.shxzskj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qa.muxihuayi.cn

[S22] C：字符串转数字
来源：http://dz.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mq.newstarts.cn

[S23] C：随机数
来源：http://do.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gx.9csxet.cn

[S24] C：获取本地时间
来源：http://fm.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gg.huanxung.cn

[S25] C：内存拷贝
来源：http://hf.huixiangedu.cn

memcpy(dst, src, n);
来源：http://et.newstarts.cn

[S26] C：内存清零
来源：http://lk.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://ul.colortex.cn

[S27] C：定义常量
来源：http://td.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://yo.bookmarksfly.cn

[S28] C：静态变量
来源：http://rk.nicolike.cn

static int counter = 0;
来源：http://cq.hahajie.cn

[S29] C：变参函数
来源：http://lw.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wn.yuexingan06.cn

[S30] C：头文件保护
来源：http://vv.hnjuh.cn

#ifndef X_H
来源：http://tf.muxihuayi.cn

#define X_H
来源：http://tt.haigaiapp.cn

#endif
来源：http://oz.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://jk.szsharing.cn

#include <iostream>
来源：http://ev.yuexingan06.cn

int main() { std::cout << "Hello\n"; }
来源：http://eb.panjiajie.cn

[S32] C++：字符串
来源：http://me.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://lz.haigaiapp.cn

[S33] C++：vector 增删
来源：http://ng.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wt.shxzskj.cn

[S34] C++：遍历 vector
来源：http://qi.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://cp.huanxung.cn

[S35] C++：map
来源：http://wq.9csxet.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qv.haigaiapp.cn

[S36] C++：unordered_map
来源：http://bl.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://us.jctech888.com.cn

[S37] C++：set
来源：http://ar.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://aq.szsharing.cn

[S38] C++：排序
来源：http://hb.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://rm.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://dd.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vm.muxihuayi.cn

[S40] C++：查找元素
来源：http://da.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vr.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://ww.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fm.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://xs.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://og.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://dg.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://ky.shxzskj.cn

[S44] C++：引用传参
来源：http://xv.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://tn.shtwfgs.cn

[S45] C++：lambda
来源：http://yk.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wg.szxytkj.cn

[S46] C++：函数模板
来源：http://jz.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gi.panjiajie.cn

[S47] C++：结构化绑定遍历
来源：http://dd.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zj.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://xe.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ah.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://mg.haigaiapp.cn

[S49] C++：写文件
来源：http://te.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://py.szxytkj.cn

[S50] C++：格式化数字
来源：http://vh.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wh.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://im.huanxung.cn

static_cast<double>(a) / b
来源：http://au.huixinmuqiang.cn

[S52] C++：const 与 noexcept
来源：http://ma.huanxung.cn

int size() const noexcept { return n_; }
来源：http://bu.shxzskj.cn

[S53] C++：移动语义
来源：http://dh.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://yt.muxihuayi.cn

[S54] C++：异常处理
来源：http://ml.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cu.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://fv.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yz.shxzukj.cn

[S56] C++：optional
来源：http://px.wgjwhj.cn


<!-- 参考信息 -->