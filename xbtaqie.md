代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qo.gzmigu.cn

[Q54] 清空表
来源：http://jp.newstarts.cn

TRUNCATE TABLE logs;
来源：http://ol.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://dz.nszjky.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hn.haigaiapp.cn

[Q56] 密集排名（并列不占位）
来源：http://em.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jr.jctech888.com.cn

[Q57] 行号
来源：http://qz.asd995.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jr.lnxyls.cn

[Q58] 累计求和
来源：http://pt.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nj.lnxyls.cn

[Q59] 分组内累计
来源：http://ne.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cw.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://ke.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ga.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xa.szsharing.cn

[Q61] 移动平均
来源：http://bh.szxytkj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xw.lnxyls.cn

[Q62] 分组占比
来源：http://hc.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fc.shxzukj.cn

[Q63] 开启事务
来源：http://jv.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lw.521024.cn

[Q64] 提交事务
来源：http://df.bookmarksfly.cn

COMMIT;
来源：http://pr.hahajie.cn

[Q65] 回滚事务
来源：http://dg.shxzskj.cn

ROLLBACK;
来源：http://th.hahajie.cn

[Q66] 行锁查询
来源：http://ku.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://al.huanxung.cn

[Q67] 设置隔离级别
来源：http://ee.huixinmuqiang.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bg.newstarts.cn

[Q68] 保存点
来源：http://tm.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://xr.muxihuayi.cn

ROLLBACK TO sp1;
来源：http://fp.yuntaijiaju.cn

[Q69] 查看执行计划
来源：http://aj.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ms.shtwfgs.cn

[Q70] 更新统计信息
来源：http://bt.asd995.cn

ANALYZE TABLE users;
来源：http://vr.hnjuh.cn

[Q71] 查看建表语句
来源：http://es.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rg.chemitech.net.cn

[Q72] 查看索引
来源：http://sn.nicolike.cn

SHOW INDEX FROM users;
来源：http://ik.yuexingan06.cn

[Q73] 查看表状态
来源：http://hh.hnjuh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ad.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://px.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zi.hnjuh.cn

[Q75] 日期格式化
来源：http://ke.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://aj.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kk.haigaiapp.cn

[Q76] 按天统计
来源：http://qv.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vu.haigaiapp.cn

[Q77] 时间加减
来源：http://yu.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mb.wgjwhj.cn

[Q78] 当前时间
来源：http://ax.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ee.chemitech.net.cn

[Q79] 字符串拼接
来源：http://lx.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nw.shtwfgs.cn

[Q80] 字符串截取
来源：http://vy.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://os.gzmigu.cn

[Q81] 字符串替换
来源：http://hg.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qh.jianghongdianzi.cn

[Q82] 字符长度与字节长度
来源：http://ks.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gr.huanxung.cn

[Q83] 大小写转换
来源：http://tq.yuntaijiaju.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://is.szxytkj.cn

[Q84] 去除首尾空格
来源：http://yu.bookmarksfly.cn

SELECT TRIM(name) FROM users;
来源：http://kt.shxzskj.cn

[Q85] 数值取整
来源：http://kt.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ef.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://pe.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rd.colortex.cn

[Q87] JSON 字段做条件
来源：http://lk.nszjky.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ws.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://yl.521024.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sb.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uo.huixinmuqiang.cn

[Q89] 判断表是否存在
来源：http://ui.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lb.colortex.cn

[Q90] 生成序号列
来源：http://ok.szsharing.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jb.hahajie.cn

================================================================================
来源：http://cw.jianghongdianzi.cn

R. Bash 专题
来源：http://ez.newstarts.cn

================================================================================
来源：http://hi.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://px.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://ub.gzmigu.cn

set -euo pipefail
来源：http://gw.asd995.cn

[R02] 变量赋值与使用
来源：http://lk.nszjky.cn

name="Tom"; echo "$name"
来源：http://wm.huixinmuqiang.cn

[R03] 只读变量
来源：http://iv.huixiangedu.cn

readonly PI=3.14
来源：http://mp.jianghongdianzi.cn

[R04] 位置参数
来源：http://sf.hnjuh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oj.lnxyls.cn

[R05] 参数默认值
来源：http://rc.9csxet.cn

name="${1:-default}"
来源：http://ee.hnjuh.cn

[R06] 判断命令是否存在
来源：http://bh.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bg.huanxung.cn

[R07] if 判断文件
来源：http://pi.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gc.nszjky.cn

[R08] 数值比较
来源：http://zm.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://op.jctech888.com.cn

[R09] 字符串比较
来源：http://sm.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jg.wgjwhj.cn

[R10] 正则匹配
来源：http://bc.yuntaijiaju.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rs.colortex.cn

