代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ht.colortex.cn

[Q52] 删除指定行
来源：http://ct.muxihuayi.cn

DELETE FROM users WHERE id = 10;
来源：http://uc.huanxung.cn

[Q53] 按条件删除
来源：http://sd.gzmigu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mn.nicolike.cn

[Q54] 清空表
来源：http://bo.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://bq.bookmarksfly.cn

[Q55] 排名（并列占位）
来源：http://gm.nicolike.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hj.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://wh.shtwfgs.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qn.wgjwhj.cn

[Q57] 行号
来源：http://pi.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://co.nicolike.cn

[Q58] 累计求和
来源：http://yg.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wk.panjiajie.cn

[Q59] 分组内累计
来源：http://jl.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qz.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://le.shxzskj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wg.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://of.szsharing.cn

[Q61] 移动平均
来源：http://jl.lnxyls.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ii.nicolike.cn

[Q62] 分组占比
来源：http://qx.muxihuayi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bf.lnxyls.cn

[Q63] 开启事务
来源：http://dl.huanxung.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jn.lnxyls.cn

[Q64] 提交事务
来源：http://ok.muxihuayi.cn

COMMIT;
来源：http://jj.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://fn.hnjuh.cn

ROLLBACK;
来源：http://hu.hahajie.cn

[Q66] 行锁查询
来源：http://jr.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hp.hahajie.cn

[Q67] 设置隔离级别
来源：http://ii.szsharing.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pe.asd995.cn

[Q68] 保存点
来源：http://fp.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://br.yuexingan06.cn

ROLLBACK TO sp1;
来源：http://lz.haigaiapp.cn

[Q69] 查看执行计划
来源：http://jq.bookmarksfly.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kk.szsharing.cn

[Q70] 更新统计信息
来源：http://eu.colortex.cn

ANALYZE TABLE users;
来源：http://nf.gzmigu.cn

[Q71] 查看建表语句
来源：http://io.jianghongdianzi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lt.huanxung.cn

[Q72] 查看索引
来源：http://lw.asd995.cn

SHOW INDEX FROM users;
来源：http://ji.nszjky.cn

[Q73] 查看表状态
来源：http://bu.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cm.521024.cn

[Q74] 强制使用索引
来源：http://ym.huixinmuqiang.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nd.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://mi.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ff.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yo.colortex.cn

[Q76] 按天统计
来源：http://db.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hp.hnjuh.cn

[Q77] 时间加减
来源：http://tz.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tt.szxytkj.cn

[Q78] 当前时间
来源：http://ws.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ws.szsharing.cn

[Q79] 字符串拼接
来源：http://kd.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hj.muxihuayi.cn

[Q80] 字符串截取
来源：http://ez.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yr.szxytkj.cn

[Q81] 字符串替换
来源：http://gm.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hp.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://xv.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sa.hahajie.cn

[Q83] 大小写转换
来源：http://qu.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sc.szsharing.cn

[Q84] 去除首尾空格
来源：http://ph.nicolike.cn

SELECT TRIM(name) FROM users;
来源：http://pm.haigaiapp.cn

[Q85] 数值取整
来源：http://gi.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vv.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://wv.nicolike.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lj.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://pa.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xj.szsharing.cn

[Q88] 行转列（条件聚合）
来源：http://tw.huanxung.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wj.wgjwhj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ng.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://qg.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nx.bookmarksfly.cn

[Q90] 生成序号列
来源：http://df.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rj.shxzskj.cn

================================================================================
来源：http://qi.lnxyls.cn

R. Bash 专题
来源：http://kx.jianghongdianzi.cn

================================================================================
来源：http://hy.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://rs.panjiajie.cn

#!/usr/bin/env bash
来源：http://em.bjjhwx.cn

set -euo pipefail
来源：http://ek.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://lm.hnjuh.cn

name="Tom"; echo "$name"
来源：http://yr.jctech888.com.cn

[R03] 只读变量
来源：http://di.szsharing.cn

readonly PI=3.14
来源：http://xp.hnjuh.cn

[R04] 位置参数
来源：http://ic.colortex.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gi.jianghongdianzi.cn

[R05] 参数默认值
来源：http://ms.szxytkj.cn

name="${1:-default}"
来源：http://ya.nszjky.cn

[R06] 判断命令是否存在
来源：http://xm.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pn.bookmarksfly.cn

[R07] if 判断文件
来源：http://aw.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bg.shxzukj.cn

[R08] 数值比较
来源：http://gb.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wj.szsharing.cn

[R09] 字符串比较
来源：http://hv.shtwfgs.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aj.lnxyls.cn

[R10] 正则匹配
来源：http://pk.colortex.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vm.yuexingan06.cn

