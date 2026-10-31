代发 wailian999

[Q84] 去除首尾空格
来源：http://wj.521024.cn

SELECT TRIM(name) FROM users;
来源：http://bi.lnxyls.cn

[Q85] 数值取整
来源：http://it.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ri.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://yy.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sd.chemitech.net.cn

[Q87] JSON 字段做条件
来源：http://ab.panjiajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xt.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://ge.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xf.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xg.newstarts.cn

[Q89] 判断表是否存在
来源：http://wd.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cu.huanxung.cn

[Q90] 生成序号列
来源：http://gu.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://az.lnxyls.cn

================================================================================
来源：http://wx.hahajie.cn

R. Bash 专题
来源：http://bs.shxzukj.cn

================================================================================
来源：http://dw.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://ho.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://wp.haigaiapp.cn

set -euo pipefail
来源：http://le.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://ag.shxzukj.cn

name="Tom"; echo "$name"
来源：http://qy.jianghongdianzi.cn

[R03] 只读变量
来源：http://fo.shxzukj.cn

readonly PI=3.14
来源：http://lw.huanxung.cn

[R04] 位置参数
来源：http://te.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qa.nszjky.cn

[R05] 参数默认值
来源：http://qt.szxytkj.cn

name="${1:-default}"
来源：http://bb.hahajie.cn

[R06] 判断命令是否存在
来源：http://bf.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zi.shxzukj.cn

[R07] if 判断文件
来源：http://vk.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eh.nszjky.cn

[R08] 数值比较
来源：http://ve.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kh.bjjhwx.cn

[R09] 字符串比较
来源：http://ii.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://va.muxihuayi.cn

[R10] 正则匹配
来源：http://ct.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://eb.521024.cn

[R11] case 多分支
来源：http://as.chemitech.net.cn

case "$1" in
来源：http://cp.huanxung.cn

start) echo "启动" ;;
来源：http://fz.huanxung.cn

stop)  echo "停止" ;;
来源：http://ct.asd995.cn

*)     echo "未知命令" ;;
来源：http://yc.521024.cn

esac
来源：http://vr.colortex.cn

[R12] for 遍历文件
来源：http://rp.newstarts.cn

for f in *.txt; do echo "$f"; done
来源：http://ld.shtwfgs.cn

[R13] for 计数循环
来源：http://bb.huanxung.cn

for i in {1..10}; do echo "$i"; done
来源：http://qc.yuntaijiaju.cn

[R14] C 风格 for
来源：http://vv.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lm.shxzskj.cn

[R15] while 逐行读文件
来源：http://zd.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yx.shxzukj.cn

[R16] until 等待条件
来源：http://ek.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lx.521024.cn

[R17] 数组定义与取值
来源：http://ta.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mc.521024.cn

[R18] 遍历数组
来源：http://ie.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cr.lnxyls.cn

[R19] 数组长度
来源：http://qy.shxzskj.cn

echo "${#arr[@]}"
来源：http://gd.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://yy.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tt.newstarts.cn

[R21] 字符串长度
来源：http://xr.nicolike.cn

echo "${#s}"
来源：http://la.newstarts.cn

[R22] 截取子串
来源：http://hd.muxihuayi.cn

echo "${s:0:5}"
来源：http://pp.newstarts.cn

[R23] 字符串替换
来源：http://mo.chemitech.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gn.lnxyls.cn

[R24] 大小写转换
来源：http://ey.nszjky.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xp.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://zb.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://so.hnjuh.cn

[R26] 命令替换
来源：http://bd.huixiangedu.cn

now=$(date +%F); echo "$now"
来源：http://xb.haigaiapp.cn

[R27] 算术展开
来源：http://hr.nicolike.cn

echo $((1 + 2 * 3))
来源：http://uc.bjjhwx.cn

[R28] 浮点运算
来源：http://fb.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://kb.nicolike.cn

[R29] 定义函数
来源：http://cg.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://re.hahajie.cn

[R30] 函数返回状态码
来源：http://mh.lnxyls.cn

f() { return 0; }; f || echo "失败了"
来源：http://wq.huixinmuqiang.cn

[R31] 局部变量
来源：http://bn.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://ei.szsharing.cn

[R32] 参数个数校验
来源：http://fx.yuexingan06.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yd.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://gq.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ci.bookmarksfly.cn

[R34] 退出时清理
来源：http://nw.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shxzskj.cn

[R35] 后台执行并等待
来源：http://bw.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yu.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://yv.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cf.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://qo.hahajie.cn

files=$(ls -1)
来源：http://rj.hahajie.cn

[R38] 管道串联
来源：http://ir.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://qx.shtwfgs.cn

[R39] 重定向标准输出与错误
来源：http://um.szsharing.cn

cmd > out.log 2>&1
来源：http://uh.muxihuayi.cn

