代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zq.szxytkj.cn

[Q56] 密集排名（并列不占位）
来源：http://rj.haigaiapp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fa.jctech888.com.cn

[Q57] 行号
来源：http://pu.shxzskj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sj.nszjky.cn

[Q58] 累计求和
来源：http://zn.nszjky.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mo.yuntaijiaju.cn

[Q59] 分组内累计
来源：http://wp.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ys.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://nn.chemitech.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ax.nszjky.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wv.wgjwhj.cn

[Q61] 移动平均
来源：http://ov.bjjhwx.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hm.yuexingan06.cn

[Q62] 分组占比
来源：http://um.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pt.panjiajie.cn

[Q63] 开启事务
来源：http://uj.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yx.jctech888.com.cn

[Q64] 提交事务
来源：http://hm.jctech888.com.cn

COMMIT;
来源：http://tz.asd995.cn

[Q65] 回滚事务
来源：http://mi.asd995.cn

ROLLBACK;
来源：http://vu.colortex.cn

[Q66] 行锁查询
来源：http://ml.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dr.szxytkj.cn

[Q67] 设置隔离级别
来源：http://to.huixiangedu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ya.shxzskj.cn

[Q68] 保存点
来源：http://pi.shxzskj.cn

SAVEPOINT sp1;
来源：http://pp.9csxet.cn

ROLLBACK TO sp1;
来源：http://hk.szsharing.cn

[Q69] 查看执行计划
来源：http://uy.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tn.haigaiapp.cn

[Q70] 更新统计信息
来源：http://is.bookmarksfly.cn

ANALYZE TABLE users;
来源：http://ty.shxzskj.cn

[Q71] 查看建表语句
来源：http://pg.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://os.hahajie.cn

[Q72] 查看索引
来源：http://ec.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://gg.hnjuh.cn

[Q73] 查看表状态
来源：http://cz.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://md.asd995.cn

[Q74] 强制使用索引
来源：http://oj.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tx.colortex.cn

[Q75] 日期格式化
来源：http://le.haigaiapp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://li.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vr.chemitech.net.cn

[Q76] 按天统计
来源：http://rj.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pt.huixinmuqiang.cn

[Q77] 时间加减
来源：http://px.jctech888.com.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yu.gzmigu.cn

[Q78] 当前时间
来源：http://am.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ic.muxihuayi.cn

[Q79] 字符串拼接
来源：http://mt.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ht.newstarts.cn

[Q80] 字符串截取
来源：http://kq.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gw.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://hb.wgjwhj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://aj.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://pw.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kd.nszjky.cn

[Q83] 大小写转换
来源：http://zt.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://aa.gzmigu.cn

[Q84] 去除首尾空格
来源：http://xs.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://vc.szsharing.cn

[Q85] 数值取整
来源：http://lt.chemitech.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pi.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://wr.nszjky.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wl.hahajie.cn

[Q87] JSON 字段做条件
来源：http://nn.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dv.nicolike.cn

[Q88] 行转列（条件聚合）
来源：http://bh.huixinmuqiang.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sf.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cy.colortex.cn

[Q89] 判断表是否存在
来源：http://cq.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ef.colortex.cn

[Q90] 生成序号列
来源：http://ti.huanxung.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://um.shxzskj.cn

================================================================================
来源：http://iw.asd995.cn

R. Bash 专题
来源：http://dw.bjjhwx.cn

================================================================================
来源：http://jn.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://or.nicolike.cn

#!/usr/bin/env bash
来源：http://ur.yuntaijiaju.cn

set -euo pipefail
来源：http://td.gzmigu.cn

[R02] 变量赋值与使用
来源：http://jo.bjjhwx.cn

name="Tom"; echo "$name"
来源：http://er.hnjuh.cn

[R03] 只读变量
来源：http://wu.asd995.cn

readonly PI=3.14
来源：http://qr.szxytkj.cn

[R04] 位置参数
来源：http://gi.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hr.yuntaijiaju.cn

[R05] 参数默认值
来源：http://gq.wgjwhj.cn

name="${1:-default}"
来源：http://zj.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://xx.asd995.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kd.jianghongdianzi.cn

[R07] if 判断文件
来源：http://aw.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pa.chemitech.net.cn

[R08] 数值比较
来源：http://gm.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pi.hnjuh.cn

[R09] 字符串比较
来源：http://ol.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zo.haigaiapp.cn

[R10] 正则匹配
来源：http://ti.lnxyls.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://el.nicolike.cn

[R11] case 多分支
来源：http://nk.newstarts.cn

case "$1" in
来源：http://lv.chemitech.net.cn

start) echo "启动" ;;
来源：http://zk.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://zp.hnjuh.cn

*)     echo "未知命令" ;;
来源：http://ui.gzmigu.cn

