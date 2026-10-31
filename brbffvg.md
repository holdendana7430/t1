代发 wailian999

[Q84] 去除首尾空格
来源：http://mb.9csxet.cn

SELECT TRIM(name) FROM users;
来源：http://li.szxytkj.cn

[Q85] 数值取整
来源：http://vk.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pp.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://ml.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zq.521024.cn

[Q87] JSON 字段做条件
来源：http://il.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nm.nicolike.cn

[Q88] 行转列（条件聚合）
来源：http://cc.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://er.wgjwhj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hc.muxihuayi.cn

[Q89] 判断表是否存在
来源：http://gt.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eg.gzmigu.cn

[Q90] 生成序号列
来源：http://wj.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ec.szxytkj.cn

================================================================================
来源：http://ij.muxihuayi.cn

R. Bash 专题
来源：http://aa.hahajie.cn

================================================================================
来源：http://ij.szxytkj.cn

[R01] shebang 与严格模式
来源：http://ws.9csxet.cn

#!/usr/bin/env bash
来源：http://up.521024.cn

set -euo pipefail
来源：http://np.colortex.cn

[R02] 变量赋值与使用
来源：http://dq.newstarts.cn

name="Tom"; echo "$name"
来源：http://qr.huixiangedu.cn

[R03] 只读变量
来源：http://us.shxzskj.cn

readonly PI=3.14
来源：http://ai.gzmigu.cn

[R04] 位置参数
来源：http://os.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kg.nicolike.cn

[R05] 参数默认值
来源：http://li.huanxung.cn

name="${1:-default}"
来源：http://fx.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://jc.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jp.gzmigu.cn

[R07] if 判断文件
来源：http://kp.9csxet.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tc.shxzukj.cn

[R08] 数值比较
来源：http://jb.jianghongdianzi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ov.huixinmuqiang.cn

[R09] 字符串比较
来源：http://pq.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cd.yuntaijiaju.cn

[R10] 正则匹配
来源：http://tj.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kf.colortex.cn

[R11] case 多分支
来源：http://gp.gzmigu.cn

case "$1" in
来源：http://og.muxihuayi.cn

start) echo "启动" ;;
来源：http://gk.lnxyls.cn

stop)  echo "停止" ;;
来源：http://pg.asd995.cn

*)     echo "未知命令" ;;
来源：http://fr.bookmarksfly.cn

esac
来源：http://ms.hnjuh.cn

[R12] for 遍历文件
来源：http://gu.colortex.cn

for f in *.txt; do echo "$f"; done
来源：http://bk.lnxyls.cn

[R13] for 计数循环
来源：http://hn.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://vv.newstarts.cn

[R14] C 风格 for
来源：http://jq.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zf.bjjhwx.cn

[R15] while 逐行读文件
来源：http://pm.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://au.asd995.cn

[R16] until 等待条件
来源：http://xo.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jp.nszjky.cn

[R17] 数组定义与取值
来源：http://ku.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ud.gzmigu.cn

[R18] 遍历数组
来源：http://zy.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wy.shxzukj.cn

[R19] 数组长度
来源：http://ik.hnjuh.cn

echo "${#arr[@]}"
来源：http://ri.hnjuh.cn

[R20] 关联数组（字典）
来源：http://bc.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pi.muxihuayi.cn

[R21] 字符串长度
来源：http://ks.muxihuayi.cn

echo "${#s}"
来源：http://nb.521024.cn

[R22] 截取子串
来源：http://vr.gzmigu.cn

echo "${s:0:5}"
来源：http://lz.hahajie.cn

[R23] 字符串替换
来源：http://zh.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tz.szsharing.cn

[R24] 大小写转换
来源：http://pa.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fe.bjjhwx.cn

[R25] 去后缀 / 去前缀
来源：http://bj.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lh.huanxung.cn

[R26] 命令替换
来源：http://li.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://dm.yuexingan06.cn

[R27] 算术展开
来源：http://au.huixinmuqiang.cn

echo $((1 + 2 * 3))
来源：http://vx.haigaiapp.cn

[R28] 浮点运算
来源：http://ew.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://xa.haigaiapp.cn

[R29] 定义函数
来源：http://gk.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rx.colortex.cn

[R30] 函数返回状态码
来源：http://ud.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://jv.jianghongdianzi.cn

[R31] 局部变量
来源：http://ka.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://du.9csxet.cn

[R32] 参数个数校验
来源：http://mo.shtwfgs.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lw.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://rb.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tq.lnxyls.cn

[R34] 退出时清理
来源：http://cr.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mo.szxytkj.cn

[R35] 后台执行并等待
来源：http://ac.szxytkj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ri.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://cj.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ft.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://np.yuntaijiaju.cn

files=$(ls -1)
来源：http://yh.haigaiapp.cn

