代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jj.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://zl.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://em.521024.cn

[Q57] 行号
来源：http://jc.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ts.chemitech.net.cn

[Q58] 累计求和
来源：http://fp.huanxung.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bm.hnjuh.cn

[Q59] 分组内累计
来源：http://at.jctech888.com.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fe.shxzukj.cn

[Q60] 取上一行 / 下一行
来源：http://kw.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lz.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vt.nicolike.cn

[Q61] 移动平均
来源：http://gl.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://if.yuexingan06.cn

[Q62] 分组占比
来源：http://tb.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xw.yuntaijiaju.cn

[Q63] 开启事务
来源：http://vr.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rz.bookmarksfly.cn

[Q64] 提交事务
来源：http://gv.jctech888.com.cn

COMMIT;
来源：http://ha.bookmarksfly.cn

[Q65] 回滚事务
来源：http://dm.panjiajie.cn

ROLLBACK;
来源：http://fj.bjjhwx.cn

[Q66] 行锁查询
来源：http://ue.asd995.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ht.lnxyls.cn

[Q67] 设置隔离级别
来源：http://vh.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://df.hnjuh.cn

[Q68] 保存点
来源：http://ra.chemitech.net.cn

SAVEPOINT sp1;
来源：http://mj.hahajie.cn

ROLLBACK TO sp1;
来源：http://rw.muxihuayi.cn

[Q69] 查看执行计划
来源：http://sz.yuntaijiaju.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mi.jctech888.com.cn

[Q70] 更新统计信息
来源：http://mb.bjjhwx.cn

ANALYZE TABLE users;
来源：http://gl.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://de.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zo.muxihuayi.cn

[Q72] 查看索引
来源：http://mz.hnjuh.cn

SHOW INDEX FROM users;
来源：http://pz.panjiajie.cn

[Q73] 查看表状态
来源：http://ob.lnxyls.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hv.hahajie.cn

[Q74] 强制使用索引
来源：http://ai.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ys.huixiangedu.cn

[Q75] 日期格式化
来源：http://ec.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pw.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ha.jctech888.com.cn

[Q76] 按天统计
来源：http://bv.muxihuayi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yf.bjjhwx.cn

[Q77] 时间加减
来源：http://ca.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://st.haigaiapp.cn

[Q78] 当前时间
来源：http://ag.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ld.muxihuayi.cn

[Q79] 字符串拼接
来源：http://uw.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nb.szxytkj.cn

[Q80] 字符串截取
来源：http://hz.shxzukj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qe.chemitech.net.cn

[Q81] 字符串替换
来源：http://bl.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yk.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://xs.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gy.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://ql.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lq.bjjhwx.cn

[Q84] 去除首尾空格
来源：http://ui.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://gl.shxzskj.cn

[Q85] 数值取整
来源：http://nw.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vf.9csxet.cn

[Q86] 读取 JSON 字段
来源：http://ne.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://al.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://oi.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kk.bookmarksfly.cn

[Q88] 行转列（条件聚合）
来源：http://tq.szsharing.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qb.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sn.shxzukj.cn

[Q89] 判断表是否存在
来源：http://fa.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yb.colortex.cn

[Q90] 生成序号列
来源：http://uk.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://co.hnjuh.cn

================================================================================
来源：http://ls.jctech888.com.cn

R. Bash 专题
来源：http://gt.yuntaijiaju.cn

================================================================================
来源：http://qi.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://jj.nszjky.cn

#!/usr/bin/env bash
来源：http://rh.szxytkj.cn

set -euo pipefail
来源：http://nm.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://jc.szsharing.cn

name="Tom"; echo "$name"
来源：http://ms.jianghongdianzi.cn

[R03] 只读变量
来源：http://tv.shtwfgs.cn

readonly PI=3.14
来源：http://qa.lnxyls.cn

[R04] 位置参数
来源：http://uz.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sq.wgjwhj.cn

[R05] 参数默认值
来源：http://bj.jctech888.com.cn

name="${1:-default}"
来源：http://hg.panjiajie.cn

[R06] 判断命令是否存在
来源：http://cq.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vu.yuntaijiaju.cn

[R07] if 判断文件
来源：http://uh.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jv.haigaiapp.cn

[R08] 数值比较
来源：http://hl.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ki.hnjuh.cn

[R09] 字符串比较
来源：http://zn.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wl.shxzskj.cn

[R10] 正则匹配
来源：http://jo.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gz.nszjky.cn

[R11] case 多分支
来源：http://hq.bookmarksfly.cn

