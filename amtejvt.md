代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cw.9csxet.cn

[Q54] 清空表
来源：http://ff.newstarts.cn

TRUNCATE TABLE logs;
来源：http://rc.asd995.cn

[Q55] 排名（并列占位）
来源：http://pp.newstarts.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hr.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://xd.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qp.asd995.cn

[Q57] 行号
来源：http://sw.nicolike.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mf.hahajie.cn

[Q58] 累计求和
来源：http://uf.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://px.chemitech.net.cn

[Q59] 分组内累计
来源：http://tq.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ie.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://tj.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tf.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vu.haigaiapp.cn

[Q61] 移动平均
来源：http://zq.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vf.panjiajie.cn

[Q62] 分组占比
来源：http://on.shtwfgs.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tf.szxytkj.cn

[Q63] 开启事务
来源：http://jm.hnjuh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rg.jctech888.com.cn

[Q64] 提交事务
来源：http://fn.lnxyls.cn

COMMIT;
来源：http://ln.newstarts.cn

[Q65] 回滚事务
来源：http://er.panjiajie.cn

ROLLBACK;
来源：http://tc.haigaiapp.cn

[Q66] 行锁查询
来源：http://ej.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sv.szxytkj.cn

[Q67] 设置隔离级别
来源：http://bf.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qe.nicolike.cn

[Q68] 保存点
来源：http://ak.szsharing.cn

SAVEPOINT sp1;
来源：http://pt.shxzukj.cn

ROLLBACK TO sp1;
来源：http://tj.huixiangedu.cn

[Q69] 查看执行计划
来源：http://hi.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hd.chemitech.net.cn

[Q70] 更新统计信息
来源：http://ah.huixiangedu.cn

ANALYZE TABLE users;
来源：http://ys.szxytkj.cn

[Q71] 查看建表语句
来源：http://hh.bjjhwx.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xn.bjjhwx.cn

[Q72] 查看索引
来源：http://ff.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://zh.521024.cn

[Q73] 查看表状态
来源：http://ly.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jl.nszjky.cn

[Q74] 强制使用索引
来源：http://pc.bookmarksfly.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gx.hnjuh.cn

[Q75] 日期格式化
来源：http://iz.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://un.bjjhwx.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://or.lnxyls.cn

[Q76] 按天统计
来源：http://sx.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sg.yuexingan06.cn

[Q77] 时间加减
来源：http://jo.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qf.haigaiapp.cn

[Q78] 当前时间
来源：http://bb.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cf.huixiangedu.cn

[Q79] 字符串拼接
来源：http://bh.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zt.yuexingan06.cn

[Q80] 字符串截取
来源：http://yw.shtwfgs.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gq.colortex.cn

[Q81] 字符串替换
来源：http://us.nszjky.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ef.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://ql.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wn.521024.cn

[Q83] 大小写转换
来源：http://et.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://er.huanxung.cn

[Q84] 去除首尾空格
来源：http://tq.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://ty.nicolike.cn

[Q85] 数值取整
来源：http://qw.jianghongdianzi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qy.newstarts.cn

[Q86] 读取 JSON 字段
来源：http://ug.bookmarksfly.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ja.colortex.cn

[Q87] JSON 字段做条件
来源：http://wn.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://je.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://if.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://it.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wj.asd995.cn

[Q89] 判断表是否存在
来源：http://zf.haigaiapp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kw.chemitech.net.cn

[Q90] 生成序号列
来源：http://kc.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tk.yuntaijiaju.cn

================================================================================
来源：http://pg.jctech888.com.cn

R. Bash 专题
来源：http://rj.szxytkj.cn

================================================================================
来源：http://lb.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://sk.panjiajie.cn

#!/usr/bin/env bash
来源：http://cv.shtwfgs.cn

set -euo pipefail
来源：http://rn.bookmarksfly.cn

[R02] 变量赋值与使用
来源：http://sa.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://xd.chemitech.net.cn

[R03] 只读变量
来源：http://dx.huanxung.cn

readonly PI=3.14
来源：http://hr.nicolike.cn

[R04] 位置参数
来源：http://rs.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://il.gzmigu.cn

[R05] 参数默认值
来源：http://se.lnxyls.cn

name="${1:-default}"
来源：http://kh.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://pu.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wa.huixinmuqiang.cn

[R07] if 判断文件
来源：http://sb.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tx.muxihuayi.cn

[R08] 数值比较
来源：http://ye.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lx.chemitech.net.cn

[R09] 字符串比较
来源：http://vs.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cb.lnxyls.cn

