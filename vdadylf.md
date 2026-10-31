代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gu.shxzukj.cn

[Q54] 清空表
来源：http://hk.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://ld.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://yz.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hq.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://kv.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qj.panjiajie.cn

[Q57] 行号
来源：http://nh.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dp.shxzukj.cn

[Q58] 累计求和
来源：http://og.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cl.gzmigu.cn

[Q59] 分组内累计
来源：http://am.9csxet.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ft.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://pm.yuntaijiaju.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vs.huixinmuqiang.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://en.bjjhwx.cn

[Q61] 移动平均
来源：http://qg.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iy.bjjhwx.cn

[Q62] 分组占比
来源：http://nv.gzmigu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ks.muxihuayi.cn

[Q63] 开启事务
来源：http://gf.9csxet.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kg.shxzukj.cn

[Q64] 提交事务
来源：http://bm.shtwfgs.cn

COMMIT;
来源：http://us.szsharing.cn

[Q65] 回滚事务
来源：http://rg.shxzskj.cn

ROLLBACK;
来源：http://yq.lnxyls.cn

[Q66] 行锁查询
来源：http://ok.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sa.yuexingan06.cn

[Q67] 设置隔离级别
来源：http://zf.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hy.hahajie.cn

[Q68] 保存点
来源：http://gy.szxytkj.cn

SAVEPOINT sp1;
来源：http://js.asd995.cn

ROLLBACK TO sp1;
来源：http://mb.yuexingan06.cn

[Q69] 查看执行计划
来源：http://ba.wgjwhj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hn.szxytkj.cn

[Q70] 更新统计信息
来源：http://pj.yuexingan06.cn

ANALYZE TABLE users;
来源：http://do.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://au.nszjky.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oe.shxzskj.cn

[Q72] 查看索引
来源：http://xk.lnxyls.cn

SHOW INDEX FROM users;
来源：http://lu.gzmigu.cn

[Q73] 查看表状态
来源：http://au.asd995.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jb.muxihuayi.cn

[Q74] 强制使用索引
来源：http://gv.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://py.panjiajie.cn

[Q75] 日期格式化
来源：http://cq.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nt.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tm.jianghongdianzi.cn

[Q76] 按天统计
来源：http://hy.hahajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cy.hnjuh.cn

[Q77] 时间加减
来源：http://bt.gzmigu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lk.huixinmuqiang.cn

[Q78] 当前时间
来源：http://xu.nicolike.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://id.jctech888.com.cn

[Q79] 字符串拼接
来源：http://ay.bookmarksfly.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zo.nszjky.cn

[Q80] 字符串截取
来源：http://vm.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sa.wgjwhj.cn

[Q81] 字符串替换
来源：http://hs.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xm.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://kq.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yi.lnxyls.cn

[Q83] 大小写转换
来源：http://wz.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tn.bjjhwx.cn

[Q84] 去除首尾空格
来源：http://cv.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://dq.shtwfgs.cn

[Q85] 数值取整
来源：http://sr.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nt.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://uc.chemitech.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eq.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://xe.newstarts.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gz.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://ah.szsharing.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nb.huixinmuqiang.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tt.szxytkj.cn

[Q89] 判断表是否存在
来源：http://cy.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cd.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://oq.muxihuayi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kv.huanxung.cn

================================================================================
来源：http://by.nicolike.cn

R. Bash 专题
来源：http://yr.colortex.cn

================================================================================
来源：http://yp.nszjky.cn

[R01] shebang 与严格模式
来源：http://wq.newstarts.cn

#!/usr/bin/env bash
来源：http://zs.lnxyls.cn

set -euo pipefail
来源：http://cl.9csxet.cn

[R02] 变量赋值与使用
来源：http://vo.huanxung.cn

name="Tom"; echo "$name"
来源：http://kp.shxzukj.cn

[R03] 只读变量
来源：http://ot.huanxung.cn

readonly PI=3.14
来源：http://sv.lnxyls.cn

[R04] 位置参数
来源：http://kn.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ak.panjiajie.cn

[R05] 参数默认值
来源：http://tw.yuexingan06.cn

name="${1:-default}"
来源：http://ju.newstarts.cn

[R06] 判断命令是否存在
来源：http://ei.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ct.szsharing.cn

[R07] if 判断文件
来源：http://gt.panjiajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jq.bookmarksfly.cn

[R08] 数值比较
来源：http://qe.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ai.bookmarksfly.cn

[R09] 字符串比较
来源：http://zl.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yc.huixiangedu.cn

[R10] 正则匹配
来源：http://ct.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ba.huanxung.cn

[R11] case 多分支
来源：http://qh.chemitech.net.cn