[R11] case 多分支
来源：http://rh.nszjky.cn

case "$1" in
来源：http://ug.9csxet.cn

start) echo "启动" ;;
来源：http://db.lnxyls.cn

stop)  echo "停止" ;;
来源：http://rp.szsharing.cn

*)     echo "未知命令" ;;
来源：http://cd.shtwfgs.cn

esac
来源：http://ch.huanxung.cn

[R12] for 遍历文件
来源：http://nr.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://mi.shxzskj.cn

[R13] for 计数循环
来源：http://lf.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://cb.gzmigu.cn

[R14] C 风格 for
来源：http://ok.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mn.haigaiapp.cn

[R15] while 逐行读文件
来源：http://jk.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://iq.bjjhwx.cn

[R16] until 等待条件
来源：http://zu.yuexingan06.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://he.yuntaijiaju.cn

[R17] 数组定义与取值
来源：http://cv.bookmarksfly.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ir.szsharing.cn

[R18] 遍历数组
来源：http://vk.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ma.huixiangedu.cn

[R19] 数组长度
来源：http://fq.huanxung.cn

echo "${#arr[@]}"
来源：http://fu.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://lk.9csxet.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gl.yuexingan06.cn

[R21] 字符串长度
来源：http://gm.huixiangedu.cn

echo "${#s}"
来源：http://rn.wgjwhj.cn

[R22] 截取子串
来源：http://jj.9csxet.cn

echo "${s:0:5}"
来源：http://ub.hnjuh.cn

[R23] 字符串替换
来源：http://jy.asd995.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://px.chemitech.net.cn

[R24] 大小写转换
来源：http://wq.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fa.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://vz.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wo.yuntaijiaju.cn

[R26] 命令替换
来源：http://ij.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://sj.chemitech.net.cn

[R27] 算术展开
来源：http://lt.colortex.cn

echo $((1 + 2 * 3))
来源：http://kp.bjjhwx.cn

[R28] 浮点运算
来源：http://pv.colortex.cn

echo "scale=2; 10/3" | bc
来源：http://yy.szsharing.cn

[R29] 定义函数
来源：http://he.bjjhwx.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mw.lnxyls.cn

[R30] 函数返回状态码
来源：http://gc.lnxyls.cn

f() { return 0; }; f || echo "失败了"
来源：http://ox.gzmigu.cn

[R31] 局部变量
来源：http://kh.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://gp.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://jj.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gi.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://du.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cr.521024.cn

[R34] 退出时清理
来源：http://pj.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sj.hnjuh.cn

[R35] 后台执行并等待
来源：http://rr.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vq.colortex.cn

[R36] 并发执行多个任务
来源：http://lr.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qx.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://uh.chemitech.net.cn

files=$(ls -1)
来源：http://gh.bjjhwx.cn

[R38] 管道串联
来源：http://su.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://an.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://hb.nszjky.cn

cmd > out.log 2>&1
来源：http://oo.jianghongdianzi.cn

[R40] 追加写日志
来源：http://mb.yuntaijiaju.cn

echo "log" >> out.log
来源：http://pm.jctech888.com.cn

[R41] 丢弃输出
来源：http://gs.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://ef.hahajie.cn

[R42] 输入重定向
来源：http://sa.szxytkj.cn

wc -l < a.txt
来源：http://xi.huanxung.cn

[R43] 按名字查找文件
来源：http://md.colortex.cn

find . -name "*.log" -type f
来源：http://dq.nicolike.cn

[R44] 按修改时间查找
来源：http://oa.huixinmuqiang.cn

find . -mtime -7 -type f
来源：http://ky.yuexingan06.cn

[R45] 批量删除
来源：http://jz.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://lx.9csxet.cn

[R46] 递归替换文件内容
来源：http://pr.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://im.wgjwhj.cn

[R47] sed 单行替换
来源：http://ml.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nz.yuexingan06.cn

[R48] awk 取指定列
来源：http://qx.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://cw.lnxyls.cn

[R49] awk 带条件
来源：http://ew.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ib.huanxung.cn

[R50] awk 求和
来源：http://iz.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://iy.lnxyls.cn

[R51] 排序去重取前几
来源：http://vo.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vo.521024.cn

[R52] 统计行数
来源：http://ji.hahajie.cn

wc -l a.txt
来源：http://jq.huanxung.cn

[R53] 查看文件头与实时尾
来源：http://yb.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dn.bookmarksfly.cn

[R54] 比较两个文件
来源：http://yy.hnjuh.cn

diff a.txt b.txt
来源：http://sm.9csxet.cn

[R55] 压缩与解压
来源：http://bd.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hr.lnxyls.cn

[R56] 远程拷贝
来源：http://xi.gzmigu.cn

