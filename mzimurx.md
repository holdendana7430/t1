代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gj.colortex.cn

[Q52] 删除指定行
来源：http://ik.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://vv.lnxyls.cn

[Q53] 按条件删除
来源：http://pc.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tb.jianghongdianzi.cn

[Q54] 清空表
来源：http://hx.nicolike.cn

TRUNCATE TABLE logs;
来源：http://ww.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://yj.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yp.szxytkj.cn

[Q56] 密集排名（并列不占位）
来源：http://yh.wgjwhj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dm.chemitech.net.cn

[Q57] 行号
来源：http://he.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cd.shtwfgs.cn

[Q58] 累计求和
来源：http://be.muxihuayi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ub.jianghongdianzi.cn

[Q59] 分组内累计
来源：http://ca.jianghongdianzi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qk.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://xi.chemitech.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dl.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ji.gzmigu.cn

[Q61] 移动平均
来源：http://gi.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hp.hnjuh.cn

[Q62] 分组占比
来源：http://mr.newstarts.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mh.panjiajie.cn

[Q63] 开启事务
来源：http://ui.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wq.chemitech.net.cn

[Q64] 提交事务
来源：http://db.huanxung.cn

COMMIT;
来源：http://zl.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://th.yuexingan06.cn

ROLLBACK;
来源：http://pq.nszjky.cn

[Q66] 行锁查询
来源：http://dd.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bt.jctech888.com.cn

[Q67] 设置隔离级别
来源：http://aq.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gt.panjiajie.cn

[Q68] 保存点
来源：http://ba.newstarts.cn

SAVEPOINT sp1;
来源：http://ne.9csxet.cn

ROLLBACK TO sp1;
来源：http://mn.szsharing.cn

[Q69] 查看执行计划
来源：http://dg.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yz.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://gj.huanxung.cn

ANALYZE TABLE users;
来源：http://tm.yuexingan06.cn

[Q71] 查看建表语句
来源：http://yr.gzmigu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jx.wgjwhj.cn

[Q72] 查看索引
来源：http://pv.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://mr.szxytkj.cn

[Q73] 查看表状态
来源：http://rc.huixiangedu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hq.shxzukj.cn

[Q74] 强制使用索引
来源：http://la.521024.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cg.szsharing.cn

[Q75] 日期格式化
来源：http://qd.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rw.hnjuh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zu.yuntaijiaju.cn

[Q76] 按天统计
来源：http://iw.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vn.huanxung.cn

[Q77] 时间加减
来源：http://rb.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jt.9csxet.cn

[Q78] 当前时间
来源：http://ve.szxytkj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ye.jianghongdianzi.cn

[Q79] 字符串拼接
来源：http://ra.bookmarksfly.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://me.lnxyls.cn

[Q80] 字符串截取
来源：http://it.asd995.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ff.shxzukj.cn

[Q81] 字符串替换
来源：http://be.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mm.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://ny.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ur.shxzskj.cn

[Q83] 大小写转换
来源：http://lt.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hy.9csxet.cn

[Q84] 去除首尾空格
来源：http://mu.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://bm.lnxyls.cn

[Q85] 数值取整
来源：http://av.szxytkj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kw.szxytkj.cn

[Q86] 读取 JSON 字段
来源：http://rj.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jz.huixinmuqiang.cn

[Q87] JSON 字段做条件
来源：http://wf.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tr.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://gy.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pi.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ya.colortex.cn

[Q89] 判断表是否存在
来源：http://pf.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tx.szsharing.cn

[Q90] 生成序号列
来源：http://rt.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ac.muxihuayi.cn

================================================================================
来源：http://ub.hnjuh.cn

R. Bash 专题
来源：http://ev.muxihuayi.cn

================================================================================
来源：http://ul.gzmigu.cn

[R01] shebang 与严格模式
来源：http://nr.yuexingan06.cn

#!/usr/bin/env bash
来源：http://dm.chemitech.net.cn

set -euo pipefail
来源：http://bk.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://pr.gzmigu.cn

name="Tom"; echo "$name"
来源：http://zh.gzmigu.cn

[R03] 只读变量
来源：http://xu.huixiangedu.cn

readonly PI=3.14
来源：http://ht.chemitech.net.cn

[R04] 位置参数
来源：http://om.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tw.hahajie.cn

[R05] 参数默认值
来源：http://rr.szsharing.cn

name="${1:-default}"
来源：http://nj.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://tx.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://aq.yuntaijiaju.cn

[R07] if 判断文件
来源：http://bd.chemitech.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fq.9csxet.cn

[R08] 数值比较
来源：http://sn.hahajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wl.jctech888.com.cn

[R09] 字符串比较
来源：http://pd.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jm.muxihuayi.cn

