代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ad.colortex.cn

[Q52] 删除指定行
来源：http://qg.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://ep.wgjwhj.cn

[Q53] 按条件删除
来源：http://mp.gzmigu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qn.huixiangedu.cn

[Q54] 清空表
来源：http://ov.jctech888.com.cn

TRUNCATE TABLE logs;
来源：http://ay.bookmarksfly.cn

[Q55] 排名（并列占位）
来源：http://zn.shxzskj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ul.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://sa.haigaiapp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://aa.jianghongdianzi.cn

[Q57] 行号
来源：http://oo.bjjhwx.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pr.panjiajie.cn

[Q58] 累计求和
来源：http://pf.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tj.jianghongdianzi.cn

[Q59] 分组内累计
来源：http://up.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ld.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://tf.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sd.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sq.yuntaijiaju.cn

[Q61] 移动平均
来源：http://wk.shtwfgs.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eg.shxzukj.cn

[Q62] 分组占比
来源：http://fy.shtwfgs.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gk.wgjwhj.cn

[Q63] 开启事务
来源：http://xq.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oy.asd995.cn

[Q64] 提交事务
来源：http://hq.wgjwhj.cn

COMMIT;
来源：http://xq.521024.cn

[Q65] 回滚事务
来源：http://tz.asd995.cn

ROLLBACK;
来源：http://fp.colortex.cn

[Q66] 行锁查询
来源：http://mg.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sf.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://dv.szsharing.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vx.chemitech.net.cn

[Q68] 保存点
来源：http://uc.shxzskj.cn

SAVEPOINT sp1;
来源：http://xx.shxzskj.cn

ROLLBACK TO sp1;
来源：http://xi.9csxet.cn

[Q69] 查看执行计划
来源：http://rw.lnxyls.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qj.panjiajie.cn

[Q70] 更新统计信息
来源：http://qi.521024.cn

ANALYZE TABLE users;
来源：http://vh.gzmigu.cn

[Q71] 查看建表语句
来源：http://vx.szxytkj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ou.szxytkj.cn

[Q72] 查看索引
来源：http://tn.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://cc.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://cn.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kd.shxzukj.cn

[Q74] 强制使用索引
来源：http://vb.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lb.nicolike.cn

[Q75] 日期格式化
来源：http://kh.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tr.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lu.gzmigu.cn

[Q76] 按天统计
来源：http://qm.nszjky.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ma.huanxung.cn

[Q77] 时间加减
来源：http://fn.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ar.jctech888.com.cn

[Q78] 当前时间
来源：http://wt.huixinmuqiang.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ni.muxihuayi.cn

[Q79] 字符串拼接
来源：http://ny.huanxung.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://np.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://oa.panjiajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kh.yuexingan06.cn

[Q81] 字符串替换
来源：http://ig.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yo.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://rw.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oa.chemitech.net.cn

[Q83] 大小写转换
来源：http://su.huanxung.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xs.panjiajie.cn

[Q84] 去除首尾空格
来源：http://hr.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://aq.jianghongdianzi.cn

[Q85] 数值取整
来源：http://th.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mu.newstarts.cn

[Q86] 读取 JSON 字段
来源：http://zo.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ul.chemitech.net.cn

[Q87] JSON 字段做条件
来源：http://le.wgjwhj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://us.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://ed.huixinmuqiang.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://it.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xt.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://an.yuexingan06.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://br.bookmarksfly.cn

[Q90] 生成序号列
来源：http://po.yuntaijiaju.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bb.shxzskj.cn

================================================================================
来源：http://ys.chemitech.net.cn

R. Bash 专题
来源：http://tv.wgjwhj.cn

================================================================================
来源：http://tq.hnjuh.cn

[R01] shebang 与严格模式
来源：http://qs.yuexingan06.cn

#!/usr/bin/env bash
来源：http://tx.yuexingan06.cn

set -euo pipefail
来源：http://hh.szsharing.cn

[R02] 变量赋值与使用
来源：http://bd.szsharing.cn

name="Tom"; echo "$name"
来源：http://nc.lnxyls.cn

[R03] 只读变量
来源：http://jd.szxytkj.cn

readonly PI=3.14
来源：http://rg.shxzukj.cn

[R04] 位置参数
来源：http://yy.panjiajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kd.shxzukj.cn

[R05] 参数默认值
来源：http://wv.jianghongdianzi.cn

name="${1:-default}"
来源：http://sk.huixinmuqiang.cn

[R06] 判断命令是否存在
来源：http://dv.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ju.521024.cn

[R07] if 判断文件
来源：http://tg.521024.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vc.wgjwhj.cn

[R08] 数值比较
来源：http://ne.jianghongdianzi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xg.szxytkj.cn

