代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nr.nicolike.cn

[Q54] 清空表
来源：http://xe.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://ff.colortex.cn

[Q55] 排名（并列占位）
来源：http://sd.wgjwhj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pt.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://ol.huixiangedu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yf.huixiangedu.cn

[Q57] 行号
来源：http://tq.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qu.hnjuh.cn

[Q58] 累计求和
来源：http://dy.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rp.shxzukj.cn

[Q59] 分组内累计
来源：http://kg.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jy.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://bk.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qm.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cv.wgjwhj.cn

[Q61] 移动平均
来源：http://xr.gzmigu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ro.szsharing.cn

[Q62] 分组占比
来源：http://mz.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mc.colortex.cn

[Q63] 开启事务
来源：http://rc.jctech888.com.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hy.huanxung.cn

[Q64] 提交事务
来源：http://gu.wgjwhj.cn

COMMIT;
来源：http://ry.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://gw.yuexingan06.cn

ROLLBACK;
来源：http://zg.huixinmuqiang.cn

[Q66] 行锁查询
来源：http://vu.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jl.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://fs.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://op.huixinmuqiang.cn

[Q68] 保存点
来源：http://oe.huixiangedu.cn

SAVEPOINT sp1;
来源：http://ad.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://ma.nszjky.cn

[Q69] 查看执行计划
来源：http://ow.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ki.chemitech.net.cn

[Q70] 更新统计信息
来源：http://qk.huixiangedu.cn

ANALYZE TABLE users;
来源：http://pc.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://hx.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hr.huanxung.cn

[Q72] 查看索引
来源：http://sf.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://nu.huixiangedu.cn

[Q73] 查看表状态
来源：http://bk.newstarts.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xr.nszjky.cn

[Q74] 强制使用索引
来源：http://cr.shtwfgs.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ha.521024.cn

[Q75] 日期格式化
来源：http://pa.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hi.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://at.chemitech.net.cn

[Q76] 按天统计
来源：http://dy.nszjky.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aa.szxytkj.cn

[Q77] 时间加减
来源：http://gq.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cf.bookmarksfly.cn

[Q78] 当前时间
来源：http://ul.huixinmuqiang.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rn.wgjwhj.cn

[Q79] 字符串拼接
来源：http://og.haigaiapp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xl.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://al.gzmigu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wp.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://vg.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xf.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://ov.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rg.wgjwhj.cn

[Q83] 大小写转换
来源：http://wc.yuntaijiaju.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ew.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://rj.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://lx.haigaiapp.cn

[Q85] 数值取整
来源：http://ho.huixinmuqiang.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cw.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://qe.shxzskj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xp.9csxet.cn

[Q87] JSON 字段做条件
来源：http://df.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zs.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://vq.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://md.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oc.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://kg.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zl.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://ds.shxzukj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bs.wgjwhj.cn

================================================================================
来源：http://ys.szxytkj.cn

R. Bash 专题
来源：http://rl.nszjky.cn

================================================================================
来源：http://lq.lnxyls.cn

[R01] shebang 与严格模式
来源：http://wi.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://af.jctech888.com.cn

set -euo pipefail
来源：http://jy.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://zq.nicolike.cn

name="Tom"; echo "$name"
来源：http://cp.huixinmuqiang.cn

[R03] 只读变量
来源：http://ud.wgjwhj.cn

readonly PI=3.14
来源：http://gx.shxzskj.cn

[R04] 位置参数
来源：http://rv.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://aa.jianghongdianzi.cn

[R05] 参数默认值
来源：http://eq.asd995.cn

name="${1:-default}"
来源：http://jx.shxzskj.cn

[R06] 判断命令是否存在
来源：http://ic.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vc.gzmigu.cn

[R07] if 判断文件
来源：http://jy.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tx.shtwfgs.cn

[R08] 数值比较
来源：http://ds.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bk.gzmigu.cn

[R09] 字符串比较
来源：http://ns.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ps.shtwfgs.cn

[R10] 正则匹配
来源：http://jq.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ra.newstarts.cn

[R11] case 多分支
来源：http://gw.hahajie.cn

case "$1" in
来源：http://ld.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://ml.9csxet.cn

stop)  echo "停止" ;;
来源：http://ze.nicolike.cn

*)     echo "未知命令" ;;
来源：http://lt.shxzukj.cn

esac
来源：http://jm.chemitech.net.cn

[R12] for 遍历文件
来源：http://ot.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://ej.jctech888.com.cn