[R10] 正则匹配
来源：http://ps.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vs.yuntaijiaju.cn

[R11] case 多分支
来源：http://wv.chemitech.net.cn

case "$1" in
来源：http://el.haigaiapp.cn

start) echo "启动" ;;
来源：http://ju.szsharing.cn

stop)  echo "停止" ;;
来源：http://yl.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://eo.yuexingan06.cn

esac
来源：http://th.huanxung.cn

[R12] for 遍历文件
来源：http://il.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://gx.nszjky.cn

[R13] for 计数循环
来源：http://gk.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://vy.shxzukj.cn

[R14] C 风格 for
来源：http://te.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pz.9csxet.cn

[R15] while 逐行读文件
来源：http://xs.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lj.yuexingan06.cn

[R16] until 等待条件
来源：http://uu.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ze.nszjky.cn

[R17] 数组定义与取值
来源：http://jn.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gl.bookmarksfly.cn

[R18] 遍历数组
来源：http://du.hnjuh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://va.lnxyls.cn

[R19] 数组长度
来源：http://ja.gzmigu.cn

echo "${#arr[@]}"
来源：http://fy.szsharing.cn

[R20] 关联数组（字典）
来源：http://zl.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uc.nszjky.cn

[R21] 字符串长度
来源：http://ut.jianghongdianzi.cn

echo "${#s}"
来源：http://ju.lnxyls.cn

[R22] 截取子串
来源：http://yu.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://tx.asd995.cn

[R23] 字符串替换
来源：http://hz.huixinmuqiang.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lf.yuntaijiaju.cn

[R24] 大小写转换
来源：http://qz.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://js.bjjhwx.cn

[R25] 去后缀 / 去前缀
来源：http://od.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ca.nszjky.cn

[R26] 命令替换
来源：http://mr.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://vd.yuexingan06.cn

[R27] 算术展开
来源：http://kl.newstarts.cn

echo $((1 + 2 * 3))
来源：http://ro.muxihuayi.cn

[R28] 浮点运算
来源：http://tg.521024.cn

echo "scale=2; 10/3" | bc
来源：http://zb.szsharing.cn

[R29] 定义函数
来源：http://kq.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ly.haigaiapp.cn

[R30] 函数返回状态码
来源：http://fr.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://ct.yuexingan06.cn

[R31] 局部变量
来源：http://ft.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://qx.yuexingan06.cn

[R32] 参数个数校验
来源：http://va.colortex.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://be.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://dc.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zb.wgjwhj.cn

[R34] 退出时清理
来源：http://sr.chemitech.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vs.nicolike.cn

[R35] 后台执行并等待
来源：http://sy.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uq.shxzskj.cn

[R36] 并发执行多个任务
来源：http://wo.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dn.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://wo.chemitech.net.cn

files=$(ls -1)
来源：http://yu.521024.cn

[R38] 管道串联
来源：http://ex.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://sa.yuexingan06.cn

[R39] 重定向标准输出与错误
来源：http://oj.yuexingan06.cn

cmd > out.log 2>&1
来源：http://qs.nicolike.cn

[R40] 追加写日志
来源：http://nt.nicolike.cn

echo "log" >> out.log
来源：http://xn.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://oc.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://fv.jianghongdianzi.cn

[R42] 输入重定向
来源：http://yl.colortex.cn

wc -l < a.txt
来源：http://nf.jctech888.com.cn

[R43] 按名字查找文件
来源：http://gm.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://ab.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://hw.shtwfgs.cn

find . -mtime -7 -type f
来源：http://fo.9csxet.cn

[R45] 批量删除
来源：http://he.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://og.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://qo.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gp.hahajie.cn

[R47] sed 单行替换
来源：http://li.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oi.nszjky.cn

[R48] awk 取指定列
来源：http://pz.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://gg.chemitech.net.cn

[R49] awk 带条件
来源：http://gq.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://an.9csxet.cn

[R50] awk 求和
来源：http://vs.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xq.muxihuayi.cn

[R51] 排序去重取前几
来源：http://jp.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tj.nszjky.cn

[R52] 统计行数
来源：http://ur.nicolike.cn

wc -l a.txt
来源：http://so.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://oc.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ul.haigaiapp.cn

[R54] 比较两个文件
来源：http://mz.bookmarksfly.cn

diff a.txt b.txt
来源：http://hu.gzmigu.cn

[R55] 压缩与解压
来源：http://yw.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sk.hahajie.cn

[R56] 远程拷贝
来源：http://vo.szxytkj.cn

scp file user@host:/path/
来源：http://nl.panjiajie.cn

