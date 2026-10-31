代发 wailian999

ANALYZE TABLE users;
来源：http://qz.newstarts.cn

[Q71] 查看建表语句
来源：http://ci.muxihuayi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ii.hahajie.cn

[Q72] 查看索引
来源：http://tp.haigaiapp.cn

SHOW INDEX FROM users;
来源：http://hy.bjjhwx.cn

[Q73] 查看表状态
来源：http://ju.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://he.lnxyls.cn

[Q74] 强制使用索引
来源：http://pc.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xd.newstarts.cn

[Q75] 日期格式化
来源：http://ho.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ca.bookmarksfly.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cc.panjiajie.cn

[Q76] 按天统计
来源：http://cp.colortex.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ht.chemitech.net.cn

[Q77] 时间加减
来源：http://rq.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ih.shxzukj.cn

[Q78] 当前时间
来源：http://rm.huixiangedu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nz.colortex.cn

[Q79] 字符串拼接
来源：http://be.asd995.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oa.muxihuayi.cn

[Q80] 字符串截取
来源：http://wp.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dz.chemitech.net.cn

[Q81] 字符串替换
来源：http://rm.newstarts.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fd.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://hd.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sk.wgjwhj.cn

[Q83] 大小写转换
来源：http://vt.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rr.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://of.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://pw.nicolike.cn

[Q85] 数值取整
来源：http://vd.9csxet.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uu.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://fz.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bv.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://zl.huixinmuqiang.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lz.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://qq.jctech888.com.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xp.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iy.newstarts.cn

[Q89] 判断表是否存在
来源：http://lf.haigaiapp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vr.hnjuh.cn

[Q90] 生成序号列
来源：http://wm.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ch.nszjky.cn

================================================================================
来源：http://qw.muxihuayi.cn

R. Bash 专题
来源：http://dh.newstarts.cn

================================================================================
来源：http://ek.9csxet.cn

[R01] shebang 与严格模式
来源：http://um.nicolike.cn

#!/usr/bin/env bash
来源：http://rf.yuntaijiaju.cn

set -euo pipefail
来源：http://da.colortex.cn

[R02] 变量赋值与使用
来源：http://gn.shxzskj.cn

name="Tom"; echo "$name"
来源：http://yx.szxytkj.cn

[R03] 只读变量
来源：http://yp.shxzskj.cn

readonly PI=3.14
来源：http://tf.bookmarksfly.cn

[R04] 位置参数
来源：http://ij.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yy.yuexingan06.cn

[R05] 参数默认值
来源：http://zl.yuexingan06.cn

name="${1:-default}"
来源：http://ry.panjiajie.cn

[R06] 判断命令是否存在
来源：http://fj.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ro.muxihuayi.cn

[R07] if 判断文件
来源：http://km.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ed.jctech888.com.cn

[R08] 数值比较
来源：http://of.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xg.521024.cn

[R09] 字符串比较
来源：http://io.szxytkj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bh.asd995.cn

[R10] 正则匹配
来源：http://gu.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mj.huixiangedu.cn

[R11] case 多分支
来源：http://rc.yuexingan06.cn

case "$1" in
来源：http://tq.hahajie.cn

start) echo "启动" ;;
来源：http://xu.colortex.cn

stop)  echo "停止" ;;
来源：http://ov.wgjwhj.cn

*)     echo "未知命令" ;;
来源：http://zg.wgjwhj.cn

esac
来源：http://hm.hahajie.cn

[R12] for 遍历文件
来源：http://qz.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://en.9csxet.cn

[R13] for 计数循环
来源：http://ta.yuntaijiaju.cn

for i in {1..10}; do echo "$i"; done
来源：http://qp.shxzukj.cn

[R14] C 风格 for
来源：http://pk.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ii.haigaiapp.cn

[R15] while 逐行读文件
来源：http://vl.huanxung.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yv.szxytkj.cn

[R16] until 等待条件
来源：http://jj.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jx.haigaiapp.cn

[R17] 数组定义与取值
来源：http://kt.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qr.shxzukj.cn

[R18] 遍历数组
来源：http://oz.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kb.muxihuayi.cn

[R19] 数组长度
来源：http://vc.9csxet.cn

echo "${#arr[@]}"
来源：http://jk.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://gr.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yg.yuntaijiaju.cn

[R21] 字符串长度
来源：http://ar.colortex.cn

echo "${#s}"
来源：http://xd.panjiajie.cn

[R22] 截取子串
来源：http://os.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://gp.jianghongdianzi.cn

[R23] 字符串替换
来源：http://cy.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fu.newstarts.cn

[R24] 大小写转换
来源：http://lv.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dc.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://va.colortex.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bo.hnjuh.cn

