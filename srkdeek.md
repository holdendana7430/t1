代发 wailian999

ROLLBACK TO sp1;
来源：http://ax.muxihuayi.cn

[Q69] 查看执行计划
来源：http://cq.newstarts.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nj.gzmigu.cn

[Q70] 更新统计信息
来源：http://og.szsharing.cn

ANALYZE TABLE users;
来源：http://fd.nicolike.cn

[Q71] 查看建表语句
来源：http://dy.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hr.shxzskj.cn

[Q72] 查看索引
来源：http://oq.asd995.cn

SHOW INDEX FROM users;
来源：http://vq.9csxet.cn

[Q73] 查看表状态
来源：http://wr.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://km.shtwfgs.cn

[Q74] 强制使用索引
来源：http://be.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sq.colortex.cn

[Q75] 日期格式化
来源：http://dw.gzmigu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rv.muxihuayi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jm.nicolike.cn

[Q76] 按天统计
来源：http://al.panjiajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lt.521024.cn

[Q77] 时间加减
来源：http://sq.9csxet.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://or.huixiangedu.cn

[Q78] 当前时间
来源：http://ws.jianghongdianzi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uw.jianghongdianzi.cn

[Q79] 字符串拼接
来源：http://sz.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xu.bjjhwx.cn

[Q80] 字符串截取
来源：http://gl.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qn.bjjhwx.cn

[Q81] 字符串替换
来源：http://af.colortex.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ag.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://kf.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yn.shxzskj.cn

[Q83] 大小写转换
来源：http://mp.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mg.9csxet.cn

[Q84] 去除首尾空格
来源：http://pv.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://ku.haigaiapp.cn

[Q85] 数值取整
来源：http://sb.panjiajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://do.asd995.cn

[Q86] 读取 JSON 字段
来源：http://ua.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pq.bookmarksfly.cn

[Q87] JSON 字段做条件
来源：http://xe.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://td.9csxet.cn

[Q88] 行转列（条件聚合）
来源：http://eb.huixiangedu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oa.lnxyls.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sf.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://yq.szsharing.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oo.lnxyls.cn

[Q90] 生成序号列
来源：http://am.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bi.bjjhwx.cn

================================================================================
来源：http://cy.haigaiapp.cn

R. Bash 专题
来源：http://ag.huixiangedu.cn

================================================================================
来源：http://hc.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://nl.nicolike.cn

#!/usr/bin/env bash
来源：http://fj.chemitech.net.cn

set -euo pipefail
来源：http://bs.colortex.cn

[R02] 变量赋值与使用
来源：http://tl.hahajie.cn

name="Tom"; echo "$name"
来源：http://jt.szsharing.cn

[R03] 只读变量
来源：http://lg.hahajie.cn

readonly PI=3.14
来源：http://bc.shxzukj.cn

[R04] 位置参数
来源：http://sn.colortex.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dr.chemitech.net.cn

[R05] 参数默认值
来源：http://eh.shxzukj.cn

name="${1:-default}"
来源：http://wm.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://co.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://os.shtwfgs.cn

[R07] if 判断文件
来源：http://yn.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aj.nszjky.cn

[R08] 数值比较
来源：http://hy.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ya.gzmigu.cn

[R09] 字符串比较
来源：http://vb.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ca.bookmarksfly.cn

[R10] 正则匹配
来源：http://bl.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jq.colortex.cn

[R11] case 多分支
来源：http://uq.hnjuh.cn

case "$1" in
来源：http://sv.asd995.cn

start) echo "启动" ;;
来源：http://rz.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://pt.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://fv.colortex.cn

esac
来源：http://xi.newstarts.cn

[R12] for 遍历文件
来源：http://tr.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://af.huixinmuqiang.cn

[R13] for 计数循环
来源：http://fj.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://rv.shtwfgs.cn

[R14] C 风格 for
来源：http://pc.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dr.hnjuh.cn

[R15] while 逐行读文件
来源：http://he.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fd.bookmarksfly.cn

[R16] until 等待条件
来源：http://as.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://np.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://zf.jianghongdianzi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nk.huanxung.cn

[R18] 遍历数组
来源：http://zs.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sv.colortex.cn

[R19] 数组长度
来源：http://vb.shtwfgs.cn

echo "${#arr[@]}"
来源：http://jb.szsharing.cn

[R20] 关联数组（字典）
来源：http://ey.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hl.muxihuayi.cn

[R21] 字符串长度
来源：http://wk.shxzukj.cn

echo "${#s}"
来源：http://mr.huixiangedu.cn

[R22] 截取子串
来源：http://is.gzmigu.cn

echo "${s:0:5}"
来源：http://fa.chemitech.net.cn

[R23] 字符串替换
来源：http://xi.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jb.lnxyls.cn

