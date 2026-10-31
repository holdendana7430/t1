代发 wailian999

[Q86] 读取 JSON 字段
来源：http://bu.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ep.haigaiapp.cn

[Q87] JSON 字段做条件
来源：http://uz.yuexingan06.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lo.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://yu.newstarts.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bt.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pn.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://sz.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dg.huanxung.cn

[Q90] 生成序号列
来源：http://pa.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://st.huixinmuqiang.cn

================================================================================
来源：http://fj.jctech888.com.cn

R. Bash 专题
来源：http://ry.521024.cn

================================================================================
来源：http://ud.nszjky.cn

[R01] shebang 与严格模式
来源：http://gm.chemitech.net.cn

#!/usr/bin/env bash
来源：http://il.shxzskj.cn

set -euo pipefail
来源：http://vg.panjiajie.cn

[R02] 变量赋值与使用
来源：http://mr.gzmigu.cn

name="Tom"; echo "$name"
来源：http://ep.szxytkj.cn

[R03] 只读变量
来源：http://hr.bookmarksfly.cn

readonly PI=3.14
来源：http://sf.huixiangedu.cn

[R04] 位置参数
来源：http://px.hnjuh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mq.huixinmuqiang.cn

[R05] 参数默认值
来源：http://rm.jctech888.com.cn

name="${1:-default}"
来源：http://ny.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://me.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cz.yuexingan06.cn

[R07] if 判断文件
来源：http://ly.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://it.lnxyls.cn

[R08] 数值比较
来源：http://ii.szxytkj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://iv.yuntaijiaju.cn

[R09] 字符串比较
来源：http://bf.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qu.chemitech.net.cn

[R10] 正则匹配
来源：http://bf.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bb.chemitech.net.cn

[R11] case 多分支
来源：http://wy.bjjhwx.cn

case "$1" in
来源：http://ll.hnjuh.cn

start) echo "启动" ;;
来源：http://gi.huixiangedu.cn

stop)  echo "停止" ;;
来源：http://dr.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://qv.lnxyls.cn

esac
来源：http://xq.newstarts.cn

[R12] for 遍历文件
来源：http://rd.9csxet.cn

for f in *.txt; do echo "$f"; done
来源：http://hm.colortex.cn

[R13] for 计数循环
来源：http://ro.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://xv.gzmigu.cn

[R14] C 风格 for
来源：http://et.hahajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://co.shtwfgs.cn

[R15] while 逐行读文件
来源：http://dh.hahajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vr.muxihuayi.cn

[R16] until 等待条件
来源：http://rn.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nv.jianghongdianzi.cn

[R17] 数组定义与取值
来源：http://zq.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://io.huixinmuqiang.cn

[R18] 遍历数组
来源：http://wt.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ka.shxzukj.cn

[R19] 数组长度
来源：http://wj.newstarts.cn

echo "${#arr[@]}"
来源：http://xx.shtwfgs.cn

[R20] 关联数组（字典）
来源：http://dw.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lc.jctech888.com.cn

[R21] 字符串长度
来源：http://ju.panjiajie.cn

echo "${#s}"
来源：http://pg.szsharing.cn

[R22] 截取子串
来源：http://kp.bookmarksfly.cn

echo "${s:0:5}"
来源：http://aj.521024.cn

[R23] 字符串替换
来源：http://ze.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pd.huixiangedu.cn

[R24] 大小写转换
来源：http://zm.nszjky.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tw.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://uf.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ml.lnxyls.cn

[R26] 命令替换
来源：http://mp.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://zj.asd995.cn

[R27] 算术展开
来源：http://pg.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://om.newstarts.cn

[R28] 浮点运算
来源：http://eu.muxihuayi.cn

echo "scale=2; 10/3" | bc
来源：http://ta.huixiangedu.cn

[R29] 定义函数
来源：http://gf.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gu.huixiangedu.cn

[R30] 函数返回状态码
来源：http://ap.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://bm.521024.cn

[R31] 局部变量
来源：http://yy.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://dc.chemitech.net.cn

[R32] 参数个数校验
来源：http://vo.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rj.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://ai.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gt.hnjuh.cn

[R34] 退出时清理
来源：http://yg.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dl.nszjky.cn

[R35] 后台执行并等待
来源：http://pg.hnjuh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wy.shxzukj.cn

[R36] 并发执行多个任务
来源：http://wf.nszjky.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ga.colortex.cn

[R37] 把输出赋给变量
来源：http://xy.huixiangedu.cn

files=$(ls -1)
来源：http://un.nszjky.cn

[R38] 管道串联
来源：http://gq.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://mo.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://me.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://fo.hahajie.cn

[R40] 追加写日志
来源：http://pk.lnxyls.cn

