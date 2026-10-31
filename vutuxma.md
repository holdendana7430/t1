代发 wailian999

[Q63] 开启事务
来源：http://yd.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ao.colortex.cn

[Q64] 提交事务
来源：http://yq.huanxung.cn

COMMIT;
来源：http://fs.shtwfgs.cn

[Q65] 回滚事务
来源：http://hm.jianghongdianzi.cn

ROLLBACK;
来源：http://sl.huanxung.cn

[Q66] 行锁查询
来源：http://dv.asd995.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xb.hnjuh.cn

[Q67] 设置隔离级别
来源：http://lh.huixinmuqiang.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yi.9csxet.cn

[Q68] 保存点
来源：http://dn.szsharing.cn

SAVEPOINT sp1;
来源：http://yv.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://db.9csxet.cn

[Q69] 查看执行计划
来源：http://gh.haigaiapp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oe.jctech888.com.cn

[Q70] 更新统计信息
来源：http://wf.jctech888.com.cn

ANALYZE TABLE users;
来源：http://md.lnxyls.cn

[Q71] 查看建表语句
来源：http://jd.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fy.haigaiapp.cn

[Q72] 查看索引
来源：http://yr.colortex.cn

SHOW INDEX FROM users;
来源：http://at.jctech888.com.cn

[Q73] 查看表状态
来源：http://qd.szxytkj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ar.asd995.cn

[Q74] 强制使用索引
来源：http://uc.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hw.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://jh.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eo.szxytkj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dx.asd995.cn

[Q76] 按天统计
来源：http://cn.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wf.wgjwhj.cn

[Q77] 时间加减
来源：http://wr.jianghongdianzi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sh.huixinmuqiang.cn

[Q78] 当前时间
来源：http://ub.yuexingan06.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yx.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://hw.asd995.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lz.shxzskj.cn

[Q80] 字符串截取
来源：http://kg.chemitech.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uw.newstarts.cn

[Q81] 字符串替换
来源：http://vj.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jx.9csxet.cn

[Q82] 字符长度与字节长度
来源：http://dh.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ty.hnjuh.cn

[Q83] 大小写转换
来源：http://tb.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yn.lnxyls.cn

[Q84] 去除首尾空格
来源：http://jp.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://xq.szxytkj.cn

[Q85] 数值取整
来源：http://jz.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rt.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://dr.9csxet.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hd.yuntaijiaju.cn

[Q87] JSON 字段做条件
来源：http://pt.newstarts.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fb.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://nc.asd995.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vz.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tm.muxihuayi.cn

[Q89] 判断表是否存在
来源：http://fz.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ep.haigaiapp.cn

[Q90] 生成序号列
来源：http://cs.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cw.wgjwhj.cn

================================================================================
来源：http://kn.huixiangedu.cn

R. Bash 专题
来源：http://sa.huanxung.cn

================================================================================
来源：http://uf.shtwfgs.cn

[R01] shebang 与严格模式
来源：http://xa.huixiangedu.cn

#!/usr/bin/env bash
来源：http://ba.newstarts.cn

set -euo pipefail
来源：http://ak.szxytkj.cn

[R02] 变量赋值与使用
来源：http://iq.huanxung.cn

name="Tom"; echo "$name"
来源：http://qy.huanxung.cn

[R03] 只读变量
来源：http://kl.jianghongdianzi.cn

readonly PI=3.14
来源：http://wa.bookmarksfly.cn

[R04] 位置参数
来源：http://zd.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wy.jctech888.com.cn

[R05] 参数默认值
来源：http://og.panjiajie.cn

name="${1:-default}"
来源：http://hk.huanxung.cn

[R06] 判断命令是否存在
来源：http://ia.yuexingan06.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ij.huixiangedu.cn

[R07] if 判断文件
来源：http://yc.newstarts.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nm.panjiajie.cn

[R08] 数值比较
来源：http://oz.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yc.szsharing.cn

[R09] 字符串比较
来源：http://rg.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xv.9csxet.cn

[R10] 正则匹配
来源：http://je.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jx.newstarts.cn

[R11] case 多分支
来源：http://ga.szsharing.cn

case "$1" in
来源：http://ax.lnxyls.cn

start) echo "启动" ;;
来源：http://gd.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://ef.wgjwhj.cn

*)     echo "未知命令" ;;
来源：http://uf.szxytkj.cn

esac
来源：http://uf.nszjky.cn

[R12] for 遍历文件
来源：http://qt.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://ql.gzmigu.cn

[R13] for 计数循环
来源：http://hl.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://kt.muxihuayi.cn

[R14] C 风格 for
来源：http://po.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qs.9csxet.cn

[R15] while 逐行读文件
来源：http://ya.gzmigu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xe.bookmarksfly.cn

[R16] until 等待条件
来源：http://rq.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nb.jctech888.com.cn

[R17] 数组定义与取值
来源：http://pu.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hb.huanxung.cn