[R57] 远程执行命令
来源：http://ty.haigaiapp.cn

ssh user@host 'uptime'
来源：http://we.hnjuh.cn

[R58] 下载文件
来源：http://cv.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ym.521024.cn

[R59] 发 POST JSON
来源：http://ra.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cu.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://yq.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://go.panjiajie.cn

[R61] 磁盘占用
来源：http://eo.nszjky.cn

df -h;  du -sh *
来源：http://kr.521024.cn

[R62] 找最占空间的文件
来源：http://zh.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://rw.huanxung.cn

[R63] 内存与进程
来源：http://ta.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://oe.bjjhwx.cn

[R64] 结束进程
来源：http://pl.hnjuh.cn

kill -9 $(pgrep -f app.py)
来源：http://ih.nszjky.cn

[R65] 查看端口占用
来源：http://si.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vt.asd995.cn

[R66] 定时任务
来源：http://ee.shxzukj.cn

crontab -e;  crontab -l
来源：http://gz.asd995.cn

[R67] 生成随机十六进制串
来源：http://so.colortex.cn

openssl rand -hex 16
来源：http://gs.huixiangedu.cn

[R68] 计算文件校验值
来源：http://yx.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xl.nszjky.cn

[R69] 生成随机密码
来源：http://fo.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://ur.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://ee.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://yj.szxytkj.cn

[R71] 日期格式化
来源：http://ji.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ml.newstarts.cn

[R72] 等待端口就绪
来源：http://cw.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ie.gzmigu.cn

[R73] 分割大日志
来源：http://pd.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://lv.colortex.cn

[R74] 批量重命名
来源：http://az.newstarts.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ae.huixinmuqiang.cn

[R75] 导出环境变量
来源：http://rg.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://gx.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://ky.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vn.nszjky.cn

[R77] 读取用户输入
来源：http://sf.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://au.shxzukj.cn

[R78] 交互式菜单
来源：http://xz.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nh.muxihuayi.cn

[R79] 解析命令行选项
来源：http://gz.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lg.9csxet.cn

[R80] 查看脚本执行耗时
来源：http://kd.nicolike.cn

time ./run.sh
来源：http://lv.yuexingan06.cn

================================================================================
来源：http://hb.jianghongdianzi.cn

S. C / C++ 专题
来源：http://at.chemitech.net.cn

================================================================================
来源：http://ow.9csxet.cn

[S01] C：Hello World
来源：http://ot.newstarts.cn

#include <stdio.h>
来源：http://ab.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uu.asd995.cn

[S02] C：变量与格式化输出
来源：http://jq.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://gq.chemitech.net.cn

[S03] C：读入整数
来源：http://sc.jianghongdianzi.cn

int x; scanf("%d", &x);
来源：http://ok.shxzukj.cn

[S04] C：字符串复制
来源：http://qt.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wv.huanxung.cn

[S05] C：字符串长度
来源：http://tl.haigaiapp.cn

strlen(s)
来源：http://gb.asd995.cn

[S06] C：字符串比较
来源：http://ge.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://nc.panjiajie.cn

[S07] C：数组遍历求和
来源：http://jp.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fp.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://ip.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lz.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://li.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xt.hahajie.cn

[S10] C：指针与解引用
来源：http://pj.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://ur.newstarts.cn

[S11] C：逐行读文件
来源：http://xw.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://qx.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vs.huixinmuqiang.cn

fclose(f);
来源：http://an.szxytkj.cn

[S12] C：写文件
来源：http://oh.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rh.wgjwhj.cn

[S13] C：宏定义
来源：http://bn.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xj.newstarts.cn

[S14] C：枚举
来源：http://ue.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://cm.huixiangedu.cn

[S15] C：类型转换
来源：http://lr.gzmigu.cn

(double) a / b
来源：http://ob.colortex.cn

[S16] C：位操作置位
来源：http://mb.nszjky.cn

x |= (1 << 3);
来源：http://za.9csxet.cn

[S17] C：安全拼接字符串
来源：http://re.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ib.nszjky.cn

[S18] C：命令行参数
来源：http://bh.chemitech.net.cn

int main(int argc, char **argv)
来源：http://wu.bjjhwx.cn

[S19] C：快速排序
来源：http://ws.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fp.9csxet.cn

[S20] C：二分查找
来源：http://ic.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xd.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://kw.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nd.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://in.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rq.colortex.cn

[S23] C：随机数
来源：http://vi.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://eq.521024.cn

[S24] C：获取本地时间
来源：http://hj.hahajie.cn


<!-- 参考信息 -->