echo "log" >> out.log
来源：http://xz.9csxet.cn

[R41] 丢弃输出
来源：http://ct.wgjwhj.cn

cmd >/dev/null 2>&1
来源：http://oc.hahajie.cn

[R42] 输入重定向
来源：http://sk.wgjwhj.cn

wc -l < a.txt
来源：http://mc.asd995.cn

[R43] 按名字查找文件
来源：http://kg.colortex.cn

find . -name "*.log" -type f
来源：http://ys.muxihuayi.cn

[R44] 按修改时间查找
来源：http://bv.jctech888.com.cn

find . -mtime -7 -type f
来源：http://qm.hnjuh.cn

[R45] 批量删除
来源：http://zq.colortex.cn

find . -name "*.tmp" -delete
来源：http://cb.shxzskj.cn

[R46] 递归替换文件内容
来源：http://mk.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cy.newstarts.cn

[R47] sed 单行替换
来源：http://zh.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mz.shtwfgs.cn

[R48] awk 取指定列
来源：http://ia.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://zy.nicolike.cn

[R49] awk 带条件
来源：http://yz.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gu.panjiajie.cn

[R50] awk 求和
来源：http://up.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uy.szxytkj.cn

[R51] 排序去重取前几
来源：http://af.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qe.gzmigu.cn

[R52] 统计行数
来源：http://eg.asd995.cn

wc -l a.txt
来源：http://jq.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://op.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dq.chemitech.net.cn

[R54] 比较两个文件
来源：http://lu.wgjwhj.cn

diff a.txt b.txt
来源：http://yl.haigaiapp.cn

[R55] 压缩与解压
来源：http://aa.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ky.yuexingan06.cn

[R56] 远程拷贝
来源：http://wy.wgjwhj.cn

scp file user@host:/path/
来源：http://ii.jctech888.com.cn

[R57] 远程执行命令
来源：http://ww.shtwfgs.cn

ssh user@host 'uptime'
来源：http://lu.gzmigu.cn

[R58] 下载文件
来源：http://hk.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sf.chemitech.net.cn

[R59] 发 POST JSON
来源：http://ba.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cs.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://ue.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ux.bjjhwx.cn

[R61] 磁盘占用
来源：http://wv.szsharing.cn

df -h;  du -sh *
来源：http://fb.szxytkj.cn

[R62] 找最占空间的文件
来源：http://pe.chemitech.net.cn

du -ah . | sort -rh | head -10
来源：http://ll.huanxung.cn

[R63] 内存与进程
来源：http://bu.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://vw.muxihuayi.cn

[R64] 结束进程
来源：http://nb.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://hs.wgjwhj.cn

[R65] 查看端口占用
来源：http://cb.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uo.hahajie.cn

[R66] 定时任务
来源：http://he.haigaiapp.cn

crontab -e;  crontab -l
来源：http://jg.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://pu.wgjwhj.cn

openssl rand -hex 16
来源：http://xe.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://ia.huixiangedu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qi.shxzukj.cn

[R69] 生成随机密码
来源：http://kk.huanxung.cn

head -c 16 /dev/urandom | base64
来源：http://dr.muxihuayi.cn

[R70] 时间戳与互转
来源：http://fb.521024.cn

date +%s;  date -d @1700000000
来源：http://er.szsharing.cn

[R71] 日期格式化
来源：http://ag.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ev.shxzskj.cn

[R72] 等待端口就绪
来源：http://kv.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kp.colortex.cn

[R73] 分割大日志
来源：http://nx.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://tj.panjiajie.cn

[R74] 批量重命名
来源：http://og.jctech888.com.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ud.nicolike.cn

[R75] 导出环境变量
来源：http://by.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://st.jctech888.com.cn

[R76] 使用临时文件
来源：http://ll.huixinmuqiang.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://er.colortex.cn

[R77] 读取用户输入
来源：http://ol.panjiajie.cn

read -rp "请输入: " ans
来源：http://un.chemitech.net.cn

[R78] 交互式菜单
来源：http://zs.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oi.asd995.cn

[R79] 解析命令行选项
来源：http://zv.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://px.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://ir.huixiangedu.cn

time ./run.sh
来源：http://bk.yuexingan06.cn

================================================================================
来源：http://ln.colortex.cn

S. C / C++ 专题
来源：http://nv.hnjuh.cn

================================================================================
来源：http://aq.lnxyls.cn

[S01] C：Hello World
来源：http://ze.shxzukj.cn

#include <stdio.h>
来源：http://be.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sh.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://ka.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://fd.asd995.cn

[S03] C：读入整数
来源：http://uu.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://im.9csxet.cn

[S04] C：字符串复制
来源：http://xn.nicolike.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mp.jctech888.com.cn

