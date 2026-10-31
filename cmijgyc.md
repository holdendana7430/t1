代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ip.nszjky.cn

[Q52] 删除指定行
来源：http://cq.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://lo.yuntaijiaju.cn

[Q53] 按条件删除
来源：http://lk.huixiangedu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bv.huanxung.cn

[Q54] 清空表
来源：http://hz.lnxyls.cn

TRUNCATE TABLE logs;
来源：http://kv.newstarts.cn

[Q55] 排名（并列占位）
来源：http://ou.yuntaijiaju.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wh.shtwfgs.cn

[Q56] 密集排名（并列不占位）
来源：http://ex.szxytkj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qj.panjiajie.cn

[Q57] 行号
来源：http://yu.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jv.jianghongdianzi.cn

[Q58] 累计求和
来源：http://ix.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uq.hahajie.cn

[Q59] 分组内累计
来源：http://yj.muxihuayi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zp.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://zt.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xe.colortex.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tx.lnxyls.cn

[Q61] 移动平均
来源：http://ln.bjjhwx.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ls.muxihuayi.cn

[Q62] 分组占比
来源：http://mc.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uu.huanxung.cn

[Q63] 开启事务
来源：http://ak.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yi.newstarts.cn

[Q64] 提交事务
来源：http://sq.hahajie.cn

COMMIT;
来源：http://zc.yuntaijiaju.cn

[Q65] 回滚事务
来源：http://qj.hnjuh.cn

ROLLBACK;
来源：http://dh.chemitech.net.cn

[Q66] 行锁查询
来源：http://vz.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pv.gzmigu.cn

[Q67] 设置隔离级别
来源：http://jz.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oy.shxzskj.cn

[Q68] 保存点
来源：http://vj.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://uk.lnxyls.cn

ROLLBACK TO sp1;
来源：http://gj.bjjhwx.cn

[Q69] 查看执行计划
来源：http://yr.szsharing.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pd.szxytkj.cn

[Q70] 更新统计信息
来源：http://pr.nszjky.cn

ANALYZE TABLE users;
来源：http://yl.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://ms.yuexingan06.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jl.hahajie.cn

[Q72] 查看索引
来源：http://oz.hahajie.cn

SHOW INDEX FROM users;
来源：http://mk.muxihuayi.cn

[Q73] 查看表状态
来源：http://gx.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xz.haigaiapp.cn

[Q74] 强制使用索引
来源：http://fe.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tv.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://tl.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sl.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ko.chemitech.net.cn

[Q76] 按天统计
来源：http://oi.huixinmuqiang.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ea.shtwfgs.cn

[Q77] 时间加减
来源：http://sf.yuexingan06.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pv.hahajie.cn

[Q78] 当前时间
来源：http://rb.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wj.jianghongdianzi.cn

[Q79] 字符串拼接
来源：http://zs.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yl.huanxung.cn

[Q80] 字符串截取
来源：http://mb.huixiangedu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://al.hahajie.cn

[Q81] 字符串替换
来源：http://ot.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mk.muxihuayi.cn

[Q82] 字符长度与字节长度
来源：http://xs.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cr.lnxyls.cn

[Q83] 大小写转换
来源：http://gv.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ou.nicolike.cn

[Q84] 去除首尾空格
来源：http://wp.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://wy.bookmarksfly.cn

[Q85] 数值取整
来源：http://om.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ti.colortex.cn

[Q86] 读取 JSON 字段
来源：http://jl.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kr.bjjhwx.cn

[Q87] JSON 字段做条件
来源：http://zh.shxzukj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pa.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://xr.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lx.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yg.huanxung.cn

[Q89] 判断表是否存在
来源：http://dh.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nf.521024.cn

[Q90] 生成序号列
来源：http://hj.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rq.gzmigu.cn

================================================================================
来源：http://iu.chemitech.net.cn

R. Bash 专题
来源：http://nt.chemitech.net.cn

================================================================================
来源：http://xo.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://gd.shxzukj.cn

#!/usr/bin/env bash
来源：http://tq.hnjuh.cn

set -euo pipefail
来源：http://dn.521024.cn

[R02] 变量赋值与使用
来源：http://kj.szsharing.cn

name="Tom"; echo "$name"
来源：http://gn.nszjky.cn

[R03] 只读变量
来源：http://qc.yuexingan06.cn

readonly PI=3.14
来源：http://oo.shxzukj.cn

[R04] 位置参数
来源：http://kq.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zp.hahajie.cn

[R05] 参数默认值
来源：http://or.521024.cn

name="${1:-default}"
来源：http://dr.lnxyls.cn

[R06] 判断命令是否存在
来源：http://my.jctech888.com.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mc.lnxyls.cn

[R07] if 判断文件
来源：http://sl.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://um.jianghongdianzi.cn

