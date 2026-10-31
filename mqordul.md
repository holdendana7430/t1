代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ks.9csxet.cn

[Q56] 密集排名（并列不占位）
来源：http://xw.szxytkj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xf.hnjuh.cn

[Q57] 行号
来源：http://mo.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qr.nicolike.cn

[Q58] 累计求和
来源：http://hn.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xx.shtwfgs.cn

[Q59] 分组内累计
来源：http://rz.huanxung.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ai.chemitech.net.cn

[Q60] 取上一行 / 下一行
来源：http://xs.szxytkj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ez.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qx.jctech888.com.cn

[Q61] 移动平均
来源：http://hp.szsharing.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rh.nszjky.cn

[Q62] 分组占比
来源：http://nm.nicolike.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hq.szsharing.cn

[Q63] 开启事务
来源：http://cc.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lo.shxzskj.cn

[Q64] 提交事务
来源：http://wo.shxzukj.cn

COMMIT;
来源：http://rq.panjiajie.cn

[Q65] 回滚事务
来源：http://xi.nszjky.cn

ROLLBACK;
来源：http://vm.jctech888.com.cn

[Q66] 行锁查询
来源：http://mq.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zz.nicolike.cn

[Q67] 设置隔离级别
来源：http://ys.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lp.bookmarksfly.cn

[Q68] 保存点
来源：http://if.panjiajie.cn

SAVEPOINT sp1;
来源：http://cd.huixiangedu.cn

ROLLBACK TO sp1;
来源：http://tx.lnxyls.cn

[Q69] 查看执行计划
来源：http://zu.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ef.shxzskj.cn

[Q70] 更新统计信息
来源：http://gx.huanxung.cn

ANALYZE TABLE users;
来源：http://ih.wgjwhj.cn

[Q71] 查看建表语句
来源：http://zs.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ll.bjjhwx.cn

[Q72] 查看索引
来源：http://lp.gzmigu.cn

SHOW INDEX FROM users;
来源：http://kx.lnxyls.cn

[Q73] 查看表状态
来源：http://eo.521024.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ba.bookmarksfly.cn

[Q74] 强制使用索引
来源：http://mg.521024.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ek.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://tc.haigaiapp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gc.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rf.gzmigu.cn

[Q76] 按天统计
来源：http://gn.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rm.bjjhwx.cn

[Q77] 时间加减
来源：http://am.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nc.hahajie.cn

[Q78] 当前时间
来源：http://ab.yuexingan06.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nm.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://xz.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gw.wgjwhj.cn

[Q80] 字符串截取
来源：http://mf.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://az.szxytkj.cn

[Q81] 字符串替换
来源：http://bl.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ga.haigaiapp.cn

[Q82] 字符长度与字节长度
来源：http://rx.jctech888.com.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hi.newstarts.cn

[Q83] 大小写转换
来源：http://xh.hahajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lk.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://oe.521024.cn

SELECT TRIM(name) FROM users;
来源：http://ms.bookmarksfly.cn

[Q85] 数值取整
来源：http://hb.panjiajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vf.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://bt.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vs.9csxet.cn

[Q87] JSON 字段做条件
来源：http://sj.huixinmuqiang.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fx.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://xt.asd995.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dx.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://od.lnxyls.cn

[Q89] 判断表是否存在
来源：http://nq.521024.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nv.haigaiapp.cn

[Q90] 生成序号列
来源：http://ah.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sc.gzmigu.cn

================================================================================
来源：http://jl.newstarts.cn

R. Bash 专题
来源：http://kg.muxihuayi.cn

================================================================================
来源：http://gq.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://ma.lnxyls.cn

#!/usr/bin/env bash
来源：http://fr.panjiajie.cn

set -euo pipefail
来源：http://dx.nszjky.cn

[R02] 变量赋值与使用
来源：http://ca.huanxung.cn

name="Tom"; echo "$name"
来源：http://hf.yuntaijiaju.cn

[R03] 只读变量
来源：http://wm.asd995.cn

readonly PI=3.14
来源：http://gf.hahajie.cn

[R04] 位置参数
来源：http://vm.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kd.huixinmuqiang.cn

[R05] 参数默认值
来源：http://fs.hnjuh.cn

name="${1:-default}"
来源：http://kd.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://rf.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tm.yuntaijiaju.cn

[R07] if 判断文件
来源：http://ai.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rv.jianghongdianzi.cn

[R08] 数值比较
来源：http://yn.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zo.9csxet.cn

[R09] 字符串比较
来源：http://ul.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xs.chemitech.net.cn

[R10] 正则匹配
来源：http://ef.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cv.muxihuayi.cn

[R11] case 多分支
来源：http://dv.521024.cn

case "$1" in
来源：http://fj.jctech888.com.cn

