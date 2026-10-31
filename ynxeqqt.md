代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kn.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://kf.nicolike.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nt.yuntaijiaju.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ui.huanxung.cn

[Q61] 移动平均
来源：http://xm.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vt.wgjwhj.cn

[Q62] 分组占比
来源：http://lq.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zn.hnjuh.cn

[Q63] 开启事务
来源：http://fz.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jr.bjjhwx.cn

[Q64] 提交事务
来源：http://gy.huanxung.cn

COMMIT;
来源：http://uu.shxzskj.cn

[Q65] 回滚事务
来源：http://gn.asd995.cn

ROLLBACK;
来源：http://jl.521024.cn

[Q66] 行锁查询
来源：http://iq.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cy.wgjwhj.cn

[Q67] 设置隔离级别
来源：http://lr.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qw.nszjky.cn

[Q68] 保存点
来源：http://hb.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://qr.9csxet.cn

ROLLBACK TO sp1;
来源：http://mz.gzmigu.cn

[Q69] 查看执行计划
来源：http://gt.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zf.asd995.cn

[Q70] 更新统计信息
来源：http://af.hahajie.cn

ANALYZE TABLE users;
来源：http://dk.huanxung.cn

[Q71] 查看建表语句
来源：http://ia.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://to.nszjky.cn

[Q72] 查看索引
来源：http://ah.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://nd.521024.cn

[Q73] 查看表状态
来源：http://we.newstarts.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kz.nicolike.cn

[Q74] 强制使用索引
来源：http://ef.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tt.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://db.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ob.bookmarksfly.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://el.hnjuh.cn

[Q76] 按天统计
来源：http://mo.nszjky.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://la.huixiangedu.cn

[Q77] 时间加减
来源：http://gb.wgjwhj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jz.nszjky.cn

[Q78] 当前时间
来源：http://sx.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nf.nszjky.cn

[Q79] 字符串拼接
来源：http://bs.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ia.huixiangedu.cn

[Q80] 字符串截取
来源：http://zu.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vw.szsharing.cn

[Q81] 字符串替换
来源：http://yl.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bl.bookmarksfly.cn

[Q82] 字符长度与字节长度
来源：http://si.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uu.nicolike.cn

[Q83] 大小写转换
来源：http://by.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ib.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://rc.jctech888.com.cn

SELECT TRIM(name) FROM users;
来源：http://ze.521024.cn

[Q85] 数值取整
来源：http://te.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mx.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://gf.9csxet.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pk.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://ub.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gx.lnxyls.cn

[Q88] 行转列（条件聚合）
来源：http://sn.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qe.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xn.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://or.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://od.hnjuh.cn

[Q90] 生成序号列
来源：http://ay.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://id.asd995.cn

================================================================================
来源：http://pj.521024.cn

R. Bash 专题
来源：http://xe.colortex.cn

================================================================================
来源：http://is.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://be.muxihuayi.cn

#!/usr/bin/env bash
来源：http://rx.chemitech.net.cn

set -euo pipefail
来源：http://aa.shxzukj.cn

[R02] 变量赋值与使用
来源：http://te.gzmigu.cn

name="Tom"; echo "$name"
来源：http://hf.chemitech.net.cn

[R03] 只读变量
来源：http://vq.hnjuh.cn

readonly PI=3.14
来源：http://ey.521024.cn

[R04] 位置参数
来源：http://fz.panjiajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hp.szsharing.cn

[R05] 参数默认值
来源：http://yn.szxytkj.cn

name="${1:-default}"
来源：http://pc.haigaiapp.cn

[R06] 判断命令是否存在
来源：http://aa.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gh.bookmarksfly.cn

[R07] if 判断文件
来源：http://gt.jctech888.com.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iu.jianghongdianzi.cn

[R08] 数值比较
来源：http://oo.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cw.9csxet.cn

[R09] 字符串比较
来源：http://yc.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jb.jctech888.com.cn

[R10] 正则匹配
来源：http://bs.shxzukj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mh.szxytkj.cn

[R11] case 多分支
来源：http://gv.hahajie.cn

case "$1" in
来源：http://op.colortex.cn

start) echo "启动" ;;
来源：http://zk.newstarts.cn

stop)  echo "停止" ;;
来源：http://ei.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://rw.lnxyls.cn

esac
来源：http://ho.haigaiapp.cn

[R12] for 遍历文件
来源：http://ph.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://fo.wgjwhj.cn

[R13] for 计数循环
来源：http://ka.colortex.cn

for i in {1..10}; do echo "$i"; done
来源：http://iu.lnxyls.cn

[R14] C 风格 for
来源：http://hv.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tl.521024.cn

[R15] while 逐行读文件
来源：http://im.yuexingan06.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fv.hnjuh.cn

