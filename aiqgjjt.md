代发 wailian999

[Q86] 读取 JSON 字段
来源：http://cq.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pc.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://rb.hnjuh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pk.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://ku.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hw.asd995.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gd.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://tx.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tq.nicolike.cn

[Q90] 生成序号列
来源：http://ab.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ee.panjiajie.cn

================================================================================
来源：http://nw.lnxyls.cn

R. Bash 专题
来源：http://ms.newstarts.cn

================================================================================
来源：http://fg.hnjuh.cn

[R01] shebang 与严格模式
来源：http://un.wgjwhj.cn

#!/usr/bin/env bash
来源：http://wc.shxzskj.cn

set -euo pipefail
来源：http://xa.huanxung.cn

[R02] 变量赋值与使用
来源：http://gs.521024.cn

name="Tom"; echo "$name"
来源：http://iw.wgjwhj.cn

[R03] 只读变量
来源：http://pw.szxytkj.cn

readonly PI=3.14
来源：http://mj.haigaiapp.cn

[R04] 位置参数
来源：http://ub.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wp.muxihuayi.cn

[R05] 参数默认值
来源：http://mc.asd995.cn

name="${1:-default}"
来源：http://rt.yuexingan06.cn

[R06] 判断命令是否存在
来源：http://oo.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uc.huixiangedu.cn

[R07] if 判断文件
来源：http://ah.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jx.lnxyls.cn

[R08] 数值比较
来源：http://kx.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://re.521024.cn

[R09] 字符串比较
来源：http://vb.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ad.newstarts.cn

[R10] 正则匹配
来源：http://um.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ub.gzmigu.cn

[R11] case 多分支
来源：http://xm.bjjhwx.cn

case "$1" in
来源：http://ic.yuexingan06.cn

start) echo "启动" ;;
来源：http://oy.shtwfgs.cn

stop)  echo "停止" ;;
来源：http://um.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://um.newstarts.cn

esac
来源：http://dh.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://vw.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://zi.asd995.cn

[R13] for 计数循环
来源：http://go.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://eq.yuexingan06.cn

[R14] C 风格 for
来源：http://lc.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jc.lnxyls.cn

[R15] while 逐行读文件
来源：http://ns.huanxung.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dz.yuntaijiaju.cn

[R16] until 等待条件
来源：http://vz.shxzskj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sk.panjiajie.cn

[R17] 数组定义与取值
来源：http://nc.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ek.yuntaijiaju.cn

[R18] 遍历数组
来源：http://iy.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gg.szxytkj.cn

[R19] 数组长度
来源：http://hf.521024.cn

echo "${#arr[@]}"
来源：http://ov.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://ti.hnjuh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://do.nicolike.cn

[R21] 字符串长度
来源：http://hj.newstarts.cn

echo "${#s}"
来源：http://hm.521024.cn

[R22] 截取子串
来源：http://ov.gzmigu.cn

echo "${s:0:5}"
来源：http://em.newstarts.cn

[R23] 字符串替换
来源：http://lv.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hl.szsharing.cn

[R24] 大小写转换
来源：http://jb.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cp.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://vi.huixiangedu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ul.muxihuayi.cn

[R26] 命令替换
来源：http://jf.yuntaijiaju.cn

now=$(date +%F); echo "$now"
来源：http://ze.huixiangedu.cn

[R27] 算术展开
来源：http://vy.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://mt.muxihuayi.cn

[R28] 浮点运算
来源：http://qc.521024.cn

echo "scale=2; 10/3" | bc
来源：http://ew.huixiangedu.cn

[R29] 定义函数
来源：http://mp.shxzskj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cx.colortex.cn

[R30] 函数返回状态码
来源：http://an.szxytkj.cn

f() { return 0; }; f || echo "失败了"
来源：http://ue.newstarts.cn

[R31] 局部变量
来源：http://go.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://er.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://fw.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ku.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://cg.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://di.lnxyls.cn

[R34] 退出时清理
来源：http://di.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tr.521024.cn

[R35] 后台执行并等待
来源：http://vz.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ps.nicolike.cn

[R36] 并发执行多个任务
来源：http://mg.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dq.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://uv.yuntaijiaju.cn

files=$(ls -1)
来源：http://ab.muxihuayi.cn

[R38] 管道串联
来源：http://dz.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://jq.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://hc.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://gu.asd995.cn

[R40] 追加写日志
来源：http://gs.shtwfgs.cn

echo "log" >> out.log
来源：http://um.hahajie.cn

[R41] 丢弃输出
来源：http://qk.hahajie.cn

cmd >/dev/null 2>&1
来源：http://av.yuntaijiaju.cn

