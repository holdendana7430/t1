代发 wailian999

[Q78] 当前时间
来源：http://gm.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://id.huixiangedu.cn

[Q79] 字符串拼接
来源：http://ty.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mp.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://ga.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://an.huixiangedu.cn

[Q81] 字符串替换
来源：http://ek.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oi.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://ly.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://au.bjjhwx.cn

[Q83] 大小写转换
来源：http://pz.jianghongdianzi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jb.nicolike.cn

[Q84] 去除首尾空格
来源：http://hw.jctech888.com.cn

SELECT TRIM(name) FROM users;
来源：http://zd.asd995.cn

[Q85] 数值取整
来源：http://mn.shxzskj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ln.jianghongdianzi.cn

[Q86] 读取 JSON 字段
来源：http://ve.bjjhwx.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://el.nicolike.cn

[Q87] JSON 字段做条件
来源：http://wi.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fy.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://lg.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ym.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bl.hahajie.cn

[Q89] 判断表是否存在
来源：http://oo.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ce.szxytkj.cn

[Q90] 生成序号列
来源：http://oh.huanxung.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yn.9csxet.cn

================================================================================
来源：http://gg.jianghongdianzi.cn

R. Bash 专题
来源：http://yn.yuexingan06.cn

================================================================================
来源：http://nl.hahajie.cn

[R01] shebang 与严格模式
来源：http://jv.huanxung.cn

#!/usr/bin/env bash
来源：http://st.gzmigu.cn

set -euo pipefail
来源：http://hv.panjiajie.cn

[R02] 变量赋值与使用
来源：http://qo.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://lq.jctech888.com.cn

[R03] 只读变量
来源：http://ou.521024.cn

readonly PI=3.14
来源：http://zu.nszjky.cn

[R04] 位置参数
来源：http://cr.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ow.hahajie.cn

[R05] 参数默认值
来源：http://we.nszjky.cn

name="${1:-default}"
来源：http://mg.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://ss.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kv.chemitech.net.cn

[R07] if 判断文件
来源：http://fw.chemitech.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fz.shtwfgs.cn

[R08] 数值比较
来源：http://xo.hahajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zv.9csxet.cn

[R09] 字符串比较
来源：http://af.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wu.bjjhwx.cn

[R10] 正则匹配
来源：http://bz.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://no.shtwfgs.cn

[R11] case 多分支
来源：http://mx.newstarts.cn

case "$1" in
来源：http://wr.yuexingan06.cn

start) echo "启动" ;;
来源：http://jt.shxzukj.cn

stop)  echo "停止" ;;
来源：http://se.nicolike.cn

*)     echo "未知命令" ;;
来源：http://md.521024.cn

esac
来源：http://hg.chemitech.net.cn

[R12] for 遍历文件
来源：http://dx.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://lp.szxytkj.cn

[R13] for 计数循环
来源：http://sk.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://zs.yuexingan06.cn

[R14] C 风格 for
来源：http://ir.shxzskj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ko.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://ns.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ev.wgjwhj.cn

[R16] until 等待条件
来源：http://ur.huixiangedu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ln.hnjuh.cn

[R17] 数组定义与取值
来源：http://vt.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xq.shxzukj.cn

[R18] 遍历数组
来源：http://sa.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cb.hnjuh.cn

[R19] 数组长度
来源：http://je.hnjuh.cn

echo "${#arr[@]}"
来源：http://fb.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://cn.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yi.shtwfgs.cn

[R21] 字符串长度
来源：http://pn.jianghongdianzi.cn

echo "${#s}"
来源：http://fp.9csxet.cn

[R22] 截取子串
来源：http://in.9csxet.cn

echo "${s:0:5}"
来源：http://ex.panjiajie.cn

[R23] 字符串替换
来源：http://gt.newstarts.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sz.newstarts.cn

[R24] 大小写转换
来源：http://mz.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ef.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://ns.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qp.yuexingan06.cn

[R26] 命令替换
来源：http://gz.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://tk.gzmigu.cn

[R27] 算术展开
来源：http://lb.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://jk.9csxet.cn

[R28] 浮点运算
来源：http://pp.huixiangedu.cn

echo "scale=2; 10/3" | bc
来源：http://lq.haigaiapp.cn

[R29] 定义函数
来源：http://ox.szsharing.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nn.shtwfgs.cn

[R30] 函数返回状态码
来源：http://es.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://ow.lnxyls.cn

[R31] 局部变量
来源：http://rt.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://fd.hahajie.cn

[R32] 参数个数校验
来源：http://xx.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kz.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://kp.hnjuh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wv.chemitech.net.cn

[R34] 退出时清理
来源：http://rw.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gk.huanxung.cn

[R35] 后台执行并等待
来源：http://kd.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mx.shxzskj.cn

