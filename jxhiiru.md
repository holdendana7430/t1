代发 wailian999

[Q67] 设置隔离级别
来源：http://sb.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iu.lnxyls.cn

[Q68] 保存点
来源：http://gf.newstarts.cn

SAVEPOINT sp1;
来源：http://fd.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://jo.lnxyls.cn

[Q69] 查看执行计划
来源：http://gc.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://us.hnjuh.cn

[Q70] 更新统计信息
来源：http://qy.nicolike.cn

ANALYZE TABLE users;
来源：http://tk.bjjhwx.cn

[Q71] 查看建表语句
来源：http://jg.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sr.newstarts.cn

[Q72] 查看索引
来源：http://sh.szsharing.cn

SHOW INDEX FROM users;
来源：http://be.nszjky.cn

[Q73] 查看表状态
来源：http://gb.huixiangedu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://of.521024.cn

[Q74] 强制使用索引
来源：http://ze.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xc.szsharing.cn

[Q75] 日期格式化
来源：http://zr.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bb.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hn.nszjky.cn

[Q76] 按天统计
来源：http://er.panjiajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vn.9csxet.cn

[Q77] 时间加减
来源：http://ed.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://es.nszjky.cn

[Q78] 当前时间
来源：http://tb.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yp.nszjky.cn

[Q79] 字符串拼接
来源：http://ic.nszjky.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mm.9csxet.cn

[Q80] 字符串截取
来源：http://kl.shxzukj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vb.hahajie.cn

[Q81] 字符串替换
来源：http://ov.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wv.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://cs.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mw.9csxet.cn

[Q83] 大小写转换
来源：http://fm.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://td.521024.cn

[Q84] 去除首尾空格
来源：http://xw.9csxet.cn

SELECT TRIM(name) FROM users;
来源：http://sh.lnxyls.cn

[Q85] 数值取整
来源：http://qd.bjjhwx.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ew.colortex.cn

[Q86] 读取 JSON 字段
来源：http://ex.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fk.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://az.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qk.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://re.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kx.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ou.muxihuayi.cn

[Q89] 判断表是否存在
来源：http://uq.521024.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vg.szsharing.cn

[Q90] 生成序号列
来源：http://hi.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cz.muxihuayi.cn

================================================================================
来源：http://lq.yuntaijiaju.cn

R. Bash 专题
来源：http://jg.jctech888.com.cn

================================================================================
来源：http://ax.nszjky.cn

[R01] shebang 与严格模式
来源：http://vr.panjiajie.cn

#!/usr/bin/env bash
来源：http://cn.bookmarksfly.cn

set -euo pipefail
来源：http://uu.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://dp.colortex.cn

name="Tom"; echo "$name"
来源：http://bb.bjjhwx.cn

[R03] 只读变量
来源：http://dp.hnjuh.cn

readonly PI=3.14
来源：http://om.bjjhwx.cn

[R04] 位置参数
来源：http://wm.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kn.szsharing.cn

[R05] 参数默认值
来源：http://sx.panjiajie.cn

name="${1:-default}"
来源：http://bp.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://li.haigaiapp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ax.szxytkj.cn

[R07] if 判断文件
来源：http://gx.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oj.jctech888.com.cn

[R08] 数值比较
来源：http://tr.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ir.jctech888.com.cn

[R09] 字符串比较
来源：http://ay.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lz.haigaiapp.cn

[R10] 正则匹配
来源：http://py.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tm.shxzskj.cn

[R11] case 多分支
来源：http://ph.szxytkj.cn

case "$1" in
来源：http://he.521024.cn

start) echo "启动" ;;
来源：http://mg.nszjky.cn

stop)  echo "停止" ;;
来源：http://wg.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://vs.bookmarksfly.cn

esac
来源：http://ll.wgjwhj.cn

[R12] for 遍历文件
来源：http://rw.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://ok.szsharing.cn

[R13] for 计数循环
来源：http://ac.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://ma.wgjwhj.cn

[R14] C 风格 for
来源：http://db.shxzskj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fz.yuexingan06.cn

[R15] while 逐行读文件
来源：http://jl.huixiangedu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wf.jianghongdianzi.cn

[R16] until 等待条件
来源：http://ew.huixiangedu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qq.shtwfgs.cn

[R17] 数组定义与取值
来源：http://bl.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fc.wgjwhj.cn

[R18] 遍历数组
来源：http://de.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xg.asd995.cn

[R19] 数组长度
来源：http://ji.chemitech.net.cn

echo "${#arr[@]}"
来源：http://cu.szxytkj.cn

[R20] 关联数组（字典）
来源：http://hl.nszjky.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ly.yuexingan06.cn

[R21] 字符串长度
来源：http://zn.muxihuayi.cn

echo "${#s}"
来源：http://sc.shtwfgs.cn

[R22] 截取子串
来源：http://iz.jctech888.com.cn

