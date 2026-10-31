代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zt.hahajie.cn

[Q75] 日期格式化
来源：http://sw.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ec.haigaiapp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qj.jianghongdianzi.cn

[Q76] 按天统计
来源：http://ia.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uj.panjiajie.cn

[Q77] 时间加减
来源：http://bm.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://km.szsharing.cn

[Q78] 当前时间
来源：http://zf.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ds.newstarts.cn

[Q79] 字符串拼接
来源：http://qs.wgjwhj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ch.hahajie.cn

[Q80] 字符串截取
来源：http://nm.hahajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aa.bookmarksfly.cn

[Q81] 字符串替换
来源：http://ck.yuexingan06.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dq.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://xi.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xo.shxzskj.cn

[Q83] 大小写转换
来源：http://po.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dr.szsharing.cn

[Q84] 去除首尾空格
来源：http://te.haigaiapp.cn

SELECT TRIM(name) FROM users;
来源：http://ox.nicolike.cn

[Q85] 数值取整
来源：http://fe.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pi.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://dt.gzmigu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mw.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://hl.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ci.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://bj.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wn.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ek.asd995.cn

[Q89] 判断表是否存在
来源：http://dk.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ru.nicolike.cn

[Q90] 生成序号列
来源：http://lt.yuntaijiaju.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ck.hahajie.cn

================================================================================
来源：http://jy.muxihuayi.cn

R. Bash 专题
来源：http://jk.yuntaijiaju.cn

================================================================================
来源：http://nz.newstarts.cn

[R01] shebang 与严格模式
来源：http://kq.lnxyls.cn

#!/usr/bin/env bash
来源：http://px.shtwfgs.cn

set -euo pipefail
来源：http://uh.jianghongdianzi.cn

[R02] 变量赋值与使用
来源：http://fs.muxihuayi.cn

name="Tom"; echo "$name"
来源：http://nl.shtwfgs.cn

[R03] 只读变量
来源：http://sq.hnjuh.cn

readonly PI=3.14
来源：http://ri.panjiajie.cn

[R04] 位置参数
来源：http://ss.hnjuh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jx.haigaiapp.cn

[R05] 参数默认值
来源：http://qc.nszjky.cn

name="${1:-default}"
来源：http://wa.huanxung.cn

[R06] 判断命令是否存在
来源：http://wg.haigaiapp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gd.521024.cn

[R07] if 判断文件
来源：http://zx.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ug.huixiangedu.cn

[R08] 数值比较
来源：http://uq.nszjky.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://il.nszjky.cn

[R09] 字符串比较
来源：http://us.bookmarksfly.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cw.huixiangedu.cn

[R10] 正则匹配
来源：http://al.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oo.bjjhwx.cn

[R11] case 多分支
来源：http://sv.yuexingan06.cn

case "$1" in
来源：http://ov.asd995.cn

start) echo "启动" ;;
来源：http://le.521024.cn

stop)  echo "停止" ;;
来源：http://rt.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://ct.lnxyls.cn

esac
来源：http://sq.huanxung.cn

[R12] for 遍历文件
来源：http://ve.huixinmuqiang.cn

for f in *.txt; do echo "$f"; done
来源：http://ui.lnxyls.cn

[R13] for 计数循环
来源：http://bk.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://zb.haigaiapp.cn

[R14] C 风格 for
来源：http://we.hahajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qj.asd995.cn

[R15] while 逐行读文件
来源：http://su.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qh.yuntaijiaju.cn

[R16] until 等待条件
来源：http://yu.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ew.asd995.cn

[R17] 数组定义与取值
来源：http://oz.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mr.hahajie.cn

[R18] 遍历数组
来源：http://hy.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vj.wgjwhj.cn

[R19] 数组长度
来源：http://mb.shtwfgs.cn

echo "${#arr[@]}"
来源：http://cj.hnjuh.cn

[R20] 关联数组（字典）
来源：http://tw.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cl.yuntaijiaju.cn

[R21] 字符串长度
来源：http://cz.hahajie.cn

echo "${#s}"
来源：http://cq.hnjuh.cn

[R22] 截取子串
来源：http://hl.shtwfgs.cn

echo "${s:0:5}"
来源：http://tu.colortex.cn

[R23] 字符串替换
来源：http://ub.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eq.yuntaijiaju.cn

[R24] 大小写转换
来源：http://cx.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://di.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://ht.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cz.yuntaijiaju.cn

[R26] 命令替换
来源：http://zb.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://ty.nszjky.cn

[R27] 算术展开
来源：http://it.yuntaijiaju.cn

echo $((1 + 2 * 3))
来源：http://lv.chemitech.net.cn

[R28] 浮点运算
来源：http://cl.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://ua.yuntaijiaju.cn

