代发 wailian999

[Q82] 字符长度与字节长度
来源：http://su.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fj.panjiajie.cn

[Q83] 大小写转换
来源：http://qr.jianghongdianzi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xj.shxzskj.cn

[Q84] 去除首尾空格
来源：http://xb.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://ww.hahajie.cn

[Q85] 数值取整
来源：http://mt.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ia.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://wp.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rc.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://ki.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fl.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://ns.huixiangedu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dc.asd995.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ph.9csxet.cn

[Q89] 判断表是否存在
来源：http://ew.yuexingan06.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yuexingan06.cn

[Q90] 生成序号列
来源：http://qs.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aw.jianghongdianzi.cn

================================================================================
来源：http://et.shxzskj.cn

R. Bash 专题
来源：http://il.haigaiapp.cn

================================================================================
来源：http://px.9csxet.cn

[R01] shebang 与严格模式
来源：http://aw.huixinmuqiang.cn

#!/usr/bin/env bash
来源：http://hp.shxzskj.cn

set -euo pipefail
来源：http://xq.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://tq.panjiajie.cn

name="Tom"; echo "$name"
来源：http://xg.shtwfgs.cn

[R03] 只读变量
来源：http://rx.colortex.cn

readonly PI=3.14
来源：http://os.szsharing.cn

[R04] 位置参数
来源：http://wk.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yz.bookmarksfly.cn

[R05] 参数默认值
来源：http://vu.huixinmuqiang.cn

name="${1:-default}"
来源：http://fn.gzmigu.cn

[R06] 判断命令是否存在
来源：http://vt.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gi.9csxet.cn

[R07] if 判断文件
来源：http://gh.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rq.yuexingan06.cn

[R08] 数值比较
来源：http://hf.nszjky.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wr.szxytkj.cn

[R09] 字符串比较
来源：http://wt.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zu.shxzskj.cn

[R10] 正则匹配
来源：http://ql.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ir.nszjky.cn

[R11] case 多分支
来源：http://wd.gzmigu.cn

case "$1" in
来源：http://tg.muxihuayi.cn

start) echo "启动" ;;
来源：http://ro.hahajie.cn

stop)  echo "停止" ;;
来源：http://do.shtwfgs.cn

*)     echo "未知命令" ;;
来源：http://eo.yuexingan06.cn

esac
来源：http://az.gzmigu.cn

[R12] for 遍历文件
来源：http://lm.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://tg.521024.cn

[R13] for 计数循环
来源：http://il.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://qz.asd995.cn

[R14] C 风格 for
来源：http://sl.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ku.hnjuh.cn

[R15] while 逐行读文件
来源：http://pf.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rm.jianghongdianzi.cn

[R16] until 等待条件
来源：http://vv.jctech888.com.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ze.panjiajie.cn

[R17] 数组定义与取值
来源：http://la.shtwfgs.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gv.huixiangedu.cn

[R18] 遍历数组
来源：http://rk.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nl.hnjuh.cn

[R19] 数组长度
来源：http://qr.szxytkj.cn

echo "${#arr[@]}"
来源：http://bp.shxzskj.cn

[R20] 关联数组（字典）
来源：http://rz.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kq.nicolike.cn

[R21] 字符串长度
来源：http://zw.9csxet.cn

echo "${#s}"
来源：http://qb.bookmarksfly.cn

[R22] 截取子串
来源：http://kl.lnxyls.cn

echo "${s:0:5}"
来源：http://dn.panjiajie.cn

[R23] 字符串替换
来源：http://kz.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yc.shtwfgs.cn

[R24] 大小写转换
来源：http://do.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mq.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://tm.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pz.lnxyls.cn

[R26] 命令替换
来源：http://rp.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://pp.colortex.cn

[R27] 算术展开
来源：http://ns.szsharing.cn

echo $((1 + 2 * 3))
来源：http://gp.nszjky.cn

[R28] 浮点运算
来源：http://tn.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://cd.gzmigu.cn

[R29] 定义函数
来源：http://jf.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xg.muxihuayi.cn

[R30] 函数返回状态码
来源：http://vk.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://ux.huixiangedu.cn

[R31] 局部变量
来源：http://ot.haigaiapp.cn

f() { local x=1; echo "$x"; }
来源：http://be.shxzskj.cn

[R32] 参数个数校验
来源：http://eq.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sr.521024.cn

[R33] 捕获错误并提示行号
来源：http://ei.bookmarksfly.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ht.yuntaijiaju.cn

[R34] 退出时清理
来源：http://jf.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kg.shxzukj.cn

[R35] 后台执行并等待
来源：http://id.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zl.hahajie.cn