[R08] 数值比较
来源：http://pq.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://li.yuntaijiaju.cn

[R09] 字符串比较
来源：http://ni.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qw.yuexingan06.cn

[R10] 正则匹配
来源：http://jj.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ej.newstarts.cn

[R11] case 多分支
来源：http://ar.wgjwhj.cn

case "$1" in
来源：http://vi.muxihuayi.cn

start) echo "启动" ;;
来源：http://ow.hnjuh.cn

stop)  echo "停止" ;;
来源：http://dm.yuntaijiaju.cn

*)     echo "未知命令" ;;
来源：http://qv.gzmigu.cn

esac
来源：http://sz.9csxet.cn

[R12] for 遍历文件
来源：http://cu.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://ex.shtwfgs.cn

[R13] for 计数循环
来源：http://wd.shxzskj.cn

for i in {1..10}; do echo "$i"; done
来源：http://zb.szxytkj.cn

[R14] C 风格 for
来源：http://yo.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lf.hahajie.cn

[R15] while 逐行读文件
来源：http://ib.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lc.yuexingan06.cn

[R16] until 等待条件
来源：http://mp.newstarts.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vn.lnxyls.cn

[R17] 数组定义与取值
来源：http://dp.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ms.szsharing.cn

[R18] 遍历数组
来源：http://kp.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gh.hnjuh.cn

[R19] 数组长度
来源：http://ti.lnxyls.cn

echo "${#arr[@]}"
来源：http://ez.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://xv.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rb.szxytkj.cn

[R21] 字符串长度
来源：http://xx.jctech888.com.cn

echo "${#s}"
来源：http://fr.gzmigu.cn

[R22] 截取子串
来源：http://kb.asd995.cn

echo "${s:0:5}"
来源：http://ku.huixiangedu.cn

[R23] 字符串替换
来源：http://lb.szxytkj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fr.szxytkj.cn

[R24] 大小写转换
来源：http://vt.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ma.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://sf.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zx.chemitech.net.cn

[R26] 命令替换
来源：http://tf.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://xd.haigaiapp.cn

[R27] 算术展开
来源：http://ge.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://vw.asd995.cn

[R28] 浮点运算
来源：http://td.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://na.haigaiapp.cn

[R29] 定义函数
来源：http://bn.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oh.9csxet.cn

[R30] 函数返回状态码
来源：http://vc.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://if.muxihuayi.cn

[R31] 局部变量
来源：http://bd.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://yu.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://ia.yuexingan06.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bj.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://xv.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lv.gzmigu.cn

[R34] 退出时清理
来源：http://oj.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gr.huanxung.cn

[R35] 后台执行并等待
来源：http://cl.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rk.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://da.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://we.hnjuh.cn

[R37] 把输出赋给变量
来源：http://ko.shtwfgs.cn

files=$(ls -1)
来源：http://uq.colortex.cn

[R38] 管道串联
来源：http://py.huixiangedu.cn

cat a.txt | grep -i error | wc -l
来源：http://ub.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://gd.wgjwhj.cn

cmd > out.log 2>&1
来源：http://cj.huixinmuqiang.cn

[R40] 追加写日志
来源：http://bx.wgjwhj.cn

echo "log" >> out.log
来源：http://lr.panjiajie.cn

[R41] 丢弃输出
来源：http://fd.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://fe.nicolike.cn

[R42] 输入重定向
来源：http://yq.bjjhwx.cn

wc -l < a.txt
来源：http://gj.bjjhwx.cn

[R43] 按名字查找文件
来源：http://ck.colortex.cn

find . -name "*.log" -type f
来源：http://wo.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://tt.huixinmuqiang.cn

find . -mtime -7 -type f
来源：http://ck.shxzskj.cn

[R45] 批量删除
来源：http://ep.hnjuh.cn

find . -name "*.tmp" -delete
来源：http://jz.gzmigu.cn

[R46] 递归替换文件内容
来源：http://ea.hnjuh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://le.shxzskj.cn

[R47] sed 单行替换
来源：http://uu.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tg.huanxung.cn

[R48] awk 取指定列
来源：http://fr.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://oj.chemitech.net.cn

[R49] awk 带条件
来源：http://lv.huixinmuqiang.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ab.shxzskj.cn

[R50] awk 求和
来源：http://bm.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sl.asd995.cn

[R51] 排序去重取前几
来源：http://mv.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://di.yuexingan06.cn

[R52] 统计行数
来源：http://fv.muxihuayi.cn

wc -l a.txt
来源：http://me.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://rf.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bk.szxytkj.cn

[R54] 比较两个文件
来源：http://wx.jctech888.com.cn

diff a.txt b.txt
来源：http://ny.shxzskj.cn

[R55] 压缩与解压
来源：http://wh.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wu.jctech888.com.cn

[R56] 远程拷贝
来源：http://nx.bookmarksfly.cn

