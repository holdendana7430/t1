代发 wailian999

SHOW INDEX FROM users;
来源：http://kn.521024.cn

[Q73] 查看表状态
来源：http://vc.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ur.shxzskj.cn

[Q74] 强制使用索引
来源：http://yp.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yh.hahajie.cn

[Q75] 日期格式化
来源：http://wj.jctech888.com.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://br.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fs.haigaiapp.cn

[Q76] 按天统计
来源：http://kx.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eo.szxytkj.cn

[Q77] 时间加减
来源：http://mj.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vl.shxzskj.cn

[Q78] 当前时间
来源：http://yu.panjiajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fy.bjjhwx.cn

[Q79] 字符串拼接
来源：http://ug.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xh.shxzukj.cn

[Q80] 字符串截取
来源：http://ny.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hr.asd995.cn

[Q81] 字符串替换
来源：http://uj.szsharing.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yb.shxzukj.cn

[Q82] 字符长度与字节长度
来源：http://ft.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vd.9csxet.cn

[Q83] 大小写转换
来源：http://ng.yuexingan06.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tb.521024.cn

[Q84] 去除首尾空格
来源：http://xp.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://ng.jctech888.com.cn

[Q85] 数值取整
来源：http://bq.521024.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ul.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://ft.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aj.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://pm.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zj.9csxet.cn

[Q88] 行转列（条件聚合）
来源：http://uq.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kj.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sw.521024.cn

[Q89] 判断表是否存在
来源：http://pu.yuntaijiaju.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kk.nszjky.cn

[Q90] 生成序号列
来源：http://bu.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ly.hahajie.cn

================================================================================
来源：http://gt.shxzukj.cn

R. Bash 专题
来源：http://bl.jianghongdianzi.cn

================================================================================
来源：http://jj.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://yt.newstarts.cn

#!/usr/bin/env bash
来源：http://zr.szsharing.cn

set -euo pipefail
来源：http://mx.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://aa.nicolike.cn

name="Tom"; echo "$name"
来源：http://mg.hahajie.cn

[R03] 只读变量
来源：http://bp.gzmigu.cn

readonly PI=3.14
来源：http://cr.shxzukj.cn

[R04] 位置参数
来源：http://ua.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jy.panjiajie.cn

[R05] 参数默认值
来源：http://bk.colortex.cn

name="${1:-default}"
来源：http://ha.9csxet.cn

[R06] 判断命令是否存在
来源：http://ci.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xx.jianghongdianzi.cn

[R07] if 判断文件
来源：http://li.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hg.9csxet.cn

[R08] 数值比较
来源：http://qx.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lp.shxzukj.cn

[R09] 字符串比较
来源：http://we.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vo.huanxung.cn

[R10] 正则匹配
来源：http://rf.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bk.hnjuh.cn

[R11] case 多分支
来源：http://xy.521024.cn

case "$1" in
来源：http://wt.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://kg.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://sp.colortex.cn

*)     echo "未知命令" ;;
来源：http://ar.colortex.cn

esac
来源：http://lt.colortex.cn

[R12] for 遍历文件
来源：http://dv.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://xh.wgjwhj.cn

[R13] for 计数循环
来源：http://jl.newstarts.cn

for i in {1..10}; do echo "$i"; done
来源：http://mq.huixiangedu.cn

[R14] C 风格 for
来源：http://wx.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sl.asd995.cn

[R15] while 逐行读文件
来源：http://lg.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lw.huanxung.cn

[R16] until 等待条件
来源：http://rr.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yd.wgjwhj.cn

[R17] 数组定义与取值
来源：http://cv.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://be.shtwfgs.cn

[R18] 遍历数组
来源：http://tm.9csxet.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aq.jianghongdianzi.cn

[R19] 数组长度
来源：http://hu.asd995.cn

echo "${#arr[@]}"
来源：http://tf.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://ml.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hu.yuexingan06.cn

[R21] 字符串长度
来源：http://ez.haigaiapp.cn

echo "${#s}"
来源：http://pi.newstarts.cn

[R22] 截取子串
来源：http://um.shtwfgs.cn

echo "${s:0:5}"
来源：http://mu.colortex.cn

[R23] 字符串替换
来源：http://wn.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kd.hahajie.cn

[R24] 大小写转换
来源：http://bo.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xy.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://zb.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ny.shxzukj.cn

[R26] 命令替换
来源：http://bu.yuexingan06.cn

now=$(date +%F); echo "$now"
来源：http://wv.chemitech.net.cn

[R27] 算术展开
来源：http://tu.asd995.cn