[R36] 并发执行多个任务
来源：http://zk.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ob.szsharing.cn

[R37] 把输出赋给变量
来源：http://oe.newstarts.cn

files=$(ls -1)
来源：http://om.haigaiapp.cn

[R38] 管道串联
来源：http://ss.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://fh.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://ly.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://mf.jianghongdianzi.cn

[R40] 追加写日志
来源：http://ze.shxzskj.cn

echo "log" >> out.log
来源：http://yc.gzmigu.cn

[R41] 丢弃输出
来源：http://ii.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://ce.haigaiapp.cn

[R42] 输入重定向
来源：http://uw.newstarts.cn

wc -l < a.txt
来源：http://vw.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://yg.yuexingan06.cn

find . -name "*.log" -type f
来源：http://dz.haigaiapp.cn

[R44] 按修改时间查找
来源：http://je.9csxet.cn

find . -mtime -7 -type f
来源：http://uh.yuexingan06.cn

[R45] 批量删除
来源：http://kj.asd995.cn

find . -name "*.tmp" -delete
来源：http://up.521024.cn

[R46] 递归替换文件内容
来源：http://ot.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://li.bjjhwx.cn

[R47] sed 单行替换
来源：http://ms.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ee.szxytkj.cn

[R48] awk 取指定列
来源：http://sc.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://lh.yuexingan06.cn

[R49] awk 带条件
来源：http://ad.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cf.521024.cn

[R50] awk 求和
来源：http://xf.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://og.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://zc.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://li.shxzskj.cn

[R52] 统计行数
来源：http://kf.bjjhwx.cn

wc -l a.txt
来源：http://an.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://ei.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rh.wgjwhj.cn

[R54] 比较两个文件
来源：http://az.jianghongdianzi.cn

diff a.txt b.txt
来源：http://lx.asd995.cn

[R55] 压缩与解压
来源：http://yj.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pv.newstarts.cn

[R56] 远程拷贝
来源：http://pa.shxzukj.cn

scp file user@host:/path/
来源：http://wu.szsharing.cn

[R57] 远程执行命令
来源：http://rn.wgjwhj.cn

ssh user@host 'uptime'
来源：http://be.shtwfgs.cn

[R58] 下载文件
来源：http://tv.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://im.newstarts.cn

[R59] 发 POST JSON
来源：http://co.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ug.wgjwhj.cn

[R60] 只看 HTTP 状态码
来源：http://hc.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pq.shxzukj.cn

[R61] 磁盘占用
来源：http://jf.szsharing.cn

df -h;  du -sh *
来源：http://lx.hnjuh.cn

[R62] 找最占空间的文件
来源：http://af.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://ai.haigaiapp.cn

[R63] 内存与进程
来源：http://yd.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://zm.asd995.cn

[R64] 结束进程
来源：http://fd.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://kn.jctech888.com.cn

[R65] 查看端口占用
来源：http://me.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lb.521024.cn

[R66] 定时任务
来源：http://zh.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://xn.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://rl.9csxet.cn

openssl rand -hex 16
来源：http://sb.nszjky.cn

[R68] 计算文件校验值
来源：http://hg.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qw.shxzskj.cn

[R69] 生成随机密码
来源：http://cg.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://sg.shxzukj.cn

[R70] 时间戳与互转
来源：http://tw.huixinmuqiang.cn

date +%s;  date -d @1700000000
来源：http://kz.nicolike.cn

[R71] 日期格式化
来源：http://db.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xm.huixinmuqiang.cn

[R72] 等待端口就绪
来源：http://lh.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rj.gzmigu.cn

[R73] 分割大日志
来源：http://kv.gzmigu.cn

split -l 1000 big.log part_
来源：http://vw.panjiajie.cn

[R74] 批量重命名
来源：http://zm.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jk.szxytkj.cn

[R75] 导出环境变量
来源：http://kl.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://gk.hnjuh.cn

[R76] 使用临时文件
来源：http://rk.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eh.nicolike.cn

[R77] 读取用户输入
来源：http://ej.wgjwhj.cn

read -rp "请输入: " ans
来源：http://fh.szxytkj.cn

[R78] 交互式菜单
来源：http://nw.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mf.bookmarksfly.cn

[R79] 解析命令行选项
来源：http://ke.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://on.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://xi.huanxung.cn

time ./run.sh
来源：http://kh.9csxet.cn

================================================================================
来源：http://vo.gzmigu.cn

S. C / C++ 专题
来源：http://qj.nszjky.cn

================================================================================
来源：http://mu.chemitech.net.cn

[S01] C：Hello World
来源：http://at.nszjky.cn