[R42] 输入重定向
来源：http://of.asd995.cn

wc -l < a.txt
来源：http://yj.hahajie.cn

[R43] 按名字查找文件
来源：http://ca.chemitech.net.cn

find . -name "*.log" -type f
来源：http://yi.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://lt.asd995.cn

find . -mtime -7 -type f
来源：http://qq.shxzukj.cn

[R45] 批量删除
来源：http://vy.asd995.cn

find . -name "*.tmp" -delete
来源：http://qn.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://ev.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lh.asd995.cn

[R47] sed 单行替换
来源：http://pf.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ou.gzmigu.cn

[R48] awk 取指定列
来源：http://wy.huixiangedu.cn

awk '{print $1, $3}' a.txt
来源：http://uc.muxihuayi.cn

[R49] awk 带条件
来源：http://yj.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xv.hahajie.cn

[R50] awk 求和
来源：http://am.shxzskj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dj.nicolike.cn

[R51] 排序去重取前几
来源：http://ga.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pl.bookmarksfly.cn

[R52] 统计行数
来源：http://lx.asd995.cn

wc -l a.txt
来源：http://rc.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://ot.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fd.jctech888.com.cn

[R54] 比较两个文件
来源：http://ua.hahajie.cn

diff a.txt b.txt
来源：http://xa.shxzskj.cn

[R55] 压缩与解压
来源：http://de.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yy.9csxet.cn

[R56] 远程拷贝
来源：http://ny.huixinmuqiang.cn

scp file user@host:/path/
来源：http://hl.nicolike.cn

[R57] 远程执行命令
来源：http://kt.haigaiapp.cn

ssh user@host 'uptime'
来源：http://lv.yuntaijiaju.cn

[R58] 下载文件
来源：http://iu.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ef.nicolike.cn

[R59] 发 POST JSON
来源：http://px.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vl.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://jc.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ci.hnjuh.cn

[R61] 磁盘占用
来源：http://gm.szsharing.cn

df -h;  du -sh *
来源：http://le.colortex.cn

[R62] 找最占空间的文件
来源：http://pq.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://mk.haigaiapp.cn

[R63] 内存与进程
来源：http://vq.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://sm.521024.cn

[R64] 结束进程
来源：http://gg.haigaiapp.cn

kill -9 $(pgrep -f app.py)
来源：http://ys.newstarts.cn

[R65] 查看端口占用
来源：http://qz.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nt.bookmarksfly.cn

[R66] 定时任务
来源：http://iy.huanxung.cn

crontab -e;  crontab -l
来源：http://zr.colortex.cn

[R67] 生成随机十六进制串
来源：http://cv.lnxyls.cn

openssl rand -hex 16
来源：http://dj.newstarts.cn

[R68] 计算文件校验值
来源：http://mu.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nk.nicolike.cn

[R69] 生成随机密码
来源：http://qt.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://mk.shxzskj.cn

[R70] 时间戳与互转
来源：http://wq.huixiangedu.cn

date +%s;  date -d @1700000000
来源：http://wl.shxzukj.cn

[R71] 日期格式化
来源：http://qi.jianghongdianzi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://se.asd995.cn

[R72] 等待端口就绪
来源：http://il.yuexingan06.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pj.lnxyls.cn

[R73] 分割大日志
来源：http://zz.asd995.cn

split -l 1000 big.log part_
来源：http://if.huanxung.cn

[R74] 批量重命名
来源：http://vb.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yk.nicolike.cn

[R75] 导出环境变量
来源：http://fs.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://ax.bookmarksfly.cn

[R76] 使用临时文件
来源：http://xk.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zt.panjiajie.cn

[R77] 读取用户输入
来源：http://nw.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://mv.szxytkj.cn

[R78] 交互式菜单
来源：http://re.hahajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ip.shtwfgs.cn

[R79] 解析命令行选项
来源：http://vn.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rs.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://cc.nicolike.cn

time ./run.sh
来源：http://kz.newstarts.cn

================================================================================
来源：http://yq.huixinmuqiang.cn

S. C / C++ 专题
来源：http://ad.shxzskj.cn

================================================================================
来源：http://rs.lnxyls.cn

[S01] C：Hello World
来源：http://ki.9csxet.cn

#include <stdio.h>
来源：http://rd.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ka.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://nl.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://gz.hnjuh.cn

[S03] C：读入整数
来源：http://rg.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://eg.bjjhwx.cn

[S04] C：字符串复制
来源：http://pw.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ru.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://ah.chemitech.net.cn

strlen(s)
来源：http://lb.nszjky.cn