echo "${s:0:5}"
来源：http://cr.nicolike.cn

[R23] 字符串替换
来源：http://zc.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gr.muxihuayi.cn

[R24] 大小写转换
来源：http://xs.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vw.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://tu.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xt.haigaiapp.cn

[R26] 命令替换
来源：http://sy.yuntaijiaju.cn

now=$(date +%F); echo "$now"
来源：http://ze.nicolike.cn

[R27] 算术展开
来源：http://bo.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://kp.yuntaijiaju.cn

[R28] 浮点运算
来源：http://jo.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://jg.jctech888.com.cn

[R29] 定义函数
来源：http://va.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tv.shxzskj.cn

[R30] 函数返回状态码
来源：http://pb.9csxet.cn

f() { return 0; }; f || echo "失败了"
来源：http://ck.szsharing.cn

[R31] 局部变量
来源：http://ta.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://sk.yuexingan06.cn

[R32] 参数个数校验
来源：http://ep.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ww.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://bk.muxihuayi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cz.chemitech.net.cn

[R34] 退出时清理
来源：http://ak.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dg.newstarts.cn

[R35] 后台执行并等待
来源：http://ry.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://za.panjiajie.cn

[R36] 并发执行多个任务
来源：http://fp.shxzukj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lk.gzmigu.cn

[R37] 把输出赋给变量
来源：http://ty.hnjuh.cn

files=$(ls -1)
来源：http://pi.panjiajie.cn

[R38] 管道串联
来源：http://jh.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://nl.521024.cn

[R39] 重定向标准输出与错误
来源：http://wu.jctech888.com.cn

cmd > out.log 2>&1
来源：http://ti.asd995.cn

[R40] 追加写日志
来源：http://jx.hahajie.cn

echo "log" >> out.log
来源：http://jg.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://kd.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://cc.panjiajie.cn

[R42] 输入重定向
来源：http://gg.colortex.cn

wc -l < a.txt
来源：http://al.yuntaijiaju.cn

[R43] 按名字查找文件
来源：http://ju.nszjky.cn

find . -name "*.log" -type f
来源：http://di.colortex.cn

[R44] 按修改时间查找
来源：http://so.asd995.cn

find . -mtime -7 -type f
来源：http://vw.521024.cn

[R45] 批量删除
来源：http://xe.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://aa.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://hb.shtwfgs.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://er.shxzskj.cn

[R47] sed 单行替换
来源：http://rt.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dy.chemitech.net.cn

[R48] awk 取指定列
来源：http://ky.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://zc.bjjhwx.cn

[R49] awk 带条件
来源：http://tr.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sq.muxihuayi.cn

[R50] awk 求和
来源：http://yy.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qq.wgjwhj.cn

[R51] 排序去重取前几
来源：http://nz.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kc.panjiajie.cn

[R52] 统计行数
来源：http://gj.panjiajie.cn

wc -l a.txt
来源：http://ly.panjiajie.cn

[R53] 查看文件头与实时尾
来源：http://wq.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fq.chemitech.net.cn

[R54] 比较两个文件
来源：http://tw.haigaiapp.cn

diff a.txt b.txt
来源：http://cl.yuexingan06.cn

[R55] 压缩与解压
来源：http://uc.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vi.yuexingan06.cn

[R56] 远程拷贝
来源：http://zj.wgjwhj.cn

scp file user@host:/path/
来源：http://sa.szxytkj.cn

[R57] 远程执行命令
来源：http://qh.jctech888.com.cn

ssh user@host 'uptime'
来源：http://hw.huixinmuqiang.cn

[R58] 下载文件
来源：http://pk.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nn.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://mb.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://az.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://an.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ji.haigaiapp.cn

[R61] 磁盘占用
来源：http://ts.huixiangedu.cn

df -h;  du -sh *
来源：http://ny.colortex.cn

[R62] 找最占空间的文件
来源：http://ma.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://ey.newstarts.cn

[R63] 内存与进程
来源：http://ks.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://up.hnjuh.cn

[R64] 结束进程
来源：http://xx.chemitech.net.cn

kill -9 $(pgrep -f app.py)
来源：http://ao.newstarts.cn

[R65] 查看端口占用
来源：http://vh.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yw.shxzukj.cn

[R66] 定时任务
来源：http://eg.szsharing.cn

crontab -e;  crontab -l
来源：http://ut.521024.cn

[R67] 生成随机十六进制串
来源：http://sh.huanxung.cn

openssl rand -hex 16
来源：http://yg.haigaiapp.cn

[R68] 计算文件校验值
来源：http://ah.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ki.hnjuh.cn

[R69] 生成随机密码
来源：http://hb.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://bw.jctech888.com.cn

[R70] 时间戳与互转
来源：http://hp.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://dt.huixiangedu.cn

[R71] 日期格式化
来源：http://no.newstarts.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zv.hnjuh.cn