[R18] 遍历数组
来源：http://ai.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zy.jianghongdianzi.cn

[R19] 数组长度
来源：http://zo.jianghongdianzi.cn

echo "${#arr[@]}"
来源：http://ud.9csxet.cn

[R20] 关联数组（字典）
来源：http://ib.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pn.yuntaijiaju.cn

[R21] 字符串长度
来源：http://ru.hahajie.cn

echo "${#s}"
来源：http://az.szsharing.cn

[R22] 截取子串
来源：http://hq.yuexingan06.cn

echo "${s:0:5}"
来源：http://vx.yuexingan06.cn

[R23] 字符串替换
来源：http://ir.lnxyls.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yi.shxzskj.cn

[R24] 大小写转换
来源：http://iq.hnjuh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qp.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://qg.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ub.huixinmuqiang.cn

[R26] 命令替换
来源：http://pm.521024.cn

now=$(date +%F); echo "$now"
来源：http://rn.bjjhwx.cn

[R27] 算术展开
来源：http://ub.9csxet.cn

echo $((1 + 2 * 3))
来源：http://wx.newstarts.cn

[R28] 浮点运算
来源：http://ye.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://if.nicolike.cn

[R29] 定义函数
来源：http://zk.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nl.521024.cn

[R30] 函数返回状态码
来源：http://hk.szxytkj.cn

f() { return 0; }; f || echo "失败了"
来源：http://bc.bjjhwx.cn

[R31] 局部变量
来源：http://qp.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://zy.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://jx.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wh.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://cm.hnjuh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oq.shxzukj.cn

[R34] 退出时清理
来源：http://pw.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qn.colortex.cn

[R35] 后台执行并等待
来源：http://kx.jianghongdianzi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vw.521024.cn

[R36] 并发执行多个任务
来源：http://gj.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wt.szxytkj.cn

[R37] 把输出赋给变量
来源：http://ut.newstarts.cn

files=$(ls -1)
来源：http://hd.haigaiapp.cn

[R38] 管道串联
来源：http://cl.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://br.lnxyls.cn

[R39] 重定向标准输出与错误
来源：http://bw.jctech888.com.cn

cmd > out.log 2>&1
来源：http://sc.asd995.cn

[R40] 追加写日志
来源：http://en.szsharing.cn

echo "log" >> out.log
来源：http://lo.bjjhwx.cn

[R41] 丢弃输出
来源：http://gc.szsharing.cn

cmd >/dev/null 2>&1
来源：http://nf.huixiangedu.cn

[R42] 输入重定向
来源：http://cq.bjjhwx.cn

wc -l < a.txt
来源：http://gj.9csxet.cn

[R43] 按名字查找文件
来源：http://qf.shtwfgs.cn

find . -name "*.log" -type f
来源：http://vb.shtwfgs.cn

[R44] 按修改时间查找
来源：http://pu.szsharing.cn

find . -mtime -7 -type f
来源：http://pf.muxihuayi.cn

[R45] 批量删除
来源：http://pk.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://ju.hahajie.cn

[R46] 递归替换文件内容
来源：http://bn.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://we.szsharing.cn

[R47] sed 单行替换
来源：http://gc.shxzukj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mv.bookmarksfly.cn

[R48] awk 取指定列
来源：http://yn.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://ve.hnjuh.cn

[R49] awk 带条件
来源：http://tp.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ik.shtwfgs.cn

[R50] awk 求和
来源：http://rr.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sy.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://ze.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gq.yuntaijiaju.cn

[R52] 统计行数
来源：http://wo.chemitech.net.cn

wc -l a.txt
来源：http://pm.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://vq.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cb.hahajie.cn

[R54] 比较两个文件
来源：http://pu.asd995.cn

diff a.txt b.txt
来源：http://bu.muxihuayi.cn

[R55] 压缩与解压
来源：http://uo.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://om.panjiajie.cn

[R56] 远程拷贝
来源：http://ez.9csxet.cn

scp file user@host:/path/
来源：http://tx.shxzukj.cn

[R57] 远程执行命令
来源：http://ua.shxzskj.cn

ssh user@host 'uptime'
来源：http://wg.huixiangedu.cn

[R58] 下载文件
来源：http://ck.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hb.shxzskj.cn

[R59] 发 POST JSON
来源：http://gp.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ye.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://cb.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jr.jctech888.com.cn

[R61] 磁盘占用
来源：http://ol.yuexingan06.cn

df -h;  du -sh *
来源：http://fq.shxzukj.cn

[R62] 找最占空间的文件
来源：http://qj.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://mg.muxihuayi.cn

[R63] 内存与进程
来源：http://hz.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://tu.521024.cn

[R64] 结束进程
来源：http://bb.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://ag.hahajie.cn

[R65] 查看端口占用
来源：http://ki.colortex.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sx.wgjwhj.cn

[R66] 定时任务
来源：http://jm.hahajie.cn

