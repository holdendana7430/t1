代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://ba.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nk.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pk.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://gs.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ll.haigaiapp.cn

[Q90] 生成序号列
来源：http://rt.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kf.haigaiapp.cn

================================================================================
来源：http://an.9csxet.cn

R. Bash 专题
来源：http://ut.521024.cn

================================================================================
来源：http://fq.shxzukj.cn

[R01] shebang 与严格模式
来源：http://oy.chemitech.net.cn

#!/usr/bin/env bash
来源：http://sp.gzmigu.cn

set -euo pipefail
来源：http://io.colortex.cn

[R02] 变量赋值与使用
来源：http://cw.shxzukj.cn

name="Tom"; echo "$name"
来源：http://sp.hahajie.cn

[R03] 只读变量
来源：http://zl.szsharing.cn

readonly PI=3.14
来源：http://ol.huixinmuqiang.cn

[R04] 位置参数
来源：http://pw.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lt.wgjwhj.cn

[R05] 参数默认值
来源：http://ce.lnxyls.cn

name="${1:-default}"
来源：http://ou.nicolike.cn

[R06] 判断命令是否存在
来源：http://vo.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nc.haigaiapp.cn

[R07] if 判断文件
来源：http://dx.shxzukj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nv.521024.cn

[R08] 数值比较
来源：http://be.jianghongdianzi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bh.yuexingan06.cn

[R09] 字符串比较
来源：http://ba.szxytkj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bh.hnjuh.cn

[R10] 正则匹配
来源：http://ue.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hu.szxytkj.cn

[R11] case 多分支
来源：http://yz.muxihuayi.cn

case "$1" in
来源：http://lf.shxzukj.cn

start) echo "启动" ;;
来源：http://ja.newstarts.cn

stop)  echo "停止" ;;
来源：http://ag.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://mh.huixiangedu.cn

esac
来源：http://dz.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://vh.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://gi.colortex.cn

[R13] for 计数循环
来源：http://bv.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://lg.muxihuayi.cn

[R14] C 风格 for
来源：http://hx.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xe.hnjuh.cn

[R15] while 逐行读文件
来源：http://vo.huanxung.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ih.colortex.cn

[R16] until 等待条件
来源：http://lq.nszjky.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eb.szxytkj.cn

[R17] 数组定义与取值
来源：http://nh.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bp.newstarts.cn

[R18] 遍历数组
来源：http://jo.szxytkj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hj.nszjky.cn

[R19] 数组长度
来源：http://qy.gzmigu.cn

echo "${#arr[@]}"
来源：http://tj.9csxet.cn

[R20] 关联数组（字典）
来源：http://my.muxihuayi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ij.yuntaijiaju.cn

[R21] 字符串长度
来源：http://kj.muxihuayi.cn

echo "${#s}"
来源：http://wl.shxzukj.cn

[R22] 截取子串
来源：http://tl.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://ur.bookmarksfly.cn

[R23] 字符串替换
来源：http://ko.shtwfgs.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ox.huanxung.cn

[R24] 大小写转换
来源：http://pf.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tx.9csxet.cn

[R25] 去后缀 / 去前缀
来源：http://ey.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cg.shxzskj.cn

[R26] 命令替换
来源：http://to.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://ay.yuntaijiaju.cn

[R27] 算术展开
来源：http://tn.newstarts.cn

echo $((1 + 2 * 3))
来源：http://jy.shxzskj.cn

[R28] 浮点运算
来源：http://oa.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://hv.colortex.cn

[R29] 定义函数
来源：http://gn.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jm.szsharing.cn

[R30] 函数返回状态码
来源：http://ha.szxytkj.cn

f() { return 0; }; f || echo "失败了"
来源：http://ps.nicolike.cn

[R31] 局部变量
来源：http://ay.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://vp.shtwfgs.cn

[R32] 参数个数校验
来源：http://ju.colortex.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ng.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://sv.haigaiapp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ru.jctech888.com.cn

[R34] 退出时清理
来源：http://kw.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ef.newstarts.cn

[R35] 后台执行并等待
来源：http://dy.szxytkj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kc.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://oi.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xh.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://ll.huanxung.cn

files=$(ls -1)
来源：http://qy.huixiangedu.cn

[R38] 管道串联
来源：http://ef.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://vy.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://ew.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://fh.huixinmuqiang.cn

[R40] 追加写日志
来源：http://rc.huixiangedu.cn

echo "log" >> out.log
来源：http://ga.9csxet.cn

[R41] 丢弃输出
来源：http://aa.wgjwhj.cn

cmd >/dev/null 2>&1
来源：http://gs.newstarts.cn

