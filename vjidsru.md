代发 wailian999

[Q78] 当前时间
来源：http://di.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hs.huixiangedu.cn

[Q79] 字符串拼接
来源：http://fq.huanxung.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zf.haigaiapp.cn

[Q80] 字符串截取
来源：http://fd.bjjhwx.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dw.newstarts.cn

[Q81] 字符串替换
来源：http://yf.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jk.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://hl.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lt.muxihuayi.cn

[Q83] 大小写转换
来源：http://jy.gzmigu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://iy.521024.cn

[Q84] 去除首尾空格
来源：http://dj.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://hd.jctech888.com.cn

[Q85] 数值取整
来源：http://xb.yuntaijiaju.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jc.nszjky.cn

[Q86] 读取 JSON 字段
来源：http://oj.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vm.chemitech.net.cn

[Q87] JSON 字段做条件
来源：http://rx.huixinmuqiang.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gy.jianghongdianzi.cn

[Q88] 行转列（条件聚合）
来源：http://ql.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ju.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zn.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://lx.521024.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jj.asd995.cn

[Q90] 生成序号列
来源：http://oa.huixiangedu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://py.asd995.cn

================================================================================
来源：http://un.chemitech.net.cn

R. Bash 专题
来源：http://za.huixiangedu.cn

================================================================================
来源：http://nv.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://qb.newstarts.cn

#!/usr/bin/env bash
来源：http://zh.shxzskj.cn

set -euo pipefail
来源：http://eu.szsharing.cn

[R02] 变量赋值与使用
来源：http://vk.panjiajie.cn

name="Tom"; echo "$name"
来源：http://hf.9csxet.cn

[R03] 只读变量
来源：http://xj.asd995.cn

readonly PI=3.14
来源：http://zi.gzmigu.cn

[R04] 位置参数
来源：http://ox.bjjhwx.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hb.9csxet.cn

[R05] 参数默认值
来源：http://zh.wgjwhj.cn

name="${1:-default}"
来源：http://ld.huanxung.cn

[R06] 判断命令是否存在
来源：http://yt.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xd.haigaiapp.cn

[R07] if 判断文件
来源：http://ti.yuntaijiaju.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wq.gzmigu.cn

[R08] 数值比较
来源：http://ka.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mm.lnxyls.cn

[R09] 字符串比较
来源：http://ye.chemitech.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gi.nicolike.cn

[R10] 正则匹配
来源：http://zg.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vb.hnjuh.cn

[R11] case 多分支
来源：http://yz.shxzukj.cn

case "$1" in
来源：http://ek.bookmarksfly.cn

start) echo "启动" ;;
来源：http://su.huanxung.cn

stop)  echo "停止" ;;
来源：http://fm.521024.cn

*)     echo "未知命令" ;;
来源：http://nh.jctech888.com.cn

esac
来源：http://zk.nicolike.cn

[R12] for 遍历文件
来源：http://zq.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://ew.haigaiapp.cn

[R13] for 计数循环
来源：http://ei.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://va.shtwfgs.cn

[R14] C 风格 for
来源：http://pv.lnxyls.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ky.asd995.cn

[R15] while 逐行读文件
来源：http://fv.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://aw.jianghongdianzi.cn

[R16] until 等待条件
来源：http://if.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ro.panjiajie.cn

[R17] 数组定义与取值
来源：http://ys.9csxet.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hi.shxzskj.cn

[R18] 遍历数组
来源：http://hk.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://za.nicolike.cn

[R19] 数组长度
来源：http://xf.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://pw.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://lt.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vv.newstarts.cn

[R21] 字符串长度
来源：http://hb.szsharing.cn

echo "${#s}"
来源：http://am.jctech888.com.cn

[R22] 截取子串
来源：http://pj.bookmarksfly.cn

echo "${s:0:5}"
来源：http://li.szsharing.cn

[R23] 字符串替换
来源：http://vw.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yd.asd995.cn

[R24] 大小写转换
来源：http://qq.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sz.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://em.szsharing.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ey.asd995.cn

[R26] 命令替换
来源：http://ad.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://jm.chemitech.net.cn

[R27] 算术展开
来源：http://do.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://qx.colortex.cn

[R28] 浮点运算
来源：http://tu.nszjky.cn

echo "scale=2; 10/3" | bc
来源：http://xa.huanxung.cn

[R29] 定义函数
来源：http://hh.shxzskj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wk.panjiajie.cn

[R30] 函数返回状态码
来源：http://xf.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://qi.bookmarksfly.cn

[R31] 局部变量
来源：http://ko.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://wc.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://oo.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eb.jctech888.com.cn

[R33] 捕获错误并提示行号
来源：http://wp.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://no.chemitech.net.cn

[R34] 退出时清理
来源：http://bb.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ul.521024.cn