[S05] C：字符串长度
来源：http://lj.lnxyls.cn

strlen(s)
来源：http://ms.chemitech.net.cn

[S06] C：字符串比较
来源：http://jg.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://ut.newstarts.cn

[S07] C：数组遍历求和
来源：http://ws.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qm.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://mf.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yb.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://uj.hnjuh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qy.panjiajie.cn

[S10] C：指针与解引用
来源：http://go.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://vi.newstarts.cn

[S11] C：逐行读文件
来源：http://ld.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://bc.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zg.bookmarksfly.cn

fclose(f);
来源：http://fi.huanxung.cn

[S12] C：写文件
来源：http://xw.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gt.yuntaijiaju.cn

[S13] C：宏定义
来源：http://vd.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yp.huixinmuqiang.cn

[S14] C：枚举
来源：http://dk.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://ph.colortex.cn

[S15] C：类型转换
来源：http://cp.jianghongdianzi.cn

(double) a / b
来源：http://fd.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://gd.yuntaijiaju.cn

x |= (1 << 3);
来源：http://nk.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://xr.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ke.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://lc.nszjky.cn

int main(int argc, char **argv)
来源：http://da.gzmigu.cn

[S19] C：快速排序
来源：http://uf.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ia.nicolike.cn

[S20] C：二分查找
来源：http://ug.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cc.wgjwhj.cn

[S21] C：字符类别判断
来源：http://ms.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rl.wgjwhj.cn

[S22] C：字符串转数字
来源：http://se.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fg.nicolike.cn

[S23] C：随机数
来源：http://ew.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yu.hnjuh.cn

[S24] C：获取本地时间
来源：http://qt.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wi.huixiangedu.cn

[S25] C：内存拷贝
来源：http://sh.szxytkj.cn

memcpy(dst, src, n);
来源：http://vm.521024.cn

[S26] C：内存清零
来源：http://ll.huanxung.cn

memset(a, 0, sizeof a);
来源：http://fs.muxihuayi.cn

[S27] C：定义常量
来源：http://pp.szxytkj.cn

const double PI = 3.14159;
来源：http://zs.muxihuayi.cn

[S28] C：静态变量
来源：http://vc.wgjwhj.cn

static int counter = 0;
来源：http://vr.muxihuayi.cn

[S29] C：变参函数
来源：http://mu.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ra.shtwfgs.cn

[S30] C：头文件保护
来源：http://hi.lnxyls.cn

#ifndef X_H
来源：http://kg.haigaiapp.cn

#define X_H
来源：http://cs.szsharing.cn

#endif
来源：http://yd.muxihuayi.cn

[S31] C++：Hello World
来源：http://do.szxytkj.cn

#include <iostream>
来源：http://ms.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://sw.gzmigu.cn

[S32] C++：字符串
来源：http://ns.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://nc.huixiangedu.cn

[S33] C++：vector 增删
来源：http://hk.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zt.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://mh.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://qg.huanxung.cn

[S35] C++：map
来源：http://hp.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jf.521024.cn

[S36] C++：unordered_map
来源：http://zg.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sn.szsharing.cn

[S37] C++：set
来源：http://zh.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kk.asd995.cn

[S38] C++：排序
来源：http://bk.521024.cn

std::sort(v.begin(), v.end());
来源：http://dp.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://fm.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nl.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://oq.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mh.newstarts.cn

[S41] C++：类与构造函数
来源：http://jt.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vs.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://ee.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://nt.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://mg.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://ox.colortex.cn

[S44] C++：引用传参
来源：http://ij.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://bf.bookmarksfly.cn

[S45] C++：lambda
来源：http://cm.yuexingan06.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qh.hahajie.cn

[S46] C++：函数模板
来源：http://nu.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hl.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://tm.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fi.szxytkj.cn

[S48] C++：逐行读文件
来源：http://dr.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mz.colortex.cn

while (std::getline(in, line)) { }
来源：http://vf.shxzukj.cn

[S49] C++：写文件
来源：http://fj.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fh.huanxung.cn

[S50] C++：格式化数字
来源：http://qc.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mb.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://xa.nicolike.cn

static_cast<double>(a) / b
来源：http://bt.colortex.cn

[S52] C++：const 与 noexcept
来源：http://qw.szsharing.cn

int size() const noexcept { return n_; }
来源：http://ux.gzmigu.cn

[S53] C++：移动语义
来源：http://zn.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://gu.shxzukj.cn

[S54] C++：异常处理
来源：http://df.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bu.szsharing.cn

[S55] C++：结构化绑定
来源：http://qo.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rx.nszjky.cn

[S56] C++：optional
来源：http://xq.haigaiapp.cn


<!-- 参考信息 -->