crontab -e;  crontab -l
来源：http://zv.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://if.chemitech.net.cn

openssl rand -hex 16
来源：http://ff.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://hf.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dd.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://id.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://fa.521024.cn

[R70] 时间戳与互转
来源：http://op.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://tu.hahajie.cn

[R71] 日期格式化
来源：http://vv.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nx.newstarts.cn

[R72] 等待端口就绪
来源：http://bf.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yi.jctech888.com.cn

[R73] 分割大日志
来源：http://ey.521024.cn

split -l 1000 big.log part_
来源：http://fw.hnjuh.cn

[R74] 批量重命名
来源：http://fj.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ww.bookmarksfly.cn

[R75] 导出环境变量
来源：http://oc.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://dk.muxihuayi.cn

[R76] 使用临时文件
来源：http://pm.jianghongdianzi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jh.chemitech.net.cn

[R77] 读取用户输入
来源：http://en.colortex.cn

read -rp "请输入: " ans
来源：http://rr.muxihuayi.cn

[R78] 交互式菜单
来源：http://ms.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zf.panjiajie.cn

[R79] 解析命令行选项
来源：http://yz.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://go.yuntaijiaju.cn

[R80] 查看脚本执行耗时
来源：http://wk.nszjky.cn

time ./run.sh
来源：http://rm.jctech888.com.cn

================================================================================
来源：http://hf.haigaiapp.cn

S. C / C++ 专题
来源：http://yd.haigaiapp.cn

================================================================================
来源：http://sq.colortex.cn

[S01] C：Hello World
来源：http://kh.wgjwhj.cn

#include <stdio.h>
来源：http://wa.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://aq.asd995.cn

[S02] C：变量与格式化输出
来源：http://fl.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://my.chemitech.net.cn

[S03] C：读入整数
来源：http://vl.9csxet.cn

int x; scanf("%d", &x);
来源：http://fi.wgjwhj.cn

[S04] C：字符串复制
来源：http://vb.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://eh.lnxyls.cn

[S05] C：字符串长度
来源：http://wc.yuntaijiaju.cn

strlen(s)
来源：http://ox.bookmarksfly.cn

[S06] C：字符串比较
来源：http://kj.colortex.cn

strcmp(a, b) == 0
来源：http://it.huanxung.cn

[S07] C：数组遍历求和
来源：http://xe.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pa.huixinmuqiang.cn

[S08] C：动态内存分配与释放
来源：http://zc.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://by.huixinmuqiang.cn

[S09] C：结构体定义与初始化
来源：http://ag.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bx.lnxyls.cn

[S10] C：指针与解引用
来源：http://ky.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://gv.panjiajie.cn

[S11] C：逐行读文件
来源：http://bb.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://nw.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zh.newstarts.cn

fclose(f);
来源：http://lh.shtwfgs.cn

[S12] C：写文件
来源：http://gz.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ow.huixinmuqiang.cn

[S13] C：宏定义
来源：http://af.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wq.jianghongdianzi.cn

[S14] C：枚举
来源：http://jg.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://mj.nicolike.cn

[S15] C：类型转换
来源：http://no.bookmarksfly.cn

(double) a / b
来源：http://jg.yuexingan06.cn

[S16] C：位操作置位
来源：http://by.colortex.cn

x |= (1 << 3);
来源：http://dn.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://kp.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dc.9csxet.cn

[S18] C：命令行参数
来源：http://ef.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://fz.szsharing.cn

[S19] C：快速排序
来源：http://nu.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gc.jctech888.com.cn

[S20] C：二分查找
来源：http://bo.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ap.yuexingan06.cn

[S21] C：字符类别判断
来源：http://kf.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nu.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://xt.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://li.nicolike.cn

[S23] C：随机数
来源：http://jo.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fd.lnxyls.cn

[S24] C：获取本地时间
来源：http://pq.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hp.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://ik.huixiangedu.cn

memcpy(dst, src, n);
来源：http://ii.shtwfgs.cn

[S26] C：内存清零
来源：http://ke.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://tl.jctech888.com.cn

[S27] C：定义常量
来源：http://ws.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://vh.bookmarksfly.cn

[S28] C：静态变量
来源：http://vc.shtwfgs.cn

static int counter = 0;
来源：http://mr.panjiajie.cn

[S29] C：变参函数
来源：http://ai.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sv.colortex.cn

[S30] C：头文件保护
来源：http://hn.chemitech.net.cn

#ifndef X_H
来源：http://dw.yuexingan06.cn

#define X_H
来源：http://tn.gzmigu.cn

#endif
来源：http://rm.nicolike.cn

[S31] C++：Hello World
来源：http://av.muxihuayi.cn

#include <iostream>
来源：http://cw.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://to.yuntaijiaju.cn

[S32] C++：字符串
来源：http://sd.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://xr.newstarts.cn


<!-- 参考信息 -->