[R38] 管道串联
来源：http://dr.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://rh.bookmarksfly.cn

[R39] 重定向标准输出与错误
来源：http://dd.521024.cn

cmd > out.log 2>&1
来源：http://gb.9csxet.cn

[R40] 追加写日志
来源：http://rf.huixiangedu.cn

echo "log" >> out.log
来源：http://sl.hahajie.cn

[R41] 丢弃输出
来源：http://pi.colortex.cn

cmd >/dev/null 2>&1
来源：http://vw.bjjhwx.cn

[R42] 输入重定向
来源：http://kj.panjiajie.cn

wc -l < a.txt
来源：http://jf.shxzukj.cn

[R43] 按名字查找文件
来源：http://ws.muxihuayi.cn

find . -name "*.log" -type f
来源：http://ps.huanxung.cn

[R44] 按修改时间查找
来源：http://oz.chemitech.net.cn

find . -mtime -7 -type f
来源：http://nr.jctech888.com.cn

[R45] 批量删除
来源：http://nm.9csxet.cn

find . -name "*.tmp" -delete
来源：http://od.colortex.cn

[R46] 递归替换文件内容
来源：http://av.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ik.hahajie.cn

[R47] sed 单行替换
来源：http://nj.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oi.shxzukj.cn

[R48] awk 取指定列
来源：http://ad.huixiangedu.cn

awk '{print $1, $3}' a.txt
来源：http://dw.newstarts.cn

[R49] awk 带条件
来源：http://pb.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ew.bjjhwx.cn

[R50] awk 求和
来源：http://ah.shxzskj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hx.szsharing.cn

[R51] 排序去重取前几
来源：http://ew.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ws.9csxet.cn

[R52] 统计行数
来源：http://ix.9csxet.cn

wc -l a.txt
来源：http://uh.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://xi.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nv.shxzskj.cn

[R54] 比较两个文件
来源：http://oz.9csxet.cn

diff a.txt b.txt
来源：http://wt.colortex.cn

[R55] 压缩与解压
来源：http://zv.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shtwfgs.cn

[R56] 远程拷贝
来源：http://ex.yuntaijiaju.cn

scp file user@host:/path/
来源：http://wx.lnxyls.cn

[R57] 远程执行命令
来源：http://ci.haigaiapp.cn

ssh user@host 'uptime'
来源：http://am.yuntaijiaju.cn

[R58] 下载文件
来源：http://hu.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iu.colortex.cn

[R59] 发 POST JSON
来源：http://ys.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gh.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://dp.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mb.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://ze.chemitech.net.cn

df -h;  du -sh *
来源：http://pl.lnxyls.cn

[R62] 找最占空间的文件
来源：http://fd.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://zg.newstarts.cn

[R63] 内存与进程
来源：http://dd.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://pg.muxihuayi.cn

[R64] 结束进程
来源：http://qb.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://re.nszjky.cn

[R65] 查看端口占用
来源：http://yi.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zm.yuexingan06.cn

[R66] 定时任务
来源：http://rq.bjjhwx.cn

crontab -e;  crontab -l
来源：http://qp.521024.cn

[R67] 生成随机十六进制串
来源：http://gp.gzmigu.cn

openssl rand -hex 16
来源：http://ma.szsharing.cn

[R68] 计算文件校验值
来源：http://vj.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xq.panjiajie.cn

[R69] 生成随机密码
来源：http://mq.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://jl.haigaiapp.cn

[R70] 时间戳与互转
来源：http://fa.nicolike.cn

date +%s;  date -d @1700000000
来源：http://if.9csxet.cn

[R71] 日期格式化
来源：http://rz.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zf.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://dg.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zi.huanxung.cn

[R73] 分割大日志
来源：http://xk.szsharing.cn

split -l 1000 big.log part_
来源：http://yv.shtwfgs.cn

[R74] 批量重命名
来源：http://io.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://co.asd995.cn

[R75] 导出环境变量
来源：http://lv.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://xa.bookmarksfly.cn

[R76] 使用临时文件
来源：http://yk.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rj.shxzskj.cn

[R77] 读取用户输入
来源：http://ka.hahajie.cn

read -rp "请输入: " ans
来源：http://hh.521024.cn

[R78] 交互式菜单
来源：http://cy.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ui.haigaiapp.cn

[R79] 解析命令行选项
来源：http://ao.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hm.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://zu.wgjwhj.cn

time ./run.sh
来源：http://oe.521024.cn

================================================================================
来源：http://yb.hahajie.cn

S. C / C++ 专题
来源：http://ed.chemitech.net.cn

================================================================================
来源：http://xf.yuexingan06.cn

[S01] C：Hello World
来源：http://ra.huanxung.cn

#include <stdio.h>
来源：http://lq.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xm.nicolike.cn

