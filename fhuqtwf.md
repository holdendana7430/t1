代发 wailian999

[Q80] 字符串截取
来源：http://rj.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bb.newstarts.cn

[Q81] 字符串替换
来源：http://ql.colortex.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gy.9csxet.cn

[Q82] 字符长度与字节长度
来源：http://uy.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cq.nicolike.cn

[Q83] 大小写转换
来源：http://bd.jianghongdianzi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ei.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://wa.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://jb.9csxet.cn

[Q85] 数值取整
来源：http://hr.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xc.9csxet.cn

[Q86] 读取 JSON 字段
来源：http://gp.panjiajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hg.huanxung.cn

[Q87] JSON 字段做条件
来源：http://ez.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mw.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://ce.521024.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tr.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aa.gzmigu.cn

[Q89] 判断表是否存在
来源：http://zv.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zr.muxihuayi.cn

[Q90] 生成序号列
来源：http://aq.huanxung.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ms.huixiangedu.cn

================================================================================
来源：http://jj.wgjwhj.cn

R. Bash 专题
来源：http://al.shtwfgs.cn

================================================================================
来源：http://qf.haigaiapp.cn

[R01] shebang 与严格模式
来源：http://mz.jctech888.com.cn

#!/usr/bin/env bash
来源：http://pj.shtwfgs.cn

set -euo pipefail
来源：http://ow.lnxyls.cn

[R02] 变量赋值与使用
来源：http://sj.yuntaijiaju.cn

name="Tom"; echo "$name"
来源：http://qr.bjjhwx.cn

[R03] 只读变量
来源：http://qi.shxzukj.cn

readonly PI=3.14
来源：http://ue.huixiangedu.cn

[R04] 位置参数
来源：http://dd.hnjuh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rd.panjiajie.cn

[R05] 参数默认值
来源：http://uf.newstarts.cn

name="${1:-default}"
来源：http://qu.szsharing.cn

[R06] 判断命令是否存在
来源：http://sz.shtwfgs.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gs.wgjwhj.cn

[R07] if 判断文件
来源：http://vy.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://we.bookmarksfly.cn

[R08] 数值比较
来源：http://mm.wgjwhj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xp.chemitech.net.cn

[R09] 字符串比较
来源：http://si.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ix.szxytkj.cn

[R10] 正则匹配
来源：http://ma.panjiajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cj.gzmigu.cn

[R11] case 多分支
来源：http://kg.9csxet.cn

case "$1" in
来源：http://sr.newstarts.cn

start) echo "启动" ;;
来源：http://bd.yuexingan06.cn

stop)  echo "停止" ;;
来源：http://lx.szsharing.cn

*)     echo "未知命令" ;;
来源：http://zi.szxytkj.cn

esac
来源：http://up.hahajie.cn

[R12] for 遍历文件
来源：http://an.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://wv.nszjky.cn

[R13] for 计数循环
来源：http://cp.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://dw.szxytkj.cn

[R14] C 风格 for
来源：http://er.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ta.bjjhwx.cn

[R15] while 逐行读文件
来源：http://nc.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rk.bookmarksfly.cn

[R16] until 等待条件
来源：http://yp.haigaiapp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://as.lnxyls.cn

[R17] 数组定义与取值
来源：http://hm.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rc.haigaiapp.cn

[R18] 遍历数组
来源：http://dr.colortex.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tk.gzmigu.cn

[R19] 数组长度
来源：http://hu.szsharing.cn

echo "${#arr[@]}"
来源：http://vb.521024.cn

[R20] 关联数组（字典）
来源：http://zo.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://px.jianghongdianzi.cn

[R21] 字符串长度
来源：http://da.szsharing.cn

echo "${#s}"
来源：http://ph.shxzukj.cn

[R22] 截取子串
来源：http://mp.lnxyls.cn

echo "${s:0:5}"
来源：http://xn.colortex.cn

[R23] 字符串替换
来源：http://yi.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bh.huanxung.cn

[R24] 大小写转换
来源：http://ff.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qp.szxytkj.cn

[R25] 去后缀 / 去前缀
来源：http://ke.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mw.newstarts.cn

[R26] 命令替换
来源：http://vv.szxytkj.cn

now=$(date +%F); echo "$now"
来源：http://wt.panjiajie.cn

[R27] 算术展开
来源：http://lo.gzmigu.cn

echo $((1 + 2 * 3))
来源：http://mm.lnxyls.cn

[R28] 浮点运算
来源：http://an.nszjky.cn

echo "scale=2; 10/3" | bc
来源：http://hj.shtwfgs.cn

[R29] 定义函数
来源：http://ug.haigaiapp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qk.huixiangedu.cn

[R30] 函数返回状态码
来源：http://aw.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://vv.asd995.cn