start) echo "启动" ;;
来源：http://pt.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://jz.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://gw.521024.cn

esac
来源：http://he.newstarts.cn

[R12] for 遍历文件
来源：http://sl.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://bi.yuexingan06.cn

[R13] for 计数循环
来源：http://il.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://yn.yuexingan06.cn

[R14] C 风格 for
来源：http://za.huanxung.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hk.hahajie.cn

[R15] while 逐行读文件
来源：http://qc.gzmigu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dz.521024.cn

[R16] until 等待条件
来源：http://vq.shxzskj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oo.huixiangedu.cn

[R17] 数组定义与取值
来源：http://vp.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ye.hahajie.cn

[R18] 遍历数组
来源：http://cj.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xe.newstarts.cn

[R19] 数组长度
来源：http://yd.shxzukj.cn

echo "${#arr[@]}"
来源：http://gs.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://qm.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gi.haigaiapp.cn

[R21] 字符串长度
来源：http://lw.wgjwhj.cn

echo "${#s}"
来源：http://ir.nszjky.cn

[R22] 截取子串
来源：http://kk.newstarts.cn

echo "${s:0:5}"
来源：http://jq.shxzskj.cn

[R23] 字符串替换
来源：http://qr.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uf.wgjwhj.cn

[R24] 大小写转换
来源：http://sd.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lz.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://eg.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nj.jianghongdianzi.cn

[R26] 命令替换
来源：http://yc.szxytkj.cn

now=$(date +%F); echo "$now"
来源：http://hj.bjjhwx.cn

[R27] 算术展开
来源：http://gc.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://sp.asd995.cn

[R28] 浮点运算
来源：http://rj.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://al.huixiangedu.cn

[R29] 定义函数
来源：http://zy.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xq.lnxyls.cn

[R30] 函数返回状态码
来源：http://le.muxihuayi.cn

f() { return 0; }; f || echo "失败了"
来源：http://kd.shtwfgs.cn

[R31] 局部变量
来源：http://ft.haigaiapp.cn

f() { local x=1; echo "$x"; }
来源：http://gw.hahajie.cn

[R32] 参数个数校验
来源：http://go.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ol.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://ud.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://og.szxytkj.cn

[R34] 退出时清理
来源：http://hu.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ma.asd995.cn

[R35] 后台执行并等待
来源：http://wz.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pl.9csxet.cn

[R36] 并发执行多个任务
来源：http://lp.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kx.9csxet.cn

[R37] 把输出赋给变量
来源：http://jm.hnjuh.cn

files=$(ls -1)
来源：http://nc.shtwfgs.cn

[R38] 管道串联
来源：http://pn.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://jj.lnxyls.cn

[R39] 重定向标准输出与错误
来源：http://zm.bjjhwx.cn

cmd > out.log 2>&1
来源：http://gs.lnxyls.cn

[R40] 追加写日志
来源：http://yd.haigaiapp.cn

echo "log" >> out.log
来源：http://qp.muxihuayi.cn

[R41] 丢弃输出
来源：http://qc.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://lm.jianghongdianzi.cn

[R42] 输入重定向
来源：http://pv.nszjky.cn

wc -l < a.txt
来源：http://ym.chemitech.net.cn

[R43] 按名字查找文件
来源：http://zk.shxzukj.cn

find . -name "*.log" -type f
来源：http://uo.newstarts.cn

[R44] 按修改时间查找
来源：http://zh.521024.cn

find . -mtime -7 -type f
来源：http://uh.bookmarksfly.cn

[R45] 批量删除
来源：http://wf.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://su.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://md.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lo.newstarts.cn

[R47] sed 单行替换
来源：http://ko.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kd.shtwfgs.cn

[R48] awk 取指定列
来源：http://iw.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://rh.lnxyls.cn

[R49] awk 带条件
来源：http://ld.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hl.chemitech.net.cn

[R50] awk 求和
来源：http://da.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nn.chemitech.net.cn

[R51] 排序去重取前几
来源：http://um.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yi.521024.cn

[R52] 统计行数
来源：http://dd.lnxyls.cn

wc -l a.txt
来源：http://xq.shxzskj.cn

[R53] 查看文件头与实时尾
来源：http://sm.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yo.muxihuayi.cn

[R54] 比较两个文件
来源：http://bf.wgjwhj.cn

diff a.txt b.txt
来源：http://el.asd995.cn

[R55] 压缩与解压
来源：http://qu.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uu.szsharing.cn

[R56] 远程拷贝
来源：http://yh.bookmarksfly.cn

scp file user@host:/path/
来源：http://pm.lnxyls.cn

[R57] 远程执行命令
来源：http://xc.gzmigu.cn

ssh user@host 'uptime'
来源：http://ox.yuntaijiaju.cn