case "$1" in
来源：http://gh.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://aq.haigaiapp.cn

stop)  echo "停止" ;;
来源：http://xc.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://db.yuexingan06.cn

esac
来源：http://wk.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://ns.szsharing.cn

for f in *.txt; do echo "$f"; done
来源：http://jb.nszjky.cn

[R13] for 计数循环
来源：http://sb.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://tp.bookmarksfly.cn

[R14] C 风格 for
来源：http://eh.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zy.wgjwhj.cn

[R15] while 逐行读文件
来源：http://pm.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://me.jianghongdianzi.cn

[R16] until 等待条件
来源：http://fg.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hd.muxihuayi.cn

[R17] 数组定义与取值
来源：http://nm.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ct.huanxung.cn

[R18] 遍历数组
来源：http://tw.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gi.yuexingan06.cn

[R19] 数组长度
来源：http://vt.nicolike.cn

echo "${#arr[@]}"
来源：http://ft.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://jk.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hw.nicolike.cn

[R21] 字符串长度
来源：http://xy.asd995.cn

echo "${#s}"
来源：http://rk.chemitech.net.cn

[R22] 截取子串
来源：http://fi.hnjuh.cn

echo "${s:0:5}"
来源：http://pu.nszjky.cn

[R23] 字符串替换
来源：http://nn.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://il.huanxung.cn

[R24] 大小写转换
来源：http://uu.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wt.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://ub.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ab.9csxet.cn

[R26] 命令替换
来源：http://rj.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://vr.bjjhwx.cn

[R27] 算术展开
来源：http://so.wgjwhj.cn

echo $((1 + 2 * 3))
来源：http://bv.hnjuh.cn

[R28] 浮点运算
来源：http://kx.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://fq.muxihuayi.cn

[R29] 定义函数
来源：http://ui.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eu.colortex.cn

[R30] 函数返回状态码
来源：http://ig.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://gi.szxytkj.cn

[R31] 局部变量
来源：http://al.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://mq.bjjhwx.cn

[R32] 参数个数校验
来源：http://sg.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ox.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://dx.asd995.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nq.shtwfgs.cn

[R34] 退出时清理
来源：http://bu.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rk.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://sj.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mm.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://xx.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uj.nszjky.cn

[R37] 把输出赋给变量
来源：http://db.bjjhwx.cn

files=$(ls -1)
来源：http://jf.shtwfgs.cn

[R38] 管道串联
来源：http://vy.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://mb.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://ph.shxzukj.cn

cmd > out.log 2>&1
来源：http://qv.wgjwhj.cn

[R40] 追加写日志
来源：http://wn.hnjuh.cn

echo "log" >> out.log
来源：http://gt.521024.cn

[R41] 丢弃输出
来源：http://eh.wgjwhj.cn

cmd >/dev/null 2>&1
来源：http://rd.chemitech.net.cn

[R42] 输入重定向
来源：http://nb.yuntaijiaju.cn

wc -l < a.txt
来源：http://ff.hnjuh.cn

[R43] 按名字查找文件
来源：http://vm.nicolike.cn

find . -name "*.log" -type f
来源：http://oj.9csxet.cn

[R44] 按修改时间查找
来源：http://fr.huixiangedu.cn

find . -mtime -7 -type f
来源：http://ck.colortex.cn

[R45] 批量删除
来源：http://bj.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://kh.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://lh.nszjky.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xu.hahajie.cn

[R47] sed 单行替换
来源：http://bh.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bm.colortex.cn

[R48] awk 取指定列
来源：http://ks.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://sg.haigaiapp.cn

[R49] awk 带条件
来源：http://bg.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ob.521024.cn

[R50] awk 求和
来源：http://cu.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ib.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://sw.yuexingan06.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rs.huanxung.cn

[R52] 统计行数
来源：http://fm.huixinmuqiang.cn

wc -l a.txt
来源：http://ct.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://nb.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zr.jctech888.com.cn

[R54] 比较两个文件
来源：http://et.panjiajie.cn

diff a.txt b.txt
来源：http://ws.shxzukj.cn

[R55] 压缩与解压
来源：http://mw.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rt.jctech888.com.cn

[R56] 远程拷贝
来源：http://ng.colortex.cn

scp file user@host:/path/
来源：http://sr.haigaiapp.cn

[R57] 远程执行命令
来源：http://fn.jianghongdianzi.cn

ssh user@host 'uptime'
来源：http://ko.asd995.cn

[R58] 下载文件
来源：http://ur.jianghongdianzi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ic.bjjhwx.cn