[R11] case 多分支
来源：http://ru.9csxet.cn

case "$1" in
来源：http://ab.muxihuayi.cn

start) echo "启动" ;;
来源：http://jy.szxytkj.cn

stop)  echo "停止" ;;
来源：http://bs.9csxet.cn

*)     echo "未知命令" ;;
来源：http://mn.yuexingan06.cn

esac
来源：http://st.szsharing.cn

[R12] for 遍历文件
来源：http://ga.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://za.shxzskj.cn

[R13] for 计数循环
来源：http://zi.newstarts.cn

for i in {1..10}; do echo "$i"; done
来源：http://nw.bjjhwx.cn

[R14] C 风格 for
来源：http://it.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nw.panjiajie.cn

[R15] while 逐行读文件
来源：http://kk.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yz.521024.cn

[R16] until 等待条件
来源：http://ro.yuexingan06.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bu.huixinmuqiang.cn

[R17] 数组定义与取值
来源：http://sf.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pa.lnxyls.cn

[R18] 遍历数组
来源：http://vj.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tk.asd995.cn

[R19] 数组长度
来源：http://xp.newstarts.cn

echo "${#arr[@]}"
来源：http://mm.hahajie.cn

[R20] 关联数组（字典）
来源：http://wv.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rw.shxzskj.cn

[R21] 字符串长度
来源：http://th.nicolike.cn

echo "${#s}"
来源：http://zn.jianghongdianzi.cn

[R22] 截取子串
来源：http://wg.nszjky.cn

echo "${s:0:5}"
来源：http://do.yuntaijiaju.cn

[R23] 字符串替换
来源：http://nb.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vy.yuexingan06.cn

[R24] 大小写转换
来源：http://qm.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pq.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://lj.colortex.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ck.lnxyls.cn

[R26] 命令替换
来源：http://uj.chemitech.net.cn

now=$(date +%F); echo "$now"
来源：http://cf.chemitech.net.cn

[R27] 算术展开
来源：http://nx.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://je.asd995.cn

[R28] 浮点运算
来源：http://vr.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://xx.wgjwhj.cn

[R29] 定义函数
来源：http://zs.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yh.521024.cn

[R30] 函数返回状态码
来源：http://cz.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://kv.jctech888.com.cn

[R31] 局部变量
来源：http://pn.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://ag.shtwfgs.cn

[R32] 参数个数校验
来源：http://yq.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gc.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://he.asd995.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xu.huixiangedu.cn

[R34] 退出时清理
来源：http://vh.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ls.asd995.cn

[R35] 后台执行并等待
来源：http://kg.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ay.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://eg.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sk.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://lf.asd995.cn

files=$(ls -1)
来源：http://pl.shtwfgs.cn

[R38] 管道串联
来源：http://zl.lnxyls.cn

cat a.txt | grep -i error | wc -l
来源：http://rr.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://yh.panjiajie.cn

cmd > out.log 2>&1
来源：http://bh.haigaiapp.cn

[R40] 追加写日志
来源：http://kx.bjjhwx.cn

echo "log" >> out.log
来源：http://ds.muxihuayi.cn

[R41] 丢弃输出
来源：http://zn.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://yb.colortex.cn

[R42] 输入重定向
来源：http://bn.szsharing.cn

wc -l < a.txt
来源：http://dr.panjiajie.cn

[R43] 按名字查找文件
来源：http://wo.shtwfgs.cn

find . -name "*.log" -type f
来源：http://ma.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://jv.bjjhwx.cn

find . -mtime -7 -type f
来源：http://ht.jctech888.com.cn

[R45] 批量删除
来源：http://bc.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://ol.hahajie.cn

[R46] 递归替换文件内容
来源：http://nx.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ww.huanxung.cn

[R47] sed 单行替换
来源：http://yd.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ej.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://kh.521024.cn

awk '{print $1, $3}' a.txt
来源：http://bi.huixiangedu.cn

[R49] awk 带条件
来源：http://pm.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lw.shtwfgs.cn

[R50] awk 求和
来源：http://iy.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pb.chemitech.net.cn

[R51] 排序去重取前几
来源：http://km.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rs.asd995.cn

[R52] 统计行数
来源：http://xb.yuexingan06.cn

wc -l a.txt
来源：http://zp.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://hz.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gy.huixiangedu.cn

[R54] 比较两个文件
来源：http://oo.huanxung.cn

diff a.txt b.txt
来源：http://ux.szsharing.cn

[R55] 压缩与解压
来源：http://cn.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cs.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://px.gzmigu.cn

scp file user@host:/path/
来源：http://ye.bookmarksfly.cn

