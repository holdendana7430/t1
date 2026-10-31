代发 wailian999

ROLLBACK TO sp1;
来源：http://zd.shtwfgs.cn

[Q69] 查看执行计划
来源：http://cc.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mo.shxzskj.cn

[Q70] 更新统计信息
来源：http://lx.asd995.cn

ANALYZE TABLE users;
来源：http://ag.haigaiapp.cn

[Q71] 查看建表语句
来源：http://sv.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nt.wgjwhj.cn

[Q72] 查看索引
来源：http://tb.nicolike.cn

SHOW INDEX FROM users;
来源：http://vi.nicolike.cn

[Q73] 查看表状态
来源：http://cn.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dh.haigaiapp.cn

[Q74] 强制使用索引
来源：http://dr.lnxyls.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ki.panjiajie.cn

[Q75] 日期格式化
来源：http://bd.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nd.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jm.szxytkj.cn

[Q76] 按天统计
来源：http://ee.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tg.shxzukj.cn

[Q77] 时间加减
来源：http://wp.jctech888.com.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rr.wgjwhj.cn

[Q78] 当前时间
来源：http://td.nicolike.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pa.colortex.cn

[Q79] 字符串拼接
来源：http://gn.colortex.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uq.muxihuayi.cn

[Q80] 字符串截取
来源：http://ks.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eh.huixiangedu.cn

[Q81] 字符串替换
来源：http://hy.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tg.muxihuayi.cn

[Q82] 字符长度与字节长度
来源：http://ek.yuntaijiaju.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hp.nicolike.cn

[Q83] 大小写转换
来源：http://xk.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gz.521024.cn

[Q84] 去除首尾空格
来源：http://bi.jctech888.com.cn

SELECT TRIM(name) FROM users;
来源：http://sj.nszjky.cn

[Q85] 数值取整
来源：http://yh.szxytkj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cw.jianghongdianzi.cn

[Q86] 读取 JSON 字段
来源：http://uq.chemitech.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ko.9csxet.cn

[Q87] JSON 字段做条件
来源：http://ln.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ef.muxihuayi.cn

[Q88] 行转列（条件聚合）
来源：http://vj.jctech888.com.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wh.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wi.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://hk.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fc.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://nb.jctech888.com.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uy.nszjky.cn

================================================================================
来源：http://iz.newstarts.cn

R. Bash 专题
来源：http://uy.asd995.cn

================================================================================
来源：http://ud.gzmigu.cn

[R01] shebang 与严格模式
来源：http://yz.jianghongdianzi.cn

#!/usr/bin/env bash
来源：http://na.yuexingan06.cn

set -euo pipefail
来源：http://nd.szxytkj.cn

[R02] 变量赋值与使用
来源：http://ti.yuntaijiaju.cn

name="Tom"; echo "$name"
来源：http://za.521024.cn

[R03] 只读变量
来源：http://po.yuexingan06.cn

readonly PI=3.14
来源：http://sp.colortex.cn

[R04] 位置参数
来源：http://vd.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vt.haigaiapp.cn

[R05] 参数默认值
来源：http://tc.shxzskj.cn

name="${1:-default}"
来源：http://ik.shxzukj.cn

[R06] 判断命令是否存在
来源：http://fg.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zq.shxzukj.cn

[R07] if 判断文件
来源：http://fl.9csxet.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ed.asd995.cn

[R08] 数值比较
来源：http://qq.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ec.lnxyls.cn

[R09] 字符串比较
来源：http://jt.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xs.hahajie.cn

[R10] 正则匹配
来源：http://tx.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ov.nszjky.cn

[R11] case 多分支
来源：http://zn.shxzukj.cn

case "$1" in
来源：http://ke.asd995.cn

start) echo "启动" ;;
来源：http://jo.panjiajie.cn

stop)  echo "停止" ;;
来源：http://gl.huanxung.cn

*)     echo "未知命令" ;;
来源：http://so.9csxet.cn

esac
来源：http://sk.shxzskj.cn

[R12] for 遍历文件
来源：http://wh.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://rd.jctech888.com.cn

[R13] for 计数循环
来源：http://fc.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://sh.haigaiapp.cn

[R14] C 风格 for
来源：http://gd.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sj.chemitech.net.cn

[R15] while 逐行读文件
来源：http://zt.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ki.gzmigu.cn

[R16] until 等待条件
来源：http://jw.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ss.shxzukj.cn

[R17] 数组定义与取值
来源：http://ep.bookmarksfly.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ut.huanxung.cn

[R18] 遍历数组
来源：http://ob.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yw.panjiajie.cn

[R19] 数组长度
来源：http://oy.szxytkj.cn

echo "${#arr[@]}"
来源：http://tr.hnjuh.cn

[R20] 关联数组（字典）
来源：http://bd.muxihuayi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uk.nicolike.cn

[R21] 字符串长度
来源：http://fz.bjjhwx.cn

