代发 wailian999

[Q61] 移动平均
来源：http://ln.huanxung.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pr.newstarts.cn

[Q62] 分组占比
来源：http://dj.huixiangedu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xm.hnjuh.cn

[Q63] 开启事务
来源：http://aj.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qf.chemitech.net.cn

[Q64] 提交事务
来源：http://id.bjjhwx.cn

COMMIT;
来源：http://cj.shxzukj.cn

[Q65] 回滚事务
来源：http://ng.colortex.cn

ROLLBACK;
来源：http://hn.szsharing.cn

[Q66] 行锁查询
来源：http://ul.muxihuayi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ez.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://cn.haigaiapp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uu.nicolike.cn

[Q68] 保存点
来源：http://wu.jianghongdianzi.cn

SAVEPOINT sp1;
来源：http://yj.huanxung.cn

ROLLBACK TO sp1;
来源：http://jc.haigaiapp.cn

[Q69] 查看执行计划
来源：http://pk.huixinmuqiang.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mk.jianghongdianzi.cn

[Q70] 更新统计信息
来源：http://jf.yuexingan06.cn

ANALYZE TABLE users;
来源：http://pk.newstarts.cn

[Q71] 查看建表语句
来源：http://ku.nicolike.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pq.bookmarksfly.cn

[Q72] 查看索引
来源：http://vp.gzmigu.cn

SHOW INDEX FROM users;
来源：http://pi.wgjwhj.cn

[Q73] 查看表状态
来源：http://nn.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qz.shxzskj.cn

[Q74] 强制使用索引
来源：http://jw.hnjuh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xe.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://jh.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cw.asd995.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zq.wgjwhj.cn

[Q76] 按天统计
来源：http://aq.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lh.szxytkj.cn

[Q77] 时间加减
来源：http://bm.huixiangedu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iv.gzmigu.cn

[Q78] 当前时间
来源：http://rk.huixinmuqiang.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ux.shxzukj.cn

[Q79] 字符串拼接
来源：http://qv.huixiangedu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ah.yuexingan06.cn

[Q80] 字符串截取
来源：http://zs.muxihuayi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gr.nicolike.cn

[Q81] 字符串替换
来源：http://yd.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://we.muxihuayi.cn

[Q82] 字符长度与字节长度
来源：http://za.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oc.shxzukj.cn

[Q83] 大小写转换
来源：http://mx.jianghongdianzi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qu.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://id.jctech888.com.cn

SELECT TRIM(name) FROM users;
来源：http://xw.haigaiapp.cn

[Q85] 数值取整
来源：http://kl.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qb.asd995.cn

[Q86] 读取 JSON 字段
来源：http://vs.bjjhwx.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bz.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://ot.asd995.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://be.muxihuayi.cn

[Q88] 行转列（条件聚合）
来源：http://jv.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zi.hnjuh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tx.nicolike.cn

[Q89] 判断表是否存在
来源：http://ya.haigaiapp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pp.colortex.cn

[Q90] 生成序号列
来源：http://hn.huanxung.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jz.shxzskj.cn

================================================================================
来源：http://qj.nicolike.cn

R. Bash 专题
来源：http://aw.chemitech.net.cn

================================================================================
来源：http://oh.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://fm.521024.cn

#!/usr/bin/env bash
来源：http://kr.9csxet.cn

set -euo pipefail
来源：http://ds.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://if.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://yr.newstarts.cn

[R03] 只读变量
来源：http://aa.huixiangedu.cn

readonly PI=3.14
来源：http://yz.chemitech.net.cn

[R04] 位置参数
来源：http://bt.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ji.colortex.cn

[R05] 参数默认值
来源：http://dv.huixinmuqiang.cn

name="${1:-default}"
来源：http://xz.wgjwhj.cn

[R06] 判断命令是否存在
来源：http://hn.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ox.asd995.cn

[R07] if 判断文件
来源：http://qo.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lh.haigaiapp.cn

[R08] 数值比较
来源：http://ig.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wj.yuexingan06.cn

[R09] 字符串比较
来源：http://wd.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yk.szxytkj.cn

[R10] 正则匹配
来源：http://oj.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qq.haigaiapp.cn

[R11] case 多分支
来源：http://zk.muxihuayi.cn

case "$1" in
来源：http://in.jctech888.com.cn

start) echo "启动" ;;
来源：http://kq.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://cm.nicolike.cn

*)     echo "未知命令" ;;
来源：http://an.yuntaijiaju.cn

esac
来源：http://ha.hahajie.cn

[R12] for 遍历文件
来源：http://pa.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://jx.muxihuayi.cn

[R13] for 计数循环
来源：http://tg.haigaiapp.cn

for i in {1..10}; do echo "$i"; done
来源：http://ig.9csxet.cn

[R14] C 风格 for
来源：http://oo.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://of.hnjuh.cn

[R15] while 逐行读文件
来源：http://fg.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://my.hnjuh.cn

[R16] until 等待条件
来源：http://lq.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tz.jctech888.com.cn