[R24] 大小写转换
来源：http://hq.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uy.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://zu.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yq.nszjky.cn

[R26] 命令替换
来源：http://jc.haigaiapp.cn

now=$(date +%F); echo "$now"
来源：http://gp.shxzskj.cn

[R27] 算术展开
来源：http://ce.521024.cn

echo $((1 + 2 * 3))
来源：http://ao.szxytkj.cn

[R28] 浮点运算
来源：http://rg.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://xi.muxihuayi.cn

[R29] 定义函数
来源：http://wz.yuexingan06.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://on.muxihuayi.cn

[R30] 函数返回状态码
来源：http://cu.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://oy.shtwfgs.cn

[R31] 局部变量
来源：http://ly.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://sl.wgjwhj.cn

[R32] 参数个数校验
来源：http://pp.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yq.521024.cn

[R33] 捕获错误并提示行号
来源：http://gx.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://li.wgjwhj.cn

[R34] 退出时清理
来源：http://yx.huixinmuqiang.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hd.panjiajie.cn

[R35] 后台执行并等待
来源：http://aa.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nj.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://iv.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pe.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://mn.szsharing.cn

files=$(ls -1)
来源：http://ky.shxzukj.cn

[R38] 管道串联
来源：http://hh.shxzukj.cn

cat a.txt | grep -i error | wc -l
来源：http://le.jianghongdianzi.cn

[R39] 重定向标准输出与错误
来源：http://ff.hnjuh.cn

cmd > out.log 2>&1
来源：http://yp.huixinmuqiang.cn

[R40] 追加写日志
来源：http://xg.huanxung.cn

echo "log" >> out.log
来源：http://uu.szxytkj.cn

[R41] 丢弃输出
来源：http://ut.nicolike.cn

cmd >/dev/null 2>&1
来源：http://vi.panjiajie.cn

[R42] 输入重定向
来源：http://ns.shxzskj.cn

wc -l < a.txt
来源：http://mf.shtwfgs.cn

[R43] 按名字查找文件
来源：http://cb.szsharing.cn

find . -name "*.log" -type f
来源：http://xw.521024.cn

[R44] 按修改时间查找
来源：http://xd.szsharing.cn

find . -mtime -7 -type f
来源：http://kt.jctech888.com.cn

[R45] 批量删除
来源：http://if.hahajie.cn

find . -name "*.tmp" -delete
来源：http://qy.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://up.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lo.panjiajie.cn

[R47] sed 单行替换
来源：http://ji.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wg.muxihuayi.cn

[R48] awk 取指定列
来源：http://ia.hahajie.cn

awk '{print $1, $3}' a.txt
来源：http://vo.shtwfgs.cn

[R49] awk 带条件
来源：http://xn.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://my.9csxet.cn

[R50] awk 求和
来源：http://dk.bookmarksfly.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fm.newstarts.cn

[R51] 排序去重取前几
来源：http://fn.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lx.yuexingan06.cn

[R52] 统计行数
来源：http://ro.hnjuh.cn

wc -l a.txt
来源：http://bk.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://vq.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lq.521024.cn

[R54] 比较两个文件
来源：http://pk.wgjwhj.cn

diff a.txt b.txt
来源：http://iy.gzmigu.cn

[R55] 压缩与解压
来源：http://lc.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jk.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://ee.521024.cn

scp file user@host:/path/
来源：http://il.shtwfgs.cn

[R57] 远程执行命令
来源：http://jv.shtwfgs.cn

ssh user@host 'uptime'
来源：http://ah.wgjwhj.cn

[R58] 下载文件
来源：http://ol.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gx.bjjhwx.cn

[R59] 发 POST JSON
来源：http://nk.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://za.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://hn.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://of.hahajie.cn

[R61] 磁盘占用
来源：http://pv.nszjky.cn

df -h;  du -sh *
来源：http://gy.panjiajie.cn

[R62] 找最占空间的文件
来源：http://su.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://kf.521024.cn

[R63] 内存与进程
来源：http://of.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://kx.yuexingan06.cn

[R64] 结束进程
来源：http://ku.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://as.shxzskj.cn

[R65] 查看端口占用
来源：http://ug.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nd.huixinmuqiang.cn

[R66] 定时任务
来源：http://lw.huanxung.cn

crontab -e;  crontab -l
来源：http://jj.szsharing.cn

[R67] 生成随机十六进制串
来源：http://pk.hahajie.cn

openssl rand -hex 16
来源：http://uu.shtwfgs.cn

[R68] 计算文件校验值
来源：http://su.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ct.bjjhwx.cn

[R69] 生成随机密码
来源：http://pf.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://es.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://jh.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://ti.521024.cn

[R71] 日期格式化
来源：http://lq.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dg.haigaiapp.cn

[R72] 等待端口就绪
来源：http://uq.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yi.huanxung.cn

