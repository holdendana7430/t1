代发 wailian999

[Q63] 开启事务
来源：http://hs.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hq.muxihuayi.cn

[Q64] 提交事务
来源：http://xl.muxihuayi.cn

COMMIT;
来源：http://yh.asd995.cn

[Q65] 回滚事务
来源：http://au.szsharing.cn

ROLLBACK;
来源：http://am.nszjky.cn

[Q66] 行锁查询
来源：http://kg.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tx.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://oq.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yi.bjjhwx.cn

[Q68] 保存点
来源：http://ws.colortex.cn

SAVEPOINT sp1;
来源：http://am.bookmarksfly.cn

ROLLBACK TO sp1;
来源：http://qr.nszjky.cn

[Q69] 查看执行计划
来源：http://ef.panjiajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://my.panjiajie.cn

[Q70] 更新统计信息
来源：http://az.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://xm.yuexingan06.cn

[Q71] 查看建表语句
来源：http://ak.521024.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://st.huixinmuqiang.cn

[Q72] 查看索引
来源：http://dj.huanxung.cn

SHOW INDEX FROM users;
来源：http://sv.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://ej.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nt.hahajie.cn

[Q74] 强制使用索引
来源：http://em.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xw.nszjky.cn

[Q75] 日期格式化
来源：http://pi.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tm.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kt.huanxung.cn

[Q76] 按天统计
来源：http://wt.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zi.huixiangedu.cn

[Q77] 时间加减
来源：http://wb.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wb.szsharing.cn

[Q78] 当前时间
来源：http://ry.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ka.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://gn.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vv.bookmarksfly.cn

[Q80] 字符串截取
来源：http://qz.jianghongdianzi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tg.jctech888.com.cn

[Q81] 字符串替换
来源：http://vr.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cw.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://xc.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hu.shxzskj.cn

[Q83] 大小写转换
来源：http://ut.szsharing.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rn.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://zi.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://eh.panjiajie.cn

[Q85] 数值取整
来源：http://te.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qu.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://pt.chemitech.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ch.chemitech.net.cn

[Q87] JSON 字段做条件
来源：http://sg.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sf.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://be.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ba.nszjky.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bg.colortex.cn

[Q89] 判断表是否存在
来源：http://kq.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eh.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://sc.huixiangedu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vc.hnjuh.cn

================================================================================
来源：http://yx.huanxung.cn

R. Bash 专题
来源：http://oo.colortex.cn

================================================================================
来源：http://aq.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://gp.521024.cn

#!/usr/bin/env bash
来源：http://cn.shxzskj.cn

set -euo pipefail
来源：http://hi.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://ck.hnjuh.cn

name="Tom"; echo "$name"
来源：http://cu.9csxet.cn

[R03] 只读变量
来源：http://le.hnjuh.cn

readonly PI=3.14
来源：http://gc.huanxung.cn

[R04] 位置参数
来源：http://mq.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yy.yuntaijiaju.cn

[R05] 参数默认值
来源：http://rn.nicolike.cn

name="${1:-default}"
来源：http://iq.shxzskj.cn

[R06] 判断命令是否存在
来源：http://gf.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://aq.bjjhwx.cn

[R07] if 判断文件
来源：http://tb.yuntaijiaju.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hs.chemitech.net.cn

[R08] 数值比较
来源：http://ga.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wi.huanxung.cn

[R09] 字符串比较
来源：http://jf.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wi.lnxyls.cn

[R10] 正则匹配
来源：http://io.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rs.yuexingan06.cn

[R11] case 多分支
来源：http://ma.521024.cn

case "$1" in
来源：http://vr.bookmarksfly.cn

start) echo "启动" ;;
来源：http://uq.hahajie.cn

stop)  echo "停止" ;;
来源：http://ry.521024.cn

*)     echo "未知命令" ;;
来源：http://jk.nszjky.cn

esac
来源：http://au.newstarts.cn

[R12] for 遍历文件
来源：http://ht.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://fi.wgjwhj.cn

[R13] for 计数循环
来源：http://ln.szsharing.cn

for i in {1..10}; do echo "$i"; done
来源：http://gu.shxzskj.cn

[R14] C 风格 for
来源：http://bt.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kh.wgjwhj.cn

[R15] while 逐行读文件
来源：http://eu.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fy.bjjhwx.cn

[R16] until 等待条件
来源：http://ht.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sj.szxytkj.cn

[R17] 数组定义与取值
来源：http://ba.muxihuayi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vv.jctech888.com.cn

[R18] 遍历数组
来源：http://cg.wgjwhj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lz.haigaiapp.cn

[R19] 数组长度
来源：http://dd.hahajie.cn

echo "${#arr[@]}"
来源：http://yh.szxytkj.cn

