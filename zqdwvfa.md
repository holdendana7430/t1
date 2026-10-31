代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fa.521024.cn

[Q52] 删除指定行
来源：http://gl.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://vr.yuntaijiaju.cn

[Q53] 按条件删除
来源：http://yw.chemitech.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://za.yuexingan06.cn

[Q54] 清空表
来源：http://oq.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://kx.szsharing.cn

[Q55] 排名（并列占位）
来源：http://jb.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fu.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://sl.szxytkj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ws.nicolike.cn

[Q57] 行号
来源：http://bb.521024.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ly.chemitech.net.cn

[Q58] 累计求和
来源：http://dg.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jr.szxytkj.cn

[Q59] 分组内累计
来源：http://le.gzmigu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bj.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://ez.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mz.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mx.gzmigu.cn

[Q61] 移动平均
来源：http://uf.bjjhwx.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://se.nszjky.cn

[Q62] 分组占比
来源：http://jr.hnjuh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oc.bjjhwx.cn

[Q63] 开启事务
来源：http://bj.9csxet.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uf.shxzskj.cn

[Q64] 提交事务
来源：http://qo.9csxet.cn

COMMIT;
来源：http://uq.asd995.cn

[Q65] 回滚事务
来源：http://lz.chemitech.net.cn

ROLLBACK;
来源：http://ul.9csxet.cn

[Q66] 行锁查询
来源：http://in.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jn.yuexingan06.cn

[Q67] 设置隔离级别
来源：http://nu.gzmigu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cl.nszjky.cn

[Q68] 保存点
来源：http://ce.yuexingan06.cn

SAVEPOINT sp1;
来源：http://gq.yuntaijiaju.cn

ROLLBACK TO sp1;
来源：http://hn.wgjwhj.cn

[Q69] 查看执行计划
来源：http://hk.yuntaijiaju.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zj.bjjhwx.cn

[Q70] 更新统计信息
来源：http://rw.chemitech.net.cn

ANALYZE TABLE users;
来源：http://jk.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://ez.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rs.hnjuh.cn

[Q72] 查看索引
来源：http://wr.asd995.cn

SHOW INDEX FROM users;
来源：http://wn.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://sn.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vj.nicolike.cn

[Q74] 强制使用索引
来源：http://na.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pm.huixiangedu.cn

[Q75] 日期格式化
来源：http://rm.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bp.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iz.gzmigu.cn

[Q76] 按天统计
来源：http://cc.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gs.chemitech.net.cn

[Q77] 时间加减
来源：http://ow.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tb.bjjhwx.cn

[Q78] 当前时间
来源：http://wc.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ee.bjjhwx.cn

[Q79] 字符串拼接
来源：http://pi.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cm.nicolike.cn

[Q80] 字符串截取
来源：http://sx.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gq.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://xa.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mm.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://vp.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sb.bjjhwx.cn

[Q83] 大小写转换
来源：http://mi.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vt.szxytkj.cn

[Q84] 去除首尾空格
来源：http://jd.jianghongdianzi.cn

SELECT TRIM(name) FROM users;
来源：http://wm.shxzskj.cn

[Q85] 数值取整
来源：http://ux.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hh.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://bz.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ye.shxzukj.cn

[Q87] JSON 字段做条件
来源：http://yo.newstarts.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qn.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://yu.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fh.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pj.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://fk.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nf.nicolike.cn

[Q90] 生成序号列
来源：http://zi.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rj.hahajie.cn

================================================================================
来源：http://pj.huixinmuqiang.cn

R. Bash 专题
来源：http://re.asd995.cn

================================================================================
来源：http://ar.szsharing.cn

[R01] shebang 与严格模式
来源：http://mv.szxytkj.cn

#!/usr/bin/env bash
来源：http://ql.shxzskj.cn

set -euo pipefail
来源：http://io.newstarts.cn

[R02] 变量赋值与使用
来源：http://ds.nicolike.cn

name="Tom"; echo "$name"
来源：http://go.asd995.cn

[R03] 只读变量
来源：http://ty.huixiangedu.cn

readonly PI=3.14
来源：http://qb.asd995.cn

[R04] 位置参数
来源：http://xg.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uy.hahajie.cn

[R05] 参数默认值
来源：http://lc.jctech888.com.cn

name="${1:-default}"
来源：http://vv.shxzskj.cn

[R06] 判断命令是否存在
来源：http://et.haigaiapp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lo.lnxyls.cn

[R07] if 判断文件
来源：http://wp.newstarts.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rl.panjiajie.cn

[R08] 数值比较
来源：http://yj.gzmigu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yj.hnjuh.cn