[R29] 定义函数
来源：http://fb.yuexingan06.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://to.hahajie.cn

[R30] 函数返回状态码
来源：http://ye.9csxet.cn

f() { return 0; }; f || echo "失败了"
来源：http://eb.panjiajie.cn

[R31] 局部变量
来源：http://ek.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://wb.asd995.cn

[R32] 参数个数校验
来源：http://vz.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kx.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://av.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pb.hnjuh.cn

[R34] 退出时清理
来源：http://vu.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wl.9csxet.cn

[R35] 后台执行并等待
来源：http://ie.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ag.521024.cn

[R36] 并发执行多个任务
来源：http://ig.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://li.newstarts.cn

[R37] 把输出赋给变量
来源：http://nd.szsharing.cn

files=$(ls -1)
来源：http://fp.jctech888.com.cn

[R38] 管道串联
来源：http://jh.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://qv.shtwfgs.cn

[R39] 重定向标准输出与错误
来源：http://qi.asd995.cn

cmd > out.log 2>&1
来源：http://nl.bookmarksfly.cn

[R40] 追加写日志
来源：http://ye.asd995.cn

echo "log" >> out.log
来源：http://ow.asd995.cn

[R41] 丢弃输出
来源：http://bg.521024.cn

cmd >/dev/null 2>&1
来源：http://xh.bjjhwx.cn

[R42] 输入重定向
来源：http://xq.521024.cn

wc -l < a.txt
来源：http://uj.huixiangedu.cn

[R43] 按名字查找文件
来源：http://am.lnxyls.cn

find . -name "*.log" -type f
来源：http://kg.shxzukj.cn

[R44] 按修改时间查找
来源：http://iz.nszjky.cn

find . -mtime -7 -type f
来源：http://jc.jctech888.com.cn

[R45] 批量删除
来源：http://if.nicolike.cn

find . -name "*.tmp" -delete
来源：http://vj.yuexingan06.cn

[R46] 递归替换文件内容
来源：http://vt.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sq.huanxung.cn

[R47] sed 单行替换
来源：http://my.bookmarksfly.cn

sed -i 's/foo/bar/g' a.txt
来源：http://de.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://ay.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://yv.yuexingan06.cn

[R49] awk 带条件
来源：http://zm.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cp.hahajie.cn

[R50] awk 求和
来源：http://sl.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yt.wgjwhj.cn

[R51] 排序去重取前几
来源：http://ri.haigaiapp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bz.yuntaijiaju.cn

[R52] 统计行数
来源：http://kh.colortex.cn

wc -l a.txt
来源：http://ot.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://pz.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fr.haigaiapp.cn

[R54] 比较两个文件
来源：http://lb.gzmigu.cn

diff a.txt b.txt
来源：http://dc.lnxyls.cn

[R55] 压缩与解压
来源：http://qd.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ri.shxzskj.cn

[R56] 远程拷贝
来源：http://sb.bjjhwx.cn

scp file user@host:/path/
来源：http://mc.shxzukj.cn

[R57] 远程执行命令
来源：http://ol.jctech888.com.cn

ssh user@host 'uptime'
来源：http://xb.szxytkj.cn

[R58] 下载文件
来源：http://ri.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mi.hnjuh.cn

[R59] 发 POST JSON
来源：http://ht.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fe.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://jh.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hh.asd995.cn

[R61] 磁盘占用
来源：http://sg.szxytkj.cn

df -h;  du -sh *
来源：http://nx.szsharing.cn

[R62] 找最占空间的文件
来源：http://ke.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://ci.hahajie.cn

[R63] 内存与进程
来源：http://oh.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://ja.bookmarksfly.cn

[R64] 结束进程
来源：http://rx.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://hj.lnxyls.cn

[R65] 查看端口占用
来源：http://tp.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zo.jianghongdianzi.cn

[R66] 定时任务
来源：http://cy.nicolike.cn

crontab -e;  crontab -l
来源：http://vb.nicolike.cn

[R67] 生成随机十六进制串
来源：http://ry.521024.cn

openssl rand -hex 16
来源：http://km.nszjky.cn

[R68] 计算文件校验值
来源：http://qu.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kk.asd995.cn

[R69] 生成随机密码
来源：http://qh.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://lz.panjiajie.cn

[R70] 时间戳与互转
来源：http://rr.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://db.yuntaijiaju.cn

[R71] 日期格式化
来源：http://gl.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hc.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://np.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mw.newstarts.cn

[R73] 分割大日志
来源：http://kh.9csxet.cn

split -l 1000 big.log part_
来源：http://rj.colortex.cn

[R74] 批量重命名
来源：http://gs.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gh.gzmigu.cn

[R75] 导出环境变量
来源：http://sv.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://oe.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://an.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zv.hnjuh.cn

[R77] 读取用户输入
来源：http://eb.lnxyls.cn