[R36] 并发执行多个任务
来源：http://ft.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rv.muxihuayi.cn

[R37] 把输出赋给变量
来源：http://qi.yuexingan06.cn

files=$(ls -1)
来源：http://iy.szsharing.cn

[R38] 管道串联
来源：http://rr.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://ck.asd995.cn

[R39] 重定向标准输出与错误
来源：http://fg.muxihuayi.cn

cmd > out.log 2>&1
来源：http://vn.haigaiapp.cn

[R40] 追加写日志
来源：http://tr.asd995.cn

echo "log" >> out.log
来源：http://xw.9csxet.cn

[R41] 丢弃输出
来源：http://ab.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://nz.wgjwhj.cn

[R42] 输入重定向
来源：http://eu.panjiajie.cn

wc -l < a.txt
来源：http://if.9csxet.cn

[R43] 按名字查找文件
来源：http://tu.muxihuayi.cn

find . -name "*.log" -type f
来源：http://ku.asd995.cn

[R44] 按修改时间查找
来源：http://gp.shxzukj.cn

find . -mtime -7 -type f
来源：http://wc.jctech888.com.cn

[R45] 批量删除
来源：http://mc.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://hc.hnjuh.cn

[R46] 递归替换文件内容
来源：http://wo.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dd.521024.cn

[R47] sed 单行替换
来源：http://fp.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ma.panjiajie.cn

[R48] awk 取指定列
来源：http://iz.hahajie.cn

awk '{print $1, $3}' a.txt
来源：http://cr.szsharing.cn

[R49] awk 带条件
来源：http://pq.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fy.newstarts.cn

[R50] awk 求和
来源：http://ah.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cr.nicolike.cn

[R51] 排序去重取前几
来源：http://fa.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pk.wgjwhj.cn

[R52] 统计行数
来源：http://mi.huixiangedu.cn

wc -l a.txt
来源：http://to.nszjky.cn

[R53] 查看文件头与实时尾
来源：http://mj.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zn.muxihuayi.cn

[R54] 比较两个文件
来源：http://gg.wgjwhj.cn

diff a.txt b.txt
来源：http://qa.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://zf.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lz.huanxung.cn

[R56] 远程拷贝
来源：http://yb.shxzukj.cn

scp file user@host:/path/
来源：http://bc.szsharing.cn

[R57] 远程执行命令
来源：http://ob.chemitech.net.cn

ssh user@host 'uptime'
来源：http://sc.muxihuayi.cn

[R58] 下载文件
来源：http://or.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bu.jctech888.com.cn

[R59] 发 POST JSON
来源：http://dv.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ta.huixiangedu.cn

[R60] 只看 HTTP 状态码
来源：http://uo.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gf.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://rx.9csxet.cn

df -h;  du -sh *
来源：http://bv.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://cp.colortex.cn

du -ah . | sort -rh | head -10
来源：http://uh.haigaiapp.cn

[R63] 内存与进程
来源：http://ms.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://nw.asd995.cn

[R64] 结束进程
来源：http://ym.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://cf.521024.cn

[R65] 查看端口占用
来源：http://wf.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mx.shtwfgs.cn

[R66] 定时任务
来源：http://gm.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://nz.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://cq.jctech888.com.cn

openssl rand -hex 16
来源：http://yr.nszjky.cn

[R68] 计算文件校验值
来源：http://sd.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yt.hnjuh.cn

[R69] 生成随机密码
来源：http://wn.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://ds.hahajie.cn

[R70] 时间戳与互转
来源：http://ek.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://qf.bookmarksfly.cn

[R71] 日期格式化
来源：http://wr.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sj.colortex.cn

[R72] 等待端口就绪
来源：http://mo.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dr.panjiajie.cn

[R73] 分割大日志
来源：http://nc.asd995.cn

split -l 1000 big.log part_
来源：http://nh.huixiangedu.cn

[R74] 批量重命名
来源：http://he.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dq.shxzskj.cn

[R75] 导出环境变量
来源：http://wk.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://cf.hahajie.cn

[R76] 使用临时文件
来源：http://vn.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qq.yuexingan06.cn

[R77] 读取用户输入
来源：http://hr.bjjhwx.cn

read -rp "请输入: " ans
来源：http://qx.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://hx.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://op.newstarts.cn

[R79] 解析命令行选项
来源：http://oy.wgjwhj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nm.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://pw.gzmigu.cn

time ./run.sh
来源：http://hi.shxzukj.cn

================================================================================
来源：http://bi.shtwfgs.cn

S. C / C++ 专题
来源：http://rr.nszjky.cn

================================================================================
来源：http://vl.colortex.cn

[S01] C：Hello World
来源：http://sd.szxytkj.cn