[S06] C：字符串比较
来源：http://ng.521024.cn

strcmp(a, b) == 0
来源：http://lk.shxzskj.cn

[S07] C：数组遍历求和
来源：http://fm.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fo.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://bk.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ei.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://cv.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tt.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://zv.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://dq.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://bq.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://li.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lc.nicolike.cn

fclose(f);
来源：http://pm.521024.cn

[S12] C：写文件
来源：http://rn.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ti.gzmigu.cn

[S13] C：宏定义
来源：http://hp.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yi.jianghongdianzi.cn

[S14] C：枚举
来源：http://oq.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://nk.szxytkj.cn

[S15] C：类型转换
来源：http://fu.shxzskj.cn

(double) a / b
来源：http://qm.panjiajie.cn

[S16] C：位操作置位
来源：http://sx.hahajie.cn

x |= (1 << 3);
来源：http://ds.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://wh.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://za.bjjhwx.cn

[S18] C：命令行参数
来源：http://fm.521024.cn

int main(int argc, char **argv)
来源：http://gv.huixiangedu.cn

[S19] C：快速排序
来源：http://iq.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ox.nicolike.cn

[S20] C：二分查找
来源：http://fs.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tq.lnxyls.cn

[S21] C：字符类别判断
来源：http://xl.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ud.shxzskj.cn

[S22] C：字符串转数字
来源：http://pa.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ro.jianghongdianzi.cn

[S23] C：随机数
来源：http://ji.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ai.gzmigu.cn

[S24] C：获取本地时间
来源：http://nv.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pu.yuexingan06.cn

[S25] C：内存拷贝
来源：http://nd.colortex.cn

memcpy(dst, src, n);
来源：http://tk.yuntaijiaju.cn

[S26] C：内存清零
来源：http://mv.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://qx.haigaiapp.cn

[S27] C：定义常量
来源：http://uh.huixiangedu.cn

const double PI = 3.14159;
来源：http://bd.shxzskj.cn

[S28] C：静态变量
来源：http://hx.huixinmuqiang.cn

static int counter = 0;
来源：http://cj.yuntaijiaju.cn

[S29] C：变参函数
来源：http://fs.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fw.shxzukj.cn

[S30] C：头文件保护
来源：http://zc.yuntaijiaju.cn

#ifndef X_H
来源：http://kx.bookmarksfly.cn

#define X_H
来源：http://sj.shxzskj.cn

#endif
来源：http://pf.newstarts.cn

[S31] C++：Hello World
来源：http://cr.colortex.cn

#include <iostream>
来源：http://yd.yuexingan06.cn

int main() { std::cout << "Hello\n"; }
来源：http://yv.bjjhwx.cn

[S32] C++：字符串
来源：http://zs.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://fb.szsharing.cn

[S33] C++：vector 增删
来源：http://dv.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kp.shxzukj.cn

[S34] C++：遍历 vector
来源：http://zm.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://aw.shxzukj.cn

[S35] C++：map
来源：http://ho.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yk.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://ko.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sp.jctech888.com.cn

[S37] C++：set
来源：http://cy.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nq.nicolike.cn

[S38] C++：排序
来源：http://ou.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://op.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://er.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xx.colortex.cn

[S40] C++：查找元素
来源：http://qc.521024.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wl.shxzukj.cn

[S41] C++：类与构造函数
来源：http://nj.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://im.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://ug.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://bi.gzmigu.cn

[S43] C++：智能指针
来源：http://ll.huixinmuqiang.cn

auto p = std::make_unique<int>(5);
来源：http://nx.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://nl.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://vb.yuexingan06.cn

[S45] C++：lambda
来源：http://hf.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xz.bjjhwx.cn

[S46] C++：函数模板
来源：http://yy.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xc.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://am.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fo.panjiajie.cn

[S48] C++：逐行读文件
来源：http://pi.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cy.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://tt.nicolike.cn

[S49] C++：写文件
来源：http://cw.chemitech.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pp.521024.cn

[S50] C++：格式化数字
来源：http://vi.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ms.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://md.muxihuayi.cn

static_cast<double>(a) / b
来源：http://kh.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://ue.9csxet.cn

int size() const noexcept { return n_; }
来源：http://hq.huixiangedu.cn

[S53] C++：移动语义
来源：http://sm.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://yb.wgjwhj.cn

[S54] C++：异常处理
来源：http://ri.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ng.yuexingan06.cn

[S55] C++：结构化绑定
来源：http://ns.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ua.huanxung.cn

[S56] C++：optional
来源：http://sf.yuexingan06.cn


<!-- 参考信息 -->