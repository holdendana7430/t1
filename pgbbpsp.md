代发 wailian999

[Q78] 当前时间
来源：http://jj.szxytkj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://eb.wgjwhj.cn

[Q79] 字符串拼接
来源：http://cq.colortex.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bk.muxihuayi.cn

[Q80] 字符串截取
来源：http://kh.521024.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ke.shxzukj.cn

[Q81] 字符串替换
来源：http://xd.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nm.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://cw.bookmarksfly.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rp.nszjky.cn

[Q83] 大小写转换
来源：http://np.asd995.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ld.asd995.cn

[Q84] 去除首尾空格
来源：http://co.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://et.shtwfgs.cn

[Q85] 数值取整
来源：http://em.521024.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://je.newstarts.cn

[Q86] 读取 JSON 字段
来源：http://el.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oc.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://le.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eo.bookmarksfly.cn

[Q88] 行转列（条件聚合）
来源：http://eq.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wp.wgjwhj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gk.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://vm.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zi.bjjhwx.cn

[Q90] 生成序号列
来源：http://xs.chemitech.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ld.jianghongdianzi.cn

================================================================================
来源：http://bk.lnxyls.cn

R. Bash 专题
来源：http://pu.colortex.cn

================================================================================
来源：http://bi.asd995.cn

[R01] shebang 与严格模式
来源：http://wx.newstarts.cn

#!/usr/bin/env bash
来源：http://kb.jianghongdianzi.cn

set -euo pipefail
来源：http://gq.newstarts.cn

[R02] 变量赋值与使用
来源：http://wh.yuntaijiaju.cn

name="Tom"; echo "$name"
来源：http://gv.9csxet.cn

[R03] 只读变量
来源：http://aa.asd995.cn

readonly PI=3.14
来源：http://na.hnjuh.cn

[R04] 位置参数
来源：http://tc.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ut.huanxung.cn

[R05] 参数默认值
来源：http://xc.newstarts.cn

name="${1:-default}"
来源：http://po.shxzskj.cn

[R06] 判断命令是否存在
来源：http://yw.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lm.huanxung.cn

[R07] if 判断文件
来源：http://ez.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zn.szxytkj.cn

[R08] 数值比较
来源：http://qf.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pd.521024.cn

[R09] 字符串比较
来源：http://oy.shtwfgs.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pn.panjiajie.cn

[R10] 正则匹配
来源：http://uj.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pg.yuntaijiaju.cn

[R11] case 多分支
来源：http://ja.gzmigu.cn

case "$1" in
来源：http://rd.huixinmuqiang.cn

start) echo "启动" ;;
来源：http://zi.bookmarksfly.cn

stop)  echo "停止" ;;
来源：http://fp.shtwfgs.cn

*)     echo "未知命令" ;;
来源：http://qk.jctech888.com.cn

esac
来源：http://oj.muxihuayi.cn

[R12] for 遍历文件
来源：http://xp.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://ux.gzmigu.cn

[R13] for 计数循环
来源：http://lu.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://ln.newstarts.cn

[R14] C 风格 for
来源：http://ze.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kp.bjjhwx.cn

[R15] while 逐行读文件
来源：http://xw.shtwfgs.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tu.muxihuayi.cn

[R16] until 等待条件
来源：http://nx.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xn.haigaiapp.cn

[R17] 数组定义与取值
来源：http://jj.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ay.muxihuayi.cn

[R18] 遍历数组
来源：http://hb.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ti.shtwfgs.cn

[R19] 数组长度
来源：http://lm.shxzukj.cn

echo "${#arr[@]}"
来源：http://fd.9csxet.cn

[R20] 关联数组（字典）
来源：http://sv.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zv.wgjwhj.cn

[R21] 字符串长度
来源：http://in.shxzukj.cn

echo "${#s}"
来源：http://do.9csxet.cn

[R22] 截取子串
来源：http://th.panjiajie.cn

echo "${s:0:5}"
来源：http://ie.huixiangedu.cn

[R23] 字符串替换
来源：http://fj.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kk.yuntaijiaju.cn

[R24] 大小写转换
来源：http://xd.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gx.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://ii.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ep.521024.cn

[R26] 命令替换
来源：http://yi.colortex.cn

now=$(date +%F); echo "$now"
来源：http://iw.bjjhwx.cn

[R27] 算术展开
来源：http://sz.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://kh.9csxet.cn

[R28] 浮点运算
来源：http://kp.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://ue.bookmarksfly.cn

[R29] 定义函数
来源：http://pb.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tn.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://wx.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://nl.521024.cn

[R31] 局部变量
来源：http://zk.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://rw.hnjuh.cn

