代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eg.chemitech.net.cn

[Q75] 日期格式化
来源：http://oc.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rl.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bl.gzmigu.cn

[Q76] 按天统计
来源：http://yh.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wx.muxihuayi.cn

[Q77] 时间加减
来源：http://cl.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uy.shxzskj.cn

[Q78] 当前时间
来源：http://ne.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yo.haigaiapp.cn

[Q79] 字符串拼接
来源：http://fd.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ms.haigaiapp.cn

[Q80] 字符串截取
来源：http://do.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://os.chemitech.net.cn

[Q81] 字符串替换
来源：http://mv.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://aq.lnxyls.cn

[Q82] 字符长度与字节长度
来源：http://nt.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qr.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://nn.hahajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://so.jianghongdianzi.cn

[Q84] 去除首尾空格
来源：http://py.newstarts.cn

SELECT TRIM(name) FROM users;
来源：http://eq.colortex.cn

[Q85] 数值取整
来源：http://vn.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cs.nicolike.cn

[Q86] 读取 JSON 字段
来源：http://wj.gzmigu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ns.yuntaijiaju.cn

[Q87] JSON 字段做条件
来源：http://jb.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vw.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://di.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lz.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dd.szxytkj.cn

[Q89] 判断表是否存在
来源：http://sx.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tp.haigaiapp.cn

[Q90] 生成序号列
来源：http://wy.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ic.gzmigu.cn

================================================================================
来源：http://ev.9csxet.cn

R. Bash 专题
来源：http://ko.hahajie.cn

================================================================================
来源：http://ru.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://hx.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://lc.huixinmuqiang.cn

set -euo pipefail
来源：http://dd.shxzukj.cn

[R02] 变量赋值与使用
来源：http://fs.bookmarksfly.cn

name="Tom"; echo "$name"
来源：http://bt.shxzukj.cn

[R03] 只读变量
来源：http://zj.bjjhwx.cn

readonly PI=3.14
来源：http://wy.gzmigu.cn

[R04] 位置参数
来源：http://xg.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xp.shxzukj.cn

[R05] 参数默认值
来源：http://jp.bookmarksfly.cn

name="${1:-default}"
来源：http://qz.szxytkj.cn

[R06] 判断命令是否存在
来源：http://mt.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xw.hnjuh.cn

[R07] if 判断文件
来源：http://iv.hahajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://no.521024.cn

[R08] 数值比较
来源：http://dr.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://oq.wgjwhj.cn

[R09] 字符串比较
来源：http://en.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ua.szxytkj.cn

[R10] 正则匹配
来源：http://db.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vl.szxytkj.cn

[R11] case 多分支
来源：http://mk.521024.cn

case "$1" in
来源：http://tk.wgjwhj.cn

start) echo "启动" ;;
来源：http://jn.haigaiapp.cn

stop)  echo "停止" ;;
来源：http://xl.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://xq.shtwfgs.cn

esac
来源：http://au.9csxet.cn

[R12] for 遍历文件
来源：http://rv.szsharing.cn

for f in *.txt; do echo "$f"; done
来源：http://rn.gzmigu.cn

[R13] for 计数循环
来源：http://qv.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://gn.huixiangedu.cn

[R14] C 风格 for
来源：http://ek.lnxyls.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aj.nicolike.cn

[R15] while 逐行读文件
来源：http://ph.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jm.colortex.cn

[R16] until 等待条件
来源：http://wa.jctech888.com.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pu.jctech888.com.cn

[R17] 数组定义与取值
来源：http://lv.lnxyls.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bd.wgjwhj.cn

[R18] 遍历数组
来源：http://ik.szxytkj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gr.jianghongdianzi.cn

[R19] 数组长度
来源：http://pm.panjiajie.cn

echo "${#arr[@]}"
来源：http://up.hnjuh.cn

[R20] 关联数组（字典）
来源：http://dg.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://go.gzmigu.cn

[R21] 字符串长度
来源：http://sf.colortex.cn

echo "${#s}"
来源：http://dq.jianghongdianzi.cn

[R22] 截取子串
来源：http://xj.shtwfgs.cn

echo "${s:0:5}"
来源：http://ry.bjjhwx.cn

[R23] 字符串替换
来源：http://ih.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tf.panjiajie.cn

[R24] 大小写转换
来源：http://xp.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gv.yuntaijiaju.cn

[R25] 去后缀 / 去前缀
来源：http://mq.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yg.hahajie.cn

[R26] 命令替换
来源：http://hq.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://bk.szsharing.cn

[R27] 算术展开
来源：http://yp.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://xr.huixiangedu.cn

[R28] 浮点运算
来源：http://kk.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://nr.hnjuh.cn