echo $((1 + 2 * 3))
来源：http://mo.muxihuayi.cn

[R28] 浮点运算
来源：http://ve.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://la.szsharing.cn

[R29] 定义函数
来源：http://tz.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mk.lnxyls.cn

[R30] 函数返回状态码
来源：http://pf.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://gi.huixinmuqiang.cn

[R31] 局部变量
来源：http://jm.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://mi.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://gn.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sc.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://jg.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rh.chemitech.net.cn

[R34] 退出时清理
来源：http://co.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nd.asd995.cn

[R35] 后台执行并等待
来源：http://ni.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pt.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://tb.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://st.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://jy.huanxung.cn

files=$(ls -1)
来源：http://nh.huanxung.cn

[R38] 管道串联
来源：http://oj.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://dw.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://am.haigaiapp.cn

cmd > out.log 2>&1
来源：http://ub.bookmarksfly.cn

[R40] 追加写日志
来源：http://zf.asd995.cn

echo "log" >> out.log
来源：http://wl.wgjwhj.cn

[R41] 丢弃输出
来源：http://st.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://ag.colortex.cn

[R42] 输入重定向
来源：http://cb.yuexingan06.cn

wc -l < a.txt
来源：http://bf.hahajie.cn

[R43] 按名字查找文件
来源：http://py.chemitech.net.cn

find . -name "*.log" -type f
来源：http://un.haigaiapp.cn

[R44] 按修改时间查找
来源：http://mw.haigaiapp.cn

find . -mtime -7 -type f
来源：http://hx.huixiangedu.cn

[R45] 批量删除
来源：http://lg.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://oy.9csxet.cn

[R46] 递归替换文件内容
来源：http://ah.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cu.521024.cn

[R47] sed 单行替换
来源：http://fq.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ka.huixiangedu.cn

[R48] awk 取指定列
来源：http://qs.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://mz.nszjky.cn

[R49] awk 带条件
来源：http://mn.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fm.shtwfgs.cn

[R50] awk 求和
来源：http://rc.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://in.521024.cn

[R51] 排序去重取前几
来源：http://cu.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yt.szsharing.cn

[R52] 统计行数
来源：http://am.chemitech.net.cn

wc -l a.txt
来源：http://ay.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://fm.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gp.newstarts.cn

[R54] 比较两个文件
来源：http://zr.bjjhwx.cn

diff a.txt b.txt
来源：http://ik.9csxet.cn

[R55] 压缩与解压
来源：http://mn.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pk.szxytkj.cn

[R56] 远程拷贝
来源：http://sx.bookmarksfly.cn

scp file user@host:/path/
来源：http://fm.bookmarksfly.cn

[R57] 远程执行命令
来源：http://eh.shxzukj.cn

ssh user@host 'uptime'
来源：http://tb.wgjwhj.cn

[R58] 下载文件
来源：http://nr.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kq.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://je.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hw.yuexingan06.cn

[R60] 只看 HTTP 状态码
来源：http://tu.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nh.521024.cn

[R61] 磁盘占用
来源：http://ci.hahajie.cn

df -h;  du -sh *
来源：http://go.shxzukj.cn

[R62] 找最占空间的文件
来源：http://um.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://xb.hnjuh.cn

[R63] 内存与进程
来源：http://op.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://bc.bookmarksfly.cn

[R64] 结束进程
来源：http://ql.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://mf.panjiajie.cn

[R65] 查看端口占用
来源：http://pk.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://os.yuexingan06.cn

[R66] 定时任务
来源：http://oz.9csxet.cn

crontab -e;  crontab -l
来源：http://md.jctech888.com.cn

[R67] 生成随机十六进制串
来源：http://ac.asd995.cn

openssl rand -hex 16
来源：http://nn.nszjky.cn

[R68] 计算文件校验值
来源：http://rv.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uz.huixiangedu.cn

[R69] 生成随机密码
来源：http://xm.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://eg.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://jv.521024.cn

date +%s;  date -d @1700000000
来源：http://da.muxihuayi.cn

[R71] 日期格式化
来源：http://bp.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cd.jctech888.com.cn

[R72] 等待端口就绪
来源：http://as.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gs.huixiangedu.cn

[R73] 分割大日志
来源：http://id.gzmigu.cn

split -l 1000 big.log part_
来源：http://vj.jctech888.com.cn

[R74] 批量重命名
来源：http://ap.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://px.huanxung.cn

[R75] 导出环境变量
来源：http://ux.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://yd.panjiajie.cn

[R76] 使用临时文件
来源：http://vc.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://am.haigaiapp.cn