[R16] until 等待条件
来源：http://ez.huixiangedu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wc.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://pv.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ix.bookmarksfly.cn

[R18] 遍历数组
来源：http://zc.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hh.jctech888.com.cn

[R19] 数组长度
来源：http://xh.jianghongdianzi.cn

echo "${#arr[@]}"
来源：http://mx.9csxet.cn

[R20] 关联数组（字典）
来源：http://rl.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yv.nszjky.cn

[R21] 字符串长度
来源：http://lr.newstarts.cn

echo "${#s}"
来源：http://xa.shxzukj.cn

[R22] 截取子串
来源：http://oq.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://jd.wgjwhj.cn

[R23] 字符串替换
来源：http://oq.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cl.chemitech.net.cn

[R24] 大小写转换
来源：http://ec.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jy.9csxet.cn

[R25] 去后缀 / 去前缀
来源：http://lj.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yl.haigaiapp.cn

[R26] 命令替换
来源：http://pc.shxzukj.cn

now=$(date +%F); echo "$now"
来源：http://zr.huixinmuqiang.cn

[R27] 算术展开
来源：http://br.asd995.cn

echo $((1 + 2 * 3))
来源：http://tj.nicolike.cn

[R28] 浮点运算
来源：http://tk.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://bk.yuexingan06.cn

[R29] 定义函数
来源：http://xm.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rp.9csxet.cn

[R30] 函数返回状态码
来源：http://zs.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://qa.bookmarksfly.cn

[R31] 局部变量
来源：http://cy.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://up.szxytkj.cn

[R32] 参数个数校验
来源：http://us.colortex.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fe.asd995.cn

[R33] 捕获错误并提示行号
来源：http://lx.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xg.szsharing.cn

[R34] 退出时清理
来源：http://ko.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hc.asd995.cn

[R35] 后台执行并等待
来源：http://tr.gzmigu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kq.gzmigu.cn

[R36] 并发执行多个任务
来源：http://mn.shxzukj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cx.huanxung.cn

[R37] 把输出赋给变量
来源：http://pe.panjiajie.cn

files=$(ls -1)
来源：http://bk.yuntaijiaju.cn

[R38] 管道串联
来源：http://yb.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://mg.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://si.hahajie.cn

cmd > out.log 2>&1
来源：http://ox.panjiajie.cn

[R40] 追加写日志
来源：http://nn.colortex.cn

echo "log" >> out.log
来源：http://tc.bookmarksfly.cn

[R41] 丢弃输出
来源：http://ov.hahajie.cn

cmd >/dev/null 2>&1
来源：http://gh.shtwfgs.cn

[R42] 输入重定向
来源：http://xb.colortex.cn

wc -l < a.txt
来源：http://mt.haigaiapp.cn

[R43] 按名字查找文件
来源：http://se.newstarts.cn

find . -name "*.log" -type f
来源：http://be.yuexingan06.cn

[R44] 按修改时间查找
来源：http://in.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://hc.hahajie.cn

[R45] 批量删除
来源：http://az.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://gy.newstarts.cn

[R46] 递归替换文件内容
来源：http://no.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xl.yuexingan06.cn

[R47] sed 单行替换
来源：http://xc.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pa.chemitech.net.cn

[R48] awk 取指定列
来源：http://mz.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://kf.huanxung.cn

[R49] awk 带条件
来源：http://bc.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oh.yuexingan06.cn

[R50] awk 求和
来源：http://zu.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uu.szsharing.cn

[R51] 排序去重取前几
来源：http://cp.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bz.huanxung.cn

[R52] 统计行数
来源：http://pc.yuntaijiaju.cn

wc -l a.txt
来源：http://ah.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://lh.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wi.hnjuh.cn

[R54] 比较两个文件
来源：http://ar.colortex.cn

diff a.txt b.txt
来源：http://cv.colortex.cn

[R55] 压缩与解压
来源：http://ua.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hs.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://rj.huanxung.cn

scp file user@host:/path/
来源：http://mn.gzmigu.cn

[R57] 远程执行命令
来源：http://rf.wgjwhj.cn

ssh user@host 'uptime'
来源：http://fx.muxihuayi.cn

[R58] 下载文件
来源：http://iu.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yt.newstarts.cn

[R59] 发 POST JSON
来源：http://nu.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fd.nicolike.cn

[R60] 只看 HTTP 状态码
来源：http://ur.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lj.shxzukj.cn

[R61] 磁盘占用
来源：http://bb.muxihuayi.cn

df -h;  du -sh *
来源：http://uj.panjiajie.cn

[R62] 找最占空间的文件
来源：http://zn.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://bp.hahajie.cn

[R63] 内存与进程
来源：http://gg.haigaiapp.cn

free -h;  ps aux | grep nginx
来源：http://iq.shxzukj.cn

