代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ul.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://jg.haigaiapp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wg.huanxung.cn

[Q57] 行号
来源：http://hc.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bz.huixinmuqiang.cn

[Q58] 累计求和
来源：http://ip.bookmarksfly.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sl.nicolike.cn

[Q59] 分组内累计
来源：http://du.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ml.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://sg.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bw.jianghongdianzi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hi.huixinmuqiang.cn

[Q61] 移动平均
来源：http://dh.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sn.shxzukj.cn

[Q62] 分组占比
来源：http://yk.hnjuh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wk.wgjwhj.cn

[Q63] 开启事务
来源：http://dx.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ir.chemitech.net.cn

[Q64] 提交事务
来源：http://ds.haigaiapp.cn

COMMIT;
来源：http://sb.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://go.panjiajie.cn

ROLLBACK;
来源：http://yh.nicolike.cn

[Q66] 行锁查询
来源：http://uz.colortex.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gn.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://cf.szsharing.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://il.nszjky.cn

[Q68] 保存点
来源：http://ms.bjjhwx.cn

SAVEPOINT sp1;
来源：http://kz.muxihuayi.cn

ROLLBACK TO sp1;
来源：http://ws.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://du.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ph.gzmigu.cn

[Q70] 更新统计信息
来源：http://il.bjjhwx.cn

ANALYZE TABLE users;
来源：http://gb.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://tb.huixinmuqiang.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xv.szsharing.cn

[Q72] 查看索引
来源：http://sh.gzmigu.cn

SHOW INDEX FROM users;
来源：http://ix.colortex.cn

[Q73] 查看表状态
来源：http://vq.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ff.chemitech.net.cn

[Q74] 强制使用索引
来源：http://tb.nicolike.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bs.hahajie.cn

[Q75] 日期格式化
来源：http://kj.521024.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ar.nicolike.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ua.yuntaijiaju.cn

[Q76] 按天统计
来源：http://cg.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dh.huixiangedu.cn

[Q77] 时间加减
来源：http://ss.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ij.colortex.cn

[Q78] 当前时间
来源：http://tu.yuexingan06.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://po.haigaiapp.cn

[Q79] 字符串拼接
来源：http://dm.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fz.nicolike.cn

[Q80] 字符串截取
来源：http://kb.bjjhwx.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lk.shxzskj.cn

[Q81] 字符串替换
来源：http://nj.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sv.chemitech.net.cn

[Q82] 字符长度与字节长度
来源：http://hc.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gt.hnjuh.cn

[Q83] 大小写转换
来源：http://bg.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hm.bjjhwx.cn

[Q84] 去除首尾空格
来源：http://pj.colortex.cn

SELECT TRIM(name) FROM users;
来源：http://kq.lnxyls.cn

[Q85] 数值取整
来源：http://rb.lnxyls.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ts.asd995.cn

[Q86] 读取 JSON 字段
来源：http://mq.haigaiapp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mb.bookmarksfly.cn

[Q87] JSON 字段做条件
来源：http://pq.huixinmuqiang.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ws.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://bx.9csxet.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mt.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hx.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://ne.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rv.asd995.cn

[Q90] 生成序号列
来源：http://xn.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ad.gzmigu.cn

================================================================================
来源：http://sv.muxihuayi.cn

R. Bash 专题
来源：http://nt.huixiangedu.cn

================================================================================
来源：http://bn.hahajie.cn

[R01] shebang 与严格模式
来源：http://he.haigaiapp.cn

#!/usr/bin/env bash
来源：http://pz.haigaiapp.cn

set -euo pipefail
来源：http://lx.bookmarksfly.cn

[R02] 变量赋值与使用
来源：http://hy.9csxet.cn

name="Tom"; echo "$name"
来源：http://wo.asd995.cn

[R03] 只读变量
来源：http://rq.bookmarksfly.cn

readonly PI=3.14
来源：http://xr.bookmarksfly.cn

[R04] 位置参数
来源：http://zt.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hs.muxihuayi.cn

[R05] 参数默认值
来源：http://px.jctech888.com.cn

name="${1:-default}"
来源：http://zr.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://ji.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gz.521024.cn

[R07] if 判断文件
来源：http://al.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wr.gzmigu.cn

[R08] 数值比较
来源：http://bu.gzmigu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pa.muxihuayi.cn

[R09] 字符串比较
来源：http://ru.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cs.muxihuayi.cn

[R10] 正则匹配
来源：http://qm.haigaiapp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ma.shxzskj.cn

[R11] case 多分支
来源：http://kw.huixiangedu.cn

case "$1" in
来源：http://ux.yuexingan06.cn

start) echo "启动" ;;
来源：http://yc.shtwfgs.cn

