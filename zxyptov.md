代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ei.bjjhwx.cn

[Q54] 清空表
来源：http://kr.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://et.nszjky.cn

[Q55] 排名（并列占位）
来源：http://yi.lnxyls.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://so.newstarts.cn

[Q56] 密集排名（并列不占位）
来源：http://pt.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pg.nszjky.cn

[Q57] 行号
来源：http://vf.gzmigu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yd.nicolike.cn

[Q58] 累计求和
来源：http://hq.lnxyls.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ru.shxzskj.cn

[Q59] 分组内累计
来源：http://cr.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ls.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://mz.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mn.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eo.szsharing.cn

[Q61] 移动平均
来源：http://xg.shxzukj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kq.jctech888.com.cn

[Q62] 分组占比
来源：http://xs.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gd.newstarts.cn

[Q63] 开启事务
来源：http://gn.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xn.huanxung.cn

[Q64] 提交事务
来源：http://un.shxzukj.cn

COMMIT;
来源：http://wq.huixiangedu.cn

[Q65] 回滚事务
来源：http://ld.521024.cn

ROLLBACK;
来源：http://cx.panjiajie.cn

[Q66] 行锁查询
来源：http://tg.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fh.hnjuh.cn

[Q67] 设置隔离级别
来源：http://do.nszjky.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yd.hnjuh.cn

[Q68] 保存点
来源：http://zq.shxzskj.cn

SAVEPOINT sp1;
来源：http://wc.huixiangedu.cn

ROLLBACK TO sp1;
来源：http://hd.colortex.cn

[Q69] 查看执行计划
来源：http://sx.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jq.hahajie.cn

[Q70] 更新统计信息
来源：http://me.shtwfgs.cn

ANALYZE TABLE users;
来源：http://ov.521024.cn

[Q71] 查看建表语句
来源：http://fm.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://od.szxytkj.cn

[Q72] 查看索引
来源：http://fe.szxytkj.cn

SHOW INDEX FROM users;
来源：http://dg.lnxyls.cn

[Q73] 查看表状态
来源：http://zq.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nl.lnxyls.cn

[Q74] 强制使用索引
来源：http://ip.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dz.hnjuh.cn

[Q75] 日期格式化
来源：http://iv.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fm.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xm.yuntaijiaju.cn

[Q76] 按天统计
来源：http://rg.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dw.wgjwhj.cn

[Q77] 时间加减
来源：http://th.gzmigu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uz.wgjwhj.cn

[Q78] 当前时间
来源：http://gp.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cd.gzmigu.cn

[Q79] 字符串拼接
来源：http://nl.lnxyls.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ft.wgjwhj.cn

[Q80] 字符串截取
来源：http://qi.hahajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://my.nicolike.cn

[Q81] 字符串替换
来源：http://kg.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wy.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://cb.colortex.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mt.szsharing.cn

[Q83] 大小写转换
来源：http://mf.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://co.shxzukj.cn

[Q84] 去除首尾空格
来源：http://mj.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://mk.colortex.cn

[Q85] 数值取整
来源：http://mx.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vt.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://ff.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ai.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://fd.huixinmuqiang.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yy.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://nz.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xf.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kb.9csxet.cn

[Q89] 判断表是否存在
来源：http://io.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qk.colortex.cn

[Q90] 生成序号列
来源：http://vw.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cq.hahajie.cn

================================================================================
来源：http://yj.nicolike.cn

R. Bash 专题
来源：http://td.shxzukj.cn

================================================================================
来源：http://dr.szsharing.cn

[R01] shebang 与严格模式
来源：http://la.nicolike.cn

#!/usr/bin/env bash
来源：http://tt.nicolike.cn

set -euo pipefail
来源：http://wl.jianghongdianzi.cn

[R02] 变量赋值与使用
来源：http://ac.szxytkj.cn

name="Tom"; echo "$name"
来源：http://ww.haigaiapp.cn

[R03] 只读变量
来源：http://zc.nszjky.cn

readonly PI=3.14
来源：http://tm.szxytkj.cn

[R04] 位置参数
来源：http://lh.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ko.huixinmuqiang.cn

[R05] 参数默认值
来源：http://fr.yuntaijiaju.cn

name="${1:-default}"
来源：http://fv.newstarts.cn

[R06] 判断命令是否存在
来源：http://ph.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://br.nszjky.cn

[R07] if 判断文件
来源：http://iw.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hu.jctech888.com.cn

[R08] 数值比较
来源：http://hv.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://oi.bookmarksfly.cn

[R09] 字符串比较
来源：http://ls.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sl.jianghongdianzi.cn

[R10] 正则匹配
来源：http://ez.521024.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jp.huanxung.cn