[R42] 输入重定向
来源：http://nm.chemitech.net.cn

wc -l < a.txt
来源：http://sn.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://gi.jctech888.com.cn

find . -name "*.log" -type f
来源：http://gz.huanxung.cn

[R44] 按修改时间查找
来源：http://is.huixiangedu.cn

find . -mtime -7 -type f
来源：http://oc.huixinmuqiang.cn

[R45] 批量删除
来源：http://kw.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://ox.muxihuayi.cn

[R46] 递归替换文件内容
来源：http://xc.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vo.bookmarksfly.cn

[R47] sed 单行替换
来源：http://wc.bookmarksfly.cn

sed -i 's/foo/bar/g' a.txt
来源：http://es.hnjuh.cn

[R48] awk 取指定列
来源：http://gb.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://vh.panjiajie.cn

[R49] awk 带条件
来源：http://iu.lnxyls.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uc.asd995.cn

[R50] awk 求和
来源：http://pj.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ik.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://um.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ir.nicolike.cn

[R52] 统计行数
来源：http://ih.yuexingan06.cn

wc -l a.txt
来源：http://td.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://am.lnxyls.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cz.521024.cn

[R54] 比较两个文件
来源：http://hx.yuntaijiaju.cn

diff a.txt b.txt
来源：http://vn.yuexingan06.cn

[R55] 压缩与解压
来源：http://dj.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rm.9csxet.cn

[R56] 远程拷贝
来源：http://lr.jianghongdianzi.cn

scp file user@host:/path/
来源：http://oz.haigaiapp.cn

[R57] 远程执行命令
来源：http://bk.shxzskj.cn

ssh user@host 'uptime'
来源：http://pa.bjjhwx.cn

[R58] 下载文件
来源：http://av.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pm.asd995.cn

[R59] 发 POST JSON
来源：http://kz.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mo.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://jq.yuexingan06.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://az.muxihuayi.cn

[R61] 磁盘占用
来源：http://ly.gzmigu.cn

df -h;  du -sh *
来源：http://ns.gzmigu.cn

[R62] 找最占空间的文件
来源：http://fm.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://jc.huixiangedu.cn

[R63] 内存与进程
来源：http://qg.wgjwhj.cn

free -h;  ps aux | grep nginx
来源：http://ke.shxzukj.cn

[R64] 结束进程
来源：http://fu.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://cg.shtwfgs.cn

[R65] 查看端口占用
来源：http://rs.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sd.jianghongdianzi.cn

[R66] 定时任务
来源：http://rp.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://sg.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://ek.yuexingan06.cn

openssl rand -hex 16
来源：http://fp.panjiajie.cn

[R68] 计算文件校验值
来源：http://ev.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ly.asd995.cn

[R69] 生成随机密码
来源：http://aj.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://yb.chemitech.net.cn

[R70] 时间戳与互转
来源：http://id.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://jp.lnxyls.cn

[R71] 日期格式化
来源：http://ro.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mf.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://mf.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ij.asd995.cn

[R73] 分割大日志
来源：http://ia.huanxung.cn

split -l 1000 big.log part_
来源：http://xl.chemitech.net.cn

[R74] 批量重命名
来源：http://cv.shxzskj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jr.jctech888.com.cn

[R75] 导出环境变量
来源：http://it.hnjuh.cn

export PATH="$HOME/bin:$PATH"
来源：http://mh.9csxet.cn

[R76] 使用临时文件
来源：http://eg.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rv.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://un.szsharing.cn

read -rp "请输入: " ans
来源：http://pi.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://te.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kr.panjiajie.cn

[R79] 解析命令行选项
来源：http://wp.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zq.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://cf.haigaiapp.cn

time ./run.sh
来源：http://zf.521024.cn

================================================================================
来源：http://ip.hahajie.cn

S. C / C++ 专题
来源：http://dg.szsharing.cn

================================================================================
来源：http://kq.bookmarksfly.cn

[S01] C：Hello World
来源：http://kk.muxihuayi.cn

#include <stdio.h>
来源：http://tp.jianghongdianzi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ur.gzmigu.cn

[S02] C：变量与格式化输出
来源：http://lr.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://oz.colortex.cn

[S03] C：读入整数
来源：http://wg.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://xc.shtwfgs.cn

[S04] C：字符串复制
来源：http://oc.gzmigu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kw.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://qo.bookmarksfly.cn

strlen(s)
来源：http://yb.nszjky.cn

[S06] C：字符串比较
来源：http://nm.gzmigu.cn

strcmp(a, b) == 0
来源：http://np.nszjky.cn