[R31] 局部变量
来源：http://pi.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://zb.521024.cn

[R32] 参数个数校验
来源：http://ma.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ci.bjjhwx.cn

[R33] 捕获错误并提示行号
来源：http://wx.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://io.szsharing.cn

[R34] 退出时清理
来源：http://cx.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yc.jctech888.com.cn

[R35] 后台执行并等待
来源：http://kz.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nl.huanxung.cn

[R36] 并发执行多个任务
来源：http://xz.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cj.huixinmuqiang.cn

[R37] 把输出赋给变量
来源：http://zb.bjjhwx.cn

files=$(ls -1)
来源：http://zq.hnjuh.cn

[R38] 管道串联
来源：http://qg.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://wo.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://hm.chemitech.net.cn

cmd > out.log 2>&1
来源：http://og.jianghongdianzi.cn

[R40] 追加写日志
来源：http://no.chemitech.net.cn

echo "log" >> out.log
来源：http://dx.bjjhwx.cn

[R41] 丢弃输出
来源：http://yg.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://pu.nicolike.cn

[R42] 输入重定向
来源：http://kv.huanxung.cn

wc -l < a.txt
来源：http://go.haigaiapp.cn

[R43] 按名字查找文件
来源：http://hj.hahajie.cn

find . -name "*.log" -type f
来源：http://ju.szxytkj.cn

[R44] 按修改时间查找
来源：http://uy.hnjuh.cn

find . -mtime -7 -type f
来源：http://mc.hnjuh.cn

[R45] 批量删除
来源：http://pa.szsharing.cn

find . -name "*.tmp" -delete
来源：http://ye.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://jn.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mp.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://ty.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xq.nicolike.cn

[R48] awk 取指定列
来源：http://qx.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://oi.yuntaijiaju.cn

[R49] awk 带条件
来源：http://vq.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qp.shxzukj.cn

[R50] awk 求和
来源：http://yb.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zx.shtwfgs.cn

[R51] 排序去重取前几
来源：http://ua.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.muxihuayi.cn

[R52] 统计行数
来源：http://rz.colortex.cn

wc -l a.txt
来源：http://fh.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://vs.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nv.colortex.cn

[R54] 比较两个文件
来源：http://wn.521024.cn

diff a.txt b.txt
来源：http://dv.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://xz.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wz.nicolike.cn

[R56] 远程拷贝
来源：http://ro.hahajie.cn

scp file user@host:/path/
来源：http://cq.wgjwhj.cn

[R57] 远程执行命令
来源：http://mo.shxzukj.cn

ssh user@host 'uptime'
来源：http://nb.huixiangedu.cn

[R58] 下载文件
来源：http://ci.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nn.nicolike.cn

[R59] 发 POST JSON
来源：http://jx.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zd.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://zk.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ug.colortex.cn

[R61] 磁盘占用
来源：http://lf.521024.cn

df -h;  du -sh *
来源：http://wn.nicolike.cn

[R62] 找最占空间的文件
来源：http://lc.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://tw.wgjwhj.cn

[R63] 内存与进程
来源：http://jm.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://mi.wgjwhj.cn

[R64] 结束进程
来源：http://vg.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://bk.nicolike.cn

[R65] 查看端口占用
来源：http://ee.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://os.huixinmuqiang.cn

[R66] 定时任务
来源：http://bn.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://nz.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://pq.colortex.cn

openssl rand -hex 16
来源：http://hh.yuntaijiaju.cn

[R68] 计算文件校验值
来源：http://zh.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jn.colortex.cn

[R69] 生成随机密码
来源：http://zy.huixinmuqiang.cn

head -c 16 /dev/urandom | base64
来源：http://gp.colortex.cn

[R70] 时间戳与互转
来源：http://cv.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://sc.asd995.cn

[R71] 日期格式化
来源：http://nw.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mh.9csxet.cn

[R72] 等待端口就绪
来源：http://bu.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kv.bjjhwx.cn

[R73] 分割大日志
来源：http://jd.wgjwhj.cn

split -l 1000 big.log part_
来源：http://oe.jctech888.com.cn

[R74] 批量重命名
来源：http://fr.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ip.hnjuh.cn

[R75] 导出环境变量
来源：http://ki.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://bp.bjjhwx.cn

[R76] 使用临时文件
来源：http://bo.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://aw.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://va.szxytkj.cn

read -rp "请输入: " ans
来源：http://ff.szxytkj.cn

[R78] 交互式菜单
来源：http://ha.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pr.chemitech.net.cn

[R79] 解析命令行选项
来源：http://ca.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nc.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://tq.gzmigu.cn

time ./run.sh
来源：http://da.nicolike.cn

================================================================================
来源：http://ej.hnjuh.cn

S. C / C++ 专题
来源：http://ic.nicolike.cn