[R11] case 多分支
来源：http://cb.shxzukj.cn

case "$1" in
来源：http://sd.asd995.cn

start) echo "启动" ;;
来源：http://bi.asd995.cn

stop)  echo "停止" ;;
来源：http://du.huanxung.cn

*)     echo "未知命令" ;;
来源：http://vu.szsharing.cn

esac
来源：http://su.521024.cn

[R12] for 遍历文件
来源：http://bo.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://bf.gzmigu.cn

[R13] for 计数循环
来源：http://gl.huanxung.cn

for i in {1..10}; do echo "$i"; done
来源：http://id.colortex.cn

[R14] C 风格 for
来源：http://qq.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tg.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://nt.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://as.bookmarksfly.cn

[R16] until 等待条件
来源：http://ne.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://au.nszjky.cn

[R17] 数组定义与取值
来源：http://rh.hahajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oe.asd995.cn

[R18] 遍历数组
来源：http://tn.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cb.huanxung.cn

[R19] 数组长度
来源：http://vm.shxzukj.cn

echo "${#arr[@]}"
来源：http://ru.hnjuh.cn

[R20] 关联数组（字典）
来源：http://yb.huixinmuqiang.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jo.wgjwhj.cn

[R21] 字符串长度
来源：http://lc.wgjwhj.cn

echo "${#s}"
来源：http://xi.huixiangedu.cn

[R22] 截取子串
来源：http://gs.hahajie.cn

echo "${s:0:5}"
来源：http://uo.9csxet.cn

[R23] 字符串替换
来源：http://cy.newstarts.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jz.521024.cn

[R24] 大小写转换
来源：http://ib.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lt.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://lm.lnxyls.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://az.521024.cn

[R26] 命令替换
来源：http://be.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://pt.chemitech.net.cn

[R27] 算术展开
来源：http://na.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://cq.newstarts.cn

[R28] 浮点运算
来源：http://gb.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://wa.muxihuayi.cn

[R29] 定义函数
来源：http://lt.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://um.asd995.cn

[R30] 函数返回状态码
来源：http://cd.shxzskj.cn

f() { return 0; }; f || echo "失败了"
来源：http://hy.newstarts.cn

[R31] 局部变量
来源：http://fm.haigaiapp.cn

f() { local x=1; echo "$x"; }
来源：http://ss.jctech888.com.cn

[R32] 参数个数校验
来源：http://wd.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iw.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://wy.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sn.gzmigu.cn

[R34] 退出时清理
来源：http://vf.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ty.asd995.cn

[R35] 后台执行并等待
来源：http://ba.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://iw.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://nz.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bu.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://ni.shxzskj.cn

files=$(ls -1)
来源：http://pz.lnxyls.cn

[R38] 管道串联
来源：http://xh.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://iy.shtwfgs.cn

[R39] 重定向标准输出与错误
来源：http://jy.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://am.hahajie.cn

[R40] 追加写日志
来源：http://rh.shtwfgs.cn

echo "log" >> out.log
来源：http://fs.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://qc.asd995.cn

cmd >/dev/null 2>&1
来源：http://mm.nszjky.cn

[R42] 输入重定向
来源：http://zz.bjjhwx.cn

wc -l < a.txt
来源：http://tk.bjjhwx.cn

[R43] 按名字查找文件
来源：http://at.nszjky.cn

find . -name "*.log" -type f
来源：http://cc.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://mt.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://yt.huixinmuqiang.cn

[R45] 批量删除
来源：http://ii.huanxung.cn

find . -name "*.tmp" -delete
来源：http://or.521024.cn

[R46] 递归替换文件内容
来源：http://nj.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ln.nicolike.cn

[R47] sed 单行替换
来源：http://pe.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cp.shtwfgs.cn

[R48] awk 取指定列
来源：http://pv.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://oz.colortex.cn

[R49] awk 带条件
来源：http://yf.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dy.jctech888.com.cn

[R50] awk 求和
来源：http://jw.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yv.9csxet.cn

[R51] 排序去重取前几
来源：http://bn.yuexingan06.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qy.hnjuh.cn

[R52] 统计行数
来源：http://tu.bookmarksfly.cn

wc -l a.txt
来源：http://cq.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://ow.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jc.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://jm.muxihuayi.cn

diff a.txt b.txt
来源：http://lo.bookmarksfly.cn

[R55] 压缩与解压
来源：http://tb.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mu.shtwfgs.cn

[R56] 远程拷贝
来源：http://kp.yuexingan06.cn

scp file user@host:/path/
来源：http://rs.colortex.cn

[R57] 远程执行命令
来源：http://pl.hahajie.cn

ssh user@host 'uptime'
来源：http://xv.shxzukj.cn

