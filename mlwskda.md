代发 wailian999

[Q65] 回滚事务
来源：http://oz.colortex.cn

ROLLBACK;
来源：http://jf.521024.cn

[Q66] 行锁查询
来源：http://ap.muxihuayi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sd.panjiajie.cn

[Q67] 设置隔离级别
来源：http://tt.yuexingan06.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xy.shxzskj.cn

[Q68] 保存点
来源：http://dl.asd995.cn

SAVEPOINT sp1;
来源：http://fs.yuntaijiaju.cn

ROLLBACK TO sp1;
来源：http://iz.shxzskj.cn

[Q69] 查看执行计划
来源：http://wv.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wt.shxzskj.cn

[Q70] 更新统计信息
来源：http://hx.asd995.cn

ANALYZE TABLE users;
来源：http://dx.nszjky.cn

[Q71] 查看建表语句
来源：http://ll.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ga.huixiangedu.cn

[Q72] 查看索引
来源：http://ag.gzmigu.cn

SHOW INDEX FROM users;
来源：http://hn.9csxet.cn

[Q73] 查看表状态
来源：http://vn.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rn.haigaiapp.cn

[Q74] 强制使用索引
来源：http://yq.jianghongdianzi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://om.yuexingan06.cn

[Q75] 日期格式化
来源：http://ni.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mg.szxytkj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ox.nicolike.cn

[Q76] 按天统计
来源：http://gq.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jg.szsharing.cn

[Q77] 时间加减
来源：http://wp.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://py.hahajie.cn

[Q78] 当前时间
来源：http://dh.haigaiapp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xi.521024.cn

[Q79] 字符串拼接
来源：http://id.colortex.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iy.nicolike.cn

[Q80] 字符串截取
来源：http://io.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ne.wgjwhj.cn

[Q81] 字符串替换
来源：http://qp.yuexingan06.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cn.chemitech.net.cn

[Q82] 字符长度与字节长度
来源：http://ap.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lm.yuntaijiaju.cn

[Q83] 大小写转换
来源：http://bq.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ot.shxzukj.cn

[Q84] 去除首尾空格
来源：http://uw.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://pc.gzmigu.cn

[Q85] 数值取整
来源：http://rq.shtwfgs.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qs.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://bk.nicolike.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hq.nicolike.cn

[Q87] JSON 字段做条件
来源：http://ql.shxzukj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hk.huixinmuqiang.cn

[Q88] 行转列（条件聚合）
来源：http://eb.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wg.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cv.huanxung.cn

[Q89] 判断表是否存在
来源：http://lk.huixinmuqiang.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hb.shtwfgs.cn

[Q90] 生成序号列
来源：http://cc.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xe.jianghongdianzi.cn

================================================================================
来源：http://qe.lnxyls.cn

R. Bash 专题
来源：http://ql.szsharing.cn

================================================================================
来源：http://qe.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://ll.chemitech.net.cn

#!/usr/bin/env bash
来源：http://rc.hahajie.cn

set -euo pipefail
来源：http://rk.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://wr.nicolike.cn

name="Tom"; echo "$name"
来源：http://vc.hnjuh.cn

[R03] 只读变量
来源：http://xp.huixiangedu.cn

readonly PI=3.14
来源：http://fm.huixinmuqiang.cn

[R04] 位置参数
来源：http://uc.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zz.colortex.cn

[R05] 参数默认值
来源：http://kb.yuexingan06.cn

name="${1:-default}"
来源：http://gh.newstarts.cn

[R06] 判断命令是否存在
来源：http://pb.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ts.huixiangedu.cn

[R07] if 判断文件
来源：http://dh.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ru.asd995.cn

[R08] 数值比较
来源：http://cn.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://oc.shxzukj.cn

[R09] 字符串比较
来源：http://cp.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ka.huanxung.cn

[R10] 正则匹配
来源：http://vo.lnxyls.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lc.colortex.cn

[R11] case 多分支
来源：http://zr.muxihuayi.cn

case "$1" in
来源：http://ka.huanxung.cn

start) echo "启动" ;;
来源：http://tz.colortex.cn

stop)  echo "停止" ;;
来源：http://rw.hnjuh.cn

*)     echo "未知命令" ;;
来源：http://zy.shtwfgs.cn

esac
来源：http://cg.chemitech.net.cn

[R12] for 遍历文件
来源：http://ii.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://kv.chemitech.net.cn

[R13] for 计数循环
来源：http://di.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://wi.yuexingan06.cn

[R14] C 风格 for
来源：http://ar.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://df.gzmigu.cn

[R15] while 逐行读文件
来源：http://sw.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ok.bookmarksfly.cn

[R16] until 等待条件
来源：http://gv.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://la.muxihuayi.cn

[R17] 数组定义与取值
来源：http://ad.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wx.shxzskj.cn

[R18] 遍历数组
来源：http://wk.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uf.szxytkj.cn