[R35] 后台执行并等待
来源：http://rk.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mg.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://fy.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zx.lnxyls.cn

[R37] 把输出赋给变量
来源：http://ws.chemitech.net.cn

files=$(ls -1)
来源：http://iz.hnjuh.cn

[R38] 管道串联
来源：http://cr.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://el.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://sp.panjiajie.cn

cmd > out.log 2>&1
来源：http://ge.szsharing.cn

[R40] 追加写日志
来源：http://tu.wgjwhj.cn

echo "log" >> out.log
来源：http://bb.9csxet.cn

[R41] 丢弃输出
来源：http://ix.newstarts.cn

cmd >/dev/null 2>&1
来源：http://fp.huixiangedu.cn

[R42] 输入重定向
来源：http://jn.nicolike.cn

wc -l < a.txt
来源：http://ov.shxzskj.cn

[R43] 按名字查找文件
来源：http://vj.hnjuh.cn

find . -name "*.log" -type f
来源：http://bx.yuexingan06.cn

[R44] 按修改时间查找
来源：http://kp.hnjuh.cn

find . -mtime -7 -type f
来源：http://zh.yuexingan06.cn

[R45] 批量删除
来源：http://mm.huanxung.cn

find . -name "*.tmp" -delete
来源：http://yw.lnxyls.cn

[R46] 递归替换文件内容
来源：http://vn.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zn.haigaiapp.cn

[R47] sed 单行替换
来源：http://uy.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xw.panjiajie.cn

[R48] awk 取指定列
来源：http://nr.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://my.asd995.cn

[R49] awk 带条件
来源：http://so.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tt.jianghongdianzi.cn

[R50] awk 求和
来源：http://jt.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fu.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://yj.jianghongdianzi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ri.yuexingan06.cn

[R52] 统计行数
来源：http://wo.panjiajie.cn

wc -l a.txt
来源：http://om.shtwfgs.cn

[R53] 查看文件头与实时尾
来源：http://tn.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pt.gzmigu.cn

[R54] 比较两个文件
来源：http://go.chemitech.net.cn

diff a.txt b.txt
来源：http://ul.bookmarksfly.cn

[R55] 压缩与解压
来源：http://bh.jctech888.com.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://we.newstarts.cn

[R56] 远程拷贝
来源：http://vh.newstarts.cn

scp file user@host:/path/
来源：http://fo.newstarts.cn

[R57] 远程执行命令
来源：http://xc.lnxyls.cn

ssh user@host 'uptime'
来源：http://km.hnjuh.cn

[R58] 下载文件
来源：http://yk.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ur.hnjuh.cn

[R59] 发 POST JSON
来源：http://tb.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ad.nicolike.cn

[R60] 只看 HTTP 状态码
来源：http://rl.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ha.haigaiapp.cn

[R61] 磁盘占用
来源：http://ln.jctech888.com.cn

df -h;  du -sh *
来源：http://yn.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://qu.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://kg.shtwfgs.cn

[R63] 内存与进程
来源：http://qp.colortex.cn

free -h;  ps aux | grep nginx
来源：http://pz.szsharing.cn

[R64] 结束进程
来源：http://yj.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://xl.hahajie.cn

[R65] 查看端口占用
来源：http://ug.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zf.panjiajie.cn

[R66] 定时任务
来源：http://tk.yuexingan06.cn

crontab -e;  crontab -l
来源：http://wk.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://px.yuexingan06.cn

openssl rand -hex 16
来源：http://od.szxytkj.cn

[R68] 计算文件校验值
来源：http://uu.huixiangedu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://us.panjiajie.cn

[R69] 生成随机密码
来源：http://ki.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://nw.gzmigu.cn

[R70] 时间戳与互转
来源：http://ty.jianghongdianzi.cn

date +%s;  date -d @1700000000
来源：http://wp.szxytkj.cn

[R71] 日期格式化
来源：http://xd.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sy.gzmigu.cn

[R72] 等待端口就绪
来源：http://yz.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xr.9csxet.cn

[R73] 分割大日志
来源：http://zu.yuexingan06.cn

split -l 1000 big.log part_
来源：http://em.gzmigu.cn

[R74] 批量重命名
来源：http://dw.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lr.huixiangedu.cn

[R75] 导出环境变量
来源：http://qc.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://nz.shxzskj.cn

[R76] 使用临时文件
来源：http://hl.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zw.colortex.cn

[R77] 读取用户输入
来源：http://jn.gzmigu.cn

read -rp "请输入: " ans
来源：http://mg.panjiajie.cn

[R78] 交互式菜单
来源：http://gv.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qt.shxzskj.cn

[R79] 解析命令行选项
来源：http://kr.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lg.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://pu.bookmarksfly.cn

time ./run.sh
来源：http://vh.shtwfgs.cn