[R32] 参数个数校验
来源：http://ud.huixinmuqiang.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ef.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://zw.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ky.jctech888.com.cn

[R34] 退出时清理
来源：http://zh.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pe.hahajie.cn

[R35] 后台执行并等待
来源：http://rf.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cj.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://tj.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pg.szxytkj.cn

[R37] 把输出赋给变量
来源：http://ez.huixiangedu.cn

files=$(ls -1)
来源：http://cy.wgjwhj.cn

[R38] 管道串联
来源：http://kq.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://dh.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://dc.shtwfgs.cn

cmd > out.log 2>&1
来源：http://tq.hahajie.cn

[R40] 追加写日志
来源：http://vu.huixinmuqiang.cn

echo "log" >> out.log
来源：http://xd.colortex.cn

[R41] 丢弃输出
来源：http://cx.huanxung.cn

cmd >/dev/null 2>&1
来源：http://ep.gzmigu.cn

[R42] 输入重定向
来源：http://sr.nszjky.cn

wc -l < a.txt
来源：http://ap.521024.cn

[R43] 按名字查找文件
来源：http://jo.jctech888.com.cn

find . -name "*.log" -type f
来源：http://uv.wgjwhj.cn

[R44] 按修改时间查找
来源：http://ae.hnjuh.cn

find . -mtime -7 -type f
来源：http://wp.521024.cn

[R45] 批量删除
来源：http://in.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://ez.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://ab.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vu.szsharing.cn

[R47] sed 单行替换
来源：http://ua.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gg.haigaiapp.cn

[R48] awk 取指定列
来源：http://pu.521024.cn

awk '{print $1, $3}' a.txt
来源：http://oc.colortex.cn

[R49] awk 带条件
来源：http://bc.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ui.hahajie.cn

[R50] awk 求和
来源：http://yj.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://py.shtwfgs.cn

[R51] 排序去重取前几
来源：http://pg.gzmigu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oj.muxihuayi.cn

[R52] 统计行数
来源：http://zz.chemitech.net.cn

wc -l a.txt
来源：http://bx.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://hd.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ry.bookmarksfly.cn

[R54] 比较两个文件
来源：http://gp.bookmarksfly.cn

diff a.txt b.txt
来源：http://tk.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://qt.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xn.nszjky.cn

[R56] 远程拷贝
来源：http://zz.yuexingan06.cn

scp file user@host:/path/
来源：http://ki.newstarts.cn

[R57] 远程执行命令
来源：http://nt.bookmarksfly.cn

ssh user@host 'uptime'
来源：http://vr.colortex.cn

[R58] 下载文件
来源：http://fx.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yy.huixiangedu.cn

[R59] 发 POST JSON
来源：http://wq.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ad.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://wc.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mc.huixiangedu.cn

[R61] 磁盘占用
来源：http://ff.huixiangedu.cn

df -h;  du -sh *
来源：http://ai.shxzukj.cn

[R62] 找最占空间的文件
来源：http://by.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://bc.9csxet.cn

[R63] 内存与进程
来源：http://sx.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://zz.newstarts.cn

[R64] 结束进程
来源：http://jn.chemitech.net.cn

kill -9 $(pgrep -f app.py)
来源：http://iv.nicolike.cn

[R65] 查看端口占用
来源：http://uq.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cq.huanxung.cn

[R66] 定时任务
来源：http://zw.haigaiapp.cn

crontab -e;  crontab -l
来源：http://fx.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://la.huixinmuqiang.cn

openssl rand -hex 16
来源：http://wz.lnxyls.cn

[R68] 计算文件校验值
来源：http://vg.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hw.shxzukj.cn

[R69] 生成随机密码
来源：http://zw.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://sj.521024.cn

[R70] 时间戳与互转
来源：http://fq.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://tx.szxytkj.cn

[R71] 日期格式化
来源：http://wd.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sf.huixiangedu.cn

[R72] 等待端口就绪
来源：http://ms.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zv.hnjuh.cn

[R73] 分割大日志
来源：http://ob.newstarts.cn

split -l 1000 big.log part_
来源：http://gg.asd995.cn

[R74] 批量重命名
来源：http://ap.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gb.szxytkj.cn

[R75] 导出环境变量
来源：http://bc.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://ut.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://th.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://as.nszjky.cn

[R77] 读取用户输入
来源：http://is.haigaiapp.cn

read -rp "请输入: " ans
来源：http://va.muxihuayi.cn

[R78] 交互式菜单
来源：http://vr.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bn.colortex.cn

[R79] 解析命令行选项
来源：http://sb.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zn.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://hd.bjjhwx.cn

time ./run.sh
来源：http://lu.bjjhwx.cn