[R64] 结束进程
来源：http://uq.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://eb.chemitech.net.cn

[R65] 查看端口占用
来源：http://xr.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mq.huixiangedu.cn

[R66] 定时任务
来源：http://an.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://ws.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://tk.521024.cn

openssl rand -hex 16
来源：http://kv.huixiangedu.cn

[R68] 计算文件校验值
来源：http://tt.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ku.jctech888.com.cn

[R69] 生成随机密码
来源：http://if.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://fv.hnjuh.cn

[R70] 时间戳与互转
来源：http://mc.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://aw.panjiajie.cn

[R71] 日期格式化
来源：http://xj.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dl.hahajie.cn

[R72] 等待端口就绪
来源：http://fx.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ua.huanxung.cn

[R73] 分割大日志
来源：http://nd.asd995.cn

split -l 1000 big.log part_
来源：http://ob.shtwfgs.cn

[R74] 批量重命名
来源：http://jd.haigaiapp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dy.panjiajie.cn

[R75] 导出环境变量
来源：http://dg.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://hj.shxzskj.cn

[R76] 使用临时文件
来源：http://jj.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jy.bookmarksfly.cn

[R77] 读取用户输入
来源：http://fw.yuntaijiaju.cn

read -rp "请输入: " ans
来源：http://ou.lnxyls.cn

[R78] 交互式菜单
来源：http://uo.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mw.colortex.cn

[R79] 解析命令行选项
来源：http://xg.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wq.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://hk.colortex.cn

time ./run.sh
来源：http://fj.bjjhwx.cn

================================================================================
来源：http://vk.shtwfgs.cn

S. C / C++ 专题
来源：http://qw.szsharing.cn

================================================================================
来源：http://py.9csxet.cn

[S01] C：Hello World
来源：http://nn.haigaiapp.cn

#include <stdio.h>
来源：http://tl.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fv.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://aq.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://fc.bjjhwx.cn

[S03] C：读入整数
来源：http://hn.szsharing.cn

int x; scanf("%d", &x);
来源：http://vc.hnjuh.cn

[S04] C：字符串复制
来源：http://jp.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bc.yuexingan06.cn

[S05] C：字符串长度
来源：http://xs.panjiajie.cn

strlen(s)
来源：http://kk.huixiangedu.cn

[S06] C：字符串比较
来源：http://lu.521024.cn

strcmp(a, b) == 0
来源：http://km.9csxet.cn

[S07] C：数组遍历求和
来源：http://sp.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vi.9csxet.cn

[S08] C：动态内存分配与释放
来源：http://rr.jctech888.com.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xn.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://vl.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vu.huanxung.cn

[S10] C：指针与解引用
来源：http://nz.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://qc.hnjuh.cn

[S11] C：逐行读文件
来源：http://tn.haigaiapp.cn

FILE *f = fopen("a.txt", "r");
来源：http://ge.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mg.gzmigu.cn

fclose(f);
来源：http://xu.huixinmuqiang.cn

[S12] C：写文件
来源：http://ga.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ie.bjjhwx.cn

[S13] C：宏定义
来源：http://hm.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yo.panjiajie.cn

[S14] C：枚举
来源：http://hc.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://ju.hnjuh.cn

[S15] C：类型转换
来源：http://en.jianghongdianzi.cn

(double) a / b
来源：http://sf.nszjky.cn

[S16] C：位操作置位
来源：http://ke.yuexingan06.cn

x |= (1 << 3);
来源：http://ov.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://oy.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ac.jctech888.com.cn

[S18] C：命令行参数
来源：http://rs.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://yg.nszjky.cn

[S19] C：快速排序
来源：http://sv.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yy.521024.cn

[S20] C：二分查找
来源：http://jk.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uk.nszjky.cn

[S21] C：字符类别判断
来源：http://kz.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://un.huixiangedu.cn

[S22] C：字符串转数字
来源：http://rw.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://er.nicolike.cn

[S23] C：随机数
来源：http://ar.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rz.hnjuh.cn

[S24] C：获取本地时间
来源：http://ru.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bu.nicolike.cn

[S25] C：内存拷贝
来源：http://yw.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://ec.panjiajie.cn

[S26] C：内存清零
来源：http://za.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://pf.haigaiapp.cn

[S27] C：定义常量
来源：http://mz.nszjky.cn

const double PI = 3.14159;
来源：http://mj.jctech888.com.cn

[S28] C：静态变量
来源：http://uv.shxzskj.cn

static int counter = 0;
来源：http://km.bookmarksfly.cn

[S29] C：变参函数
来源：http://jc.panjiajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fh.gzmigu.cn

[S30] C：头文件保护
来源：http://oq.jianghongdianzi.cn


<!-- 参考信息 -->