#include <stdio.h>
来源：http://hq.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sj.nszjky.cn

[S02] C：变量与格式化输出
来源：http://au.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://yt.jianghongdianzi.cn

[S03] C：读入整数
来源：http://fi.hnjuh.cn

int x; scanf("%d", &x);
来源：http://ow.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://dh.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://or.szsharing.cn

[S05] C：字符串长度
来源：http://ns.hnjuh.cn

strlen(s)
来源：http://ck.gzmigu.cn

[S06] C：字符串比较
来源：http://mm.huanxung.cn

strcmp(a, b) == 0
来源：http://jh.szxytkj.cn

[S07] C：数组遍历求和
来源：http://et.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bv.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://rj.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xs.asd995.cn

[S09] C：结构体定义与初始化
来源：http://xp.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rj.jctech888.com.cn

[S10] C：指针与解引用
来源：http://fm.huanxung.cn

int *p = &a;  *p = 5;
来源：http://qm.wgjwhj.cn

[S11] C：逐行读文件
来源：http://ru.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://yl.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fa.jctech888.com.cn

fclose(f);
来源：http://is.haigaiapp.cn

[S12] C：写文件
来源：http://dn.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ao.chemitech.net.cn

[S13] C：宏定义
来源：http://jv.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yy.gzmigu.cn

[S14] C：枚举
来源：http://ht.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://kv.hnjuh.cn

[S15] C：类型转换
来源：http://ks.jctech888.com.cn

(double) a / b
来源：http://rt.gzmigu.cn

[S16] C：位操作置位
来源：http://gr.nszjky.cn

x |= (1 << 3);
来源：http://tq.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://av.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wa.hnjuh.cn

[S18] C：命令行参数
来源：http://ar.nicolike.cn

int main(int argc, char **argv)
来源：http://mm.asd995.cn

[S19] C：快速排序
来源：http://mo.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ug.newstarts.cn

[S20] C：二分查找
来源：http://eq.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sa.asd995.cn

[S21] C：字符类别判断
来源：http://xs.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://am.hnjuh.cn

[S22] C：字符串转数字
来源：http://sn.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gk.asd995.cn

[S23] C：随机数
来源：http://ew.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ie.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://my.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gi.asd995.cn

[S25] C：内存拷贝
来源：http://iz.panjiajie.cn

memcpy(dst, src, n);
来源：http://zr.shtwfgs.cn

[S26] C：内存清零
来源：http://vk.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://an.asd995.cn

[S27] C：定义常量
来源：http://uc.muxihuayi.cn

const double PI = 3.14159;
来源：http://lg.nszjky.cn

[S28] C：静态变量
来源：http://ck.chemitech.net.cn

static int counter = 0;
来源：http://gr.asd995.cn

[S29] C：变参函数
来源：http://uz.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wj.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://vs.huixinmuqiang.cn

#ifndef X_H
来源：http://wu.lnxyls.cn

#define X_H
来源：http://gw.yuexingan06.cn

#endif
来源：http://lx.521024.cn

[S31] C++：Hello World
来源：http://vx.szsharing.cn

#include <iostream>
来源：http://as.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://za.521024.cn

[S32] C++：字符串
来源：http://gb.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://ws.hahajie.cn

[S33] C++：vector 增删
来源：http://dp.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ah.nszjky.cn

[S34] C++：遍历 vector
来源：http://aw.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://fn.521024.cn

[S35] C++：map
来源：http://dv.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dq.gzmigu.cn

[S36] C++：unordered_map
来源：http://yq.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uu.colortex.cn

[S37] C++：set
来源：http://wr.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ye.szxytkj.cn

[S38] C++：排序
来源：http://gp.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://za.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://qw.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tk.shxzukj.cn

[S40] C++：查找元素
来源：http://in.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qj.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://wn.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oe.colortex.cn

[S42] C++：继承与虚函数
来源：http://hs.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://fq.hahajie.cn

[S43] C++：智能指针
来源：http://da.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://lp.szsharing.cn

[S44] C++：引用传参
来源：http://nr.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://op.colortex.cn

[S45] C++：lambda
来源：http://zw.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yx.shxzukj.cn

[S46] C++：函数模板
来源：http://rb.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ez.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://cu.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tk.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://ej.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wb.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://oh.521024.cn

[S49] C++：写文件
来源：http://cn.huixinmuqiang.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zc.newstarts.cn

[S50] C++：格式化数字
来源：http://zs.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jc.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://ct.szxytkj.cn

static_cast<double>(a) / b
来源：http://fv.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://fx.hnjuh.cn


<!-- 参考信息 -->