[R58] 下载文件
来源：http://cn.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://po.szxytkj.cn

[R59] 发 POST JSON
来源：http://ew.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ry.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://dv.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wh.shtwfgs.cn

[R61] 磁盘占用
来源：http://lx.huanxung.cn

df -h;  du -sh *
来源：http://vt.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://oi.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://ph.huixiangedu.cn

[R63] 内存与进程
来源：http://gh.panjiajie.cn

free -h;  ps aux | grep nginx
来源：http://zi.jianghongdianzi.cn

[R64] 结束进程
来源：http://np.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://so.colortex.cn

[R65] 查看端口占用
来源：http://kp.huixinmuqiang.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uc.shxzukj.cn

[R66] 定时任务
来源：http://tf.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://yn.nicolike.cn

[R67] 生成随机十六进制串
来源：http://mp.jianghongdianzi.cn

openssl rand -hex 16
来源：http://cj.szsharing.cn

[R68] 计算文件校验值
来源：http://rq.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://je.huixiangedu.cn

[R69] 生成随机密码
来源：http://kc.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://mu.shxzskj.cn

[R70] 时间戳与互转
来源：http://jv.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://sz.wgjwhj.cn

[R71] 日期格式化
来源：http://pw.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mb.huixiangedu.cn

[R72] 等待端口就绪
来源：http://si.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gl.panjiajie.cn

[R73] 分割大日志
来源：http://kw.hahajie.cn

split -l 1000 big.log part_
来源：http://xg.yuexingan06.cn

[R74] 批量重命名
来源：http://xh.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jc.huixiangedu.cn

[R75] 导出环境变量
来源：http://lt.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://cc.jctech888.com.cn

[R76] 使用临时文件
来源：http://xj.asd995.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mo.szsharing.cn

[R77] 读取用户输入
来源：http://lt.asd995.cn

read -rp "请输入: " ans
来源：http://ea.huanxung.cn

[R78] 交互式菜单
来源：http://kr.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tn.huixiangedu.cn

[R79] 解析命令行选项
来源：http://ev.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cd.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://ic.hahajie.cn

time ./run.sh
来源：http://ta.9csxet.cn

================================================================================
来源：http://hz.9csxet.cn

S. C / C++ 专题
来源：http://fm.lnxyls.cn

================================================================================
来源：http://gs.huanxung.cn

[S01] C：Hello World
来源：http://vh.huixiangedu.cn

#include <stdio.h>
来源：http://ji.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ah.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://ac.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://fr.huanxung.cn

[S03] C：读入整数
来源：http://mi.colortex.cn

int x; scanf("%d", &x);
来源：http://kv.chemitech.net.cn

[S04] C：字符串复制
来源：http://cw.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://md.nicolike.cn

[S05] C：字符串长度
来源：http://tp.yuexingan06.cn

strlen(s)
来源：http://ws.521024.cn

[S06] C：字符串比较
来源：http://on.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://pg.colortex.cn

[S07] C：数组遍历求和
来源：http://dk.szxytkj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cc.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://jf.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eu.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://yp.hnjuh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hx.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://kn.9csxet.cn

int *p = &a;  *p = 5;
来源：http://ij.shtwfgs.cn

[S11] C：逐行读文件
来源：http://oq.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://rq.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pi.huixinmuqiang.cn

fclose(f);
来源：http://sz.szsharing.cn

[S12] C：写文件
来源：http://aj.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cp.muxihuayi.cn

[S13] C：宏定义
来源：http://vj.nicolike.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ep.lnxyls.cn

[S14] C：枚举
来源：http://zq.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://dc.asd995.cn

[S15] C：类型转换
来源：http://fw.yuexingan06.cn

(double) a / b
来源：http://xj.9csxet.cn

[S16] C：位操作置位
来源：http://jg.szsharing.cn

x |= (1 << 3);
来源：http://mq.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://lv.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kr.muxihuayi.cn

[S18] C：命令行参数
来源：http://cm.521024.cn

int main(int argc, char **argv)
来源：http://mh.521024.cn

[S19] C：快速排序
来源：http://qm.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ek.nicolike.cn

[S20] C：二分查找
来源：http://ng.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://np.haigaiapp.cn

[S21] C：字符类别判断
来源：http://rr.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qo.newstarts.cn

[S22] C：字符串转数字
来源：http://tz.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lo.szsharing.cn

[S23] C：随机数
来源：http://bi.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ts.bjjhwx.cn

[S24] C：获取本地时间
来源：http://ye.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yn.huanxung.cn

[S25] C：内存拷贝
来源：http://rq.huixiangedu.cn

memcpy(dst, src, n);
来源：http://tg.chemitech.net.cn

[S26] C：内存清零
来源：http://uf.9csxet.cn


<!-- 参考信息 -->