[R19] 数组长度
来源：http://fc.521024.cn

echo "${#arr[@]}"
来源：http://eg.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://gr.hnjuh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kn.lnxyls.cn

[R21] 字符串长度
来源：http://mj.panjiajie.cn

echo "${#s}"
来源：http://db.colortex.cn

[R22] 截取子串
来源：http://nk.shxzukj.cn

echo "${s:0:5}"
来源：http://di.lnxyls.cn

[R23] 字符串替换
来源：http://po.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tv.szsharing.cn

[R24] 大小写转换
来源：http://fh.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://op.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://on.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hy.lnxyls.cn

[R26] 命令替换
来源：http://pz.haigaiapp.cn

now=$(date +%F); echo "$now"
来源：http://ha.muxihuayi.cn

[R27] 算术展开
来源：http://ja.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://jb.wgjwhj.cn

[R28] 浮点运算
来源：http://ud.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://sx.shxzukj.cn

[R29] 定义函数
来源：http://oh.newstarts.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jw.szsharing.cn

[R30] 函数返回状态码
来源：http://me.muxihuayi.cn

f() { return 0; }; f || echo "失败了"
来源：http://op.bjjhwx.cn

[R31] 局部变量
来源：http://ju.haigaiapp.cn

f() { local x=1; echo "$x"; }
来源：http://cd.huixiangedu.cn

[R32] 参数个数校验
来源：http://po.colortex.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qt.521024.cn

[R33] 捕获错误并提示行号
来源：http://it.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ww.asd995.cn

[R34] 退出时清理
来源：http://wt.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://oi.hnjuh.cn

[R35] 后台执行并等待
来源：http://ad.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ta.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://xo.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fq.asd995.cn

[R37] 把输出赋给变量
来源：http://uw.muxihuayi.cn

files=$(ls -1)
来源：http://fk.wgjwhj.cn

[R38] 管道串联
来源：http://ys.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://hi.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://mb.asd995.cn

cmd > out.log 2>&1
来源：http://cp.asd995.cn

[R40] 追加写日志
来源：http://ue.newstarts.cn

echo "log" >> out.log
来源：http://wu.chemitech.net.cn

[R41] 丢弃输出
来源：http://sg.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://xg.9csxet.cn

[R42] 输入重定向
来源：http://hm.colortex.cn

wc -l < a.txt
来源：http://tp.shtwfgs.cn

[R43] 按名字查找文件
来源：http://pa.521024.cn

find . -name "*.log" -type f
来源：http://ur.shtwfgs.cn

[R44] 按修改时间查找
来源：http://ff.shxzskj.cn

find . -mtime -7 -type f
来源：http://ws.9csxet.cn

[R45] 批量删除
来源：http://yr.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://ey.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://mn.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dz.bookmarksfly.cn

[R47] sed 单行替换
来源：http://fm.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pt.szsharing.cn

[R48] awk 取指定列
来源：http://yw.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://et.shxzskj.cn

[R49] awk 带条件
来源：http://kg.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aj.huixinmuqiang.cn

[R50] awk 求和
来源：http://dc.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yu.asd995.cn

[R51] 排序去重取前几
来源：http://zo.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tc.colortex.cn

[R52] 统计行数
来源：http://lj.szsharing.cn

wc -l a.txt
来源：http://nh.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://gu.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ht.szsharing.cn

[R54] 比较两个文件
来源：http://vk.hahajie.cn

diff a.txt b.txt
来源：http://hj.nicolike.cn

[R55] 压缩与解压
来源：http://kb.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ec.9csxet.cn

[R56] 远程拷贝
来源：http://tj.shtwfgs.cn

scp file user@host:/path/
来源：http://vl.shxzskj.cn

[R57] 远程执行命令
来源：http://cj.muxihuayi.cn

ssh user@host 'uptime'
来源：http://jy.jctech888.com.cn

[R58] 下载文件
来源：http://yb.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://og.chemitech.net.cn

[R59] 发 POST JSON
来源：http://tn.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vp.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://sy.huanxung.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://in.colortex.cn

[R61] 磁盘占用
来源：http://pq.muxihuayi.cn

df -h;  du -sh *
来源：http://li.9csxet.cn

[R62] 找最占空间的文件
来源：http://ye.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://tn.muxihuayi.cn

[R63] 内存与进程
来源：http://iz.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://hr.yuexingan06.cn

[R64] 结束进程
来源：http://fk.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://py.huanxung.cn

[R65] 查看端口占用
来源：http://ow.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ro.huanxung.cn

[R66] 定时任务
来源：http://kt.jctech888.com.cn

crontab -e;  crontab -l
来源：http://di.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://ed.bookmarksfly.cn

openssl rand -hex 16
来源：http://io.huixiangedu.cn

[R68] 计算文件校验值
来源：http://nx.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vp.jctech888.com.cn

