代发 wailian999

SHOW INDEX FROM users;
来源：http://xo.bookmarksfly.cn

[Q73] 查看表状态
来源：http://uq.newstarts.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pm.szsharing.cn

[Q74] 强制使用索引
来源：http://hp.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lx.bjjhwx.cn

[Q75] 日期格式化
来源：http://fl.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://po.bjjhwx.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ud.hnjuh.cn

[Q76] 按天统计
来源：http://cb.muxihuayi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yd.nicolike.cn

[Q77] 时间加减
来源：http://ch.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mz.muxihuayi.cn

[Q78] 当前时间
来源：http://kn.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jz.asd995.cn

[Q79] 字符串拼接
来源：http://kd.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gf.shxzskj.cn

[Q80] 字符串截取
来源：http://kk.hahajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fs.gzmigu.cn

[Q81] 字符串替换
来源：http://jw.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ec.chemitech.net.cn

[Q82] 字符长度与字节长度
来源：http://eb.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cy.chemitech.net.cn

[Q83] 大小写转换
来源：http://qw.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gc.9csxet.cn

[Q84] 去除首尾空格
来源：http://px.colortex.cn

SELECT TRIM(name) FROM users;
来源：http://rb.wgjwhj.cn

[Q85] 数值取整
来源：http://vt.huixinmuqiang.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ny.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://jp.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pu.huixinmuqiang.cn

[Q87] JSON 字段做条件
来源：http://at.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xz.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://se.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ni.lnxyls.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bu.521024.cn

[Q89] 判断表是否存在
来源：http://qc.521024.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ix.huixiangedu.cn

[Q90] 生成序号列
来源：http://xh.shxzukj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gp.nicolike.cn

================================================================================
来源：http://hk.bjjhwx.cn

R. Bash 专题
来源：http://oo.jctech888.com.cn

================================================================================
来源：http://fs.asd995.cn

[R01] shebang 与严格模式
来源：http://eo.shtwfgs.cn

#!/usr/bin/env bash
来源：http://be.newstarts.cn

set -euo pipefail
来源：http://dk.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://qp.szxytkj.cn

name="Tom"; echo "$name"
来源：http://pq.chemitech.net.cn

[R03] 只读变量
来源：http://uv.521024.cn

readonly PI=3.14
来源：http://vl.jctech888.com.cn

[R04] 位置参数
来源：http://tj.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lf.haigaiapp.cn

[R05] 参数默认值
来源：http://ga.muxihuayi.cn

name="${1:-default}"
来源：http://oq.shxzskj.cn

[R06] 判断命令是否存在
来源：http://uo.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vl.bjjhwx.cn

[R07] if 判断文件
来源：http://lt.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gg.nszjky.cn

[R08] 数值比较
来源：http://al.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dt.9csxet.cn

[R09] 字符串比较
来源：http://zm.nszjky.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zn.newstarts.cn

[R10] 正则匹配
来源：http://nl.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dm.shxzskj.cn

[R11] case 多分支
来源：http://jy.newstarts.cn

case "$1" in
来源：http://au.jctech888.com.cn

start) echo "启动" ;;
来源：http://fu.bookmarksfly.cn

stop)  echo "停止" ;;
来源：http://am.asd995.cn

*)     echo "未知命令" ;;
来源：http://qw.9csxet.cn

esac
来源：http://ea.521024.cn

[R12] for 遍历文件
来源：http://of.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://bn.huixinmuqiang.cn

[R13] for 计数循环
来源：http://kz.haigaiapp.cn

for i in {1..10}; do echo "$i"; done
来源：http://xe.shtwfgs.cn

[R14] C 风格 for
来源：http://qt.yuexingan06.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mb.wgjwhj.cn

[R15] while 逐行读文件
来源：http://iw.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sy.lnxyls.cn

[R16] until 等待条件
来源：http://vp.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oc.hnjuh.cn

[R17] 数组定义与取值
来源：http://fa.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pd.lnxyls.cn

[R18] 遍历数组
来源：http://qu.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gq.lnxyls.cn

[R19] 数组长度
来源：http://gl.hnjuh.cn

echo "${#arr[@]}"
来源：http://gr.colortex.cn

[R20] 关联数组（字典）
来源：http://cj.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nk.jctech888.com.cn

[R21] 字符串长度
来源：http://vb.muxihuayi.cn

echo "${#s}"
来源：http://hh.9csxet.cn

[R22] 截取子串
来源：http://pt.shxzukj.cn

echo "${s:0:5}"
来源：http://fm.yuntaijiaju.cn

[R23] 字符串替换
来源：http://kv.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ag.szsharing.cn

[R24] 大小写转换
来源：http://fn.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tz.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://jo.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dl.chemitech.net.cn

[R26] 命令替换
来源：http://jh.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://vr.chemitech.net.cn