[R40] 追加写日志
来源：http://cz.szxytkj.cn

echo "log" >> out.log
来源：http://av.bookmarksfly.cn

[R41] 丢弃输出
来源：http://nh.shtwfgs.cn

cmd >/dev/null 2>&1
来源：http://iy.hnjuh.cn

[R42] 输入重定向
来源：http://zz.wgjwhj.cn

wc -l < a.txt
来源：http://fg.chemitech.net.cn

[R43] 按名字查找文件
来源：http://gk.lnxyls.cn

find . -name "*.log" -type f
来源：http://hh.panjiajie.cn

[R44] 按修改时间查找
来源：http://lz.muxihuayi.cn

find . -mtime -7 -type f
来源：http://df.panjiajie.cn

[R45] 批量删除
来源：http://vt.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://ox.huixiangedu.cn

[R46] 递归替换文件内容
来源：http://in.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pb.huixiangedu.cn

[R47] sed 单行替换
来源：http://sp.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ga.hnjuh.cn

[R48] awk 取指定列
来源：http://zx.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://pj.asd995.cn

[R49] awk 带条件
来源：http://sx.lnxyls.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kh.yuexingan06.cn

[R50] awk 求和
来源：http://xb.bookmarksfly.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yb.huanxung.cn

[R51] 排序去重取前几
来源：http://yh.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nm.huixinmuqiang.cn

[R52] 统计行数
来源：http://st.lnxyls.cn

wc -l a.txt
来源：http://yj.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://wj.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://up.colortex.cn

[R54] 比较两个文件
来源：http://gw.bjjhwx.cn

diff a.txt b.txt
来源：http://rk.jctech888.com.cn

[R55] 压缩与解压
来源：http://rr.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ho.muxihuayi.cn

[R56] 远程拷贝
来源：http://qv.haigaiapp.cn

scp file user@host:/path/
来源：http://mm.szsharing.cn

[R57] 远程执行命令
来源：http://hx.wgjwhj.cn

ssh user@host 'uptime'
来源：http://ls.haigaiapp.cn

[R58] 下载文件
来源：http://vi.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nc.szsharing.cn

[R59] 发 POST JSON
来源：http://zy.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sx.wgjwhj.cn

[R60] 只看 HTTP 状态码
来源：http://tp.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fa.hnjuh.cn

[R61] 磁盘占用
来源：http://ac.huanxung.cn

df -h;  du -sh *
来源：http://yj.huanxung.cn

[R62] 找最占空间的文件
来源：http://ts.jctech888.com.cn

du -ah . | sort -rh | head -10
来源：http://ed.shtwfgs.cn

[R63] 内存与进程
来源：http://un.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://vp.shtwfgs.cn

[R64] 结束进程
来源：http://ue.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://mr.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://tg.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rg.9csxet.cn

[R66] 定时任务
来源：http://ji.jctech888.com.cn

crontab -e;  crontab -l
来源：http://zc.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://wo.lnxyls.cn

openssl rand -hex 16
来源：http://lc.521024.cn

[R68] 计算文件校验值
来源：http://vd.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://oa.shxzskj.cn

[R69] 生成随机密码
来源：http://an.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://xu.szsharing.cn

[R70] 时间戳与互转
来源：http://vf.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://ac.szxytkj.cn

[R71] 日期格式化
来源：http://dy.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rc.chemitech.net.cn

[R72] 等待端口就绪
来源：http://wb.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qc.shxzskj.cn

[R73] 分割大日志
来源：http://ih.bjjhwx.cn

split -l 1000 big.log part_
来源：http://tg.bjjhwx.cn

[R74] 批量重命名
来源：http://zh.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dy.jctech888.com.cn

[R75] 导出环境变量
来源：http://vi.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://yd.newstarts.cn

[R76] 使用临时文件
来源：http://dt.szxytkj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qv.newstarts.cn

[R77] 读取用户输入
来源：http://ph.colortex.cn

read -rp "请输入: " ans
来源：http://dd.lnxyls.cn

[R78] 交互式菜单
来源：http://lr.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gl.huanxung.cn

[R79] 解析命令行选项
来源：http://os.9csxet.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zs.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://os.jianghongdianzi.cn

time ./run.sh
来源：http://jv.huixinmuqiang.cn

================================================================================
来源：http://yq.wgjwhj.cn

S. C / C++ 专题
来源：http://qs.shxzukj.cn

================================================================================
来源：http://ai.jctech888.com.cn

[S01] C：Hello World
来源：http://zz.nszjky.cn

#include <stdio.h>
来源：http://fn.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://eu.nicolike.cn

[S02] C：变量与格式化输出
来源：http://tv.gzmigu.cn

int a = 10; printf("%d\n", a);
来源：http://eq.huixinmuqiang.cn

[S03] C：读入整数
来源：http://jz.shxzskj.cn