[R77] 读取用户输入
来源：http://qy.colortex.cn

read -rp "请输入: " ans
来源：http://na.shtwfgs.cn

[R78] 交互式菜单
来源：http://bp.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://to.asd995.cn

[R79] 解析命令行选项
来源：http://lm.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://je.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://wb.huanxung.cn

time ./run.sh
来源：http://qs.newstarts.cn

================================================================================
来源：http://og.gzmigu.cn

S. C / C++ 专题
来源：http://jr.huixinmuqiang.cn

================================================================================
来源：http://xk.muxihuayi.cn

[S01] C：Hello World
来源：http://tk.chemitech.net.cn

#include <stdio.h>
来源：http://wk.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ha.szxytkj.cn

[S02] C：变量与格式化输出
来源：http://rj.shxzukj.cn

int a = 10; printf("%d\n", a);
来源：http://km.jianghongdianzi.cn

[S03] C：读入整数
来源：http://rt.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://ys.asd995.cn

[S04] C：字符串复制
来源：http://bj.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rt.szxytkj.cn

[S05] C：字符串长度
来源：http://sz.shxzskj.cn

strlen(s)
来源：http://vk.huanxung.cn

[S06] C：字符串比较
来源：http://mv.hnjuh.cn

strcmp(a, b) == 0
来源：http://ra.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://xv.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pn.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://jt.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fe.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://pg.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hb.asd995.cn

[S10] C：指针与解引用
来源：http://kv.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://em.hnjuh.cn

[S11] C：逐行读文件
来源：http://gb.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://xm.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nn.jctech888.com.cn

fclose(f);
来源：http://ae.huixinmuqiang.cn

[S12] C：写文件
来源：http://tw.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ro.hnjuh.cn

[S13] C：宏定义
来源：http://ke.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ft.jctech888.com.cn

[S14] C：枚举
来源：http://th.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://sj.asd995.cn

[S15] C：类型转换
来源：http://ta.chemitech.net.cn

(double) a / b
来源：http://cu.yuexingan06.cn

[S16] C：位操作置位
来源：http://jw.lnxyls.cn

x |= (1 << 3);
来源：http://ge.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://qw.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://og.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://fc.huanxung.cn

int main(int argc, char **argv)
来源：http://xy.nszjky.cn

[S19] C：快速排序
来源：http://ag.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zl.wgjwhj.cn

[S20] C：二分查找
来源：http://gt.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rq.521024.cn

[S21] C：字符类别判断
来源：http://cx.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bc.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://io.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tt.nszjky.cn

[S23] C：随机数
来源：http://eo.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ov.shxzskj.cn

[S24] C：获取本地时间
来源：http://ck.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ay.huanxung.cn

[S25] C：内存拷贝
来源：http://qh.wgjwhj.cn

memcpy(dst, src, n);
来源：http://li.huanxung.cn

[S26] C：内存清零
来源：http://kh.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://jy.szxytkj.cn

[S27] C：定义常量
来源：http://xn.shtwfgs.cn

const double PI = 3.14159;
来源：http://is.nicolike.cn

[S28] C：静态变量
来源：http://au.nszjky.cn

static int counter = 0;
来源：http://th.szsharing.cn

[S29] C：变参函数
来源：http://vb.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hs.jctech888.com.cn

[S30] C：头文件保护
来源：http://gx.lnxyls.cn

#ifndef X_H
来源：http://iz.yuntaijiaju.cn

#define X_H
来源：http://sp.huanxung.cn

#endif
来源：http://ff.asd995.cn

[S31] C++：Hello World
来源：http://fe.521024.cn

#include <iostream>
来源：http://hn.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://eo.9csxet.cn

[S32] C++：字符串
来源：http://qi.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://uz.hnjuh.cn

[S33] C++：vector 增删
来源：http://gl.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tx.asd995.cn

[S34] C++：遍历 vector
来源：http://hc.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://nz.yuntaijiaju.cn

[S35] C++：map
来源：http://al.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mi.colortex.cn

[S36] C++：unordered_map
来源：http://pz.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dz.wgjwhj.cn

[S37] C++：set
来源：http://vp.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wl.huixinmuqiang.cn

[S38] C++：排序
来源：http://lt.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://ze.521024.cn

[S39] C++：自定义比较器排序
来源：http://ez.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://le.shxzskj.cn

[S40] C++：查找元素
来源：http://qo.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yz.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://kx.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hh.colortex.cn

[S42] C++：继承与虚函数
来源：http://dj.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://oa.colortex.cn


<!-- 参考信息 -->