[R26] 命令替换
来源：http://co.chemitech.net.cn

now=$(date +%F); echo "$now"
来源：http://du.bjjhwx.cn

[R27] 算术展开
来源：http://of.hnjuh.cn

echo $((1 + 2 * 3))
来源：http://ca.szsharing.cn

[R28] 浮点运算
来源：http://ul.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://ri.chemitech.net.cn

[R29] 定义函数
来源：http://jh.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ld.hahajie.cn

[R30] 函数返回状态码
来源：http://jc.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://dx.521024.cn

[R31] 局部变量
来源：http://wy.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://lg.panjiajie.cn

[R32] 参数个数校验
来源：http://md.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ku.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://sn.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oj.huixiangedu.cn

[R34] 退出时清理
来源：http://oq.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dx.haigaiapp.cn

[R35] 后台执行并等待
来源：http://rn.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ng.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://vn.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://av.nszjky.cn

[R37] 把输出赋给变量
来源：http://en.wgjwhj.cn

files=$(ls -1)
来源：http://ab.asd995.cn

[R38] 管道串联
来源：http://se.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://vt.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://cq.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://hu.lnxyls.cn

[R40] 追加写日志
来源：http://ib.gzmigu.cn

echo "log" >> out.log
来源：http://kz.haigaiapp.cn

[R41] 丢弃输出
来源：http://pn.colortex.cn

cmd >/dev/null 2>&1
来源：http://vr.chemitech.net.cn

[R42] 输入重定向
来源：http://wb.gzmigu.cn

wc -l < a.txt
来源：http://go.yuexingan06.cn

[R43] 按名字查找文件
来源：http://aa.muxihuayi.cn

find . -name "*.log" -type f
来源：http://ed.521024.cn

[R44] 按修改时间查找
来源：http://dd.lnxyls.cn

find . -mtime -7 -type f
来源：http://sm.nicolike.cn

[R45] 批量删除
来源：http://yw.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://zg.521024.cn

[R46] 递归替换文件内容
来源：http://qv.shxzukj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://et.szxytkj.cn

[R47] sed 单行替换
来源：http://sa.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ks.9csxet.cn

[R48] awk 取指定列
来源：http://pm.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://fl.lnxyls.cn

[R49] awk 带条件
来源：http://xy.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lt.szxytkj.cn

[R50] awk 求和
来源：http://lu.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wo.newstarts.cn

[R51] 排序去重取前几
来源：http://ti.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ma.newstarts.cn

[R52] 统计行数
来源：http://bb.jctech888.com.cn

wc -l a.txt
来源：http://jo.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://tn.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nc.bookmarksfly.cn

[R54] 比较两个文件
来源：http://yw.shxzskj.cn

diff a.txt b.txt
来源：http://fb.shtwfgs.cn

[R55] 压缩与解压
来源：http://or.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jj.huanxung.cn

[R56] 远程拷贝
来源：http://tm.nszjky.cn

scp file user@host:/path/
来源：http://wq.szsharing.cn

[R57] 远程执行命令
来源：http://wf.szxytkj.cn

ssh user@host 'uptime'
来源：http://zm.lnxyls.cn

[R58] 下载文件
来源：http://kz.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hy.gzmigu.cn

[R59] 发 POST JSON
来源：http://pi.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rj.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://kk.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zx.bjjhwx.cn

[R61] 磁盘占用
来源：http://cp.bjjhwx.cn

df -h;  du -sh *
来源：http://jh.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://wh.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://mx.muxihuayi.cn

[R63] 内存与进程
来源：http://rc.haigaiapp.cn

free -h;  ps aux | grep nginx
来源：http://uv.huanxung.cn

[R64] 结束进程
来源：http://ub.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://ez.hnjuh.cn

[R65] 查看端口占用
来源：http://ox.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mx.panjiajie.cn

[R66] 定时任务
来源：http://lw.hnjuh.cn

crontab -e;  crontab -l
来源：http://ou.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://tl.shtwfgs.cn

openssl rand -hex 16
来源：http://rs.lnxyls.cn

[R68] 计算文件校验值
来源：http://im.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hn.panjiajie.cn

[R69] 生成随机密码
来源：http://cw.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://cr.521024.cn

[R70] 时间戳与互转
来源：http://hw.szsharing.cn

date +%s;  date -d @1700000000
来源：http://of.bjjhwx.cn

[R71] 日期格式化
来源：http://rj.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cj.nicolike.cn

[R72] 等待端口就绪
来源：http://ue.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ge.yuexingan06.cn

[R73] 分割大日志
来源：http://zb.gzmigu.cn

split -l 1000 big.log part_
来源：http://ge.shxzukj.cn