[R29] 定义函数
来源：http://tp.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nz.hnjuh.cn

[R30] 函数返回状态码
来源：http://uy.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://io.szsharing.cn

[R31] 局部变量
来源：http://ae.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://rf.yuexingan06.cn

[R32] 参数个数校验
来源：http://da.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sc.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://ce.bookmarksfly.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vi.jctech888.com.cn

[R34] 退出时清理
来源：http://wr.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ln.hnjuh.cn

[R35] 后台执行并等待
来源：http://sw.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://og.gzmigu.cn

[R36] 并发执行多个任务
来源：http://oo.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ck.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://mq.huixiangedu.cn

files=$(ls -1)
来源：http://lb.huixiangedu.cn

[R38] 管道串联
来源：http://bs.nszjky.cn

cat a.txt | grep -i error | wc -l
来源：http://vd.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://fr.521024.cn

cmd > out.log 2>&1
来源：http://cq.bookmarksfly.cn

[R40] 追加写日志
来源：http://wz.haigaiapp.cn

echo "log" >> out.log
来源：http://zy.huanxung.cn

[R41] 丢弃输出
来源：http://tu.wgjwhj.cn

cmd >/dev/null 2>&1
来源：http://zu.nszjky.cn

[R42] 输入重定向
来源：http://nr.huixinmuqiang.cn

wc -l < a.txt
来源：http://wo.gzmigu.cn

[R43] 按名字查找文件
来源：http://af.lnxyls.cn

find . -name "*.log" -type f
来源：http://ab.wgjwhj.cn

[R44] 按修改时间查找
来源：http://lk.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://yl.shxzskj.cn

[R45] 批量删除
来源：http://da.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://sh.szxytkj.cn

[R46] 递归替换文件内容
来源：http://tl.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ay.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://ej.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ar.haigaiapp.cn

[R48] awk 取指定列
来源：http://fh.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://nv.bjjhwx.cn

[R49] awk 带条件
来源：http://xv.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kp.hahajie.cn

[R50] awk 求和
来源：http://yo.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vk.chemitech.net.cn

[R51] 排序去重取前几
来源：http://jv.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qf.newstarts.cn

[R52] 统计行数
来源：http://rz.nicolike.cn

wc -l a.txt
来源：http://oj.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://of.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xt.colortex.cn

[R54] 比较两个文件
来源：http://eb.nszjky.cn

diff a.txt b.txt
来源：http://os.hnjuh.cn

[R55] 压缩与解压
来源：http://jw.shxzukj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tq.bjjhwx.cn

[R56] 远程拷贝
来源：http://ce.yuntaijiaju.cn

scp file user@host:/path/
来源：http://ei.bookmarksfly.cn

[R57] 远程执行命令
来源：http://ym.shtwfgs.cn

ssh user@host 'uptime'
来源：http://rk.lnxyls.cn

[R58] 下载文件
来源：http://ev.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tf.yuexingan06.cn

[R59] 发 POST JSON
来源：http://ak.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cx.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://vn.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wp.bookmarksfly.cn

[R61] 磁盘占用
来源：http://vr.huanxung.cn

df -h;  du -sh *
来源：http://sv.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://jn.bjjhwx.cn

du -ah . | sort -rh | head -10
来源：http://tl.huixinmuqiang.cn

[R63] 内存与进程
来源：http://cy.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://af.huanxung.cn

[R64] 结束进程
来源：http://dh.hnjuh.cn

kill -9 $(pgrep -f app.py)
来源：http://oz.nszjky.cn

[R65] 查看端口占用
来源：http://po.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hj.haigaiapp.cn

[R66] 定时任务
来源：http://pi.colortex.cn

crontab -e;  crontab -l
来源：http://yq.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://et.huixiangedu.cn

openssl rand -hex 16
来源：http://fr.521024.cn

[R68] 计算文件校验值
来源：http://to.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://iy.bjjhwx.cn

[R69] 生成随机密码
来源：http://bk.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://nw.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://nc.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://oz.newstarts.cn

[R71] 日期格式化
来源：http://ei.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://oa.panjiajie.cn

[R72] 等待端口就绪
来源：http://lf.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ga.9csxet.cn

[R73] 分割大日志
来源：http://tj.9csxet.cn

split -l 1000 big.log part_
来源：http://ym.bjjhwx.cn

[R74] 批量重命名
来源：http://yd.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jn.bjjhwx.cn

[R75] 导出环境变量
来源：http://kq.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://tp.chemitech.net.cn

[R76] 使用临时文件
来源：http://iy.asd995.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gd.nicolike.cn

[R77] 读取用户输入
来源：http://ip.jctech888.com.cn

read -rp "请输入: " ans
来源：http://ov.nicolike.cn