[R58] 下载文件
来源：http://sq.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bi.nicolike.cn

[R59] 发 POST JSON
来源：http://yg.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kx.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://uf.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bk.shtwfgs.cn

[R61] 磁盘占用
来源：http://ug.hahajie.cn

df -h;  du -sh *
来源：http://ji.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://nr.bookmarksfly.cn

du -ah . | sort -rh | head -10
来源：http://mg.shxzukj.cn

[R63] 内存与进程
来源：http://zo.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://fm.chemitech.net.cn

[R64] 结束进程
来源：http://oi.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://sd.muxihuayi.cn

[R65] 查看端口占用
来源：http://wp.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mn.bjjhwx.cn

[R66] 定时任务
来源：http://yb.gzmigu.cn

crontab -e;  crontab -l
来源：http://ii.nszjky.cn

[R67] 生成随机十六进制串
来源：http://fc.huixinmuqiang.cn

openssl rand -hex 16
来源：http://ky.521024.cn

[R68] 计算文件校验值
来源：http://lx.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gn.yuexingan06.cn

[R69] 生成随机密码
来源：http://ob.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://zu.asd995.cn

[R70] 时间戳与互转
来源：http://ay.nicolike.cn

date +%s;  date -d @1700000000
来源：http://qd.bookmarksfly.cn

[R71] 日期格式化
来源：http://el.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zx.gzmigu.cn

[R72] 等待端口就绪
来源：http://qt.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tq.wgjwhj.cn

[R73] 分割大日志
来源：http://hu.huanxung.cn

split -l 1000 big.log part_
来源：http://dp.shxzskj.cn

[R74] 批量重命名
来源：http://ku.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://io.muxihuayi.cn

[R75] 导出环境变量
来源：http://rh.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://ua.521024.cn

[R76] 使用临时文件
来源：http://xi.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kd.jctech888.com.cn

[R77] 读取用户输入
来源：http://ug.lnxyls.cn

read -rp "请输入: " ans
来源：http://mc.gzmigu.cn

[R78] 交互式菜单
来源：http://gy.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oj.shxzskj.cn

[R79] 解析命令行选项
来源：http://ec.yuexingan06.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fz.9csxet.cn

[R80] 查看脚本执行耗时
来源：http://dc.bookmarksfly.cn

time ./run.sh
来源：http://af.yuntaijiaju.cn

================================================================================
来源：http://qu.muxihuayi.cn

S. C / C++ 专题
来源：http://ec.colortex.cn

================================================================================
来源：http://bn.huixiangedu.cn

[S01] C：Hello World
来源：http://eh.gzmigu.cn

#include <stdio.h>
来源：http://ds.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bj.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://wm.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://rt.lnxyls.cn

[S03] C：读入整数
来源：http://lr.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://eh.muxihuayi.cn

[S04] C：字符串复制
来源：http://ms.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dj.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://dx.szsharing.cn

strlen(s)
来源：http://ns.shtwfgs.cn

[S06] C：字符串比较
来源：http://ss.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://rd.nszjky.cn

[S07] C：数组遍历求和
来源：http://so.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uq.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://ok.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zd.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://up.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nx.muxihuayi.cn

[S10] C：指针与解引用
来源：http://zc.asd995.cn

int *p = &a;  *p = 5;
来源：http://vk.colortex.cn

[S11] C：逐行读文件
来源：http://iz.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://nf.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vp.shtwfgs.cn

fclose(f);
来源：http://mb.jctech888.com.cn

[S12] C：写文件
来源：http://ct.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dl.wgjwhj.cn

[S13] C：宏定义
来源：http://sx.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bv.nicolike.cn

[S14] C：枚举
来源：http://gv.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://fe.yuexingan06.cn

[S15] C：类型转换
来源：http://vk.asd995.cn

(double) a / b
来源：http://fk.lnxyls.cn

[S16] C：位操作置位
来源：http://px.yuntaijiaju.cn

x |= (1 << 3);
来源：http://xd.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://ed.bjjhwx.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pb.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://uc.muxihuayi.cn

int main(int argc, char **argv)
来源：http://bz.lnxyls.cn

[S19] C：快速排序
来源：http://jq.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hn.huixinmuqiang.cn

[S20] C：二分查找
来源：http://ig.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lx.shxzskj.cn

[S21] C：字符类别判断
来源：http://qg.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qg.muxihuayi.cn

[S22] C：字符串转数字
来源：http://dq.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sa.bjjhwx.cn

[S23] C：随机数
来源：http://cp.huixinmuqiang.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fz.szsharing.cn

[S24] C：获取本地时间
来源：http://fd.huanxung.cn


<!-- 参考信息 -->