[R10] 正则匹配
来源：http://hx.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hd.newstarts.cn

[R11] case 多分支
来源：http://pl.asd995.cn

case "$1" in
来源：http://ak.huixinmuqiang.cn

start) echo "启动" ;;
来源：http://jw.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://in.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://su.szxytkj.cn

esac
来源：http://nj.muxihuayi.cn

[R12] for 遍历文件
来源：http://va.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://ju.bjjhwx.cn

[R13] for 计数循环
来源：http://lj.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://pk.newstarts.cn

[R14] C 风格 for
来源：http://kp.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://go.jctech888.com.cn

[R15] while 逐行读文件
来源：http://bw.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tt.yuexingan06.cn

[R16] until 等待条件
来源：http://bw.haigaiapp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ba.9csxet.cn

[R17] 数组定义与取值
来源：http://sv.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://iv.szxytkj.cn

[R18] 遍历数组
来源：http://mt.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vj.shxzukj.cn

[R19] 数组长度
来源：http://bw.hahajie.cn

echo "${#arr[@]}"
来源：http://vh.szxytkj.cn

[R20] 关联数组（字典）
来源：http://la.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wu.huixinmuqiang.cn

[R21] 字符串长度
来源：http://ky.huixiangedu.cn

echo "${#s}"
来源：http://jh.jctech888.com.cn

[R22] 截取子串
来源：http://pr.panjiajie.cn

echo "${s:0:5}"
来源：http://tg.szsharing.cn

[R23] 字符串替换
来源：http://dd.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ql.wgjwhj.cn

[R24] 大小写转换
来源：http://ul.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://da.521024.cn

[R25] 去后缀 / 去前缀
来源：http://rt.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lu.huanxung.cn

[R26] 命令替换
来源：http://gz.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://cs.gzmigu.cn

[R27] 算术展开
来源：http://om.hahajie.cn

echo $((1 + 2 * 3))
来源：http://cn.nicolike.cn

[R28] 浮点运算
来源：http://ms.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://np.shxzskj.cn

[R29] 定义函数
来源：http://ah.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lh.lnxyls.cn

[R30] 函数返回状态码
来源：http://sy.bookmarksfly.cn

f() { return 0; }; f || echo "失败了"
来源：http://jz.nszjky.cn

[R31] 局部变量
来源：http://ao.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://dv.gzmigu.cn

[R32] 参数个数校验
来源：http://pk.shtwfgs.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bg.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://ma.gzmigu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yg.wgjwhj.cn

[R34] 退出时清理
来源：http://og.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://li.shxzukj.cn

[R35] 后台执行并等待
来源：http://kr.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sx.colortex.cn

[R36] 并发执行多个任务
来源：http://so.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uq.huixinmuqiang.cn

[R37] 把输出赋给变量
来源：http://uk.szxytkj.cn

files=$(ls -1)
来源：http://to.521024.cn

[R38] 管道串联
来源：http://li.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://mh.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://jk.panjiajie.cn

cmd > out.log 2>&1
来源：http://wp.9csxet.cn

[R40] 追加写日志
来源：http://zx.9csxet.cn

echo "log" >> out.log
来源：http://tc.nicolike.cn

[R41] 丢弃输出
来源：http://dd.nicolike.cn

cmd >/dev/null 2>&1
来源：http://ww.yuntaijiaju.cn

[R42] 输入重定向
来源：http://jl.huixinmuqiang.cn

wc -l < a.txt
来源：http://uh.chemitech.net.cn

[R43] 按名字查找文件
来源：http://bs.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://pn.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://li.wgjwhj.cn

find . -mtime -7 -type f
来源：http://pt.szsharing.cn

[R45] 批量删除
来源：http://zr.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://ok.nicolike.cn

[R46] 递归替换文件内容
来源：http://tj.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wb.bookmarksfly.cn

[R47] sed 单行替换
来源：http://yv.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dd.muxihuayi.cn

[R48] awk 取指定列
来源：http://yj.521024.cn

awk '{print $1, $3}' a.txt
来源：http://kz.panjiajie.cn

[R49] awk 带条件
来源：http://bv.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vk.szsharing.cn

[R50] awk 求和
来源：http://xc.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cb.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://tq.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mb.gzmigu.cn

[R52] 统计行数
来源：http://ks.muxihuayi.cn

wc -l a.txt
来源：http://yc.huanxung.cn

[R53] 查看文件头与实时尾
来源：http://ym.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dv.szsharing.cn

[R54] 比较两个文件
来源：http://fa.jianghongdianzi.cn

diff a.txt b.txt
来源：http://rr.521024.cn

[R55] 压缩与解压
来源：http://xm.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vw.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://di.wgjwhj.cn