[R13] for 计数循环
来源：http://pl.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://sn.newstarts.cn

[R14] C 风格 for
来源：http://yi.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://db.hnjuh.cn

[R15] while 逐行读文件
来源：http://zm.haigaiapp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xk.muxihuayi.cn

[R16] until 等待条件
来源：http://ta.muxihuayi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fa.szsharing.cn

[R17] 数组定义与取值
来源：http://dj.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gu.chemitech.net.cn

[R18] 遍历数组
来源：http://tm.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ab.asd995.cn

[R19] 数组长度
来源：http://bt.9csxet.cn

echo "${#arr[@]}"
来源：http://za.lnxyls.cn

[R20] 关联数组（字典）
来源：http://tu.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uv.shxzskj.cn

[R21] 字符串长度
来源：http://kx.newstarts.cn

echo "${#s}"
来源：http://kq.bjjhwx.cn

[R22] 截取子串
来源：http://nd.szxytkj.cn

echo "${s:0:5}"
来源：http://ce.chemitech.net.cn

[R23] 字符串替换
来源：http://sz.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ls.hahajie.cn

[R24] 大小写转换
来源：http://as.newstarts.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vp.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://gv.wgjwhj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zf.9csxet.cn

[R26] 命令替换
来源：http://fz.szxytkj.cn

now=$(date +%F); echo "$now"
来源：http://bo.521024.cn

[R27] 算术展开
来源：http://db.huanxung.cn

echo $((1 + 2 * 3))
来源：http://xj.jctech888.com.cn

[R28] 浮点运算
来源：http://wv.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://ue.szsharing.cn

[R29] 定义函数
来源：http://zj.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oe.bjjhwx.cn

[R30] 函数返回状态码
来源：http://qq.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://hv.yuntaijiaju.cn

[R31] 局部变量
来源：http://vn.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://qh.panjiajie.cn

[R32] 参数个数校验
来源：http://cm.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://va.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://jh.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fe.hahajie.cn

[R34] 退出时清理
来源：http://aw.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gk.szsharing.cn

[R35] 后台执行并等待
来源：http://zr.szxytkj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lq.nszjky.cn

[R36] 并发执行多个任务
来源：http://qp.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pu.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://sp.hnjuh.cn

files=$(ls -1)
来源：http://tc.wgjwhj.cn

[R38] 管道串联
来源：http://xp.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://ix.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://mh.yuexingan06.cn

cmd > out.log 2>&1
来源：http://zh.colortex.cn

[R40] 追加写日志
来源：http://kl.yuexingan06.cn

echo "log" >> out.log
来源：http://ze.nicolike.cn

[R41] 丢弃输出
来源：http://ef.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://rg.nszjky.cn

[R42] 输入重定向
来源：http://nq.huixiangedu.cn

wc -l < a.txt
来源：http://ml.asd995.cn

[R43] 按名字查找文件
来源：http://kf.wgjwhj.cn

find . -name "*.log" -type f
来源：http://mc.haigaiapp.cn

[R44] 按修改时间查找
来源：http://ms.chemitech.net.cn

find . -mtime -7 -type f
来源：http://rt.jctech888.com.cn

[R45] 批量删除
来源：http://up.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://ca.muxihuayi.cn

[R46] 递归替换文件内容
来源：http://cm.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ut.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://wr.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://uq.colortex.cn

[R48] awk 取指定列
来源：http://ep.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://wp.huixinmuqiang.cn

[R49] awk 带条件
来源：http://ov.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rl.szxytkj.cn

[R50] awk 求和
来源：http://ei.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ns.huixiangedu.cn

[R51] 排序去重取前几
来源：http://no.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ig.bjjhwx.cn

[R52] 统计行数
来源：http://pn.521024.cn

wc -l a.txt
来源：http://vd.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://le.gzmigu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iz.muxihuayi.cn

[R54] 比较两个文件
来源：http://eu.521024.cn

diff a.txt b.txt
来源：http://sl.521024.cn

[R55] 压缩与解压
来源：http://kr.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wd.huixiangedu.cn

[R56] 远程拷贝
来源：http://ou.yuexingan06.cn

scp file user@host:/path/
来源：http://ur.shxzukj.cn

[R57] 远程执行命令
来源：http://ht.szsharing.cn

ssh user@host 'uptime'
来源：http://tk.hahajie.cn

[R58] 下载文件
来源：http://mo.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wm.huixiangedu.cn