[R20] 关联数组（字典）
来源：http://br.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ft.szsharing.cn

[R21] 字符串长度
来源：http://be.bjjhwx.cn

echo "${#s}"
来源：http://me.newstarts.cn

[R22] 截取子串
来源：http://ds.shxzukj.cn

echo "${s:0:5}"
来源：http://ov.gzmigu.cn

[R23] 字符串替换
来源：http://yo.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xq.bookmarksfly.cn

[R24] 大小写转换
来源：http://pf.newstarts.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ol.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://xs.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://se.haigaiapp.cn

[R26] 命令替换
来源：http://rd.huixiangedu.cn

now=$(date +%F); echo "$now"
来源：http://ij.9csxet.cn

[R27] 算术展开
来源：http://sh.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://sl.bookmarksfly.cn

[R28] 浮点运算
来源：http://ol.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://xb.huixiangedu.cn

[R29] 定义函数
来源：http://ah.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kr.jctech888.com.cn

[R30] 函数返回状态码
来源：http://ty.newstarts.cn

f() { return 0; }; f || echo "失败了"
来源：http://yh.yuntaijiaju.cn

[R31] 局部变量
来源：http://fw.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://nx.shxzukj.cn

[R32] 参数个数校验
来源：http://az.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xe.bjjhwx.cn

[R33] 捕获错误并提示行号
来源：http://vv.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ii.haigaiapp.cn

[R34] 退出时清理
来源：http://us.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ab.colortex.cn

[R35] 后台执行并等待
来源：http://cb.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tm.521024.cn

[R36] 并发执行多个任务
来源：http://bq.shxzukj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zs.gzmigu.cn

[R37] 把输出赋给变量
来源：http://as.jctech888.com.cn

files=$(ls -1)
来源：http://kq.hahajie.cn

[R38] 管道串联
来源：http://ow.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://tq.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://dg.muxihuayi.cn

cmd > out.log 2>&1
来源：http://wo.huixiangedu.cn

[R40] 追加写日志
来源：http://mx.huanxung.cn

echo "log" >> out.log
来源：http://mz.nszjky.cn

[R41] 丢弃输出
来源：http://mo.jctech888.com.cn

cmd >/dev/null 2>&1
来源：http://ow.bookmarksfly.cn

[R42] 输入重定向
来源：http://hf.nszjky.cn

wc -l < a.txt
来源：http://wb.huanxung.cn

[R43] 按名字查找文件
来源：http://ew.nicolike.cn

find . -name "*.log" -type f
来源：http://hc.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://gu.asd995.cn

find . -mtime -7 -type f
来源：http://jp.wgjwhj.cn

[R45] 批量删除
来源：http://my.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://rj.shxzukj.cn

[R46] 递归替换文件内容
来源：http://oy.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://on.9csxet.cn

[R47] sed 单行替换
来源：http://yd.bjjhwx.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sy.szsharing.cn

[R48] awk 取指定列
来源：http://ei.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://zk.jctech888.com.cn

[R49] awk 带条件
来源：http://vg.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cy.newstarts.cn

[R50] awk 求和
来源：http://wy.jctech888.com.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jc.gzmigu.cn

[R51] 排序去重取前几
来源：http://in.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sr.panjiajie.cn

[R52] 统计行数
来源：http://us.nszjky.cn

wc -l a.txt
来源：http://qz.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://az.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ch.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://cc.szsharing.cn

diff a.txt b.txt
来源：http://qj.lnxyls.cn

[R55] 压缩与解压
来源：http://cg.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pm.chemitech.net.cn

[R56] 远程拷贝
来源：http://sn.hahajie.cn

scp file user@host:/path/
来源：http://ri.muxihuayi.cn

[R57] 远程执行命令
来源：http://pm.muxihuayi.cn

ssh user@host 'uptime'
来源：http://qs.jctech888.com.cn

[R58] 下载文件
来源：http://jr.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ro.nicolike.cn

[R59] 发 POST JSON
来源：http://cv.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bx.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://bo.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fy.yuexingan06.cn

[R61] 磁盘占用
来源：http://ig.hahajie.cn

df -h;  du -sh *
来源：http://hj.colortex.cn

[R62] 找最占空间的文件
来源：http://pt.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://pp.hahajie.cn

[R63] 内存与进程
来源：http://qg.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://ba.newstarts.cn

[R64] 结束进程
来源：http://tw.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://gh.szsharing.cn

[R65] 查看端口占用
来源：http://rl.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nv.9csxet.cn

[R66] 定时任务
来源：http://tu.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://hc.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://nl.jctech888.com.cn

openssl rand -hex 16
来源：http://az.nszjky.cn

[R68] 计算文件校验值
来源：http://qv.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rf.panjiajie.cn