================================================================================
来源：http://xy.shtwfgs.cn

S. C / C++ 专题
来源：http://fa.521024.cn

================================================================================
来源：http://pw.shtwfgs.cn

[S01] C：Hello World
来源：http://qr.nicolike.cn

#include <stdio.h>
来源：http://lx.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cs.asd995.cn

[S02] C：变量与格式化输出
来源：http://qa.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://de.szsharing.cn

[S03] C：读入整数
来源：http://qy.shxzskj.cn

int x; scanf("%d", &x);
来源：http://uo.yuexingan06.cn

[S04] C：字符串复制
来源：http://xu.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://iq.colortex.cn

[S05] C：字符串长度
来源：http://nj.hahajie.cn

strlen(s)
来源：http://jz.yuexingan06.cn

[S06] C：字符串比较
来源：http://an.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://vd.9csxet.cn

[S07] C：数组遍历求和
来源：http://me.szxytkj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sr.colortex.cn

[S08] C：动态内存分配与释放
来源：http://xn.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tu.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://vk.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eh.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://ul.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://mc.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://zo.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://at.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dk.colortex.cn

fclose(f);
来源：http://jd.chemitech.net.cn

[S12] C：写文件
来源：http://xj.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sr.szxytkj.cn

[S13] C：宏定义
来源：http://bt.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ol.panjiajie.cn

[S14] C：枚举
来源：http://lp.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://yl.hahajie.cn

[S15] C：类型转换
来源：http://vb.bjjhwx.cn

(double) a / b
来源：http://ux.szsharing.cn

[S16] C：位操作置位
来源：http://xs.lnxyls.cn

x |= (1 << 3);
来源：http://tu.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://yj.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hs.bookmarksfly.cn

[S18] C：命令行参数
来源：http://ca.nicolike.cn

int main(int argc, char **argv)
来源：http://gk.521024.cn

[S19] C：快速排序
来源：http://qc.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yv.hnjuh.cn

[S20] C：二分查找
来源：http://wh.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vj.bookmarksfly.cn

[S21] C：字符类别判断
来源：http://pd.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jq.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://lm.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ay.bookmarksfly.cn

[S23] C：随机数
来源：http://dt.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xd.shxzukj.cn

[S24] C：获取本地时间
来源：http://rj.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pi.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://dm.colortex.cn

memcpy(dst, src, n);
来源：http://ad.jianghongdianzi.cn

[S26] C：内存清零
来源：http://td.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://oh.hahajie.cn

[S27] C：定义常量
来源：http://pn.wgjwhj.cn

const double PI = 3.14159;
来源：http://uo.newstarts.cn

[S28] C：静态变量
来源：http://uy.gzmigu.cn

static int counter = 0;
来源：http://fx.wgjwhj.cn

[S29] C：变参函数
来源：http://rg.yuexingan06.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://to.hahajie.cn

[S30] C：头文件保护
来源：http://sn.shxzskj.cn

#ifndef X_H
来源：http://sw.bookmarksfly.cn

#define X_H
来源：http://pg.huanxung.cn

#endif
来源：http://bq.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://gd.hahajie.cn

#include <iostream>
来源：http://yw.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://qb.hnjuh.cn

[S32] C++：字符串
来源：http://oj.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://do.haigaiapp.cn

[S33] C++：vector 增删
来源：http://zv.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tw.huanxung.cn

[S34] C++：遍历 vector
来源：http://bp.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://mt.nicolike.cn

[S35] C++：map
来源：http://ea.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qj.szxytkj.cn

[S36] C++：unordered_map
来源：http://nl.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vn.szsharing.cn

[S37] C++：set
来源：http://gu.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://er.chemitech.net.cn

[S38] C++：排序
来源：http://nr.asd995.cn

std::sort(v.begin(), v.end());
来源：http://pp.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://st.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bd.bjjhwx.cn

[S40] C++：查找元素
来源：http://lo.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dd.gzmigu.cn

[S41] C++：类与构造函数
来源：http://pw.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yb.huanxung.cn

[S42] C++：继承与虚函数
来源：http://mt.521024.cn

class B : public Base { public: void f() override {} };
来源：http://zu.chemitech.net.cn

[S43] C++：智能指针
来源：http://mt.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://sr.huixiangedu.cn

[S44] C++：引用传参
来源：http://wv.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://sd.jctech888.com.cn

[S45] C++：lambda
来源：http://nd.hahajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://iz.haigaiapp.cn

[S46] C++：函数模板
来源：http://xp.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fd.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://rw.huixiangedu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uh.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://qs.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dm.nszjky.cn


<!-- 参考信息 -->