echo "${#s}"
来源：http://ll.szxytkj.cn

[R22] 截取子串
来源：http://hv.gzmigu.cn

echo "${s:0:5}"
来源：http://yg.bookmarksfly.cn

[R23] 字符串替换
来源：http://hc.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aw.gzmigu.cn

[R24] 大小写转换
来源：http://ie.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ud.521024.cn

[R25] 去后缀 / 去前缀
来源：http://zn.huanxung.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xv.shtwfgs.cn

[R26] 命令替换
来源：http://ob.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://pl.huanxung.cn

[R27] 算术展开
来源：http://zt.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://xq.hahajie.cn

[R28] 浮点运算
来源：http://as.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://mx.nszjky.cn

[R29] 定义函数
来源：http://tf.yuexingan06.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tl.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://gu.shxzskj.cn

f() { return 0; }; f || echo "失败了"
来源：http://ei.hnjuh.cn

[R31] 局部变量
来源：http://nq.haigaiapp.cn

f() { local x=1; echo "$x"; }
来源：http://jk.szxytkj.cn

[R32] 参数个数校验
来源：http://rx.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gz.muxihuayi.cn

[R33] 捕获错误并提示行号
来源：http://ol.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xv.bjjhwx.cn

[R34] 退出时清理
来源：http://fr.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ju.lnxyls.cn

[R35] 后台执行并等待
来源：http://er.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://za.9csxet.cn

[R36] 并发执行多个任务
来源：http://li.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gh.huixinmuqiang.cn

[R37] 把输出赋给变量
来源：http://im.nszjky.cn

files=$(ls -1)
来源：http://dd.haigaiapp.cn

[R38] 管道串联
来源：http://on.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://ig.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://fn.hahajie.cn

cmd > out.log 2>&1
来源：http://ml.yuexingan06.cn

[R40] 追加写日志
来源：http://nx.yuexingan06.cn

echo "log" >> out.log
来源：http://gm.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://tw.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://rc.panjiajie.cn

[R42] 输入重定向
来源：http://qn.shtwfgs.cn

wc -l < a.txt
来源：http://ee.yuntaijiaju.cn

[R43] 按名字查找文件
来源：http://xf.szsharing.cn

find . -name "*.log" -type f
来源：http://fg.haigaiapp.cn

[R44] 按修改时间查找
来源：http://nt.bjjhwx.cn

find . -mtime -7 -type f
来源：http://kf.bjjhwx.cn

[R45] 批量删除
来源：http://pw.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://uj.yuexingan06.cn

[R46] 递归替换文件内容
来源：http://da.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ik.gzmigu.cn

[R47] sed 单行替换
来源：http://eh.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vg.huixiangedu.cn

[R48] awk 取指定列
来源：http://ed.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://ex.521024.cn

[R49] awk 带条件
来源：http://nv.muxihuayi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vk.hahajie.cn

[R50] awk 求和
来源：http://lg.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wh.gzmigu.cn

[R51] 排序去重取前几
来源：http://xy.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wt.szsharing.cn

[R52] 统计行数
来源：http://ss.huixiangedu.cn

wc -l a.txt
来源：http://gk.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://jw.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xc.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://nn.nicolike.cn

diff a.txt b.txt
来源：http://sq.huixiangedu.cn

[R55] 压缩与解压
来源：http://rt.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sz.shtwfgs.cn

[R56] 远程拷贝
来源：http://cb.huanxung.cn

scp file user@host:/path/
来源：http://pt.wgjwhj.cn

[R57] 远程执行命令
来源：http://gw.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://gr.gzmigu.cn

[R58] 下载文件
来源：http://ib.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mg.bjjhwx.cn

[R59] 发 POST JSON
来源：http://sp.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cm.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://vr.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hl.bjjhwx.cn

[R61] 磁盘占用
来源：http://xi.wgjwhj.cn

df -h;  du -sh *
来源：http://zm.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://fa.lnxyls.cn

du -ah . | sort -rh | head -10
来源：http://ba.newstarts.cn

[R63] 内存与进程
来源：http://ae.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://kr.chemitech.net.cn

[R64] 结束进程
来源：http://re.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://sb.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://vf.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ie.nicolike.cn

[R66] 定时任务
来源：http://zu.hnjuh.cn

crontab -e;  crontab -l
来源：http://el.521024.cn

[R67] 生成随机十六进制串
来源：http://of.panjiajie.cn

openssl rand -hex 16
来源：http://gu.lnxyls.cn

[R68] 计算文件校验值
来源：http://lu.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pl.wgjwhj.cn

[R69] 生成随机密码
来源：http://zo.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://nr.gzmigu.cn

[R70] 时间戳与互转
来源：http://op.hahajie.cn

date +%s;  date -d @1700000000
来源：http://xs.yuntaijiaju.cn

[R71] 日期格式化
来源：http://sq.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nm.shxzskj.cn

[R72] 等待端口就绪
来源：http://kx.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lv.9csxet.cn