[S07] C：数组遍历求和
来源：http://pt.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yn.9csxet.cn

[S08] C：动态内存分配与释放
来源：http://oy.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ks.colortex.cn

[S09] C：结构体定义与初始化
来源：http://to.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://id.jctech888.com.cn

[S10] C：指针与解引用
来源：http://lc.asd995.cn

int *p = &a;  *p = 5;
来源：http://he.colortex.cn

[S11] C：逐行读文件
来源：http://hl.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://yi.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://la.yuexingan06.cn

fclose(f);
来源：http://wf.nszjky.cn

[S12] C：写文件
来源：http://ig.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ab.hnjuh.cn

[S13] C：宏定义
来源：http://pj.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cm.jctech888.com.cn

[S14] C：枚举
来源：http://rs.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://zw.gzmigu.cn

[S15] C：类型转换
来源：http://sr.shxzukj.cn

(double) a / b
来源：http://zy.lnxyls.cn

[S16] C：位操作置位
来源：http://uq.bookmarksfly.cn

x |= (1 << 3);
来源：http://ye.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://am.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zh.yuexingan06.cn

[S18] C：命令行参数
来源：http://bf.huanxung.cn

int main(int argc, char **argv)
来源：http://ar.lnxyls.cn

[S19] C：快速排序
来源：http://yx.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qv.gzmigu.cn

[S20] C：二分查找
来源：http://mt.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://px.haigaiapp.cn

[S21] C：字符类别判断
来源：http://sc.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ni.lnxyls.cn

[S22] C：字符串转数字
来源：http://yz.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mp.521024.cn

[S23] C：随机数
来源：http://hz.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cz.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://xp.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rr.shxzskj.cn

[S25] C：内存拷贝
来源：http://hx.shxzukj.cn

memcpy(dst, src, n);
来源：http://uz.nicolike.cn

[S26] C：内存清零
来源：http://ai.521024.cn

memset(a, 0, sizeof a);
来源：http://bo.huixinmuqiang.cn

[S27] C：定义常量
来源：http://wo.panjiajie.cn

const double PI = 3.14159;
来源：http://nt.huixiangedu.cn

[S28] C：静态变量
来源：http://mk.yuexingan06.cn

static int counter = 0;
来源：http://ed.wgjwhj.cn

[S29] C：变参函数
来源：http://hq.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jw.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://el.panjiajie.cn

#ifndef X_H
来源：http://tt.muxihuayi.cn

#define X_H
来源：http://sm.newstarts.cn

#endif
来源：http://qz.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://hy.asd995.cn

#include <iostream>
来源：http://lq.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ck.muxihuayi.cn

[S32] C++：字符串
来源：http://ll.521024.cn

std::string s = "hi";  s += "!";
来源：http://ts.huanxung.cn

[S33] C++：vector 增删
来源：http://oa.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rq.hahajie.cn

[S34] C++：遍历 vector
来源：http://ua.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://yy.hahajie.cn

[S35] C++：map
来源：http://ez.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pf.huixiangedu.cn

[S36] C++：unordered_map
来源：http://xa.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://za.jctech888.com.cn

[S37] C++：set
来源：http://uz.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://az.hahajie.cn

[S38] C++：排序
来源：http://ce.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://ky.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://uk.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ux.bookmarksfly.cn

[S40] C++：查找元素
来源：http://td.jianghongdianzi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tf.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://kv.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://eo.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://wi.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://eb.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://lc.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://nd.huanxung.cn

[S44] C++：引用传参
来源：http://hp.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://vw.jctech888.com.cn

[S45] C++：lambda
来源：http://zd.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sz.szxytkj.cn

[S46] C++：函数模板
来源：http://vt.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sf.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://tr.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ph.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://zs.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://my.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://we.nszjky.cn

[S49] C++：写文件
来源：http://ne.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dz.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://nb.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bx.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://ud.chemitech.net.cn

static_cast<double>(a) / b
来源：http://mu.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://rx.521024.cn

int size() const noexcept { return n_; }
来源：http://hc.szxytkj.cn

[S53] C++：移动语义
来源：http://ci.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://ol.wgjwhj.cn

[S54] C++：异常处理
来源：http://hf.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ti.szxytkj.cn

[S55] C++：结构化绑定
来源：http://dj.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cl.nicolike.cn

[S56] C++：optional
来源：http://kx.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zk.hnjuh.cn

[S57] C++：编译期常量
来源：http://sf.huixinmuqiang.cn

constexpr int N = 10;
来源：http://vq.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://nr.bjjhwx.cn


<!-- 参考信息 -->