stop)  echo "停止" ;;
来源：http://im.szxytkj.cn

*)     echo "未知命令" ;;
来源：http://zy.shxzukj.cn

esac
来源：http://df.lnxyls.cn

[R12] for 遍历文件
来源：http://zo.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://zj.gzmigu.cn

[R13] for 计数循环
来源：http://tb.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://ny.nszjky.cn

[R14] C 风格 for
来源：http://tt.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://le.jianghongdianzi.cn

[R15] while 逐行读文件
来源：http://df.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xc.yuexingan06.cn

[R16] until 等待条件
来源：http://al.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yo.bjjhwx.cn

[R17] 数组定义与取值
来源：http://bn.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jc.chemitech.net.cn

[R18] 遍历数组
来源：http://kp.newstarts.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lu.gzmigu.cn

[R19] 数组长度
来源：http://io.lnxyls.cn

echo "${#arr[@]}"
来源：http://mt.nicolike.cn

[R20] 关联数组（字典）
来源：http://sq.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cb.muxihuayi.cn

[R21] 字符串长度
来源：http://bp.nszjky.cn

echo "${#s}"
来源：http://mr.muxihuayi.cn

[R22] 截取子串
来源：http://zr.huixiangedu.cn

echo "${s:0:5}"
来源：http://vs.jctech888.com.cn

[R23] 字符串替换
来源：http://kw.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ge.wgjwhj.cn

[R24] 大小写转换
来源：http://li.hnjuh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vd.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://cj.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ka.jianghongdianzi.cn

[R26] 命令替换
来源：http://qk.colortex.cn

now=$(date +%F); echo "$now"
来源：http://cw.nicolike.cn

[R27] 算术展开
来源：http://lt.yuntaijiaju.cn

echo $((1 + 2 * 3))
来源：http://mz.szxytkj.cn

[R28] 浮点运算
来源：http://kr.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://uh.huixinmuqiang.cn

[R29] 定义函数
来源：http://kc.haigaiapp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xg.hahajie.cn

[R30] 函数返回状态码
来源：http://nf.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://uo.yuntaijiaju.cn

[R31] 局部变量
来源：http://tf.huanxung.cn

f() { local x=1; echo "$x"; }
来源：http://lo.jctech888.com.cn

[R32] 参数个数校验
来源：http://bp.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sv.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://uq.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ey.huanxung.cn

[R34] 退出时清理
来源：http://ou.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xw.newstarts.cn

[R35] 后台执行并等待
来源：http://by.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jl.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://kw.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mc.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://gl.shxzskj.cn

files=$(ls -1)
来源：http://od.szsharing.cn

[R38] 管道串联
来源：http://ub.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://bq.asd995.cn

[R39] 重定向标准输出与错误
来源：http://du.bjjhwx.cn

cmd > out.log 2>&1
来源：http://il.bjjhwx.cn

[R40] 追加写日志
来源：http://ho.huixiangedu.cn

echo "log" >> out.log
来源：http://ff.bjjhwx.cn

[R41] 丢弃输出
来源：http://oh.huanxung.cn

cmd >/dev/null 2>&1
来源：http://jd.nszjky.cn

[R42] 输入重定向
来源：http://nn.wgjwhj.cn

wc -l < a.txt
来源：http://tu.lnxyls.cn

[R43] 按名字查找文件
来源：http://gd.colortex.cn

find . -name "*.log" -type f
来源：http://xl.521024.cn

[R44] 按修改时间查找
来源：http://hp.huanxung.cn

find . -mtime -7 -type f
来源：http://ez.muxihuayi.cn

[R45] 批量删除
来源：http://ug.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://rw.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://ug.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jv.yuexingan06.cn

[R47] sed 单行替换
来源：http://nm.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zi.wgjwhj.cn

[R48] awk 取指定列
来源：http://vi.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://pn.yuntaijiaju.cn

[R49] awk 带条件
来源：http://wk.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nh.9csxet.cn

[R50] awk 求和
来源：http://zu.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xh.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://co.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jm.lnxyls.cn

[R52] 统计行数
来源：http://re.bookmarksfly.cn

wc -l a.txt
来源：http://ol.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://qe.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mr.colortex.cn

[R54] 比较两个文件
来源：http://gg.yuntaijiaju.cn

diff a.txt b.txt
来源：http://pu.hahajie.cn

[R55] 压缩与解压
来源：http://ac.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oi.shtwfgs.cn

[R56] 远程拷贝
来源：http://ze.szsharing.cn

scp file user@host:/path/
来源：http://to.shtwfgs.cn

[R57] 远程执行命令
来源：http://gq.szsharing.cn

ssh user@host 'uptime'
来源：http://hf.bookmarksfly.cn