[R59] 发 POST JSON
来源：http://pi.shxzskj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://be.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://hy.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ua.bookmarksfly.cn

[R61] 磁盘占用
来源：http://ag.jctech888.com.cn

df -h;  du -sh *
来源：http://cm.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://ir.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://wk.szxytkj.cn

[R63] 内存与进程
来源：http://uh.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://xt.hahajie.cn

[R64] 结束进程
来源：http://ij.nicolike.cn

kill -9 $(pgrep -f app.py)
来源：http://ud.szxytkj.cn

[R65] 查看端口占用
来源：http://cl.nicolike.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ta.huixiangedu.cn

[R66] 定时任务
来源：http://hd.hahajie.cn

crontab -e;  crontab -l
来源：http://os.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://zm.szsharing.cn

openssl rand -hex 16
来源：http://nc.yuntaijiaju.cn

[R68] 计算文件校验值
来源：http://no.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hg.lnxyls.cn

[R69] 生成随机密码
来源：http://oh.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://ib.yuexingan06.cn

[R70] 时间戳与互转
来源：http://ly.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://iq.colortex.cn

[R71] 日期格式化
来源：http://lc.newstarts.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://li.jctech888.com.cn

[R72] 等待端口就绪
来源：http://ix.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uc.huixiangedu.cn

[R73] 分割大日志
来源：http://pj.panjiajie.cn

split -l 1000 big.log part_
来源：http://qw.shxzukj.cn

[R74] 批量重命名
来源：http://th.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jq.chemitech.net.cn

[R75] 导出环境变量
来源：http://yd.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://in.haigaiapp.cn

[R76] 使用临时文件
来源：http://cv.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ts.shxzukj.cn

[R77] 读取用户输入
来源：http://ws.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://pa.gzmigu.cn

[R78] 交互式菜单
来源：http://bu.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zk.bjjhwx.cn

[R79] 解析命令行选项
来源：http://cm.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vb.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://hd.jctech888.com.cn

time ./run.sh
来源：http://ti.newstarts.cn

================================================================================
来源：http://pt.shxzukj.cn

S. C / C++ 专题
来源：http://fr.huixiangedu.cn

================================================================================
来源：http://bq.szxytkj.cn

[S01] C：Hello World
来源：http://ca.hnjuh.cn

#include <stdio.h>
来源：http://yf.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xk.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://xx.chemitech.net.cn

int a = 10; printf("%d\n", a);
来源：http://po.bookmarksfly.cn

[S03] C：读入整数
来源：http://xt.panjiajie.cn

int x; scanf("%d", &x);
来源：http://aq.gzmigu.cn

[S04] C：字符串复制
来源：http://zi.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gy.yuexingan06.cn

[S05] C：字符串长度
来源：http://hs.521024.cn

strlen(s)
来源：http://uy.asd995.cn

[S06] C：字符串比较
来源：http://en.hnjuh.cn

strcmp(a, b) == 0
来源：http://yq.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://qr.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qh.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://jm.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hu.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://ct.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ba.jctech888.com.cn

[S10] C：指针与解引用
来源：http://hi.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://fv.hahajie.cn

[S11] C：逐行读文件
来源：http://bh.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://io.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tm.colortex.cn

fclose(f);
来源：http://vj.yuntaijiaju.cn

[S12] C：写文件
来源：http://te.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wv.bookmarksfly.cn

[S13] C：宏定义
来源：http://kv.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ra.wgjwhj.cn

[S14] C：枚举
来源：http://vw.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://dt.shtwfgs.cn

[S15] C：类型转换
来源：http://fk.newstarts.cn

(double) a / b
来源：http://tz.hahajie.cn

[S16] C：位操作置位
来源：http://cj.jianghongdianzi.cn

x |= (1 << 3);
来源：http://rd.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://oc.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yx.521024.cn

[S18] C：命令行参数
来源：http://sf.muxihuayi.cn

int main(int argc, char **argv)
来源：http://po.huanxung.cn

[S19] C：快速排序
来源：http://lx.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fy.yuntaijiaju.cn

[S20] C：二分查找
来源：http://do.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bv.panjiajie.cn

[S21] C：字符类别判断
来源：http://ev.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kp.wgjwhj.cn

[S22] C：字符串转数字
来源：http://da.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zq.chemitech.net.cn

[S23] C：随机数
来源：http://ha.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://eh.szxytkj.cn

[S24] C：获取本地时间
来源：http://lm.szsharing.cn


<!-- 参考信息 -->