代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://no.haigaiapp.cn

[Q54] 清空表
来源：http://im.gzmigu.cn

TRUNCATE TABLE logs;
来源：http://pf.colortex.cn

[Q55] 排名（并列占位）
来源：http://jp.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gd.hnjuh.cn

[Q56] 密集排名（并列不占位）
来源：http://ms.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oo.huixinmuqiang.cn

[Q57] 行号
来源：http://la.muxihuayi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pu.hahajie.cn

[Q58] 累计求和
来源：http://oj.chemitech.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dp.bookmarksfly.cn

[Q59] 分组内累计
来源：http://vk.gzmigu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ki.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://ok.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tb.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sy.newstarts.cn

[Q61] 移动平均
来源：http://ze.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ba.muxihuayi.cn

[Q62] 分组占比
来源：http://qk.521024.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://de.huanxung.cn

[Q63] 开启事务
来源：http://eh.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jp.szsharing.cn

[Q64] 提交事务
来源：http://vw.huixinmuqiang.cn

COMMIT;
来源：http://wm.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://gq.huixinmuqiang.cn

ROLLBACK;
来源：http://cb.colortex.cn

[Q66] 行锁查询
来源：http://ti.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cz.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://gc.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pe.yuexingan06.cn

[Q68] 保存点
来源：http://ax.szxytkj.cn

SAVEPOINT sp1;
来源：http://nb.shxzukj.cn

ROLLBACK TO sp1;
来源：http://gz.panjiajie.cn

[Q69] 查看执行计划
来源：http://jv.yuntaijiaju.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://is.szsharing.cn

[Q70] 更新统计信息
来源：http://lp.muxihuayi.cn

ANALYZE TABLE users;
来源：http://qu.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://pq.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wj.szsharing.cn

[Q72] 查看索引
来源：http://zl.colortex.cn

SHOW INDEX FROM users;
来源：http://vq.hnjuh.cn

[Q73] 查看表状态
来源：http://by.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://as.asd995.cn

[Q74] 强制使用索引
来源：http://dr.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ev.shxzskj.cn

[Q75] 日期格式化
来源：http://oi.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bd.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bz.nszjky.cn

[Q76] 按天统计
来源：http://ji.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tx.szxytkj.cn

[Q77] 时间加减
来源：http://jk.huixinmuqiang.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mf.9csxet.cn

[Q78] 当前时间
来源：http://jo.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sy.521024.cn

[Q79] 字符串拼接
来源：http://ni.jctech888.com.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nl.muxihuayi.cn

[Q80] 字符串截取
来源：http://gk.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://je.shtwfgs.cn

[Q81] 字符串替换
来源：http://lk.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tm.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://gz.shxzukj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fi.yuexingan06.cn

[Q83] 大小写转换
来源：http://jk.gzmigu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://il.huixinmuqiang.cn

[Q84] 去除首尾空格
来源：http://cz.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://xj.lnxyls.cn

[Q85] 数值取整
来源：http://as.nicolike.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zp.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://la.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pi.9csxet.cn

[Q87] JSON 字段做条件
来源：http://vf.huixinmuqiang.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wh.nicolike.cn

[Q88] 行转列（条件聚合）
来源：http://zh.asd995.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nt.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wm.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://cu.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bz.jctech888.com.cn

[Q90] 生成序号列
来源：http://mc.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://re.521024.cn

================================================================================
来源：http://nn.gzmigu.cn

R. Bash 专题
来源：http://mv.szxytkj.cn

================================================================================
来源：http://pm.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://so.9csxet.cn

#!/usr/bin/env bash
来源：http://lg.szxytkj.cn

set -euo pipefail
来源：http://lm.hahajie.cn

[R02] 变量赋值与使用
来源：http://ey.521024.cn

name="Tom"; echo "$name"
来源：http://ag.jianghongdianzi.cn

[R03] 只读变量
来源：http://sf.szxytkj.cn

readonly PI=3.14
来源：http://ug.hahajie.cn

[R04] 位置参数
来源：http://kw.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://de.shtwfgs.cn

[R05] 参数默认值
来源：http://rm.muxihuayi.cn

name="${1:-default}"
来源：http://xf.panjiajie.cn

[R06] 判断命令是否存在
来源：http://ux.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hu.bjjhwx.cn

[R07] if 判断文件
来源：http://rg.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pg.shxzukj.cn

[R08] 数值比较
来源：http://fu.gzmigu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wd.huixinmuqiang.cn

[R09] 字符串比较
来源：http://nz.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vf.panjiajie.cn

[R10] 正则匹配
来源：http://fh.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pj.lnxyls.cn

[R11] case 多分支
来源：http://wx.colortex.cn