[R58] 下载文件
来源：http://xq.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ji.yuntaijiaju.cn

[R59] 发 POST JSON
来源：http://mk.panjiajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vl.wgjwhj.cn

[R60] 只看 HTTP 状态码
来源：http://mz.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xh.shxzukj.cn

[R61] 磁盘占用
来源：http://hu.colortex.cn

df -h;  du -sh *
来源：http://er.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://cm.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://dh.szxytkj.cn

[R63] 内存与进程
来源：http://jq.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://jq.wgjwhj.cn

[R64] 结束进程
来源：http://hu.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://je.bjjhwx.cn

[R65] 查看端口占用
来源：http://hs.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yn.szsharing.cn

[R66] 定时任务
来源：http://pl.colortex.cn

crontab -e;  crontab -l
来源：http://xm.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://fz.nicolike.cn

openssl rand -hex 16
来源：http://ss.yuntaijiaju.cn

[R68] 计算文件校验值
来源：http://rq.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uj.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://ke.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://ou.yuexingan06.cn

[R70] 时间戳与互转
来源：http://wl.hahajie.cn

date +%s;  date -d @1700000000
来源：http://ps.huixiangedu.cn

[R71] 日期格式化
来源：http://yx.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jc.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://zw.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dh.newstarts.cn

[R73] 分割大日志
来源：http://ml.yuexingan06.cn

split -l 1000 big.log part_
来源：http://ih.chemitech.net.cn

[R74] 批量重命名
来源：http://co.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iu.newstarts.cn

[R75] 导出环境变量
来源：http://ys.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://rf.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://ut.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vb.shtwfgs.cn

[R77] 读取用户输入
来源：http://zc.gzmigu.cn

read -rp "请输入: " ans
来源：http://za.nicolike.cn

[R78] 交互式菜单
来源：http://nt.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qf.hahajie.cn

[R79] 解析命令行选项
来源：http://gi.521024.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ju.521024.cn

[R80] 查看脚本执行耗时
来源：http://lz.nszjky.cn

time ./run.sh
来源：http://za.szxytkj.cn

================================================================================
来源：http://vm.chemitech.net.cn

S. C / C++ 专题
来源：http://wc.lnxyls.cn

================================================================================
来源：http://vc.asd995.cn

[S01] C：Hello World
来源：http://zt.jctech888.com.cn

#include <stdio.h>
来源：http://hd.huixiangedu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://iy.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://zo.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://ax.colortex.cn

[S03] C：读入整数
来源：http://tx.jianghongdianzi.cn

int x; scanf("%d", &x);
来源：http://zp.szsharing.cn

[S04] C：字符串复制
来源：http://pc.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dd.nicolike.cn

[S05] C：字符串长度
来源：http://vv.bookmarksfly.cn

strlen(s)
来源：http://xz.nicolike.cn

[S06] C：字符串比较
来源：http://mt.nicolike.cn

strcmp(a, b) == 0
来源：http://dm.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://nn.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zv.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://on.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bg.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://xs.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tl.asd995.cn

[S10] C：指针与解引用
来源：http://he.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://nr.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://fw.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://wm.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ul.jctech888.com.cn

fclose(f);
来源：http://qb.colortex.cn

[S12] C：写文件
来源：http://lb.asd995.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wp.hnjuh.cn

[S13] C：宏定义
来源：http://tt.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nx.hnjuh.cn

[S14] C：枚举
来源：http://xt.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://wn.hnjuh.cn

[S15] C：类型转换
来源：http://ew.bookmarksfly.cn

(double) a / b
来源：http://gp.huixiangedu.cn

[S16] C：位操作置位
来源：http://am.huixinmuqiang.cn

x |= (1 << 3);
来源：http://cm.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://qb.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cr.bookmarksfly.cn

[S18] C：命令行参数
来源：http://gc.yuexingan06.cn

int main(int argc, char **argv)
来源：http://mj.lnxyls.cn

[S19] C：快速排序
来源：http://zl.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vx.shxzskj.cn

[S20] C：二分查找
来源：http://wq.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gv.huanxung.cn

[S21] C：字符类别判断
来源：http://sl.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fu.lnxyls.cn

[S22] C：字符串转数字
来源：http://lq.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xi.colortex.cn

[S23] C：随机数
来源：http://cu.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pj.wgjwhj.cn

[S24] C：获取本地时间
来源：http://yl.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wu.lnxyls.cn

[S25] C：内存拷贝
来源：http://bo.shtwfgs.cn

memcpy(dst, src, n);
来源：http://bn.hahajie.cn

[S26] C：内存清零
来源：http://fg.huixiangedu.cn


<!-- 参考信息 -->