scp file user@host:/path/
来源：http://cr.jctech888.com.cn

[R57] 远程执行命令
来源：http://jp.lnxyls.cn

ssh user@host 'uptime'
来源：http://nh.nicolike.cn

[R58] 下载文件
来源：http://mj.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://re.newstarts.cn

[R59] 发 POST JSON
来源：http://yp.szxytkj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jy.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://sb.hnjuh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aw.haigaiapp.cn

[R61] 磁盘占用
来源：http://kf.shtwfgs.cn

df -h;  du -sh *
来源：http://vd.521024.cn

[R62] 找最占空间的文件
来源：http://bn.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://yp.colortex.cn

[R63] 内存与进程
来源：http://qh.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://zp.shtwfgs.cn

[R64] 结束进程
来源：http://mi.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://lt.muxihuayi.cn

[R65] 查看端口占用
来源：http://tt.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ge.yuexingan06.cn

[R66] 定时任务
来源：http://nw.hahajie.cn

crontab -e;  crontab -l
来源：http://iq.jctech888.com.cn

[R67] 生成随机十六进制串
来源：http://df.newstarts.cn

openssl rand -hex 16
来源：http://zq.shtwfgs.cn

[R68] 计算文件校验值
来源：http://po.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pu.chemitech.net.cn

[R69] 生成随机密码
来源：http://vb.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://bg.521024.cn

[R70] 时间戳与互转
来源：http://xx.asd995.cn

date +%s;  date -d @1700000000
来源：http://li.haigaiapp.cn

[R71] 日期格式化
来源：http://nl.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yv.muxihuayi.cn

[R72] 等待端口就绪
来源：http://jd.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jz.shxzskj.cn

[R73] 分割大日志
来源：http://mw.shxzukj.cn

split -l 1000 big.log part_
来源：http://we.hahajie.cn

[R74] 批量重命名
来源：http://kg.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vk.nicolike.cn

[R75] 导出环境变量
来源：http://jy.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://qk.hnjuh.cn

[R76] 使用临时文件
来源：http://wh.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ai.panjiajie.cn

[R77] 读取用户输入
来源：http://ed.yuntaijiaju.cn

read -rp "请输入: " ans
来源：http://ma.shtwfgs.cn

[R78] 交互式菜单
来源：http://vb.9csxet.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gk.nszjky.cn

[R79] 解析命令行选项
来源：http://cl.wgjwhj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://if.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://fl.panjiajie.cn

time ./run.sh
来源：http://fw.nszjky.cn

================================================================================
来源：http://jx.muxihuayi.cn

S. C / C++ 专题
来源：http://pv.bjjhwx.cn

================================================================================
来源：http://jl.521024.cn

[S01] C：Hello World
来源：http://dh.jianghongdianzi.cn

#include <stdio.h>
来源：http://yf.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://so.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://qw.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://lz.szxytkj.cn

[S03] C：读入整数
来源：http://ay.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://mm.bjjhwx.cn

[S04] C：字符串复制
来源：http://xg.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wq.newstarts.cn

[S05] C：字符串长度
来源：http://ey.haigaiapp.cn

strlen(s)
来源：http://oa.shxzskj.cn

[S06] C：字符串比较
来源：http://bp.haigaiapp.cn

strcmp(a, b) == 0
来源：http://am.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://aa.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://db.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://ih.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vl.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://vd.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ec.newstarts.cn

[S10] C：指针与解引用
来源：http://kj.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://ie.colortex.cn

[S11] C：逐行读文件
来源：http://sm.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://ml.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pk.nicolike.cn

fclose(f);
来源：http://zc.yuntaijiaju.cn

[S12] C：写文件
来源：http://vg.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tm.huanxung.cn

[S13] C：宏定义
来源：http://qv.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qu.asd995.cn

[S14] C：枚举
来源：http://pq.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://as.jianghongdianzi.cn

[S15] C：类型转换
来源：http://yv.muxihuayi.cn

(double) a / b
来源：http://df.szsharing.cn

[S16] C：位操作置位
来源：http://qg.lnxyls.cn

x |= (1 << 3);
来源：http://wk.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://vc.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hg.shxzukj.cn

[S18] C：命令行参数
来源：http://vt.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://mo.chemitech.net.cn

[S19] C：快速排序
来源：http://yg.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iu.shtwfgs.cn

[S20] C：二分查找
来源：http://ic.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ar.chemitech.net.cn

[S21] C：字符类别判断
来源：http://jw.shxzskj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cf.haigaiapp.cn

[S22] C：字符串转数字
来源：http://di.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ns.muxihuayi.cn

[S23] C：随机数
来源：http://fn.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nn.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://qx.muxihuayi.cn


<!-- 参考信息 -->