================================================================================
来源：http://ip.huixinmuqiang.cn

S. C / C++ 专题
来源：http://oo.chemitech.net.cn

================================================================================
来源：http://sx.szxytkj.cn

[S01] C：Hello World
来源：http://fy.9csxet.cn

#include <stdio.h>
来源：http://xf.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cb.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://ur.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://bk.szxytkj.cn

[S03] C：读入整数
来源：http://je.shxzskj.cn

int x; scanf("%d", &x);
来源：http://yt.shxzukj.cn

[S04] C：字符串复制
来源：http://zj.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fq.gzmigu.cn

[S05] C：字符串长度
来源：http://hm.asd995.cn

strlen(s)
来源：http://kz.huanxung.cn

[S06] C：字符串比较
来源：http://lg.haigaiapp.cn

strcmp(a, b) == 0
来源：http://he.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://cx.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pc.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://ab.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yp.bjjhwx.cn

[S09] C：结构体定义与初始化
来源：http://gk.lnxyls.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wz.bjjhwx.cn

[S10] C：指针与解引用
来源：http://vm.colortex.cn

int *p = &a;  *p = 5;
来源：http://bh.lnxyls.cn

[S11] C：逐行读文件
来源：http://ny.lnxyls.cn

FILE *f = fopen("a.txt", "r");
来源：http://iq.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://oj.9csxet.cn

fclose(f);
来源：http://wk.panjiajie.cn

[S12] C：写文件
来源：http://rz.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ek.asd995.cn

[S13] C：宏定义
来源：http://mk.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oa.asd995.cn

[S14] C：枚举
来源：http://bi.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://ki.yuntaijiaju.cn

[S15] C：类型转换
来源：http://ox.chemitech.net.cn

(double) a / b
来源：http://yq.hahajie.cn

[S16] C：位操作置位
来源：http://to.huanxung.cn

x |= (1 << 3);
来源：http://rj.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://ix.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gk.chemitech.net.cn

[S18] C：命令行参数
来源：http://tw.huixiangedu.cn

int main(int argc, char **argv)
来源：http://se.9csxet.cn

[S19] C：快速排序
来源：http://ri.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ja.jianghongdianzi.cn

[S20] C：二分查找
来源：http://cl.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qw.bjjhwx.cn

[S21] C：字符类别判断
来源：http://aw.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://et.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://qr.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hm.chemitech.net.cn

[S23] C：随机数
来源：http://js.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://iq.jctech888.com.cn

[S24] C：获取本地时间
来源：http://xz.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vt.jctech888.com.cn

[S25] C：内存拷贝
来源：http://sj.shxzukj.cn

memcpy(dst, src, n);
来源：http://ch.wgjwhj.cn

[S26] C：内存清零
来源：http://ot.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://kf.bjjhwx.cn

[S27] C：定义常量
来源：http://tj.jctech888.com.cn

const double PI = 3.14159;
来源：http://mo.asd995.cn

[S28] C：静态变量
来源：http://et.shtwfgs.cn

static int counter = 0;
来源：http://ch.yuexingan06.cn

[S29] C：变参函数
来源：http://rp.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rb.haigaiapp.cn

[S30] C：头文件保护
来源：http://kt.bjjhwx.cn

#ifndef X_H
来源：http://kr.panjiajie.cn

#define X_H
来源：http://gj.shtwfgs.cn

#endif
来源：http://ds.asd995.cn

[S31] C++：Hello World
来源：http://bi.muxihuayi.cn

#include <iostream>
来源：http://jo.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ju.huixiangedu.cn

[S32] C++：字符串
来源：http://ls.bookmarksfly.cn

std::string s = "hi";  s += "!";
来源：http://ly.bjjhwx.cn

[S33] C++：vector 增删
来源：http://fj.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tf.shtwfgs.cn

[S34] C++：遍历 vector
来源：http://gg.szsharing.cn

for (auto &x : v) { std::cout << x; }
来源：http://we.panjiajie.cn

[S35] C++：map
来源：http://oy.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kk.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://im.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ue.yuntaijiaju.cn

[S37] C++：set
来源：http://dm.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wy.colortex.cn

[S38] C++：排序
来源：http://zw.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://mb.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://ij.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qv.szxytkj.cn

[S40] C++：查找元素
来源：http://ty.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oq.gzmigu.cn

[S41] C++：类与构造函数
来源：http://jy.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wb.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://lv.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://ov.nicolike.cn

[S43] C++：智能指针
来源：http://uq.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://qc.bjjhwx.cn

[S44] C++：引用传参
来源：http://cb.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://gz.asd995.cn

[S45] C++：lambda
来源：http://bo.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ue.newstarts.cn

[S46] C++：函数模板
来源：http://rr.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kd.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://hb.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oi.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://ho.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://we.gzmigu.cn


<!-- 参考信息 -->