[R09] 字符串比较
来源：http://wg.chemitech.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qp.jianghongdianzi.cn

[R10] 正则匹配
来源：http://ll.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sq.lnxyls.cn

[R11] case 多分支
来源：http://iv.hnjuh.cn

case "$1" in
来源：http://rw.shxzukj.cn

start) echo "启动" ;;
来源：http://lc.nszjky.cn

stop)  echo "停止" ;;
来源：http://hl.hnjuh.cn

*)     echo "未知命令" ;;
来源：http://os.chemitech.net.cn

esac
来源：http://js.nicolike.cn

[R12] for 遍历文件
来源：http://bt.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://hh.gzmigu.cn

[R13] for 计数循环
来源：http://dj.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://tt.bjjhwx.cn

[R14] C 风格 for
来源：http://wu.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xv.bjjhwx.cn

[R15] while 逐行读文件
来源：http://nx.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lw.szsharing.cn

[R16] until 等待条件
来源：http://bm.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://to.wgjwhj.cn

[R17] 数组定义与取值
来源：http://sf.bjjhwx.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yp.asd995.cn

[R18] 遍历数组
来源：http://no.nicolike.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wc.wgjwhj.cn

[R19] 数组长度
来源：http://ot.lnxyls.cn

echo "${#arr[@]}"
来源：http://xu.gzmigu.cn

[R20] 关联数组（字典）
来源：http://pe.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cs.asd995.cn

[R21] 字符串长度
来源：http://xt.jianghongdianzi.cn

echo "${#s}"
来源：http://vg.nicolike.cn

[R22] 截取子串
来源：http://cw.yuexingan06.cn

echo "${s:0:5}"
来源：http://vp.panjiajie.cn

[R23] 字符串替换
来源：http://zb.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xz.521024.cn

[R24] 大小写转换
来源：http://jm.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tn.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://ta.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fe.szsharing.cn

[R26] 命令替换
来源：http://dc.521024.cn

now=$(date +%F); echo "$now"
来源：http://af.huanxung.cn

[R27] 算术展开
来源：http://wd.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://xb.shxzukj.cn

[R28] 浮点运算
来源：http://nj.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://ie.muxihuayi.cn

[R29] 定义函数
来源：http://rp.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zy.huanxung.cn

[R30] 函数返回状态码
来源：http://if.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://zh.lnxyls.cn

[R31] 局部变量
来源：http://pv.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://ni.szxytkj.cn

[R32] 参数个数校验
来源：http://vz.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://no.asd995.cn

[R33] 捕获错误并提示行号
来源：http://wy.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qh.jianghongdianzi.cn

[R34] 退出时清理
来源：http://mv.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://en.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://ks.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kf.shxzskj.cn

[R36] 并发执行多个任务
来源：http://lw.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yt.newstarts.cn

[R37] 把输出赋给变量
来源：http://ru.panjiajie.cn

files=$(ls -1)
来源：http://rk.gzmigu.cn

[R38] 管道串联
来源：http://ax.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://dg.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://yl.hnjuh.cn

cmd > out.log 2>&1
来源：http://ja.szsharing.cn

[R40] 追加写日志
来源：http://pq.9csxet.cn

echo "log" >> out.log
来源：http://lx.9csxet.cn

[R41] 丢弃输出
来源：http://yz.nszjky.cn

cmd >/dev/null 2>&1
来源：http://um.shxzskj.cn

[R42] 输入重定向
来源：http://lz.shtwfgs.cn

wc -l < a.txt
来源：http://yr.shxzskj.cn

[R43] 按名字查找文件
来源：http://kz.huixiangedu.cn

find . -name "*.log" -type f
来源：http://cp.shxzukj.cn

[R44] 按修改时间查找
来源：http://pb.chemitech.net.cn

find . -mtime -7 -type f
来源：http://mk.haigaiapp.cn

[R45] 批量删除
来源：http://vu.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://sb.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://ab.hnjuh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zv.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://fx.shxzskj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dn.jctech888.com.cn

[R48] awk 取指定列
来源：http://vg.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://eh.lnxyls.cn

[R49] awk 带条件
来源：http://ja.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lv.521024.cn

[R50] awk 求和
来源：http://wk.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jf.huixiangedu.cn

[R51] 排序去重取前几
来源：http://zt.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sc.newstarts.cn

[R52] 统计行数
来源：http://ur.shxzskj.cn

wc -l a.txt
来源：http://bz.521024.cn

[R53] 查看文件头与实时尾
来源：http://nb.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tq.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://zv.gzmigu.cn

diff a.txt b.txt
来源：http://cb.haigaiapp.cn

[R55] 压缩与解压
来源：http://ur.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ri.hahajie.cn