scp file user@host:/path/
来源：http://uh.gzmigu.cn

[R57] 远程执行命令
来源：http://qr.bjjhwx.cn

ssh user@host 'uptime'
来源：http://ih.bjjhwx.cn

[R58] 下载文件
来源：http://mr.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ym.muxihuayi.cn

[R59] 发 POST JSON
来源：http://tf.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oy.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://ea.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ji.shxzskj.cn

[R61] 磁盘占用
来源：http://hv.huixinmuqiang.cn

df -h;  du -sh *
来源：http://ff.nszjky.cn

[R62] 找最占空间的文件
来源：http://cf.bookmarksfly.cn

du -ah . | sort -rh | head -10
来源：http://bx.panjiajie.cn

[R63] 内存与进程
来源：http://aa.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://wb.jianghongdianzi.cn

[R64] 结束进程
来源：http://pa.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://gr.yuexingan06.cn

[R65] 查看端口占用
来源：http://ua.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pt.nicolike.cn

[R66] 定时任务
来源：http://mk.hahajie.cn

crontab -e;  crontab -l
来源：http://wt.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://xl.huixiangedu.cn

openssl rand -hex 16
来源：http://jh.wgjwhj.cn

[R68] 计算文件校验值
来源：http://pi.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ub.szxytkj.cn

[R69] 生成随机密码
来源：http://nr.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://ec.huanxung.cn

[R70] 时间戳与互转
来源：http://zx.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://fc.muxihuayi.cn

[R71] 日期格式化
来源：http://ss.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fo.colortex.cn

[R72] 等待端口就绪
来源：http://tp.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://st.shxzukj.cn

[R73] 分割大日志
来源：http://gp.newstarts.cn

split -l 1000 big.log part_
来源：http://dn.colortex.cn

[R74] 批量重命名
来源：http://ks.bookmarksfly.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ih.panjiajie.cn

[R75] 导出环境变量
来源：http://eb.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://jj.hnjuh.cn

[R76] 使用临时文件
来源：http://ud.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ny.huixiangedu.cn

[R77] 读取用户输入
来源：http://np.huixiangedu.cn

read -rp "请输入: " ans
来源：http://fc.huixiangedu.cn

[R78] 交互式菜单
来源：http://cl.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://do.muxihuayi.cn

[R79] 解析命令行选项
来源：http://ro.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gb.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://ux.shxzukj.cn

time ./run.sh
来源：http://in.nszjky.cn

================================================================================
来源：http://za.lnxyls.cn

S. C / C++ 专题
来源：http://ui.huixinmuqiang.cn

================================================================================
来源：http://dw.asd995.cn

[S01] C：Hello World
来源：http://ih.lnxyls.cn

#include <stdio.h>
来源：http://sr.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lx.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://tp.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://mc.shxzukj.cn

[S03] C：读入整数
来源：http://sw.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://we.chemitech.net.cn

[S04] C：字符串复制
来源：http://zf.gzmigu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cb.shxzukj.cn

[S05] C：字符串长度
来源：http://oa.haigaiapp.cn

strlen(s)
来源：http://be.wgjwhj.cn

[S06] C：字符串比较
来源：http://wg.szxytkj.cn

strcmp(a, b) == 0
来源：http://fe.shxzukj.cn

[S07] C：数组遍历求和
来源：http://bh.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lg.gzmigu.cn

[S08] C：动态内存分配与释放
来源：http://vs.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ny.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://ba.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rg.huanxung.cn

[S10] C：指针与解引用
来源：http://pl.shxzukj.cn

int *p = &a;  *p = 5;
来源：http://zp.521024.cn

[S11] C：逐行读文件
来源：http://zt.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://zb.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hi.hnjuh.cn

fclose(f);
来源：http://qf.shxzskj.cn

[S12] C：写文件
来源：http://fb.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gv.shxzukj.cn

[S13] C：宏定义
来源：http://pd.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://go.szxytkj.cn

[S14] C：枚举
来源：http://uj.huanxung.cn

enum Color { RED, GREEN, BLUE };
来源：http://vw.huixinmuqiang.cn

[S15] C：类型转换
来源：http://me.asd995.cn

(double) a / b
来源：http://be.hahajie.cn

[S16] C：位操作置位
来源：http://my.yuexingan06.cn

x |= (1 << 3);
来源：http://ju.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://pi.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mn.nszjky.cn

[S18] C：命令行参数
来源：http://hj.huanxung.cn

int main(int argc, char **argv)
来源：http://st.haigaiapp.cn

[S19] C：快速排序
来源：http://hn.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sz.asd995.cn

[S20] C：二分查找
来源：http://sj.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cz.hnjuh.cn

[S21] C：字符类别判断
来源：http://kc.shxzskj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tg.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://sj.panjiajie.cn


<!-- 参考信息 -->