[R72] 等待端口就绪
来源：http://os.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bn.huixiangedu.cn

[R73] 分割大日志
来源：http://bt.bjjhwx.cn

split -l 1000 big.log part_
来源：http://ke.bookmarksfly.cn

[R74] 批量重命名
来源：http://oi.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qs.haigaiapp.cn

[R75] 导出环境变量
来源：http://wx.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://ur.shxzskj.cn

[R76] 使用临时文件
来源：http://xm.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zz.gzmigu.cn

[R77] 读取用户输入
来源：http://ft.muxihuayi.cn

read -rp "请输入: " ans
来源：http://sp.panjiajie.cn

[R78] 交互式菜单
来源：http://nr.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://eb.wgjwhj.cn

[R79] 解析命令行选项
来源：http://we.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kw.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://ed.huanxung.cn

time ./run.sh
来源：http://kj.colortex.cn

================================================================================
来源：http://sn.haigaiapp.cn

S. C / C++ 专题
来源：http://rw.yuntaijiaju.cn

================================================================================
来源：http://jz.panjiajie.cn

[S01] C：Hello World
来源：http://yp.panjiajie.cn

#include <stdio.h>
来源：http://pn.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uw.szsharing.cn

[S02] C：变量与格式化输出
来源：http://rv.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://qk.shxzukj.cn

[S03] C：读入整数
来源：http://np.gzmigu.cn

int x; scanf("%d", &x);
来源：http://qo.wgjwhj.cn

[S04] C：字符串复制
来源：http://bu.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jb.wgjwhj.cn

[S05] C：字符串长度
来源：http://qk.9csxet.cn

strlen(s)
来源：http://mb.chemitech.net.cn

[S06] C：字符串比较
来源：http://bu.shxzskj.cn

strcmp(a, b) == 0
来源：http://go.521024.cn

[S07] C：数组遍历求和
来源：http://cc.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nh.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://zh.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wo.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://tj.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://va.colortex.cn

[S10] C：指针与解引用
来源：http://kj.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://me.lnxyls.cn

[S11] C：逐行读文件
来源：http://yz.muxihuayi.cn

FILE *f = fopen("a.txt", "r");
来源：http://zy.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yl.chemitech.net.cn

fclose(f);
来源：http://fn.gzmigu.cn

[S12] C：写文件
来源：http://cn.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sb.shxzukj.cn

[S13] C：宏定义
来源：http://fl.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cb.haigaiapp.cn

[S14] C：枚举
来源：http://pa.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://sd.muxihuayi.cn

[S15] C：类型转换
来源：http://bx.yuexingan06.cn

(double) a / b
来源：http://ff.huixiangedu.cn

[S16] C：位操作置位
来源：http://vh.hahajie.cn

x |= (1 << 3);
来源：http://ol.hahajie.cn

[S17] C：安全拼接字符串
来源：http://ly.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wt.lnxyls.cn

[S18] C：命令行参数
来源：http://uj.gzmigu.cn

int main(int argc, char **argv)
来源：http://wl.huixiangedu.cn

[S19] C：快速排序
来源：http://hx.gzmigu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gi.asd995.cn

[S20] C：二分查找
来源：http://hv.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ht.shxzskj.cn

[S21] C：字符类别判断
来源：http://al.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hu.521024.cn

[S22] C：字符串转数字
来源：http://ip.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zp.nszjky.cn

[S23] C：随机数
来源：http://he.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ur.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://vl.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://du.muxihuayi.cn

[S25] C：内存拷贝
来源：http://ut.shtwfgs.cn

memcpy(dst, src, n);
来源：http://os.panjiajie.cn

[S26] C：内存清零
来源：http://fc.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://ag.shxzskj.cn

[S27] C：定义常量
来源：http://dd.chemitech.net.cn

const double PI = 3.14159;
来源：http://ho.hnjuh.cn

[S28] C：静态变量
来源：http://qg.lnxyls.cn

static int counter = 0;
来源：http://la.bookmarksfly.cn

[S29] C：变参函数
来源：http://il.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jx.bookmarksfly.cn

[S30] C：头文件保护
来源：http://wb.panjiajie.cn

#ifndef X_H
来源：http://ut.haigaiapp.cn

#define X_H
来源：http://op.muxihuayi.cn

#endif
来源：http://qt.9csxet.cn

[S31] C++：Hello World
来源：http://tv.shtwfgs.cn

#include <iostream>
来源：http://go.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://qe.asd995.cn

[S32] C++：字符串
来源：http://qf.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://ce.nicolike.cn

[S33] C++：vector 增删
来源：http://ng.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wj.nszjky.cn

[S34] C++：遍历 vector
来源：http://co.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://td.panjiajie.cn

[S35] C++：map
来源：http://ap.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qz.shtwfgs.cn

[S36] C++：unordered_map
来源：http://an.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cr.9csxet.cn


<!-- 参考信息 -->