int x; scanf("%d", &x);
来源：http://jl.szxytkj.cn

[S04] C：字符串复制
来源：http://pr.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cc.shxzukj.cn

[S05] C：字符串长度
来源：http://rl.bookmarksfly.cn

strlen(s)
来源：http://mo.jctech888.com.cn

[S06] C：字符串比较
来源：http://bx.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://oq.szsharing.cn

[S07] C：数组遍历求和
来源：http://ns.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jl.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://xr.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fd.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://ri.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xa.gzmigu.cn

[S10] C：指针与解引用
来源：http://ol.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://pp.shtwfgs.cn

[S11] C：逐行读文件
来源：http://uu.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://ce.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fj.huixinmuqiang.cn

fclose(f);
来源：http://bs.huanxung.cn

[S12] C：写文件
来源：http://ob.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fu.asd995.cn

[S13] C：宏定义
来源：http://ec.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hi.asd995.cn

[S14] C：枚举
来源：http://ek.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://yy.jianghongdianzi.cn

[S15] C：类型转换
来源：http://km.newstarts.cn

(double) a / b
来源：http://iy.lnxyls.cn

[S16] C：位操作置位
来源：http://ex.jctech888.com.cn

x |= (1 << 3);
来源：http://qv.lnxyls.cn

[S17] C：安全拼接字符串
来源：http://pz.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zm.muxihuayi.cn

[S18] C：命令行参数
来源：http://ft.9csxet.cn

int main(int argc, char **argv)
来源：http://rk.colortex.cn

[S19] C：快速排序
来源：http://vw.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fj.colortex.cn

[S20] C：二分查找
来源：http://wu.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://db.muxihuayi.cn

[S21] C：字符类别判断
来源：http://dz.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yf.shxzukj.cn

[S22] C：字符串转数字
来源：http://qw.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://op.yuntaijiaju.cn

[S23] C：随机数
来源：http://vo.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qq.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://ez.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://my.shxzskj.cn

[S25] C：内存拷贝
来源：http://eq.asd995.cn

memcpy(dst, src, n);
来源：http://pn.yuntaijiaju.cn

[S26] C：内存清零
来源：http://xg.521024.cn

memset(a, 0, sizeof a);
来源：http://na.szsharing.cn

[S27] C：定义常量
来源：http://pp.muxihuayi.cn

const double PI = 3.14159;
来源：http://zt.newstarts.cn

[S28] C：静态变量
来源：http://tg.muxihuayi.cn

static int counter = 0;
来源：http://qp.nicolike.cn

[S29] C：变参函数
来源：http://jy.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yp.huixiangedu.cn

[S30] C：头文件保护
来源：http://bu.yuexingan06.cn

#ifndef X_H
来源：http://tn.nszjky.cn

#define X_H
来源：http://rt.bookmarksfly.cn

#endif
来源：http://xz.huixiangedu.cn

[S31] C++：Hello World
来源：http://yy.hahajie.cn

#include <iostream>
来源：http://gl.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://su.huixiangedu.cn

[S32] C++：字符串
来源：http://fx.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://vu.jctech888.com.cn

[S33] C++：vector 增删
来源：http://wn.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uj.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://am.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://qv.lnxyls.cn

[S35] C++：map
来源：http://pv.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bu.szsharing.cn

[S36] C++：unordered_map
来源：http://tm.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xg.panjiajie.cn

[S37] C++：set
来源：http://ws.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wy.9csxet.cn

[S38] C++：排序
来源：http://yy.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://rq.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://tj.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ji.newstarts.cn

[S40] C++：查找元素
来源：http://fc.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vn.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://bn.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vk.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://ie.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://io.szxytkj.cn

[S43] C++：智能指针
来源：http://uc.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://by.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://tp.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://nl.szsharing.cn

[S45] C++：lambda
来源：http://jn.szxytkj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ri.muxihuayi.cn

[S46] C++：函数模板
来源：http://mb.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xa.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://vb.huanxung.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://br.gzmigu.cn

[S48] C++：逐行读文件
来源：http://rb.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rc.hahajie.cn

while (std::getline(in, line)) { }
来源：http://mo.szsharing.cn

[S49] C++：写文件
来源：http://lt.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sn.szxytkj.cn

[S50] C++：格式化数字
来源：http://lc.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://en.bookmarksfly.cn

[S51] C++：显式类型转换
来源：http://fm.bjjhwx.cn

static_cast<double>(a) / b
来源：http://vi.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://sn.huanxung.cn

int size() const noexcept { return n_; }
来源：http://vi.jctech888.com.cn

[S53] C++：移动语义
来源：http://cd.colortex.cn

std::vector<int> w = std::move(v);
来源：http://qx.bookmarksfly.cn

[S54] C++：异常处理
来源：http://hp.nicolike.cn


<!-- 参考信息 -->