[S02] C：变量与格式化输出
来源：http://os.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://ih.lnxyls.cn

[S03] C：读入整数
来源：http://lm.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://rf.hahajie.cn

[S04] C：字符串复制
来源：http://iq.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lt.huixiangedu.cn

[S05] C：字符串长度
来源：http://nb.shxzukj.cn

strlen(s)
来源：http://ij.nszjky.cn

[S06] C：字符串比较
来源：http://em.lnxyls.cn

strcmp(a, b) == 0
来源：http://bi.lnxyls.cn

[S07] C：数组遍历求和
来源：http://go.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gm.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://vt.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://am.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://se.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hnjuh.cn

[S10] C：指针与解引用
来源：http://kj.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://su.nicolike.cn

[S11] C：逐行读文件
来源：http://oy.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://rn.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://em.chemitech.net.cn

fclose(f);
来源：http://un.hnjuh.cn

[S12] C：写文件
来源：http://ir.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fh.asd995.cn

[S13] C：宏定义
来源：http://oh.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hv.shxzukj.cn

[S14] C：枚举
来源：http://yd.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://ue.jctech888.com.cn

[S15] C：类型转换
来源：http://gu.gzmigu.cn

(double) a / b
来源：http://uc.colortex.cn

[S16] C：位操作置位
来源：http://mj.haigaiapp.cn

x |= (1 << 3);
来源：http://bd.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://pj.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yb.huixiangedu.cn

[S18] C：命令行参数
来源：http://yi.hahajie.cn

int main(int argc, char **argv)
来源：http://vh.shxzskj.cn

[S19] C：快速排序
来源：http://ug.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zz.jctech888.com.cn

[S20] C：二分查找
来源：http://hq.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ir.shxzskj.cn

[S21] C：字符类别判断
来源：http://mq.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yz.asd995.cn

[S22] C：字符串转数字
来源：http://ak.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sw.colortex.cn

[S23] C：随机数
来源：http://rk.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yv.huanxung.cn

[S24] C：获取本地时间
来源：http://qc.521024.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://in.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://pd.szsharing.cn

memcpy(dst, src, n);
来源：http://ro.jianghongdianzi.cn

[S26] C：内存清零
来源：http://gd.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://ck.521024.cn

[S27] C：定义常量
来源：http://ub.wgjwhj.cn

const double PI = 3.14159;
来源：http://dy.gzmigu.cn

[S28] C：静态变量
来源：http://tz.jianghongdianzi.cn

static int counter = 0;
来源：http://hc.yuntaijiaju.cn

[S29] C：变参函数
来源：http://ak.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iv.newstarts.cn

[S30] C：头文件保护
来源：http://di.jianghongdianzi.cn

#ifndef X_H
来源：http://mh.yuexingan06.cn

#define X_H
来源：http://be.shxzukj.cn

#endif
来源：http://nq.9csxet.cn

[S31] C++：Hello World
来源：http://yg.asd995.cn

#include <iostream>
来源：http://op.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://of.szxytkj.cn

[S32] C++：字符串
来源：http://cu.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://mn.shxzskj.cn

[S33] C++：vector 增删
来源：http://yb.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dq.hnjuh.cn

[S34] C++：遍历 vector
来源：http://hi.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://lw.bookmarksfly.cn

[S35] C++：map
来源：http://lo.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qd.9csxet.cn

[S36] C++：unordered_map
来源：http://eg.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zi.lnxyls.cn

[S37] C++：set
来源：http://bo.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://to.asd995.cn

[S38] C++：排序
来源：http://ez.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://rc.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://gj.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ch.muxihuayi.cn

[S40] C++：查找元素
来源：http://ku.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ev.szsharing.cn

[S41] C++：类与构造函数
来源：http://ba.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vw.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://ai.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://qg.jctech888.com.cn

[S43] C++：智能指针
来源：http://ap.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://qg.521024.cn

[S44] C++：引用传参
来源：http://nv.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://gu.chemitech.net.cn

[S45] C++：lambda
来源：http://en.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://os.huanxung.cn

[S46] C++：函数模板
来源：http://kh.shxzukj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://if.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://eh.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rx.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://ug.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jw.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://es.hahajie.cn

[S49] C++：写文件
来源：http://oz.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mv.chemitech.net.cn

[S50] C++：格式化数字
来源：http://rb.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://um.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://he.newstarts.cn

static_cast<double>(a) / b
来源：http://xb.colortex.cn

[S52] C++：const 与 noexcept
来源：http://of.nicolike.cn

int size() const noexcept { return n_; }
来源：http://wp.9csxet.cn

[S53] C++：移动语义
来源：http://wf.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://qp.huixiangedu.cn

[S54] C++：异常处理
来源：http://gm.huanxung.cn


<!-- 参考信息 -->