#include <stdio.h>
来源：http://tq.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wz.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://fn.chemitech.net.cn

int a = 10; printf("%d\n", a);
来源：http://ab.huixinmuqiang.cn

[S03] C：读入整数
来源：http://kw.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://ut.szxytkj.cn

[S04] C：字符串复制
来源：http://po.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cd.bookmarksfly.cn

[S05] C：字符串长度
来源：http://ke.jianghongdianzi.cn

strlen(s)
来源：http://ki.haigaiapp.cn

[S06] C：字符串比较
来源：http://mo.9csxet.cn

strcmp(a, b) == 0
来源：http://my.gzmigu.cn

[S07] C：数组遍历求和
来源：http://cl.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://go.colortex.cn

[S08] C：动态内存分配与释放
来源：http://um.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gc.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://xa.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ms.hnjuh.cn

[S10] C：指针与解引用
来源：http://wf.521024.cn

int *p = &a;  *p = 5;
来源：http://yi.nicolike.cn

[S11] C：逐行读文件
来源：http://lc.yuexingan06.cn

FILE *f = fopen("a.txt", "r");
来源：http://ce.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pi.nszjky.cn

fclose(f);
来源：http://kh.bjjhwx.cn

[S12] C：写文件
来源：http://sq.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lw.huixiangedu.cn

[S13] C：宏定义
来源：http://pd.newstarts.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vd.panjiajie.cn

[S14] C：枚举
来源：http://yr.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://vc.shxzukj.cn

[S15] C：类型转换
来源：http://bm.bookmarksfly.cn

(double) a / b
来源：http://rb.nszjky.cn

[S16] C：位操作置位
来源：http://rk.huixinmuqiang.cn

x |= (1 << 3);
来源：http://oh.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://ra.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://te.nicolike.cn

[S18] C：命令行参数
来源：http://vx.haigaiapp.cn

int main(int argc, char **argv)
来源：http://iy.bjjhwx.cn

[S19] C：快速排序
来源：http://ib.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kj.hahajie.cn

[S20] C：二分查找
来源：http://de.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ip.shxzskj.cn

[S21] C：字符类别判断
来源：http://sq.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ro.jctech888.com.cn

[S22] C：字符串转数字
来源：http://fz.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bz.hnjuh.cn

[S23] C：随机数
来源：http://hx.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ww.szsharing.cn

[S24] C：获取本地时间
来源：http://xl.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vk.newstarts.cn

[S25] C：内存拷贝
来源：http://if.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://un.huixinmuqiang.cn

[S26] C：内存清零
来源：http://st.szsharing.cn

memset(a, 0, sizeof a);
来源：http://iz.haigaiapp.cn

[S27] C：定义常量
来源：http://xe.muxihuayi.cn

const double PI = 3.14159;
来源：http://au.muxihuayi.cn

[S28] C：静态变量
来源：http://is.chemitech.net.cn

static int counter = 0;
来源：http://gy.hahajie.cn

[S29] C：变参函数
来源：http://mn.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jd.newstarts.cn

[S30] C：头文件保护
来源：http://lh.colortex.cn

#ifndef X_H
来源：http://zx.bookmarksfly.cn

#define X_H
来源：http://gs.colortex.cn

#endif
来源：http://xl.hahajie.cn

[S31] C++：Hello World
来源：http://ba.hahajie.cn

#include <iostream>
来源：http://ky.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://xq.haigaiapp.cn

[S32] C++：字符串
来源：http://wf.bookmarksfly.cn

std::string s = "hi";  s += "!";
来源：http://yb.szsharing.cn

[S33] C++：vector 增删
来源：http://sg.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hf.shxzskj.cn

[S34] C++：遍历 vector
来源：http://hv.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://iy.jianghongdianzi.cn

[S35] C++：map
来源：http://ci.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vl.jctech888.com.cn

[S36] C++：unordered_map
来源：http://fj.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xb.bookmarksfly.cn

[S37] C++：set
来源：http://ce.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ah.shxzukj.cn

[S38] C++：排序
来源：http://bu.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://mr.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://fq.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nd.colortex.cn

[S40] C++：查找元素
来源：http://jw.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ix.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://zv.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tj.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://fj.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://xj.521024.cn

[S43] C++：智能指针
来源：http://wl.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://ar.wgjwhj.cn

[S44] C++：引用传参
来源：http://ju.newstarts.cn

void inc(int &x) { ++x; }
来源：http://qy.newstarts.cn

[S45] C++：lambda
来源：http://te.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nu.panjiajie.cn

[S46] C++：函数模板
来源：http://ye.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fn.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://ta.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ja.szsharing.cn

[S48] C++：逐行读文件
来源：http://ao.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://td.bjjhwx.cn


<!-- 参考信息 -->