esac
来源：http://la.9csxet.cn

[R12] for 遍历文件
来源：http://is.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://cy.yuexingan06.cn

[R13] for 计数循环
来源：http://zy.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://lm.muxihuayi.cn

[R14] C 风格 for
来源：http://mv.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ht.huixiangedu.cn

[R15] while 逐行读文件
来源：http://jl.haigaiapp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xn.newstarts.cn

[R16] until 等待条件
来源：http://fz.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rg.9csxet.cn

[R17] 数组定义与取值
来源：http://yz.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bv.asd995.cn

[R18] 遍历数组
来源：http://am.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ie.bookmarksfly.cn

[R19] 数组长度
来源：http://xd.bjjhwx.cn

echo "${#arr[@]}"
来源：http://ii.hahajie.cn

[R20] 关联数组（字典）
来源：http://ol.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gj.colortex.cn

[R21] 字符串长度
来源：http://ms.huanxung.cn

echo "${#s}"
来源：http://en.panjiajie.cn

[R22] 截取子串
来源：http://bz.yuexingan06.cn

echo "${s:0:5}"
来源：http://pd.lnxyls.cn

[R23] 字符串替换
来源：http://ua.yuexingan06.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vi.bookmarksfly.cn

[R24] 大小写转换
来源：http://qa.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://an.szxytkj.cn

[R25] 去后缀 / 去前缀
来源：http://ys.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gz.wgjwhj.cn

[R26] 命令替换
来源：http://cx.yuexingan06.cn

now=$(date +%F); echo "$now"
来源：http://nt.huanxung.cn

[R27] 算术展开
来源：http://gx.newstarts.cn

echo $((1 + 2 * 3))
来源：http://hi.jianghongdianzi.cn

[R28] 浮点运算
来源：http://vz.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://qi.hnjuh.cn

[R29] 定义函数
来源：http://rt.bjjhwx.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yg.yuexingan06.cn

[R30] 函数返回状态码
来源：http://gr.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://pt.wgjwhj.cn

[R31] 局部变量
来源：http://fa.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://hb.wgjwhj.cn

[R32] 参数个数校验
来源：http://of.chemitech.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tz.bjjhwx.cn

[R33] 捕获错误并提示行号
来源：http://mq.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uh.muxihuayi.cn

[R34] 退出时清理
来源：http://hv.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pu.nicolike.cn

[R35] 后台执行并等待
来源：http://fe.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://it.newstarts.cn

[R36] 并发执行多个任务
来源：http://ua.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kd.lnxyls.cn

[R37] 把输出赋给变量
来源：http://wm.jctech888.com.cn

files=$(ls -1)
来源：http://cz.muxihuayi.cn

[R38] 管道串联
来源：http://ch.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://sk.jctech888.com.cn

[R39] 重定向标准输出与错误
来源：http://ql.jctech888.com.cn

cmd > out.log 2>&1
来源：http://dn.haigaiapp.cn

[R40] 追加写日志
来源：http://dl.muxihuayi.cn

echo "log" >> out.log
来源：http://sv.huanxung.cn

[R41] 丢弃输出
来源：http://dq.nicolike.cn

cmd >/dev/null 2>&1
来源：http://ae.huixiangedu.cn

[R42] 输入重定向
来源：http://uu.muxihuayi.cn

wc -l < a.txt
来源：http://lb.nszjky.cn

[R43] 按名字查找文件
来源：http://ah.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://nx.chemitech.net.cn

[R44] 按修改时间查找
来源：http://ga.9csxet.cn

find . -mtime -7 -type f
来源：http://ha.9csxet.cn

[R45] 批量删除
来源：http://ya.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://vf.newstarts.cn

[R46] 递归替换文件内容
来源：http://wg.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gm.wgjwhj.cn

[R47] sed 单行替换
来源：http://ez.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qu.szsharing.cn

[R48] awk 取指定列
来源：http://al.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://vv.huanxung.cn

[R49] awk 带条件
来源：http://pr.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tc.yuntaijiaju.cn

[R50] awk 求和
来源：http://mx.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yf.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://hd.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zu.szsharing.cn

[R52] 统计行数
来源：http://oq.colortex.cn

wc -l a.txt
来源：http://wt.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://fy.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ik.lnxyls.cn

[R54] 比较两个文件
来源：http://ph.jctech888.com.cn

diff a.txt b.txt
来源：http://zh.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://qr.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rn.hahajie.cn

[R56] 远程拷贝
来源：http://ac.gzmigu.cn

scp file user@host:/path/
来源：http://xx.chemitech.net.cn

[R57] 远程执行命令
来源：http://xn.nicolike.cn

ssh user@host 'uptime'
来源：http://li.521024.cn

[R58] 下载文件
来源：http://it.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nf.asd995.cn