read -rp "请输入: " ans
来源：http://vq.newstarts.cn

[R78] 交互式菜单
来源：http://gj.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ux.szsharing.cn

[R79] 解析命令行选项
来源：http://yy.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fj.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://ff.huanxung.cn

time ./run.sh
来源：http://qf.lnxyls.cn

================================================================================
来源：http://na.hahajie.cn

S. C / C++ 专题
来源：http://kq.jctech888.com.cn

================================================================================
来源：http://zp.gzmigu.cn

[S01] C：Hello World
来源：http://qs.huixiangedu.cn

#include <stdio.h>
来源：http://nm.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ys.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://dm.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://cc.colortex.cn

[S03] C：读入整数
来源：http://gq.hnjuh.cn

int x; scanf("%d", &x);
来源：http://du.szsharing.cn

[S04] C：字符串复制
来源：http://xo.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wv.szsharing.cn

[S05] C：字符串长度
来源：http://fd.9csxet.cn

strlen(s)
来源：http://kq.shtwfgs.cn

[S06] C：字符串比较
来源：http://ue.nicolike.cn

strcmp(a, b) == 0
来源：http://lq.shxzskj.cn

[S07] C：数组遍历求和
来源：http://ks.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qm.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://uq.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xw.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://fi.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ps.hnjuh.cn

[S10] C：指针与解引用
来源：http://he.nszjky.cn

int *p = &a;  *p = 5;
来源：http://ot.hahajie.cn

[S11] C：逐行读文件
来源：http://fh.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://bm.hnjuh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fd.bjjhwx.cn

fclose(f);
来源：http://ix.shxzskj.cn

[S12] C：写文件
来源：http://sh.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qm.nicolike.cn

[S13] C：宏定义
来源：http://pw.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cu.nicolike.cn

[S14] C：枚举
来源：http://qz.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://id.gzmigu.cn

[S15] C：类型转换
来源：http://vx.lnxyls.cn

(double) a / b
来源：http://zm.newstarts.cn

[S16] C：位操作置位
来源：http://mn.wgjwhj.cn

x |= (1 << 3);
来源：http://ag.hahajie.cn

[S17] C：安全拼接字符串
来源：http://zu.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ui.asd995.cn

[S18] C：命令行参数
来源：http://qo.asd995.cn

int main(int argc, char **argv)
来源：http://sn.bookmarksfly.cn

[S19] C：快速排序
来源：http://cw.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fk.huanxung.cn

[S20] C：二分查找
来源：http://en.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wy.panjiajie.cn

[S21] C：字符类别判断
来源：http://ws.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vu.huanxung.cn

[S22] C：字符串转数字
来源：http://ar.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ib.szsharing.cn

[S23] C：随机数
来源：http://du.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vt.shtwfgs.cn

[S24] C：获取本地时间
来源：http://br.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ew.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://eh.haigaiapp.cn

memcpy(dst, src, n);
来源：http://sx.muxihuayi.cn

[S26] C：内存清零
来源：http://yr.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://bm.shxzskj.cn

[S27] C：定义常量
来源：http://iw.haigaiapp.cn

const double PI = 3.14159;
来源：http://ia.yuntaijiaju.cn

[S28] C：静态变量
来源：http://kn.haigaiapp.cn

static int counter = 0;
来源：http://zc.yuntaijiaju.cn

[S29] C：变参函数
来源：http://fz.huixinmuqiang.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fs.wgjwhj.cn

[S30] C：头文件保护
来源：http://iz.panjiajie.cn

#ifndef X_H
来源：http://cu.gzmigu.cn

#define X_H
来源：http://tc.huanxung.cn

#endif
来源：http://gi.bookmarksfly.cn

[S31] C++：Hello World
来源：http://qh.shtwfgs.cn

#include <iostream>
来源：http://ll.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://wh.shxzukj.cn

[S32] C++：字符串
来源：http://yn.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://lt.nicolike.cn

[S33] C++：vector 增删
来源：http://zt.jctech888.com.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rl.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://ak.shxzskj.cn

for (auto &x : v) { std::cout << x; }
来源：http://iq.colortex.cn

[S35] C++：map
来源：http://de.lnxyls.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gc.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://tc.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cs.panjiajie.cn

[S37] C++：set
来源：http://gl.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bq.shxzskj.cn

[S38] C++：排序
来源：http://ki.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://zt.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://zu.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fo.jctech888.com.cn

[S40] C++：查找元素
来源：http://yq.jianghongdianzi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ta.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://yj.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fr.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://ht.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://cv.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://rs.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://ts.newstarts.cn

[S44] C++：引用传参
来源：http://ih.nszjky.cn

void inc(int &x) { ++x; }
来源：http://xn.colortex.cn


<!-- 参考信息 -->