[R73] 分割大日志
来源：http://nn.szsharing.cn

split -l 1000 big.log part_
来源：http://bm.nicolike.cn

[R74] 批量重命名
来源：http://yg.jctech888.com.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zv.wgjwhj.cn

[R75] 导出环境变量
来源：http://rr.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://rk.muxihuayi.cn

[R76] 使用临时文件
来源：http://dg.hahajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cb.521024.cn

[R77] 读取用户输入
来源：http://hy.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://aj.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://tp.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zf.bookmarksfly.cn

[R79] 解析命令行选项
来源：http://cb.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ou.nszjky.cn

[R80] 查看脚本执行耗时
来源：http://xc.yuexingan06.cn

time ./run.sh
来源：http://hw.shxzukj.cn

================================================================================
来源：http://ju.bookmarksfly.cn

S. C / C++ 专题
来源：http://et.panjiajie.cn

================================================================================
来源：http://dd.521024.cn

[S01] C：Hello World
来源：http://ws.yuntaijiaju.cn

#include <stdio.h>
来源：http://be.panjiajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sw.szxytkj.cn

[S02] C：变量与格式化输出
来源：http://mr.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://bj.huixiangedu.cn

[S03] C：读入整数
来源：http://sz.nszjky.cn

int x; scanf("%d", &x);
来源：http://to.shtwfgs.cn

[S04] C：字符串复制
来源：http://su.panjiajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qc.nicolike.cn

[S05] C：字符串长度
来源：http://gs.shxzukj.cn

strlen(s)
来源：http://nz.521024.cn

[S06] C：字符串比较
来源：http://sz.szxytkj.cn

strcmp(a, b) == 0
来源：http://do.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://gm.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://en.521024.cn

[S08] C：动态内存分配与释放
来源：http://ml.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rm.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://xg.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xp.wgjwhj.cn

[S10] C：指针与解引用
来源：http://nz.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://xr.shxzukj.cn

[S11] C：逐行读文件
来源：http://um.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://to.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wc.yuntaijiaju.cn

fclose(f);
来源：http://rf.gzmigu.cn

[S12] C：写文件
来源：http://lt.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ri.9csxet.cn

[S13] C：宏定义
来源：http://ml.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jw.shtwfgs.cn

[S14] C：枚举
来源：http://mm.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://kh.huanxung.cn

[S15] C：类型转换
来源：http://hn.521024.cn

(double) a / b
来源：http://na.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://sy.asd995.cn

x |= (1 << 3);
来源：http://gs.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://vy.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ji.szsharing.cn

[S18] C：命令行参数
来源：http://pm.jctech888.com.cn

int main(int argc, char **argv)
来源：http://cv.521024.cn

[S19] C：快速排序
来源：http://ii.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fl.asd995.cn

[S20] C：二分查找
来源：http://vs.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://un.newstarts.cn

[S21] C：字符类别判断
来源：http://iw.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zc.9csxet.cn

[S22] C：字符串转数字
来源：http://ya.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sq.nszjky.cn

[S23] C：随机数
来源：http://jl.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rs.bjjhwx.cn

[S24] C：获取本地时间
来源：http://ev.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gt.wgjwhj.cn

[S25] C：内存拷贝
来源：http://jr.shtwfgs.cn

memcpy(dst, src, n);
来源：http://cu.huixiangedu.cn

[S26] C：内存清零
来源：http://ka.colortex.cn

memset(a, 0, sizeof a);
来源：http://kx.asd995.cn

[S27] C：定义常量
来源：http://cb.yuexingan06.cn

const double PI = 3.14159;
来源：http://ki.szsharing.cn

[S28] C：静态变量
来源：http://tu.asd995.cn

static int counter = 0;
来源：http://wu.shxzukj.cn

[S29] C：变参函数
来源：http://gn.huanxung.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ez.haigaiapp.cn

[S30] C：头文件保护
来源：http://up.yuexingan06.cn

#ifndef X_H
来源：http://nx.shtwfgs.cn

#define X_H
来源：http://lg.huixinmuqiang.cn

#endif
来源：http://ex.9csxet.cn

[S31] C++：Hello World
来源：http://iw.colortex.cn

#include <iostream>
来源：http://ed.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://au.newstarts.cn

[S32] C++：字符串
来源：http://kx.huixinmuqiang.cn

std::string s = "hi";  s += "!";
来源：http://lw.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://kj.haigaiapp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://is.szxytkj.cn

[S34] C++：遍历 vector
来源：http://in.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://zb.jianghongdianzi.cn

[S35] C++：map
来源：http://xo.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tf.yuexingan06.cn

[S36] C++：unordered_map
来源：http://ra.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://la.huanxung.cn

[S37] C++：set
来源：http://pq.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ln.panjiajie.cn

[S38] C++：排序
来源：http://dh.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://cs.asd995.cn


<!-- 参考信息 -->