case "$1" in
来源：http://xz.huanxung.cn

start) echo "启动" ;;
来源：http://rx.szxytkj.cn

stop)  echo "停止" ;;
来源：http://bm.wgjwhj.cn

*)     echo "未知命令" ;;
来源：http://ef.hnjuh.cn

esac
来源：http://eb.haigaiapp.cn

[R12] for 遍历文件
来源：http://ce.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://yy.huixinmuqiang.cn

[R13] for 计数循环
来源：http://ga.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://eo.9csxet.cn

[R14] C 风格 for
来源：http://az.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hu.haigaiapp.cn

[R15] while 逐行读文件
来源：http://jc.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ia.asd995.cn

[R16] until 等待条件
来源：http://nk.haigaiapp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hv.gzmigu.cn

[R17] 数组定义与取值
来源：http://ox.bookmarksfly.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qq.9csxet.cn

[R18] 遍历数组
来源：http://tr.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ho.newstarts.cn

[R19] 数组长度
来源：http://nx.shxzskj.cn

echo "${#arr[@]}"
来源：http://zx.hahajie.cn

[R20] 关联数组（字典）
来源：http://em.bookmarksfly.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gn.nicolike.cn

[R21] 字符串长度
来源：http://qv.shxzukj.cn

echo "${#s}"
来源：http://ot.shxzukj.cn

[R22] 截取子串
来源：http://tn.colortex.cn

echo "${s:0:5}"
来源：http://uq.yuntaijiaju.cn

[R23] 字符串替换
来源：http://yg.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bp.gzmigu.cn

[R24] 大小写转换
来源：http://lk.521024.cn

echo "${s^^}"; echo "${s,,}"
来源：http://da.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://ih.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ck.asd995.cn

[R26] 命令替换
来源：http://yw.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://wz.shxzskj.cn

[R27] 算术展开
来源：http://gc.huanxung.cn

echo $((1 + 2 * 3))
来源：http://fl.colortex.cn

[R28] 浮点运算
来源：http://ao.asd995.cn

echo "scale=2; 10/3" | bc
来源：http://qm.shtwfgs.cn

[R29] 定义函数
来源：http://gs.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://of.huixiangedu.cn

[R30] 函数返回状态码
来源：http://el.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://wk.haigaiapp.cn

[R31] 局部变量
来源：http://mx.nszjky.cn

f() { local x=1; echo "$x"; }
来源：http://jm.9csxet.cn

[R32] 参数个数校验
来源：http://tv.szxytkj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ls.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://yp.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pf.huanxung.cn

[R34] 退出时清理
来源：http://jq.yuntaijiaju.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mn.9csxet.cn

[R35] 后台执行并等待
来源：http://lq.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rh.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://am.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wv.szxytkj.cn

[R37] 把输出赋给变量
来源：http://qe.shxzukj.cn

files=$(ls -1)
来源：http://rd.szsharing.cn

[R38] 管道串联
来源：http://lv.szxytkj.cn

cat a.txt | grep -i error | wc -l
来源：http://nr.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://rb.gzmigu.cn

cmd > out.log 2>&1
来源：http://so.nszjky.cn

[R40] 追加写日志
来源：http://qp.jianghongdianzi.cn

echo "log" >> out.log
来源：http://kd.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://wd.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://bk.asd995.cn

[R42] 输入重定向
来源：http://ek.gzmigu.cn

wc -l < a.txt
来源：http://ms.szsharing.cn

[R43] 按名字查找文件
来源：http://qo.chemitech.net.cn

find . -name "*.log" -type f
来源：http://ji.asd995.cn

[R44] 按修改时间查找
来源：http://sb.nszjky.cn

find . -mtime -7 -type f
来源：http://us.bookmarksfly.cn

[R45] 批量删除
来源：http://yo.jianghongdianzi.cn

find . -name "*.tmp" -delete
来源：http://zq.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://jw.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xr.jianghongdianzi.cn

[R47] sed 单行替换
来源：http://gu.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zg.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://au.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://os.newstarts.cn

[R49] awk 带条件
来源：http://xo.muxihuayi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rh.szxytkj.cn

[R50] awk 求和
来源：http://hi.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dv.nszjky.cn

[R51] 排序去重取前几
来源：http://aq.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ld.shxzskj.cn

[R52] 统计行数
来源：http://ry.haigaiapp.cn

wc -l a.txt
来源：http://ae.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://ud.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gf.bookmarksfly.cn

[R54] 比较两个文件
来源：http://dg.bjjhwx.cn

diff a.txt b.txt
来源：http://xn.bookmarksfly.cn

[R55] 压缩与解压
来源：http://nb.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pj.yuexingan06.cn