[R57] 远程执行命令
来源：http://hb.jctech888.com.cn

ssh user@host 'uptime'
来源：http://la.yuntaijiaju.cn

[R58] 下载文件
来源：http://qh.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bh.hahajie.cn

[R59] 发 POST JSON
来源：http://bf.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jx.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://pb.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fs.bookmarksfly.cn

[R61] 磁盘占用
来源：http://uk.colortex.cn

df -h;  du -sh *
来源：http://sn.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://aj.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://lg.hnjuh.cn

[R63] 内存与进程
来源：http://jj.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://na.panjiajie.cn

[R64] 结束进程
来源：http://ru.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://ry.newstarts.cn

[R65] 查看端口占用
来源：http://nu.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zq.jctech888.com.cn

[R66] 定时任务
来源：http://hk.shxzukj.cn

crontab -e;  crontab -l
来源：http://gx.newstarts.cn

[R67] 生成随机十六进制串
来源：http://qn.shxzskj.cn

openssl rand -hex 16
来源：http://yk.asd995.cn

[R68] 计算文件校验值
来源：http://he.521024.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xy.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://ae.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://ye.lnxyls.cn

[R70] 时间戳与互转
来源：http://tt.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://yy.bookmarksfly.cn

[R71] 日期格式化
来源：http://yg.newstarts.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bm.jctech888.com.cn

[R72] 等待端口就绪
来源：http://bl.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dt.jctech888.com.cn

[R73] 分割大日志
来源：http://qa.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://hl.shxzskj.cn

[R74] 批量重命名
来源：http://pn.haigaiapp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yc.wgjwhj.cn

[R75] 导出环境变量
来源：http://fc.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://sr.jctech888.com.cn

[R76] 使用临时文件
来源：http://kr.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zp.hnjuh.cn

[R77] 读取用户输入
来源：http://un.asd995.cn

read -rp "请输入: " ans
来源：http://yh.nszjky.cn

[R78] 交互式菜单
来源：http://xz.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wb.yuexingan06.cn

[R79] 解析命令行选项
来源：http://px.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://he.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://aw.yuntaijiaju.cn

time ./run.sh
来源：http://xu.asd995.cn

================================================================================
来源：http://kx.huanxung.cn

S. C / C++ 专题
来源：http://id.szxytkj.cn

================================================================================
来源：http://wz.szxytkj.cn

[S01] C：Hello World
来源：http://te.yuexingan06.cn

#include <stdio.h>
来源：http://gi.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cb.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://wv.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://if.shxzukj.cn

[S03] C：读入整数
来源：http://eu.asd995.cn

int x; scanf("%d", &x);
来源：http://yj.hahajie.cn

[S04] C：字符串复制
来源：http://pf.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ps.wgjwhj.cn

[S05] C：字符串长度
来源：http://ew.huixinmuqiang.cn

strlen(s)
来源：http://gv.panjiajie.cn

[S06] C：字符串比较
来源：http://ip.haigaiapp.cn

strcmp(a, b) == 0
来源：http://ed.newstarts.cn

[S07] C：数组遍历求和
来源：http://rm.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xu.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://wc.chemitech.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jg.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://kd.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://go.szxytkj.cn

[S10] C：指针与解引用
来源：http://jg.hahajie.cn

int *p = &a;  *p = 5;
来源：http://lt.9csxet.cn

[S11] C：逐行读文件
来源：http://bv.yuexingan06.cn

FILE *f = fopen("a.txt", "r");
来源：http://de.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dx.haigaiapp.cn

fclose(f);
来源：http://ab.gzmigu.cn

[S12] C：写文件
来源：http://jk.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wo.shtwfgs.cn

[S13] C：宏定义
来源：http://kr.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bg.huixinmuqiang.cn

[S14] C：枚举
来源：http://dk.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://dl.9csxet.cn

[S15] C：类型转换
来源：http://fn.lnxyls.cn

(double) a / b
来源：http://hd.huanxung.cn

[S16] C：位操作置位
来源：http://km.wgjwhj.cn

x |= (1 << 3);
来源：http://ef.szsharing.cn

[S17] C：安全拼接字符串
来源：http://gb.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ln.bjjhwx.cn

[S18] C：命令行参数
来源：http://jd.bjjhwx.cn

int main(int argc, char **argv)
来源：http://kk.haigaiapp.cn

[S19] C：快速排序
来源：http://qc.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ba.gzmigu.cn

[S20] C：二分查找
来源：http://ad.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sr.wgjwhj.cn

[S21] C：字符类别判断
来源：http://ht.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iz.szsharing.cn

[S22] C：字符串转数字
来源：http://wx.gzmigu.cn


<!-- 参考信息 -->