[R69] 生成随机密码
来源：http://id.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://sd.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://ma.yuntaijiaju.cn

date +%s;  date -d @1700000000
来源：http://ih.gzmigu.cn

[R71] 日期格式化
来源：http://bq.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sw.gzmigu.cn

[R72] 等待端口就绪
来源：http://zr.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pu.colortex.cn

[R73] 分割大日志
来源：http://rg.wgjwhj.cn

split -l 1000 big.log part_
来源：http://le.jctech888.com.cn

[R74] 批量重命名
来源：http://ig.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://we.huixiangedu.cn

[R75] 导出环境变量
来源：http://ut.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://sa.szxytkj.cn

[R76] 使用临时文件
来源：http://nr.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ff.lnxyls.cn

[R77] 读取用户输入
来源：http://ih.521024.cn

read -rp "请输入: " ans
来源：http://nc.jctech888.com.cn

[R78] 交互式菜单
来源：http://ej.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yr.szsharing.cn

[R79] 解析命令行选项
来源：http://re.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fp.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://we.panjiajie.cn

time ./run.sh
来源：http://hh.newstarts.cn

================================================================================
来源：http://no.jctech888.com.cn

S. C / C++ 专题
来源：http://cc.asd995.cn

================================================================================
来源：http://is.chemitech.net.cn

[S01] C：Hello World
来源：http://va.szxytkj.cn

#include <stdio.h>
来源：http://ed.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://of.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://rf.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://mw.shxzukj.cn

[S03] C：读入整数
来源：http://fr.newstarts.cn

int x; scanf("%d", &x);
来源：http://ug.shtwfgs.cn

[S04] C：字符串复制
来源：http://kp.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dj.bjjhwx.cn

[S05] C：字符串长度
来源：http://wz.chemitech.net.cn

strlen(s)
来源：http://pq.colortex.cn

[S06] C：字符串比较
来源：http://jk.asd995.cn

strcmp(a, b) == 0
来源：http://az.hnjuh.cn

[S07] C：数组遍历求和
来源：http://lw.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cf.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://zp.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jo.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://bd.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qh.colortex.cn

[S10] C：指针与解引用
来源：http://by.hahajie.cn

int *p = &a;  *p = 5;
来源：http://xi.hahajie.cn

[S11] C：逐行读文件
来源：http://sv.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://vh.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nk.jianghongdianzi.cn

fclose(f);
来源：http://ls.huixinmuqiang.cn

[S12] C：写文件
来源：http://oh.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rz.muxihuayi.cn

[S13] C：宏定义
来源：http://sp.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ti.bookmarksfly.cn

[S14] C：枚举
来源：http://nx.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://jf.colortex.cn

[S15] C：类型转换
来源：http://ln.bjjhwx.cn

(double) a / b
来源：http://oi.521024.cn

[S16] C：位操作置位
来源：http://au.bjjhwx.cn

x |= (1 << 3);
来源：http://sa.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://ez.huixiangedu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dd.shxzukj.cn

[S18] C：命令行参数
来源：http://hp.colortex.cn

int main(int argc, char **argv)
来源：http://mz.nszjky.cn

[S19] C：快速排序
来源：http://xv.gzmigu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zm.yuexingan06.cn

[S20] C：二分查找
来源：http://ew.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qu.haigaiapp.cn

[S21] C：字符类别判断
来源：http://wt.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ca.nszjky.cn

[S22] C：字符串转数字
来源：http://hd.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://eo.newstarts.cn

[S23] C：随机数
来源：http://ej.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://re.chemitech.net.cn

[S24] C：获取本地时间
来源：http://wi.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lj.newstarts.cn

[S25] C：内存拷贝
来源：http://vq.haigaiapp.cn

memcpy(dst, src, n);
来源：http://gw.jctech888.com.cn

[S26] C：内存清零
来源：http://ht.asd995.cn

memset(a, 0, sizeof a);
来源：http://dc.yuntaijiaju.cn

[S27] C：定义常量
来源：http://ms.shxzukj.cn

const double PI = 3.14159;
来源：http://by.huanxung.cn

[S28] C：静态变量
来源：http://pq.hnjuh.cn

static int counter = 0;
来源：http://wp.9csxet.cn

[S29] C：变参函数
来源：http://ie.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ii.shxzskj.cn

[S30] C：头文件保护
来源：http://rc.lnxyls.cn

#ifndef X_H
来源：http://ws.jctech888.com.cn

#define X_H
来源：http://oa.yuexingan06.cn

#endif
来源：http://vu.newstarts.cn

[S31] C++：Hello World
来源：http://yi.colortex.cn

#include <iostream>
来源：http://fb.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://uz.nszjky.cn

[S32] C++：字符串
来源：http://rg.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://zm.newstarts.cn

[S33] C++：vector 增删
来源：http://ww.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sh.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://aa.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://zu.haigaiapp.cn


<!-- 参考信息 -->