[R78] 交互式菜单
来源：http://hf.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ff.hnjuh.cn

[R79] 解析命令行选项
来源：http://yy.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lp.nszjky.cn

[R80] 查看脚本执行耗时
来源：http://px.9csxet.cn

time ./run.sh
来源：http://mt.nicolike.cn

================================================================================
来源：http://dj.szxytkj.cn

S. C / C++ 专题
来源：http://fu.yuexingan06.cn

================================================================================
来源：http://vl.shxzskj.cn

[S01] C：Hello World
来源：http://xf.hnjuh.cn

#include <stdio.h>
来源：http://np.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://az.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://sv.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://dv.shxzskj.cn

[S03] C：读入整数
来源：http://og.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://iq.lnxyls.cn

[S04] C：字符串复制
来源：http://ry.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://it.muxihuayi.cn

[S05] C：字符串长度
来源：http://os.szsharing.cn

strlen(s)
来源：http://rp.huanxung.cn

[S06] C：字符串比较
来源：http://jj.jctech888.com.cn

strcmp(a, b) == 0
来源：http://tm.nicolike.cn

[S07] C：数组遍历求和
来源：http://de.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://de.huixinmuqiang.cn

[S08] C：动态内存分配与释放
来源：http://wt.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xt.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://fo.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jt.jctech888.com.cn

[S10] C：指针与解引用
来源：http://tk.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://rs.bjjhwx.cn

[S11] C：逐行读文件
来源：http://yv.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://sy.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nt.panjiajie.cn

fclose(f);
来源：http://cs.szsharing.cn

[S12] C：写文件
来源：http://wc.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fg.huixiangedu.cn

[S13] C：宏定义
来源：http://wb.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bq.9csxet.cn

[S14] C：枚举
来源：http://qa.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://yb.newstarts.cn

[S15] C：类型转换
来源：http://ip.yuexingan06.cn

(double) a / b
来源：http://vg.shtwfgs.cn

[S16] C：位操作置位
来源：http://vt.521024.cn

x |= (1 << 3);
来源：http://xp.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://br.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ud.shtwfgs.cn

[S18] C：命令行参数
来源：http://gk.haigaiapp.cn

int main(int argc, char **argv)
来源：http://pi.shxzukj.cn

[S19] C：快速排序
来源：http://lt.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qi.hahajie.cn

[S20] C：二分查找
来源：http://yc.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pq.huanxung.cn

[S21] C：字符类别判断
来源：http://tg.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ne.shtwfgs.cn

[S22] C：字符串转数字
来源：http://oc.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qk.szxytkj.cn

[S23] C：随机数
来源：http://hx.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cb.szxytkj.cn

[S24] C：获取本地时间
来源：http://km.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kv.lnxyls.cn

[S25] C：内存拷贝
来源：http://vr.nszjky.cn

memcpy(dst, src, n);
来源：http://vb.colortex.cn

[S26] C：内存清零
来源：http://yq.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://nt.wgjwhj.cn

[S27] C：定义常量
来源：http://jb.haigaiapp.cn

const double PI = 3.14159;
来源：http://xm.chemitech.net.cn

[S28] C：静态变量
来源：http://bf.wgjwhj.cn

static int counter = 0;
来源：http://cw.shxzukj.cn

[S29] C：变参函数
来源：http://yv.huixinmuqiang.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lx.colortex.cn

[S30] C：头文件保护
来源：http://uj.huixinmuqiang.cn

#ifndef X_H
来源：http://ln.shxzskj.cn

#define X_H
来源：http://ar.nszjky.cn

#endif
来源：http://gc.gzmigu.cn

[S31] C++：Hello World
来源：http://xq.colortex.cn

#include <iostream>
来源：http://me.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ay.shtwfgs.cn

[S32] C++：字符串
来源：http://aq.521024.cn

std::string s = "hi";  s += "!";
来源：http://dz.chemitech.net.cn

[S33] C++：vector 增删
来源：http://mj.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pt.shxzskj.cn

[S34] C++：遍历 vector
来源：http://yg.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://gt.huanxung.cn

[S35] C++：map
来源：http://vs.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ox.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://xr.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oh.colortex.cn

[S37] C++：set
来源：http://rv.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hu.szxytkj.cn

[S38] C++：排序
来源：http://qi.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://yr.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://vd.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wb.muxihuayi.cn

[S40] C++：查找元素
来源：http://nh.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yz.szsharing.cn

[S41] C++：类与构造函数
来源：http://np.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://va.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://lf.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://rx.bookmarksfly.cn

[S43] C++：智能指针
来源：http://yk.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://hh.nicolike.cn

[S44] C++：引用传参
来源：http://vr.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://wm.szsharing.cn


<!-- 参考信息 -->