[R17] 数组定义与取值
来源：http://tl.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sm.hnjuh.cn

[R18] 遍历数组
来源：http://iv.colortex.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://du.hahajie.cn

[R19] 数组长度
来源：http://sj.huanxung.cn

echo "${#arr[@]}"
来源：http://iz.9csxet.cn

[R20] 关联数组（字典）
来源：http://ja.muxihuayi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hv.szsharing.cn

[R21] 字符串长度
来源：http://zi.jianghongdianzi.cn

echo "${#s}"
来源：http://sz.hahajie.cn

[R22] 截取子串
来源：http://hh.haigaiapp.cn

echo "${s:0:5}"
来源：http://bn.bjjhwx.cn

[R23] 字符串替换
来源：http://xe.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ha.hnjuh.cn

[R24] 大小写转换
来源：http://vd.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://my.9csxet.cn

[R25] 去后缀 / 去前缀
来源：http://pe.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qu.bjjhwx.cn

[R26] 命令替换
来源：http://uo.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://mf.hahajie.cn

[R27] 算术展开
来源：http://ph.bookmarksfly.cn

echo $((1 + 2 * 3))
来源：http://ym.szsharing.cn

[R28] 浮点运算
来源：http://cp.colortex.cn

echo "scale=2; 10/3" | bc
来源：http://zv.nszjky.cn

[R29] 定义函数
来源：http://wx.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gz.shtwfgs.cn

[R30] 函数返回状态码
来源：http://gw.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://ll.gzmigu.cn

[R31] 局部变量
来源：http://ed.hnjuh.cn

f() { local x=1; echo "$x"; }
来源：http://ha.bookmarksfly.cn

[R32] 参数个数校验
来源：http://bo.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zj.colortex.cn

[R33] 捕获错误并提示行号
来源：http://gu.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://it.huixinmuqiang.cn

[R34] 退出时清理
来源：http://vk.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gs.hnjuh.cn

[R35] 后台执行并等待
来源：http://ww.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jz.lnxyls.cn

[R36] 并发执行多个任务
来源：http://dt.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wq.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://xk.huixinmuqiang.cn

files=$(ls -1)
来源：http://ha.hnjuh.cn

[R38] 管道串联
来源：http://lp.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://sj.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://qq.huanxung.cn

cmd > out.log 2>&1
来源：http://bf.gzmigu.cn

[R40] 追加写日志
来源：http://sy.jianghongdianzi.cn

echo "log" >> out.log
来源：http://ei.haigaiapp.cn

[R41] 丢弃输出
来源：http://xn.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://oj.hahajie.cn

[R42] 输入重定向
来源：http://rh.521024.cn

wc -l < a.txt
来源：http://vq.szxytkj.cn

[R43] 按名字查找文件
来源：http://tn.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://ij.lnxyls.cn

[R44] 按修改时间查找
来源：http://hk.nszjky.cn

find . -mtime -7 -type f
来源：http://bg.nicolike.cn

[R45] 批量删除
来源：http://no.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://nw.nicolike.cn

[R46] 递归替换文件内容
来源：http://ch.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bf.huanxung.cn

[R47] sed 单行替换
来源：http://ec.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nl.asd995.cn

[R48] awk 取指定列
来源：http://pd.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://cy.yuexingan06.cn

[R49] awk 带条件
来源：http://yy.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cs.szsharing.cn

[R50] awk 求和
来源：http://wh.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jz.nicolike.cn

[R51] 排序去重取前几
来源：http://fl.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qe.hahajie.cn

[R52] 统计行数
来源：http://kl.hnjuh.cn

wc -l a.txt
来源：http://ac.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://do.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://az.szxytkj.cn

[R54] 比较两个文件
来源：http://rf.yuntaijiaju.cn

diff a.txt b.txt
来源：http://dg.jctech888.com.cn

[R55] 压缩与解压
来源：http://ys.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hh.9csxet.cn

[R56] 远程拷贝
来源：http://fw.chemitech.net.cn

scp file user@host:/path/
来源：http://yl.szxytkj.cn

[R57] 远程执行命令
来源：http://cz.szxytkj.cn

ssh user@host 'uptime'
来源：http://cc.yuntaijiaju.cn

[R58] 下载文件
来源：http://cw.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dt.shtwfgs.cn

[R59] 发 POST JSON
来源：http://pp.521024.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nx.nicolike.cn

[R60] 只看 HTTP 状态码
来源：http://qr.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zh.colortex.cn

[R61] 磁盘占用
来源：http://ql.bjjhwx.cn

df -h;  du -sh *
来源：http://qc.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://gb.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://cl.hahajie.cn

[R63] 内存与进程
来源：http://im.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://oi.hnjuh.cn

[R64] 结束进程
来源：http://un.nicolike.cn

kill -9 $(pgrep -f app.py)
来源：http://yu.colortex.cn

[R65] 查看端口占用
来源：http://dt.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xw.asd995.cn