[R74] 批量重命名
来源：http://le.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fz.shtwfgs.cn

[R75] 导出环境变量
来源：http://wa.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://rs.asd995.cn

[R76] 使用临时文件
来源：http://pg.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pq.521024.cn

[R77] 读取用户输入
来源：http://wi.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://tt.szsharing.cn

[R78] 交互式菜单
来源：http://gy.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lw.lnxyls.cn

[R79] 解析命令行选项
来源：http://wb.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fr.9csxet.cn

[R80] 查看脚本执行耗时
来源：http://up.shtwfgs.cn

time ./run.sh
来源：http://rv.huanxung.cn

================================================================================
来源：http://sa.haigaiapp.cn

S. C / C++ 专题
来源：http://si.wgjwhj.cn

================================================================================
来源：http://pv.yuntaijiaju.cn

[S01] C：Hello World
来源：http://me.lnxyls.cn

#include <stdio.h>
来源：http://qx.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lr.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://ht.panjiajie.cn

int a = 10; printf("%d\n", a);
来源：http://ov.gzmigu.cn

[S03] C：读入整数
来源：http://oh.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://zd.521024.cn

[S04] C：字符串复制
来源：http://uv.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://db.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://cf.bjjhwx.cn

strlen(s)
来源：http://kw.jctech888.com.cn

[S06] C：字符串比较
来源：http://ex.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://kh.colortex.cn

[S07] C：数组遍历求和
来源：http://gu.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://em.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://bn.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zo.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://fz.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iq.hahajie.cn

[S10] C：指针与解引用
来源：http://fz.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://ja.9csxet.cn

[S11] C：逐行读文件
来源：http://ee.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://lx.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jo.lnxyls.cn

fclose(f);
来源：http://gr.bjjhwx.cn

[S12] C：写文件
来源：http://qk.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hk.chemitech.net.cn

[S13] C：宏定义
来源：http://ff.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dz.huixiangedu.cn

[S14] C：枚举
来源：http://hl.szsharing.cn

enum Color { RED, GREEN, BLUE };
来源：http://ce.colortex.cn

[S15] C：类型转换
来源：http://kv.huixiangedu.cn

(double) a / b
来源：http://mh.colortex.cn

[S16] C：位操作置位
来源：http://hr.9csxet.cn

x |= (1 << 3);
来源：http://ft.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://ut.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vh.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://wb.szsharing.cn

int main(int argc, char **argv)
来源：http://kh.shtwfgs.cn

[S19] C：快速排序
来源：http://fl.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://su.huixinmuqiang.cn

[S20] C：二分查找
来源：http://rz.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kv.panjiajie.cn

[S21] C：字符类别判断
来源：http://kh.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://li.szxytkj.cn

[S22] C：字符串转数字
来源：http://rl.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cq.huixinmuqiang.cn

[S23] C：随机数
来源：http://bq.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cw.colortex.cn

[S24] C：获取本地时间
来源：http://fs.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uo.hnjuh.cn

[S25] C：内存拷贝
来源：http://cy.shxzukj.cn

memcpy(dst, src, n);
来源：http://pa.asd995.cn

[S26] C：内存清零
来源：http://ei.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://jn.nszjky.cn

[S27] C：定义常量
来源：http://df.nszjky.cn

const double PI = 3.14159;
来源：http://ip.haigaiapp.cn

[S28] C：静态变量
来源：http://ua.muxihuayi.cn

static int counter = 0;
来源：http://ng.chemitech.net.cn

[S29] C：变参函数
来源：http://rz.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lw.newstarts.cn

[S30] C：头文件保护
来源：http://ik.chemitech.net.cn

#ifndef X_H
来源：http://jr.asd995.cn

#define X_H
来源：http://mu.huixiangedu.cn

#endif
来源：http://ou.lnxyls.cn

[S31] C++：Hello World
来源：http://rv.newstarts.cn

#include <iostream>
来源：http://ag.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://tp.hnjuh.cn

[S32] C++：字符串
来源：http://bn.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://am.bjjhwx.cn

[S33] C++：vector 增删
来源：http://ch.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://di.hahajie.cn

[S34] C++：遍历 vector
来源：http://wp.asd995.cn

for (auto &x : v) { std::cout << x; }
来源：http://bp.jctech888.com.cn

[S35] C++：map
来源：http://hz.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pg.hnjuh.cn

[S36] C++：unordered_map
来源：http://ib.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xl.hahajie.cn

[S37] C++：set
来源：http://cr.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xf.shtwfgs.cn

[S38] C++：排序
来源：http://uq.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://qm.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://lw.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uv.wgjwhj.cn

[S40] C++：查找元素
来源：http://zy.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cu.haigaiapp.cn


<!-- 参考信息 -->