[R69] 生成随机密码
来源：http://su.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://jv.shtwfgs.cn

[R70] 时间戳与互转
来源：http://jj.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://jf.colortex.cn

[R71] 日期格式化
来源：http://pq.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ow.chemitech.net.cn

[R72] 等待端口就绪
来源：http://iu.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wf.shxzukj.cn

[R73] 分割大日志
来源：http://gl.9csxet.cn

split -l 1000 big.log part_
来源：http://em.szxytkj.cn

[R74] 批量重命名
来源：http://de.nszjky.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kf.newstarts.cn

[R75] 导出环境变量
来源：http://xx.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://jr.muxihuayi.cn

[R76] 使用临时文件
来源：http://rb.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tu.9csxet.cn

[R77] 读取用户输入
来源：http://lt.lnxyls.cn

read -rp "请输入: " ans
来源：http://rw.shtwfgs.cn

[R78] 交互式菜单
来源：http://jk.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ru.lnxyls.cn

[R79] 解析命令行选项
来源：http://wf.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fb.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://dz.panjiajie.cn

time ./run.sh
来源：http://kq.asd995.cn

================================================================================
来源：http://ii.jctech888.com.cn

S. C / C++ 专题
来源：http://qm.bjjhwx.cn

================================================================================
来源：http://cz.colortex.cn

[S01] C：Hello World
来源：http://bp.bjjhwx.cn

#include <stdio.h>
来源：http://rf.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ow.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://jb.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://ws.hahajie.cn

[S03] C：读入整数
来源：http://mu.hnjuh.cn

int x; scanf("%d", &x);
来源：http://bf.hnjuh.cn

[S04] C：字符串复制
来源：http://cc.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cq.szsharing.cn

[S05] C：字符串长度
来源：http://in.yuexingan06.cn

strlen(s)
来源：http://fg.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://ny.colortex.cn

strcmp(a, b) == 0
来源：http://ui.newstarts.cn

[S07] C：数组遍历求和
来源：http://zc.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hp.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://rn.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zl.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://uw.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oo.shxzukj.cn

[S10] C：指针与解引用
来源：http://vq.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://zx.9csxet.cn

[S11] C：逐行读文件
来源：http://ur.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://sk.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pd.bookmarksfly.cn

fclose(f);
来源：http://na.521024.cn

[S12] C：写文件
来源：http://vt.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jk.gzmigu.cn

[S13] C：宏定义
来源：http://kf.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://du.huixinmuqiang.cn

[S14] C：枚举
来源：http://jz.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://vg.panjiajie.cn

[S15] C：类型转换
来源：http://be.colortex.cn

(double) a / b
来源：http://ux.nszjky.cn

[S16] C：位操作置位
来源：http://ga.haigaiapp.cn

x |= (1 << 3);
来源：http://la.nicolike.cn

[S17] C：安全拼接字符串
来源：http://zz.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xl.panjiajie.cn

[S18] C：命令行参数
来源：http://la.chemitech.net.cn

int main(int argc, char **argv)
来源：http://fr.lnxyls.cn

[S19] C：快速排序
来源：http://dl.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ar.muxihuayi.cn

[S20] C：二分查找
来源：http://gn.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ox.jctech888.com.cn

[S21] C：字符类别判断
来源：http://ek.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://es.shtwfgs.cn

[S22] C：字符串转数字
来源：http://rk.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jk.huanxung.cn

[S23] C：随机数
来源：http://my.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ff.nicolike.cn

[S24] C：获取本地时间
来源：http://wt.yuexingan06.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xb.lnxyls.cn

[S25] C：内存拷贝
来源：http://qg.szxytkj.cn

memcpy(dst, src, n);
来源：http://lm.shxzukj.cn

[S26] C：内存清零
来源：http://bt.9csxet.cn

memset(a, 0, sizeof a);
来源：http://uw.shtwfgs.cn

[S27] C：定义常量
来源：http://gu.shxzskj.cn

const double PI = 3.14159;
来源：http://pw.jianghongdianzi.cn

[S28] C：静态变量
来源：http://fc.hnjuh.cn

static int counter = 0;
来源：http://js.asd995.cn

[S29] C：变参函数
来源：http://wq.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sy.gzmigu.cn

[S30] C：头文件保护
来源：http://qk.hnjuh.cn

#ifndef X_H
来源：http://gm.jctech888.com.cn

#define X_H
来源：http://qf.colortex.cn

#endif
来源：http://ii.nszjky.cn

[S31] C++：Hello World
来源：http://bi.colortex.cn

#include <iostream>
来源：http://lt.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://wp.lnxyls.cn

[S32] C++：字符串
来源：http://ku.521024.cn

std::string s = "hi";  s += "!";
来源：http://um.nicolike.cn


<!-- 参考信息 -->