[R59] 发 POST JSON
来源：http://jq.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ia.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://vb.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fu.szsharing.cn

[R61] 磁盘占用
来源：http://qh.colortex.cn

df -h;  du -sh *
来源：http://bp.hnjuh.cn

[R62] 找最占空间的文件
来源：http://oo.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://ux.shtwfgs.cn

[R63] 内存与进程
来源：http://aj.colortex.cn

free -h;  ps aux | grep nginx
来源：http://wc.jctech888.com.cn

[R64] 结束进程
来源：http://gf.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://qx.chemitech.net.cn

[R65] 查看端口占用
来源：http://kz.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sl.9csxet.cn

[R66] 定时任务
来源：http://ru.shtwfgs.cn

crontab -e;  crontab -l
来源：http://sk.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://xa.huixinmuqiang.cn

openssl rand -hex 16
来源：http://fz.bjjhwx.cn

[R68] 计算文件校验值
来源：http://yn.gzmigu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cm.colortex.cn

[R69] 生成随机密码
来源：http://as.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://cm.shtwfgs.cn

[R70] 时间戳与互转
来源：http://lp.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://dr.szxytkj.cn

[R71] 日期格式化
来源：http://rw.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yo.asd995.cn

[R72] 等待端口就绪
来源：http://dx.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fd.shxzskj.cn

[R73] 分割大日志
来源：http://xq.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://ts.huixiangedu.cn

[R74] 批量重命名
来源：http://uc.nszjky.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uw.hnjuh.cn

[R75] 导出环境变量
来源：http://rd.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://oo.chemitech.net.cn

[R76] 使用临时文件
来源：http://yl.hahajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kg.521024.cn

[R77] 读取用户输入
来源：http://fp.muxihuayi.cn

read -rp "请输入: " ans
来源：http://ze.szsharing.cn

[R78] 交互式菜单
来源：http://wi.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gn.szsharing.cn

[R79] 解析命令行选项
来源：http://fb.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://is.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://al.bjjhwx.cn

time ./run.sh
来源：http://av.bookmarksfly.cn

================================================================================
来源：http://ea.yuntaijiaju.cn

S. C / C++ 专题
来源：http://ym.shtwfgs.cn

================================================================================
来源：http://tj.szxytkj.cn

[S01] C：Hello World
来源：http://nq.chemitech.net.cn

#include <stdio.h>
来源：http://gp.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ge.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://jj.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://bf.jianghongdianzi.cn

[S03] C：读入整数
来源：http://uq.nszjky.cn

int x; scanf("%d", &x);
来源：http://ju.gzmigu.cn

[S04] C：字符串复制
来源：http://si.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zn.9csxet.cn

[S05] C：字符串长度
来源：http://zo.nszjky.cn

strlen(s)
来源：http://rp.szsharing.cn

[S06] C：字符串比较
来源：http://jq.shxzskj.cn

strcmp(a, b) == 0
来源：http://aj.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://cl.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ea.521024.cn

[S08] C：动态内存分配与释放
来源：http://gm.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dt.521024.cn

[S09] C：结构体定义与初始化
来源：http://gn.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://os.wgjwhj.cn

[S10] C：指针与解引用
来源：http://zi.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://bf.szsharing.cn

[S11] C：逐行读文件
来源：http://aw.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://co.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://im.shtwfgs.cn

fclose(f);
来源：http://qu.chemitech.net.cn

[S12] C：写文件
来源：http://jk.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ma.newstarts.cn

[S13] C：宏定义
来源：http://hj.newstarts.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vj.wgjwhj.cn

[S14] C：枚举
来源：http://wp.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://rv.huixinmuqiang.cn

[S15] C：类型转换
来源：http://yi.huixinmuqiang.cn

(double) a / b
来源：http://yt.hnjuh.cn

[S16] C：位操作置位
来源：http://ll.wgjwhj.cn

x |= (1 << 3);
来源：http://mb.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://ge.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nq.wgjwhj.cn

[S18] C：命令行参数
来源：http://br.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://cl.9csxet.cn

[S19] C：快速排序
来源：http://wm.521024.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oe.shxzskj.cn

[S20] C：二分查找
来源：http://eq.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zx.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://qa.shxzskj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://da.colortex.cn

[S22] C：字符串转数字
来源：http://wt.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wf.chemitech.net.cn

[S23] C：随机数
来源：http://tc.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gn.asd995.cn

[S24] C：获取本地时间
来源：http://dm.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jz.nicolike.cn

[S25] C：内存拷贝
来源：http://xc.asd995.cn

memcpy(dst, src, n);
来源：http://rv.lnxyls.cn

[S26] C：内存清零
来源：http://fp.yuntaijiaju.cn


<!-- 参考信息 -->