[R73] 分割大日志
来源：http://jo.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://ac.szsharing.cn

[R74] 批量重命名
来源：http://yv.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wt.nicolike.cn

[R75] 导出环境变量
来源：http://zg.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://ou.nszjky.cn

[R76] 使用临时文件
来源：http://vh.huixinmuqiang.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xj.haigaiapp.cn

[R77] 读取用户输入
来源：http://ja.hahajie.cn

read -rp "请输入: " ans
来源：http://yn.hahajie.cn

[R78] 交互式菜单
来源：http://qf.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fy.shtwfgs.cn

[R79] 解析命令行选项
来源：http://eq.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nk.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://na.bookmarksfly.cn

time ./run.sh
来源：http://kn.jctech888.com.cn

================================================================================
来源：http://sl.szxytkj.cn

S. C / C++ 专题
来源：http://hu.shtwfgs.cn

================================================================================
来源：http://bg.nszjky.cn

[S01] C：Hello World
来源：http://ms.huanxung.cn

#include <stdio.h>
来源：http://oz.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jm.9csxet.cn

[S02] C：变量与格式化输出
来源：http://rt.gzmigu.cn

int a = 10; printf("%d\n", a);
来源：http://uo.wgjwhj.cn

[S03] C：读入整数
来源：http://pp.huanxung.cn

int x; scanf("%d", &x);
来源：http://ru.szsharing.cn

[S04] C：字符串复制
来源：http://rp.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ln.jianghongdianzi.cn

[S05] C：字符串长度
来源：http://sg.gzmigu.cn

strlen(s)
来源：http://ip.haigaiapp.cn

[S06] C：字符串比较
来源：http://jv.panjiajie.cn

strcmp(a, b) == 0
来源：http://yd.lnxyls.cn

[S07] C：数组遍历求和
来源：http://ze.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://er.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://nm.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gx.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://gl.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ph.hnjuh.cn

[S10] C：指针与解引用
来源：http://od.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://se.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://co.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://yc.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mr.521024.cn

fclose(f);
来源：http://fc.colortex.cn

[S12] C：写文件
来源：http://my.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eu.panjiajie.cn

[S13] C：宏定义
来源：http://mn.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qn.nszjky.cn

[S14] C：枚举
来源：http://fm.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://vi.haigaiapp.cn

[S15] C：类型转换
来源：http://uj.yuexingan06.cn

(double) a / b
来源：http://ue.yuexingan06.cn

[S16] C：位操作置位
来源：http://fa.huanxung.cn

x |= (1 << 3);
来源：http://gf.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://jz.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ob.bookmarksfly.cn

[S18] C：命令行参数
来源：http://zd.shxzukj.cn

int main(int argc, char **argv)
来源：http://kx.szxytkj.cn

[S19] C：快速排序
来源：http://mx.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kw.haigaiapp.cn

[S20] C：二分查找
来源：http://jn.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://co.szxytkj.cn

[S21] C：字符类别判断
来源：http://xp.jianghongdianzi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zl.szsharing.cn

[S22] C：字符串转数字
来源：http://dv.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ax.lnxyls.cn

[S23] C：随机数
来源：http://qx.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://iv.shxzukj.cn

[S24] C：获取本地时间
来源：http://nt.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dz.shxzukj.cn

[S25] C：内存拷贝
来源：http://xz.gzmigu.cn

memcpy(dst, src, n);
来源：http://zc.muxihuayi.cn

[S26] C：内存清零
来源：http://zf.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://jr.bookmarksfly.cn

[S27] C：定义常量
来源：http://zz.521024.cn

const double PI = 3.14159;
来源：http://pt.huanxung.cn

[S28] C：静态变量
来源：http://vh.hnjuh.cn

static int counter = 0;
来源：http://wg.521024.cn

[S29] C：变参函数
来源：http://fo.huixinmuqiang.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ai.nszjky.cn

[S30] C：头文件保护
来源：http://gd.panjiajie.cn

#ifndef X_H
来源：http://ut.newstarts.cn

#define X_H
来源：http://un.szsharing.cn

#endif
来源：http://lt.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://ly.yuntaijiaju.cn

#include <iostream>
来源：http://fx.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://bj.asd995.cn

[S32] C++：字符串
来源：http://xf.colortex.cn

std::string s = "hi";  s += "!";
来源：http://jz.gzmigu.cn

[S33] C++：vector 增删
来源：http://js.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yf.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://br.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://xl.yuexingan06.cn

[S35] C++：map
来源：http://za.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gi.wgjwhj.cn

[S36] C++：unordered_map
来源：http://jr.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://aq.gzmigu.cn

[S37] C++：set
来源：http://mn.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ev.shxzukj.cn

[S38] C++：排序
来源：http://xv.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://ur.szsharing.cn


<!-- 参考信息 -->