case "$1" in
来源：http://up.shtwfgs.cn

start) echo "启动" ;;
来源：http://lx.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://zi.521024.cn

*)     echo "未知命令" ;;
来源：http://kg.yuexingan06.cn

esac
来源：http://cl.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://ld.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://bf.jctech888.com.cn

[R13] for 计数循环
来源：http://tr.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://ql.szxytkj.cn

[R14] C 风格 for
来源：http://bl.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tc.muxihuayi.cn

[R15] while 逐行读文件
来源：http://ob.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ml.shxzskj.cn

[R16] until 等待条件
来源：http://qs.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pz.szsharing.cn

[R17] 数组定义与取值
来源：http://ez.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pi.gzmigu.cn

[R18] 遍历数组
来源：http://jw.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xi.yuexingan06.cn

[R19] 数组长度
来源：http://dt.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://ha.hnjuh.cn

[R20] 关联数组（字典）
来源：http://dn.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xm.huanxung.cn

[R21] 字符串长度
来源：http://bs.521024.cn

echo "${#s}"
来源：http://gd.huanxung.cn

[R22] 截取子串
来源：http://ij.gzmigu.cn

echo "${s:0:5}"
来源：http://mm.9csxet.cn

[R23] 字符串替换
来源：http://um.521024.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jz.jctech888.com.cn

[R24] 大小写转换
来源：http://zw.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cl.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://uf.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gp.huixiangedu.cn

[R26] 命令替换
来源：http://qp.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://cq.lnxyls.cn

[R27] 算术展开
来源：http://rp.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://wv.huixinmuqiang.cn

[R28] 浮点运算
来源：http://th.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://ve.huixinmuqiang.cn

[R29] 定义函数
来源：http://kw.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nb.muxihuayi.cn

[R30] 函数返回状态码
来源：http://ut.bookmarksfly.cn

f() { return 0; }; f || echo "失败了"
来源：http://ha.chemitech.net.cn

[R31] 局部变量
来源：http://ea.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://cv.shxzskj.cn

[R32] 参数个数校验
来源：http://wn.shtwfgs.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ou.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://gi.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ua.huixiangedu.cn

[R34] 退出时清理
来源：http://ka.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dk.gzmigu.cn

[R35] 后台执行并等待
来源：http://gx.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ba.9csxet.cn

[R36] 并发执行多个任务
来源：http://yw.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ar.newstarts.cn

[R37] 把输出赋给变量
来源：http://dc.wgjwhj.cn

files=$(ls -1)
来源：http://hw.shtwfgs.cn

[R38] 管道串联
来源：http://zn.nszjky.cn

cat a.txt | grep -i error | wc -l
来源：http://zv.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://nj.gzmigu.cn

cmd > out.log 2>&1
来源：http://mz.yuexingan06.cn

[R40] 追加写日志
来源：http://dz.shxzukj.cn

echo "log" >> out.log
来源：http://uc.huixiangedu.cn

[R41] 丢弃输出
来源：http://pv.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://ic.lnxyls.cn

[R42] 输入重定向
来源：http://kq.huanxung.cn

wc -l < a.txt
来源：http://wf.yuexingan06.cn

[R43] 按名字查找文件
来源：http://dc.hahajie.cn

find . -name "*.log" -type f
来源：http://qw.shtwfgs.cn

[R44] 按修改时间查找
来源：http://as.panjiajie.cn

find . -mtime -7 -type f
来源：http://op.shtwfgs.cn

[R45] 批量删除
来源：http://da.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://yd.huixiangedu.cn

[R46] 递归替换文件内容
来源：http://ym.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sy.nszjky.cn

[R47] sed 单行替换
来源：http://sh.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bf.szxytkj.cn

[R48] awk 取指定列
来源：http://pd.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://ue.yuexingan06.cn

[R49] awk 带条件
来源：http://qn.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dk.panjiajie.cn

[R50] awk 求和
来源：http://fd.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pv.jctech888.com.cn

[R51] 排序去重取前几
来源：http://zw.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oe.hahajie.cn

[R52] 统计行数
来源：http://rc.szsharing.cn

wc -l a.txt
来源：http://jd.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://un.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uz.jctech888.com.cn

[R54] 比较两个文件
来源：http://sr.shxzskj.cn

diff a.txt b.txt
来源：http://lx.panjiajie.cn

[R55] 压缩与解压
来源：http://lc.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xy.bookmarksfly.cn

[R56] 远程拷贝
来源：http://rs.gzmigu.cn

scp file user@host:/path/
来源：http://fr.521024.cn

[R57] 远程执行命令
来源：http://sd.shtwfgs.cn