[R09] 字符串比较
来源：http://fr.jctech888.com.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://el.newstarts.cn

[R10] 正则匹配
来源：http://us.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fs.huixiangedu.cn

[R11] case 多分支
来源：http://nt.chemitech.net.cn

case "$1" in
来源：http://pk.yuexingan06.cn

start) echo "启动" ;;
来源：http://cf.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://fo.huanxung.cn

*)     echo "未知命令" ;;
来源：http://kp.shxzukj.cn

esac
来源：http://hp.huixiangedu.cn

[R12] for 遍历文件
来源：http://sd.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://gj.jianghongdianzi.cn

[R13] for 计数循环
来源：http://nn.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://th.bookmarksfly.cn

[R14] C 风格 for
来源：http://vs.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gm.nicolike.cn

[R15] while 逐行读文件
来源：http://oz.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wk.bjjhwx.cn

[R16] until 等待条件
来源：http://gs.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vg.chemitech.net.cn

[R17] 数组定义与取值
来源：http://sn.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tn.gzmigu.cn

[R18] 遍历数组
来源：http://fq.wgjwhj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kj.szxytkj.cn

[R19] 数组长度
来源：http://ce.szxytkj.cn

echo "${#arr[@]}"
来源：http://dm.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://tp.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xk.newstarts.cn

[R21] 字符串长度
来源：http://el.huanxung.cn

echo "${#s}"
来源：http://fd.panjiajie.cn

[R22] 截取子串
来源：http://ys.hahajie.cn

echo "${s:0:5}"
来源：http://wv.panjiajie.cn

[R23] 字符串替换
来源：http://yl.bjjhwx.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ww.huanxung.cn

[R24] 大小写转换
来源：http://sq.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nn.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://tc.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dw.9csxet.cn

[R26] 命令替换
来源：http://pe.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://bo.haigaiapp.cn

[R27] 算术展开
来源：http://pc.wgjwhj.cn

echo $((1 + 2 * 3))
来源：http://tj.521024.cn

[R28] 浮点运算
来源：http://fj.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://mm.521024.cn

[R29] 定义函数
来源：http://vw.haigaiapp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ka.huanxung.cn

[R30] 函数返回状态码
来源：http://xp.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://kv.chemitech.net.cn

[R31] 局部变量
来源：http://wz.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://hh.9csxet.cn

[R32] 参数个数校验
来源：http://jh.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ft.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://oy.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pj.hnjuh.cn

[R34] 退出时清理
来源：http://pa.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fh.colortex.cn

[R35] 后台执行并等待
来源：http://ku.nicolike.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lb.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://ud.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tf.gzmigu.cn

[R37] 把输出赋给变量
来源：http://ym.szxytkj.cn

files=$(ls -1)
来源：http://uw.chemitech.net.cn

[R38] 管道串联
来源：http://kt.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://os.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://hh.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://jr.newstarts.cn

[R40] 追加写日志
来源：http://sk.shxzukj.cn

echo "log" >> out.log
来源：http://uw.panjiajie.cn

[R41] 丢弃输出
来源：http://lm.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://pj.panjiajie.cn

[R42] 输入重定向
来源：http://zi.colortex.cn

wc -l < a.txt
来源：http://ll.bjjhwx.cn

[R43] 按名字查找文件
来源：http://ts.bjjhwx.cn

find . -name "*.log" -type f
来源：http://jj.gzmigu.cn

[R44] 按修改时间查找
来源：http://wd.9csxet.cn

find . -mtime -7 -type f
来源：http://ui.hahajie.cn

[R45] 批量删除
来源：http://wp.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://nn.asd995.cn

[R46] 递归替换文件内容
来源：http://fd.shtwfgs.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mb.jianghongdianzi.cn

[R47] sed 单行替换
来源：http://en.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sn.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://ch.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://av.wgjwhj.cn

[R49] awk 带条件
来源：http://ed.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zw.521024.cn

[R50] awk 求和
来源：http://fv.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jm.9csxet.cn

[R51] 排序去重取前几
来源：http://fl.nszjky.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nd.gzmigu.cn

[R52] 统计行数
来源：http://ry.nszjky.cn

wc -l a.txt
来源：http://iq.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://vx.shxzskj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ia.newstarts.cn

[R54] 比较两个文件
来源：http://mm.nicolike.cn

diff a.txt b.txt
来源：http://ev.wgjwhj.cn

[R55] 压缩与解压
来源：http://if.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ny.huanxung.cn

[R56] 远程拷贝
来源：http://xn.shtwfgs.cn

scp file user@host:/path/
来源：http://hh.shtwfgs.cn