[R27] 算术展开
来源：http://vk.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://yx.yuntaijiaju.cn

[R28] 浮点运算
来源：http://pj.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://lg.muxihuayi.cn

[R29] 定义函数
来源：http://yj.colortex.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tz.lnxyls.cn

[R30] 函数返回状态码
来源：http://gg.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://bf.huixinmuqiang.cn

[R31] 局部变量
来源：http://sp.hnjuh.cn

f() { local x=1; echo "$x"; }
来源：http://wz.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://cq.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fu.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://lf.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bv.yuntaijiaju.cn

[R34] 退出时清理
来源：http://gb.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://oy.lnxyls.cn

[R35] 后台执行并等待
来源：http://fe.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oh.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://sh.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sb.szsharing.cn

[R37] 把输出赋给变量
来源：http://bv.yuexingan06.cn

files=$(ls -1)
来源：http://vs.9csxet.cn

[R38] 管道串联
来源：http://cf.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://ov.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://ph.szxytkj.cn

cmd > out.log 2>&1
来源：http://ly.9csxet.cn

[R40] 追加写日志
来源：http://kz.jianghongdianzi.cn

echo "log" >> out.log
来源：http://mw.lnxyls.cn

[R41] 丢弃输出
来源：http://gg.jctech888.com.cn

cmd >/dev/null 2>&1
来源：http://mr.panjiajie.cn

[R42] 输入重定向
来源：http://fh.bjjhwx.cn

wc -l < a.txt
来源：http://kk.gzmigu.cn

[R43] 按名字查找文件
来源：http://xl.jctech888.com.cn

find . -name "*.log" -type f
来源：http://sx.nicolike.cn

[R44] 按修改时间查找
来源：http://se.muxihuayi.cn

find . -mtime -7 -type f
来源：http://da.shtwfgs.cn

[R45] 批量删除
来源：http://qk.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://ki.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://pg.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://do.shxzukj.cn

[R47] sed 单行替换
来源：http://rk.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yc.huanxung.cn

[R48] awk 取指定列
来源：http://fw.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://nj.yuntaijiaju.cn

[R49] awk 带条件
来源：http://am.huixinmuqiang.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vq.huixiangedu.cn

[R50] awk 求和
来源：http://ti.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tl.asd995.cn

[R51] 排序去重取前几
来源：http://ix.yuexingan06.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ok.lnxyls.cn

[R52] 统计行数
来源：http://ai.colortex.cn

wc -l a.txt
来源：http://rv.shtwfgs.cn

[R53] 查看文件头与实时尾
来源：http://ub.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://eo.shxzskj.cn

[R54] 比较两个文件
来源：http://jf.asd995.cn

diff a.txt b.txt
来源：http://vj.hahajie.cn

[R55] 压缩与解压
来源：http://qs.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xj.colortex.cn

[R56] 远程拷贝
来源：http://io.muxihuayi.cn

scp file user@host:/path/
来源：http://to.nicolike.cn

[R57] 远程执行命令
来源：http://wa.szxytkj.cn

ssh user@host 'uptime'
来源：http://hh.jctech888.com.cn

[R58] 下载文件
来源：http://lr.colortex.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nq.panjiajie.cn

[R59] 发 POST JSON
来源：http://cz.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://og.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://th.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vn.haigaiapp.cn

[R61] 磁盘占用
来源：http://vc.chemitech.net.cn

df -h;  du -sh *
来源：http://wf.hahajie.cn

[R62] 找最占空间的文件
来源：http://yp.colortex.cn

du -ah . | sort -rh | head -10
来源：http://xm.colortex.cn

[R63] 内存与进程
来源：http://au.newstarts.cn

free -h;  ps aux | grep nginx
来源：http://yw.shtwfgs.cn

[R64] 结束进程
来源：http://sv.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://nq.bookmarksfly.cn

[R65] 查看端口占用
来源：http://jo.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ly.chemitech.net.cn

[R66] 定时任务
来源：http://lp.huanxung.cn

crontab -e;  crontab -l
来源：http://bs.asd995.cn

[R67] 生成随机十六进制串
来源：http://kq.bookmarksfly.cn

openssl rand -hex 16
来源：http://xk.yuexingan06.cn

[R68] 计算文件校验值
来源：http://kw.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gh.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://ax.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://ec.gzmigu.cn

[R70] 时间戳与互转
来源：http://lz.panjiajie.cn

date +%s;  date -d @1700000000
来源：http://nx.bjjhwx.cn

[R71] 日期格式化
来源：http://fs.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ob.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://fa.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rj.asd995.cn

[R73] 分割大日志
来源：http://kr.wgjwhj.cn

split -l 1000 big.log part_
来源：http://ba.521024.cn

[R74] 批量重命名
来源：http://dd.haigaiapp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://um.nszjky.cn

[R75] 导出环境变量
来源：http://gl.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://wz.shtwfgs.cn