scp file user@host:/path/
来源：http://vt.muxihuayi.cn

[R57] 远程执行命令
来源：http://ol.hahajie.cn

ssh user@host 'uptime'
来源：http://vc.haigaiapp.cn

[R58] 下载文件
来源：http://vx.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qy.newstarts.cn

[R59] 发 POST JSON
来源：http://wt.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vd.huixiangedu.cn

[R60] 只看 HTTP 状态码
来源：http://ci.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xa.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://yk.hahajie.cn

df -h;  du -sh *
来源：http://gv.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://ly.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://fj.hnjuh.cn

[R63] 内存与进程
来源：http://xp.asd995.cn

free -h;  ps aux | grep nginx
来源：http://rq.newstarts.cn

[R64] 结束进程
来源：http://gd.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://mo.huixiangedu.cn

[R65] 查看端口占用
来源：http://zo.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xc.nicolike.cn

[R66] 定时任务
来源：http://vp.lnxyls.cn

crontab -e;  crontab -l
来源：http://pn.colortex.cn

[R67] 生成随机十六进制串
来源：http://zj.bjjhwx.cn

openssl rand -hex 16
来源：http://up.szsharing.cn

[R68] 计算文件校验值
来源：http://bk.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kg.haigaiapp.cn

[R69] 生成随机密码
来源：http://ts.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://bl.huixiangedu.cn

[R70] 时间戳与互转
来源：http://dy.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://st.colortex.cn

[R71] 日期格式化
来源：http://bn.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cx.lnxyls.cn

[R72] 等待端口就绪
来源：http://uc.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qj.hnjuh.cn

[R73] 分割大日志
来源：http://yz.szsharing.cn

split -l 1000 big.log part_
来源：http://ny.hnjuh.cn

[R74] 批量重命名
来源：http://ru.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yv.shtwfgs.cn

[R75] 导出环境变量
来源：http://uq.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://ld.gzmigu.cn

[R76] 使用临时文件
来源：http://nn.hahajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vo.shxzukj.cn

[R77] 读取用户输入
来源：http://id.asd995.cn

read -rp "请输入: " ans
来源：http://ok.yuexingan06.cn

[R78] 交互式菜单
来源：http://es.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yz.chemitech.net.cn

[R79] 解析命令行选项
来源：http://hv.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yt.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://dc.9csxet.cn

time ./run.sh
来源：http://tu.newstarts.cn

================================================================================
来源：http://cf.shtwfgs.cn

S. C / C++ 专题
来源：http://gr.haigaiapp.cn

================================================================================
来源：http://io.yuexingan06.cn

[S01] C：Hello World
来源：http://ju.haigaiapp.cn

#include <stdio.h>
来源：http://qf.jianghongdianzi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jk.huanxung.cn

[S02] C：变量与格式化输出
来源：http://uo.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://qx.bjjhwx.cn

[S03] C：读入整数
来源：http://dr.9csxet.cn

int x; scanf("%d", &x);
来源：http://he.asd995.cn

[S04] C：字符串复制
来源：http://ff.panjiajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qi.nicolike.cn

[S05] C：字符串长度
来源：http://et.9csxet.cn

strlen(s)
来源：http://ig.bjjhwx.cn

[S06] C：字符串比较
来源：http://jj.gzmigu.cn

strcmp(a, b) == 0
来源：http://eq.newstarts.cn

[S07] C：数组遍历求和
来源：http://yu.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ua.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://fr.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ww.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://pj.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uh.shtwfgs.cn

[S10] C：指针与解引用
来源：http://yh.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://zi.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://cu.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://xn.hnjuh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ud.asd995.cn

fclose(f);
来源：http://ma.yuntaijiaju.cn

[S12] C：写文件
来源：http://mk.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fc.shxzukj.cn

[S13] C：宏定义
来源：http://vu.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sm.chemitech.net.cn

[S14] C：枚举
来源：http://zj.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://go.asd995.cn

[S15] C：类型转换
来源：http://rt.szxytkj.cn

(double) a / b
来源：http://gl.9csxet.cn

[S16] C：位操作置位
来源：http://wx.jianghongdianzi.cn

x |= (1 << 3);
来源：http://bl.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://bf.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mb.newstarts.cn

[S18] C：命令行参数
来源：http://kj.lnxyls.cn

int main(int argc, char **argv)
来源：http://fn.huixinmuqiang.cn

[S19] C：快速排序
来源：http://vv.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://va.hahajie.cn

[S20] C：二分查找
来源：http://kr.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sf.jctech888.com.cn

[S21] C：字符类别判断
来源：http://tf.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tk.9csxet.cn

[S22] C：字符串转数字
来源：http://fd.asd995.cn


<!-- 参考信息 -->