================================================================================
来源：http://ca.hahajie.cn

[S01] C：Hello World
来源：http://hl.gzmigu.cn

#include <stdio.h>
来源：http://tl.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hc.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://dd.shxzukj.cn

int a = 10; printf("%d\n", a);
来源：http://us.muxihuayi.cn

[S03] C：读入整数
来源：http://je.shxzukj.cn

int x; scanf("%d", &x);
来源：http://os.lnxyls.cn

[S04] C：字符串复制
来源：http://aa.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ow.hnjuh.cn

[S05] C：字符串长度
来源：http://kp.haigaiapp.cn

strlen(s)
来源：http://pk.shtwfgs.cn

[S06] C：字符串比较
来源：http://wg.haigaiapp.cn

strcmp(a, b) == 0
来源：http://un.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://lu.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xd.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://zm.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ee.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://ij.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ka.szsharing.cn

[S10] C：指针与解引用
来源：http://rn.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://ne.haigaiapp.cn

[S11] C：逐行读文件
来源：http://pk.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://nq.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vl.9csxet.cn

fclose(f);
来源：http://rj.hnjuh.cn

[S12] C：写文件
来源：http://xh.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gm.jctech888.com.cn

[S13] C：宏定义
来源：http://qi.huanxung.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uo.szxytkj.cn

[S14] C：枚举
来源：http://zt.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://tq.shxzskj.cn

[S15] C：类型转换
来源：http://cn.bjjhwx.cn

(double) a / b
来源：http://tj.szsharing.cn

[S16] C：位操作置位
来源：http://lp.huixiangedu.cn

x |= (1 << 3);
来源：http://pu.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://no.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://su.muxihuayi.cn

[S18] C：命令行参数
来源：http://kw.shtwfgs.cn

int main(int argc, char **argv)
来源：http://wk.colortex.cn

[S19] C：快速排序
来源：http://cd.newstarts.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vk.huixinmuqiang.cn

[S20] C：二分查找
来源：http://wh.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ot.muxihuayi.cn

[S21] C：字符类别判断
来源：http://zr.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sm.szsharing.cn

[S22] C：字符串转数字
来源：http://ph.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tf.gzmigu.cn

[S23] C：随机数
来源：http://ox.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kp.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://nw.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ub.yuexingan06.cn

[S25] C：内存拷贝
来源：http://iu.bjjhwx.cn

memcpy(dst, src, n);
来源：http://su.521024.cn

[S26] C：内存清零
来源：http://mm.nicolike.cn

memset(a, 0, sizeof a);
来源：http://xz.muxihuayi.cn

[S27] C：定义常量
来源：http://pe.hahajie.cn

const double PI = 3.14159;
来源：http://fs.huixiangedu.cn

[S28] C：静态变量
来源：http://hf.bookmarksfly.cn

static int counter = 0;
来源：http://xf.szxytkj.cn

[S29] C：变参函数
来源：http://bv.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fj.hnjuh.cn

[S30] C：头文件保护
来源：http://ah.shxzskj.cn

#ifndef X_H
来源：http://pj.newstarts.cn

#define X_H
来源：http://fy.wgjwhj.cn

#endif
来源：http://tp.nicolike.cn

[S31] C++：Hello World
来源：http://cx.newstarts.cn

#include <iostream>
来源：http://jj.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://ux.huixiangedu.cn

[S32] C++：字符串
来源：http://hd.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://ef.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://ju.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ob.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://rt.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://oa.nszjky.cn

[S35] C++：map
来源：http://ak.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://au.colortex.cn

[S36] C++：unordered_map
来源：http://kg.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gk.jianghongdianzi.cn

[S37] C++：set
来源：http://fk.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tf.wgjwhj.cn

[S38] C++：排序
来源：http://jy.521024.cn

std::sort(v.begin(), v.end());
来源：http://th.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://ui.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nl.yuexingan06.cn

[S40] C++：查找元素
来源：http://vo.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xe.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://ga.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zp.huanxung.cn

[S42] C++：继承与虚函数
来源：http://gb.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://go.newstarts.cn

[S43] C++：智能指针
来源：http://mz.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://wu.shxzukj.cn

[S44] C++：引用传参
来源：http://rs.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://rq.chemitech.net.cn

[S45] C++：lambda
来源：http://tx.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mu.wgjwhj.cn

[S46] C++：函数模板
来源：http://vp.yuntaijiaju.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://no.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://ma.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cv.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://zg.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cu.nszjky.cn

while (std::getline(in, line)) { }
来源：http://ll.newstarts.cn

[S49] C++：写文件
来源：http://cz.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zc.gzmigu.cn

[S50] C++：格式化数字
来源：http://tz.jianghongdianzi.cn


<!-- 参考信息 -->