[R76] 使用临时文件
来源：http://as.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cj.hahajie.cn

[R77] 读取用户输入
来源：http://uo.nszjky.cn

read -rp "请输入: " ans
来源：http://un.huixiangedu.cn

[R78] 交互式菜单
来源：http://pm.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lp.szxytkj.cn

[R79] 解析命令行选项
来源：http://rv.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ce.wgjwhj.cn

[R80] 查看脚本执行耗时
来源：http://gq.muxihuayi.cn

time ./run.sh
来源：http://bn.gzmigu.cn

================================================================================
来源：http://np.shtwfgs.cn

S. C / C++ 专题
来源：http://iv.gzmigu.cn

================================================================================
来源：http://we.panjiajie.cn

[S01] C：Hello World
来源：http://ok.nszjky.cn

#include <stdio.h>
来源：http://jm.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qr.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://qh.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://jo.shxzskj.cn

[S03] C：读入整数
来源：http://va.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://ss.shxzukj.cn

[S04] C：字符串复制
来源：http://tk.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://px.colortex.cn

[S05] C：字符串长度
来源：http://sq.szsharing.cn

strlen(s)
来源：http://jq.newstarts.cn

[S06] C：字符串比较
来源：http://ml.jctech888.com.cn

strcmp(a, b) == 0
来源：http://lo.bookmarksfly.cn

[S07] C：数组遍历求和
来源：http://so.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fv.asd995.cn

[S08] C：动态内存分配与释放
来源：http://wt.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vy.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://rp.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hq.shtwfgs.cn

[S10] C：指针与解引用
来源：http://ae.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://cc.bjjhwx.cn

[S11] C：逐行读文件
来源：http://rl.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://pt.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sj.huanxung.cn

fclose(f);
来源：http://mp.szxytkj.cn

[S12] C：写文件
来源：http://ui.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://en.bookmarksfly.cn

[S13] C：宏定义
来源：http://sj.newstarts.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wa.haigaiapp.cn

[S14] C：枚举
来源：http://bo.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://ov.bookmarksfly.cn

[S15] C：类型转换
来源：http://xt.haigaiapp.cn

(double) a / b
来源：http://fi.jctech888.com.cn

[S16] C：位操作置位
来源：http://mc.bookmarksfly.cn

x |= (1 << 3);
来源：http://ti.9csxet.cn

[S17] C：安全拼接字符串
来源：http://xm.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://en.muxihuayi.cn

[S18] C：命令行参数
来源：http://hc.panjiajie.cn

int main(int argc, char **argv)
来源：http://np.9csxet.cn

[S19] C：快速排序
来源：http://aw.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wp.nszjky.cn

[S20] C：二分查找
来源：http://tu.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ue.jctech888.com.cn

[S21] C：字符类别判断
来源：http://ym.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bz.panjiajie.cn

[S22] C：字符串转数字
来源：http://yf.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cn.nszjky.cn

[S23] C：随机数
来源：http://rh.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tr.jctech888.com.cn

[S24] C：获取本地时间
来源：http://yf.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ni.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://qz.shxzukj.cn

memcpy(dst, src, n);
来源：http://dd.521024.cn

[S26] C：内存清零
来源：http://bp.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://oi.yuexingan06.cn

[S27] C：定义常量
来源：http://eb.nicolike.cn

const double PI = 3.14159;
来源：http://ij.bookmarksfly.cn

[S28] C：静态变量
来源：http://jg.szsharing.cn

static int counter = 0;
来源：http://hh.huixiangedu.cn

[S29] C：变参函数
来源：http://kc.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uq.hahajie.cn

[S30] C：头文件保护
来源：http://fg.huanxung.cn

#ifndef X_H
来源：http://jk.nicolike.cn

#define X_H
来源：http://wb.521024.cn

#endif
来源：http://rm.bookmarksfly.cn

[S31] C++：Hello World
来源：http://kd.gzmigu.cn

#include <iostream>
来源：http://jg.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://zq.huixiangedu.cn

[S32] C++：字符串
来源：http://gc.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://ed.9csxet.cn

[S33] C++：vector 增删
来源：http://zq.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://he.lnxyls.cn

[S34] C++：遍历 vector
来源：http://ng.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://pg.bookmarksfly.cn

[S35] C++：map
来源：http://cg.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zm.jctech888.com.cn

[S36] C++：unordered_map
来源：http://mc.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vu.gzmigu.cn

[S37] C++：set
来源：http://qg.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://un.nszjky.cn

[S38] C++：排序
来源：http://pb.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://iz.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://qt.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cr.huixiangedu.cn

[S40] C++：查找元素
来源：http://hk.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://he.colortex.cn

[S41] C++：类与构造函数
来源：http://ot.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mu.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://pz.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://ke.wgjwhj.cn


<!-- 参考信息 -->