[R57] 远程执行命令
来源：http://au.nszjky.cn

ssh user@host 'uptime'
来源：http://uf.521024.cn

[R58] 下载文件
来源：http://bl.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xf.huixiangedu.cn

[R59] 发 POST JSON
来源：http://ca.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vm.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://gw.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cm.asd995.cn

[R61] 磁盘占用
来源：http://ms.jctech888.com.cn

df -h;  du -sh *
来源：http://mv.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://sa.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://zi.huixiangedu.cn

[R63] 内存与进程
来源：http://bq.colortex.cn

free -h;  ps aux | grep nginx
来源：http://xp.panjiajie.cn

[R64] 结束进程
来源：http://vr.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://yo.haigaiapp.cn

[R65] 查看端口占用
来源：http://xz.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sq.colortex.cn

[R66] 定时任务
来源：http://xd.hahajie.cn

crontab -e;  crontab -l
来源：http://mo.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://hr.nszjky.cn

openssl rand -hex 16
来源：http://dv.nszjky.cn

[R68] 计算文件校验值
来源：http://nn.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qz.gzmigu.cn

[R69] 生成随机密码
来源：http://kg.hahajie.cn

head -c 16 /dev/urandom | base64
来源：http://yw.wgjwhj.cn

[R70] 时间戳与互转
来源：http://si.nicolike.cn

date +%s;  date -d @1700000000
来源：http://aa.521024.cn

[R71] 日期格式化
来源：http://qd.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ud.huanxung.cn

[R72] 等待端口就绪
来源：http://bl.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nf.hahajie.cn

[R73] 分割大日志
来源：http://zr.muxihuayi.cn

split -l 1000 big.log part_
来源：http://ja.shxzukj.cn

[R74] 批量重命名
来源：http://jr.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hg.muxihuayi.cn

[R75] 导出环境变量
来源：http://bs.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://zg.bjjhwx.cn

[R76] 使用临时文件
来源：http://xu.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://es.nszjky.cn

[R77] 读取用户输入
来源：http://hp.chemitech.net.cn

read -rp "请输入: " ans
来源：http://sx.chemitech.net.cn

[R78] 交互式菜单
来源：http://kb.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xe.wgjwhj.cn

[R79] 解析命令行选项
来源：http://qa.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nh.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://rx.jianghongdianzi.cn

time ./run.sh
来源：http://ad.newstarts.cn

================================================================================
来源：http://ia.szxytkj.cn

S. C / C++ 专题
来源：http://xm.huanxung.cn

================================================================================
来源：http://zf.newstarts.cn

[S01] C：Hello World
来源：http://us.nicolike.cn

#include <stdio.h>
来源：http://gk.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tg.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://sn.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://bs.yuexingan06.cn

[S03] C：读入整数
来源：http://ya.asd995.cn

int x; scanf("%d", &x);
来源：http://wm.lnxyls.cn

[S04] C：字符串复制
来源：http://bd.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mg.yuexingan06.cn

[S05] C：字符串长度
来源：http://hp.jianghongdianzi.cn

strlen(s)
来源：http://fm.yuexingan06.cn

[S06] C：字符串比较
来源：http://kq.lnxyls.cn

strcmp(a, b) == 0
来源：http://kx.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://mu.521024.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ak.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://zx.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xa.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://df.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lx.yuexingan06.cn

[S10] C：指针与解引用
来源：http://xz.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://uk.shtwfgs.cn

[S11] C：逐行读文件
来源：http://jm.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://ss.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ok.shxzskj.cn

fclose(f);
来源：http://tf.muxihuayi.cn

[S12] C：写文件
来源：http://ae.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mi.shxzukj.cn

[S13] C：宏定义
来源：http://zs.newstarts.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nl.wgjwhj.cn

[S14] C：枚举
来源：http://cz.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://jj.yuntaijiaju.cn

[S15] C：类型转换
来源：http://fy.colortex.cn

(double) a / b
来源：http://nk.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://kd.newstarts.cn

x |= (1 << 3);
来源：http://wy.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://gj.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ay.jctech888.com.cn

[S18] C：命令行参数
来源：http://bh.bjjhwx.cn

int main(int argc, char **argv)
来源：http://az.shxzukj.cn

[S19] C：快速排序
来源：http://is.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rx.huixinmuqiang.cn

[S20] C：二分查找
来源：http://gy.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://me.shtwfgs.cn

[S21] C：字符类别判断
来源：http://oy.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://le.lnxyls.cn

[S22] C：字符串转数字
来源：http://sv.asd995.cn


<!-- 参考信息 -->