[R66] 定时任务
来源：http://ve.haigaiapp.cn

crontab -e;  crontab -l
来源：http://xg.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://jo.szsharing.cn

openssl rand -hex 16
来源：http://uj.shxzskj.cn

[R68] 计算文件校验值
来源：http://hx.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wc.bookmarksfly.cn

[R69] 生成随机密码
来源：http://xc.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://ne.nszjky.cn

[R70] 时间戳与互转
来源：http://ti.521024.cn

date +%s;  date -d @1700000000
来源：http://dk.huixiangedu.cn

[R71] 日期格式化
来源：http://wl.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dd.haigaiapp.cn

[R72] 等待端口就绪
来源：http://wv.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gr.hahajie.cn

[R73] 分割大日志
来源：http://si.muxihuayi.cn

split -l 1000 big.log part_
来源：http://dv.panjiajie.cn

[R74] 批量重命名
来源：http://ok.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bk.bookmarksfly.cn

[R75] 导出环境变量
来源：http://eu.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://xm.szsharing.cn

[R76] 使用临时文件
来源：http://cq.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dq.hnjuh.cn

[R77] 读取用户输入
来源：http://bb.shxzskj.cn

read -rp "请输入: " ans
来源：http://ef.hnjuh.cn

[R78] 交互式菜单
来源：http://bv.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tp.wgjwhj.cn

[R79] 解析命令行选项
来源：http://ub.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zz.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://cx.panjiajie.cn

time ./run.sh
来源：http://hy.shxzukj.cn

================================================================================
来源：http://fa.huixiangedu.cn

S. C / C++ 专题
来源：http://ff.colortex.cn

================================================================================
来源：http://px.nicolike.cn

[S01] C：Hello World
来源：http://tt.bjjhwx.cn

#include <stdio.h>
来源：http://vh.panjiajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wh.nszjky.cn

[S02] C：变量与格式化输出
来源：http://ht.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://zx.muxihuayi.cn

[S03] C：读入整数
来源：http://qp.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://ek.shxzukj.cn

[S04] C：字符串复制
来源：http://jb.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kf.haigaiapp.cn

[S05] C：字符串长度
来源：http://cc.nicolike.cn

strlen(s)
来源：http://rl.panjiajie.cn

[S06] C：字符串比较
来源：http://ig.colortex.cn

strcmp(a, b) == 0
来源：http://lr.shxzskj.cn

[S07] C：数组遍历求和
来源：http://qf.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://me.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://mg.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rp.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://mc.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ro.szsharing.cn

[S10] C：指针与解引用
来源：http://bv.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://bj.jctech888.com.cn

[S11] C：逐行读文件
来源：http://cy.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://nm.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vs.chemitech.net.cn

fclose(f);
来源：http://ny.9csxet.cn

[S12] C：写文件
来源：http://aj.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://re.hnjuh.cn

[S13] C：宏定义
来源：http://ga.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qn.szsharing.cn

[S14] C：枚举
来源：http://qt.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://hj.colortex.cn

[S15] C：类型转换
来源：http://bx.jianghongdianzi.cn

(double) a / b
来源：http://du.lnxyls.cn

[S16] C：位操作置位
来源：http://ot.szsharing.cn

x |= (1 << 3);
来源：http://jm.hahajie.cn

[S17] C：安全拼接字符串
来源：http://kg.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lj.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://ul.lnxyls.cn

int main(int argc, char **argv)
来源：http://ie.chemitech.net.cn

[S19] C：快速排序
来源：http://hk.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oq.yuntaijiaju.cn

[S20] C：二分查找
来源：http://aq.9csxet.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wv.nszjky.cn

[S21] C：字符类别判断
来源：http://mn.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hp.shtwfgs.cn

[S22] C：字符串转数字
来源：http://bf.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yh.lnxyls.cn

[S23] C：随机数
来源：http://iy.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zq.muxihuayi.cn

[S24] C：获取本地时间
来源：http://qm.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gt.shtwfgs.cn

[S25] C：内存拷贝
来源：http://fe.shxzskj.cn

memcpy(dst, src, n);
来源：http://qd.bookmarksfly.cn

[S26] C：内存清零
来源：http://kq.szsharing.cn

memset(a, 0, sizeof a);
来源：http://xf.huixiangedu.cn

[S27] C：定义常量
来源：http://se.yuexingan06.cn

const double PI = 3.14159;
来源：http://co.shtwfgs.cn

[S28] C：静态变量
来源：http://ul.huixinmuqiang.cn

static int counter = 0;
来源：http://qe.shtwfgs.cn

[S29] C：变参函数
来源：http://yy.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fb.bjjhwx.cn

[S30] C：头文件保护
来源：http://ib.huixinmuqiang.cn

#ifndef X_H
来源：http://hj.nszjky.cn

#define X_H
来源：http://dx.jianghongdianzi.cn

#endif
来源：http://jj.shtwfgs.cn

[S31] C++：Hello World
来源：http://xe.yuexingan06.cn


<!-- 参考信息 -->