[R59] 发 POST JSON
来源：http://od.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://up.yuexingan06.cn

[R60] 只看 HTTP 状态码
来源：http://bb.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gk.szsharing.cn

[R61] 磁盘占用
来源：http://ot.szxytkj.cn

df -h;  du -sh *
来源：http://di.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://ay.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://xm.newstarts.cn

[R63] 内存与进程
来源：http://jg.newstarts.cn

free -h;  ps aux | grep nginx
来源：http://en.newstarts.cn

[R64] 结束进程
来源：http://vz.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://pq.wgjwhj.cn

[R65] 查看端口占用
来源：http://zf.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lf.wgjwhj.cn

[R66] 定时任务
来源：http://pq.huixiangedu.cn

crontab -e;  crontab -l
来源：http://dg.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://fv.colortex.cn

openssl rand -hex 16
来源：http://ti.wgjwhj.cn

[R68] 计算文件校验值
来源：http://ri.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ez.szxytkj.cn

[R69] 生成随机密码
来源：http://xd.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://wq.gzmigu.cn

[R70] 时间戳与互转
来源：http://je.521024.cn

date +%s;  date -d @1700000000
来源：http://cj.nszjky.cn

[R71] 日期格式化
来源：http://lb.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kb.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://co.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uu.huanxung.cn

[R73] 分割大日志
来源：http://ve.yuexingan06.cn

split -l 1000 big.log part_
来源：http://jm.haigaiapp.cn

[R74] 批量重命名
来源：http://nz.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vd.gzmigu.cn

[R75] 导出环境变量
来源：http://lb.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://lz.shxzskj.cn

[R76] 使用临时文件
来源：http://pj.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dr.haigaiapp.cn

[R77] 读取用户输入
来源：http://rj.jctech888.com.cn

read -rp "请输入: " ans
来源：http://cp.521024.cn

[R78] 交互式菜单
来源：http://rq.panjiajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vt.nicolike.cn

[R79] 解析命令行选项
来源：http://ow.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zz.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://ro.panjiajie.cn

time ./run.sh
来源：http://pb.yuexingan06.cn

================================================================================
来源：http://ys.szsharing.cn

S. C / C++ 专题
来源：http://wc.jianghongdianzi.cn

================================================================================
来源：http://rp.shxzukj.cn

[S01] C：Hello World
来源：http://ic.521024.cn

#include <stdio.h>
来源：http://cg.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zo.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://nj.lnxyls.cn

int a = 10; printf("%d\n", a);
来源：http://fn.haigaiapp.cn

[S03] C：读入整数
来源：http://cd.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://fd.asd995.cn

[S04] C：字符串复制
来源：http://zd.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kq.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://gg.panjiajie.cn

strlen(s)
来源：http://nl.wgjwhj.cn

[S06] C：字符串比较
来源：http://jv.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://fd.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://ns.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lr.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://ng.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yj.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://qq.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uj.hahajie.cn

[S10] C：指针与解引用
来源：http://yv.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://uq.szsharing.cn

[S11] C：逐行读文件
来源：http://ws.yuexingan06.cn

FILE *f = fopen("a.txt", "r");
来源：http://kk.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pj.yuntaijiaju.cn

fclose(f);
来源：http://lu.shtwfgs.cn

[S12] C：写文件
来源：http://fm.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ep.lnxyls.cn

[S13] C：宏定义
来源：http://fa.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hn.szsharing.cn

[S14] C：枚举
来源：http://xp.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://dd.bookmarksfly.cn

[S15] C：类型转换
来源：http://at.521024.cn

(double) a / b
来源：http://ov.521024.cn

[S16] C：位操作置位
来源：http://lv.szsharing.cn

x |= (1 << 3);
来源：http://os.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://py.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ov.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://aa.nicolike.cn

int main(int argc, char **argv)
来源：http://cr.jianghongdianzi.cn

[S19] C：快速排序
来源：http://ur.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ti.521024.cn

[S20] C：二分查找
来源：http://iv.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jv.shxzukj.cn

[S21] C：字符类别判断
来源：http://al.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://er.gzmigu.cn

[S22] C：字符串转数字
来源：http://io.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vr.jctech888.com.cn

[S23] C：随机数
来源：http://bg.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cv.huanxung.cn

[S24] C：获取本地时间
来源：http://jr.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ys.szsharing.cn

[S25] C：内存拷贝
来源：http://dm.huanxung.cn

memcpy(dst, src, n);
来源：http://nd.colortex.cn

[S26] C：内存清零
来源：http://so.shtwfgs.cn


<!-- 参考信息 -->