ssh user@host 'uptime'
来源：http://ro.newstarts.cn

[R58] 下载文件
来源：http://mv.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://di.szxytkj.cn

[R59] 发 POST JSON
来源：http://jq.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sj.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://ia.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hp.shxzukj.cn

[R61] 磁盘占用
来源：http://lj.szsharing.cn

df -h;  du -sh *
来源：http://up.nicolike.cn

[R62] 找最占空间的文件
来源：http://pa.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://ye.szxytkj.cn

[R63] 内存与进程
来源：http://vb.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://pj.panjiajie.cn

[R64] 结束进程
来源：http://lj.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://km.huixiangedu.cn

[R65] 查看端口占用
来源：http://ro.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bl.bjjhwx.cn

[R66] 定时任务
来源：http://zm.muxihuayi.cn

crontab -e;  crontab -l
来源：http://gq.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://uk.bjjhwx.cn

openssl rand -hex 16
来源：http://wd.chemitech.net.cn

[R68] 计算文件校验值
来源：http://zh.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hh.haigaiapp.cn

[R69] 生成随机密码
来源：http://ya.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://qo.nicolike.cn

[R70] 时间戳与互转
来源：http://oc.9csxet.cn

date +%s;  date -d @1700000000
来源：http://uq.szsharing.cn

[R71] 日期格式化
来源：http://eo.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xq.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://io.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oy.yuntaijiaju.cn

[R73] 分割大日志
来源：http://ov.gzmigu.cn

split -l 1000 big.log part_
来源：http://rn.hnjuh.cn

[R74] 批量重命名
来源：http://rl.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dy.huanxung.cn

[R75] 导出环境变量
来源：http://sq.hnjuh.cn

export PATH="$HOME/bin:$PATH"
来源：http://ot.newstarts.cn

[R76] 使用临时文件
来源：http://xi.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zy.hahajie.cn

[R77] 读取用户输入
来源：http://hk.shxzskj.cn

read -rp "请输入: " ans
来源：http://ii.lnxyls.cn

[R78] 交互式菜单
来源：http://sr.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://se.jctech888.com.cn

[R79] 解析命令行选项
来源：http://yb.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mo.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://ex.9csxet.cn

time ./run.sh
来源：http://fm.wgjwhj.cn

================================================================================
来源：http://qy.hnjuh.cn

S. C / C++ 专题
来源：http://kk.jianghongdianzi.cn

================================================================================
来源：http://so.bookmarksfly.cn

[S01] C：Hello World
来源：http://dp.yuntaijiaju.cn

#include <stdio.h>
来源：http://ek.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rd.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://uk.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://jb.panjiajie.cn

[S03] C：读入整数
来源：http://ru.haigaiapp.cn

int x; scanf("%d", &x);
来源：http://if.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://ju.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xh.yuexingan06.cn

[S05] C：字符串长度
来源：http://rx.szsharing.cn

strlen(s)
来源：http://cq.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://fq.hnjuh.cn

strcmp(a, b) == 0
来源：http://gq.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://eo.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://io.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://is.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://io.bjjhwx.cn

[S09] C：结构体定义与初始化
来源：http://qt.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ye.newstarts.cn

[S10] C：指针与解引用
来源：http://kc.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://rk.szsharing.cn

[S11] C：逐行读文件
来源：http://ob.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://gl.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://di.jianghongdianzi.cn

fclose(f);
来源：http://vr.lnxyls.cn

[S12] C：写文件
来源：http://li.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lr.yuntaijiaju.cn

[S13] C：宏定义
来源：http://ap.newstarts.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pj.colortex.cn

[S14] C：枚举
来源：http://pg.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://lc.shxzskj.cn

[S15] C：类型转换
来源：http://fe.nszjky.cn

(double) a / b
来源：http://uc.lnxyls.cn

[S16] C：位操作置位
来源：http://mb.9csxet.cn

x |= (1 << 3);
来源：http://ha.asd995.cn

[S17] C：安全拼接字符串
来源：http://ed.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wo.nicolike.cn

[S18] C：命令行参数
来源：http://bh.nicolike.cn

int main(int argc, char **argv)
来源：http://pe.wgjwhj.cn

[S19] C：快速排序
来源：http://js.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cr.asd995.cn

[S20] C：二分查找
来源：http://hk.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ee.521024.cn

[S21] C：字符类别判断
来源：http://yc.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://je.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://bh.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nt.bookmarksfly.cn

[S23] C：随机数
来源：http://za.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tp.yuexingan06.cn

[S24] C：获取本地时间
来源：http://rr.asd995.cn


<!-- 参考信息 -->