[R56] 远程拷贝
来源：http://dg.bookmarksfly.cn

scp file user@host:/path/
来源：http://ae.shxzukj.cn

[R57] 远程执行命令
来源：http://vo.szsharing.cn

ssh user@host 'uptime'
来源：http://wy.wgjwhj.cn

[R58] 下载文件
来源：http://ca.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://it.hahajie.cn

[R59] 发 POST JSON
来源：http://qb.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://is.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://zs.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fd.hnjuh.cn

[R61] 磁盘占用
来源：http://hp.521024.cn

df -h;  du -sh *
来源：http://ec.muxihuayi.cn

[R62] 找最占空间的文件
来源：http://nk.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://wy.panjiajie.cn

[R63] 内存与进程
来源：http://bq.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://hj.nszjky.cn

[R64] 结束进程
来源：http://lc.muxihuayi.cn

kill -9 $(pgrep -f app.py)
来源：http://sq.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://dp.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xg.haigaiapp.cn

[R66] 定时任务
来源：http://fv.colortex.cn

crontab -e;  crontab -l
来源：http://cx.newstarts.cn

[R67] 生成随机十六进制串
来源：http://az.chemitech.net.cn

openssl rand -hex 16
来源：http://jh.huanxung.cn

[R68] 计算文件校验值
来源：http://sx.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rd.gzmigu.cn

[R69] 生成随机密码
来源：http://as.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://tz.9csxet.cn

[R70] 时间戳与互转
来源：http://kz.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://vy.jianghongdianzi.cn

[R71] 日期格式化
来源：http://pn.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zd.asd995.cn

[R72] 等待端口就绪
来源：http://ky.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://aq.gzmigu.cn

[R73] 分割大日志
来源：http://rn.jctech888.com.cn

split -l 1000 big.log part_
来源：http://vm.huixiangedu.cn

[R74] 批量重命名
来源：http://yx.nszjky.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wd.haigaiapp.cn

[R75] 导出环境变量
来源：http://at.szsharing.cn

export PATH="$HOME/bin:$PATH"
来源：http://ug.chemitech.net.cn

[R76] 使用临时文件
来源：http://ai.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ld.haigaiapp.cn

[R77] 读取用户输入
来源：http://db.asd995.cn

read -rp "请输入: " ans
来源：http://do.521024.cn

[R78] 交互式菜单
来源：http://xy.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ky.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://mm.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pf.asd995.cn

[R80] 查看脚本执行耗时
来源：http://tl.huixinmuqiang.cn

time ./run.sh
来源：http://pb.hahajie.cn

================================================================================
来源：http://fa.panjiajie.cn

S. C / C++ 专题
来源：http://ao.gzmigu.cn

================================================================================
来源：http://zu.haigaiapp.cn

[S01] C：Hello World
来源：http://ks.521024.cn

#include <stdio.h>
来源：http://be.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xb.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://jz.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://jm.huanxung.cn

[S03] C：读入整数
来源：http://kj.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://hu.asd995.cn

[S04] C：字符串复制
来源：http://sc.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nb.huanxung.cn

[S05] C：字符串长度
来源：http://tu.9csxet.cn

strlen(s)
来源：http://jw.yuexingan06.cn

[S06] C：字符串比较
来源：http://ru.nszjky.cn

strcmp(a, b) == 0
来源：http://tk.nszjky.cn

[S07] C：数组遍历求和
来源：http://ad.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ak.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://bx.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://co.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://ef.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sk.bjjhwx.cn

[S10] C：指针与解引用
来源：http://xl.huanxung.cn

int *p = &a;  *p = 5;
来源：http://up.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://xp.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://yw.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jf.jctech888.com.cn

fclose(f);
来源：http://nd.gzmigu.cn

[S12] C：写文件
来源：http://xe.lnxyls.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jr.huixiangedu.cn

[S13] C：宏定义
来源：http://sn.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hx.jianghongdianzi.cn

[S14] C：枚举
来源：http://kk.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://jf.huixiangedu.cn

[S15] C：类型转换
来源：http://dy.bjjhwx.cn

(double) a / b
来源：http://is.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://gc.yuexingan06.cn

x |= (1 << 3);
来源：http://em.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://mm.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hv.newstarts.cn

[S18] C：命令行参数
来源：http://dg.panjiajie.cn

int main(int argc, char **argv)
来源：http://ut.szsharing.cn

[S19] C：快速排序
来源：http://uq.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pf.chemitech.net.cn

[S20] C：二分查找
来源：http://xv.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jx.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://kg.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zb.colortex.cn

[S22] C：字符串转数字
来源：http://xr.panjiajie.cn


<!-- 参考信息 -->