[R56] 远程拷贝
来源：http://dm.hahajie.cn

scp file user@host:/path/
来源：http://fi.nicolike.cn

[R57] 远程执行命令
来源：http://dr.nicolike.cn

ssh user@host 'uptime'
来源：http://te.shxzukj.cn

[R58] 下载文件
来源：http://gc.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yc.jctech888.com.cn

[R59] 发 POST JSON
来源：http://ek.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kq.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://nf.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://md.szxytkj.cn

[R61] 磁盘占用
来源：http://lu.muxihuayi.cn

df -h;  du -sh *
来源：http://ib.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://lq.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://fw.szxytkj.cn

[R63] 内存与进程
来源：http://de.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://dz.shxzskj.cn

[R64] 结束进程
来源：http://xe.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://wm.asd995.cn

[R65] 查看端口占用
来源：http://gp.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pg.panjiajie.cn

[R66] 定时任务
来源：http://rm.nicolike.cn

crontab -e;  crontab -l
来源：http://em.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://ua.chemitech.net.cn

openssl rand -hex 16
来源：http://ky.shxzskj.cn

[R68] 计算文件校验值
来源：http://yb.hnjuh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://un.shtwfgs.cn

[R69] 生成随机密码
来源：http://fy.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://nt.chemitech.net.cn

[R70] 时间戳与互转
来源：http://gv.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://em.huixiangedu.cn

[R71] 日期格式化
来源：http://cl.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://be.muxihuayi.cn

[R72] 等待端口就绪
来源：http://ym.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://az.muxihuayi.cn

[R73] 分割大日志
来源：http://uh.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://ra.jctech888.com.cn

[R74] 批量重命名
来源：http://nr.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ee.bookmarksfly.cn

[R75] 导出环境变量
来源：http://en.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://hd.lnxyls.cn

[R76] 使用临时文件
来源：http://ly.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rk.chemitech.net.cn

[R77] 读取用户输入
来源：http://jb.bjjhwx.cn

read -rp "请输入: " ans
来源：http://va.nicolike.cn

[R78] 交互式菜单
来源：http://na.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lf.yuexingan06.cn

[R79] 解析命令行选项
来源：http://vd.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pq.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://yc.521024.cn

time ./run.sh
来源：http://rp.shxzukj.cn

================================================================================
来源：http://oa.hahajie.cn

S. C / C++ 专题
来源：http://yw.huixinmuqiang.cn

================================================================================
来源：http://sp.nicolike.cn

[S01] C：Hello World
来源：http://zz.hahajie.cn

#include <stdio.h>
来源：http://al.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://io.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://cn.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://gx.nicolike.cn

[S03] C：读入整数
来源：http://pf.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://rp.gzmigu.cn

[S04] C：字符串复制
来源：http://fm.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ql.asd995.cn

[S05] C：字符串长度
来源：http://iw.huixiangedu.cn

strlen(s)
来源：http://kr.nicolike.cn

[S06] C：字符串比较
来源：http://io.shxzskj.cn

strcmp(a, b) == 0
来源：http://pa.huanxung.cn

[S07] C：数组遍历求和
来源：http://ae.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://te.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://mx.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nr.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://ej.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dz.gzmigu.cn

[S10] C：指针与解引用
来源：http://qe.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://dr.nicolike.cn

[S11] C：逐行读文件
来源：http://hu.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://ry.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ti.jianghongdianzi.cn

fclose(f);
来源：http://nl.jianghongdianzi.cn

[S12] C：写文件
来源：http://yr.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ja.jianghongdianzi.cn

[S13] C：宏定义
来源：http://fp.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eq.yuexingan06.cn

[S14] C：枚举
来源：http://ff.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://hm.521024.cn

[S15] C：类型转换
来源：http://ro.yuexingan06.cn

(double) a / b
来源：http://fp.lnxyls.cn

[S16] C：位操作置位
来源：http://xl.bjjhwx.cn

x |= (1 << 3);
来源：http://vt.asd995.cn

[S17] C：安全拼接字符串
来源：http://zy.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zq.colortex.cn

[S18] C：命令行参数
来源：http://nk.shtwfgs.cn

int main(int argc, char **argv)
来源：http://js.yuexingan06.cn

[S19] C：快速排序
来源：http://vn.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ou.newstarts.cn

[S20] C：二分查找
来源：http://vo.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://td.shxzskj.cn

[S21] C：字符类别判断
来源：http://fj.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gg.521024.cn

[S22] C：字符串转数字
来源：http://tt.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gw.haigaiapp.cn

[S23] C：随机数
来源：http://nd.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rv.newstarts.cn

[S24] C：获取本地时间
来源：http://gr.hahajie.cn


<!-- 参考信息 -->