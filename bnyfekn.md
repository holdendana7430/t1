代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yh.asd995.cn

[Q50] 批量更新
来源：http://fo.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pz.jctech888.com.cn

[Q51] 用子查询更新
来源：http://oc.huixiangedu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yp.bjjhwx.cn

[Q52] 删除指定行
来源：http://ay.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://yh.szsharing.cn

[Q53] 按条件删除
来源：http://xe.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hf.asd995.cn

[Q54] 清空表
来源：http://re.9csxet.cn

TRUNCATE TABLE logs;
来源：http://qr.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://bn.newstarts.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hg.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://cc.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://aj.szsharing.cn

[Q57] 行号
来源：http://an.chemitech.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mm.haigaiapp.cn

[Q58] 累计求和
来源：http://zl.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://es.shtwfgs.cn

[Q59] 分组内累计
来源：http://lt.9csxet.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yc.shxzukj.cn

[Q60] 取上一行 / 下一行
来源：http://je.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jx.shtwfgs.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ts.nszjky.cn

[Q61] 移动平均
来源：http://rp.colortex.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ll.szxytkj.cn

[Q62] 分组占比
来源：http://ad.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xd.bookmarksfly.cn

[Q63] 开启事务
来源：http://wi.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sy.shtwfgs.cn

[Q64] 提交事务
来源：http://qc.hahajie.cn

COMMIT;
来源：http://po.nszjky.cn

[Q65] 回滚事务
来源：http://pr.9csxet.cn

ROLLBACK;
来源：http://nf.nszjky.cn

[Q66] 行锁查询
来源：http://rw.jianghongdianzi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lo.szxytkj.cn

[Q67] 设置隔离级别
来源：http://um.huixiangedu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gn.huixiangedu.cn

[Q68] 保存点
来源：http://mb.szxytkj.cn

SAVEPOINT sp1;
来源：http://cf.muxihuayi.cn

ROLLBACK TO sp1;
来源：http://un.nszjky.cn

[Q69] 查看执行计划
来源：http://wi.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dq.yuexingan06.cn

[Q70] 更新统计信息
来源：http://za.huixiangedu.cn

ANALYZE TABLE users;
来源：http://wz.szxytkj.cn

[Q71] 查看建表语句
来源：http://eu.wgjwhj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hn.521024.cn

[Q72] 查看索引
来源：http://of.lnxyls.cn

SHOW INDEX FROM users;
来源：http://ws.gzmigu.cn

[Q73] 查看表状态
来源：http://mk.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nv.chemitech.net.cn

[Q74] 强制使用索引
来源：http://aw.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fh.lnxyls.cn

[Q75] 日期格式化
来源：http://ma.huixiangedu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fd.shxzukj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qa.asd995.cn

[Q76] 按天统计
来源：http://dr.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://by.bookmarksfly.cn

[Q77] 时间加减
来源：http://qd.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cp.jianghongdianzi.cn

[Q78] 当前时间
来源：http://mw.nszjky.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://de.nicolike.cn

[Q79] 字符串拼接
来源：http://vh.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xq.wgjwhj.cn

[Q80] 字符串截取
来源：http://yk.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://py.jctech888.com.cn

[Q81] 字符串替换
来源：http://ta.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ja.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://ou.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wo.panjiajie.cn

[Q83] 大小写转换
来源：http://ej.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vq.nszjky.cn

[Q84] 去除首尾空格
来源：http://in.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://it.hnjuh.cn

[Q85] 数值取整
来源：http://fz.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ag.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://fy.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vj.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://yj.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zz.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://wi.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yp.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iw.shxzukj.cn

[Q89] 判断表是否存在
来源：http://vr.asd995.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kk.nicolike.cn

[Q90] 生成序号列
来源：http://nf.hahajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gk.jctech888.com.cn

================================================================================
来源：http://jx.wgjwhj.cn

R. Bash 专题
来源：http://ra.yuexingan06.cn

================================================================================
来源：http://ya.9csxet.cn

[R01] shebang 与严格模式
来源：http://tg.lnxyls.cn

#!/usr/bin/env bash
来源：http://zs.colortex.cn

set -euo pipefail
来源：http://sl.bjjhwx.cn

[R02] 变量赋值与使用
来源：http://sv.shxzskj.cn

name="Tom"; echo "$name"
来源：http://zv.nicolike.cn

[R03] 只读变量
来源：http://hi.szsharing.cn

readonly PI=3.14
来源：http://gq.haigaiapp.cn

[R04] 位置参数
来源：http://db.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ui.huanxung.cn

[R05] 参数默认值
来源：http://ue.nicolike.cn

name="${1:-default}"
来源：http://jc.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://mg.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pp.jianghongdianzi.cn

[R07] if 判断文件
来源：http://wj.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xt.shxzukj.cn

[R08] 数值比较
来源：http://zl.hahajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tn.haigaiapp.cn

[R09] 字符串比较
来源：http://jl.shtwfgs.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pz.bjjhwx.cn

[R10] 正则匹配
来源：http://pf.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lx.hnjuh.cn

[R11] case 多分支
来源：http://kr.huixiangedu.cn

case "$1" in
来源：http://qd.hnjuh.cn

start) echo "启动" ;;
来源：http://au.szxytkj.cn

stop)  echo "停止" ;;
来源：http://kd.yuntaijiaju.cn

*)     echo "未知命令" ;;
来源：http://pb.bookmarksfly.cn

esac
来源：http://qp.szxytkj.cn

[R12] for 遍历文件
来源：http://ex.szsharing.cn

for f in *.txt; do echo "$f"; done
来源：http://tt.szsharing.cn

[R13] for 计数循环
来源：http://sx.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://wx.szsharing.cn

[R14] C 风格 for
来源：http://by.lnxyls.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ek.shxzskj.cn

[R15] while 逐行读文件
来源：http://xf.bjjhwx.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ln.hnjuh.cn

[R16] until 等待条件
来源：http://tj.panjiajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rd.panjiajie.cn

[R17] 数组定义与取值
来源：http://xg.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cg.hnjuh.cn

[R18] 遍历数组
来源：http://xe.szsharing.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ju.asd995.cn

[R19] 数组长度
来源：http://sf.jianghongdianzi.cn

echo "${#arr[@]}"
来源：http://hv.panjiajie.cn

[R20] 关联数组（字典）
来源：http://od.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oj.shxzukj.cn

[R21] 字符串长度
来源：http://mi.colortex.cn

echo "${#s}"
来源：http://nk.bookmarksfly.cn

[R22] 截取子串
来源：http://bj.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://qj.shxzukj.cn

[R23] 字符串替换
来源：http://ol.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jo.huixiangedu.cn

[R24] 大小写转换
来源：http://dw.colortex.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wl.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://ev.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ru.9csxet.cn

[R26] 命令替换
来源：http://yk.chemitech.net.cn

now=$(date +%F); echo "$now"
来源：http://od.hnjuh.cn

[R27] 算术展开
来源：http://pr.colortex.cn

echo $((1 + 2 * 3))
来源：http://cb.bookmarksfly.cn

[R28] 浮点运算
来源：http://va.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://sc.hnjuh.cn

[R29] 定义函数
来源：http://on.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rb.nszjky.cn

[R30] 函数返回状态码
来源：http://yf.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://no.panjiajie.cn

[R31] 局部变量
来源：http://bz.huanxung.cn

f() { local x=1; echo "$x"; }
来源：http://cw.panjiajie.cn

[R32] 参数个数校验
来源：http://px.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ts.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://sz.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vz.panjiajie.cn

[R34] 退出时清理
来源：http://dw.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zh.shxzskj.cn

[R35] 后台执行并等待
来源：http://up.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rs.huanxung.cn

[R36] 并发执行多个任务
来源：http://jb.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bu.hahajie.cn

[R37] 把输出赋给变量
来源：http://og.lnxyls.cn

files=$(ls -1)
来源：http://my.jianghongdianzi.cn

[R38] 管道串联
来源：http://ki.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://or.colortex.cn

[R39] 重定向标准输出与错误
来源：http://jz.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://xl.colortex.cn

[R40] 追加写日志
来源：http://bq.bjjhwx.cn

echo "log" >> out.log
来源：http://ch.nszjky.cn

[R41] 丢弃输出
来源：http://hm.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://lk.haigaiapp.cn

[R42] 输入重定向
来源：http://gz.jctech888.com.cn

wc -l < a.txt
来源：http://mg.lnxyls.cn

[R43] 按名字查找文件
来源：http://mn.lnxyls.cn

find . -name "*.log" -type f
来源：http://se.gzmigu.cn

[R44] 按修改时间查找
来源：http://bt.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://ns.9csxet.cn

[R45] 批量删除
来源：http://no.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://gz.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://sr.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eo.nicolike.cn

[R47] sed 单行替换
来源：http://bv.shxzukj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://td.hnjuh.cn

[R48] awk 取指定列
来源：http://fw.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://bk.hahajie.cn

[R49] awk 带条件
来源：http://ap.muxihuayi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ug.newstarts.cn

[R50] awk 求和
来源：http://um.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tv.wgjwhj.cn

[R51] 排序去重取前几
来源：http://kw.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nl.lnxyls.cn

[R52] 统计行数
来源：http://je.yuexingan06.cn

wc -l a.txt
来源：http://wo.shxzskj.cn

[R53] 查看文件头与实时尾
来源：http://ob.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gj.lnxyls.cn

[R54] 比较两个文件
来源：http://gp.colortex.cn

diff a.txt b.txt
来源：http://mk.jianghongdianzi.cn

[R55] 压缩与解压
来源：http://nd.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tl.muxihuayi.cn

[R56] 远程拷贝
来源：http://mt.szxytkj.cn

scp file user@host:/path/
来源：http://fg.asd995.cn

[R57] 远程执行命令
来源：http://vy.9csxet.cn

ssh user@host 'uptime'
来源：http://kt.huixiangedu.cn

[R58] 下载文件
来源：http://qc.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mm.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://mn.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mc.521024.cn

[R60] 只看 HTTP 状态码
来源：http://vk.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zd.chemitech.net.cn

[R61] 磁盘占用
来源：http://du.newstarts.cn

df -h;  du -sh *
来源：http://ml.9csxet.cn

[R62] 找最占空间的文件
来源：http://tk.bookmarksfly.cn

du -ah . | sort -rh | head -10
来源：http://zz.colortex.cn

[R63] 内存与进程
来源：http://yd.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://sb.wgjwhj.cn

[R64] 结束进程
来源：http://df.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://jw.9csxet.cn

[R65] 查看端口占用
来源：http://cz.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ij.9csxet.cn

[R66] 定时任务
来源：http://mh.wgjwhj.cn

crontab -e;  crontab -l
来源：http://kj.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://cd.hahajie.cn

openssl rand -hex 16
来源：http://ue.szsharing.cn

[R68] 计算文件校验值
来源：http://mf.newstarts.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wu.szsharing.cn

[R69] 生成随机密码
来源：http://ch.hahajie.cn

head -c 16 /dev/urandom | base64
来源：http://py.chemitech.net.cn

[R70] 时间戳与互转
来源：http://og.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://dm.colortex.cn

[R71] 日期格式化
来源：http://rp.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fc.nicolike.cn

[R72] 等待端口就绪
来源：http://rf.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ek.hahajie.cn

[R73] 分割大日志
来源：http://zo.szsharing.cn

split -l 1000 big.log part_
来源：http://hb.jianghongdianzi.cn

[R74] 批量重命名
来源：http://mo.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ap.asd995.cn

[R75] 导出环境变量
来源：http://bu.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://no.szxytkj.cn

[R76] 使用临时文件
来源：http://im.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wx.lnxyls.cn

[R77] 读取用户输入
来源：http://bw.9csxet.cn

read -rp "请输入: " ans
来源：http://ir.shxzskj.cn

[R78] 交互式菜单
来源：http://nj.hahajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nn.huanxung.cn

[R79] 解析命令行选项
来源：http://pj.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ue.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://ac.jctech888.com.cn

time ./run.sh
来源：http://co.panjiajie.cn

================================================================================
来源：http://so.panjiajie.cn

S. C / C++ 专题
来源：http://gc.szxytkj.cn

================================================================================
来源：http://fc.yuexingan06.cn

[S01] C：Hello World
来源：http://wy.jctech888.com.cn

#include <stdio.h>
来源：http://ol.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hl.hahajie.cn

[S02] C：变量与格式化输出
来源：http://aq.521024.cn

int a = 10; printf("%d\n", a);
来源：http://mq.szxytkj.cn

[S03] C：读入整数
来源：http://cq.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://ib.newstarts.cn

[S04] C：字符串复制
来源：http://zf.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wi.gzmigu.cn

[S05] C：字符串长度
来源：http://pu.nicolike.cn

strlen(s)
来源：http://hn.521024.cn

[S06] C：字符串比较
来源：http://xs.jctech888.com.cn

strcmp(a, b) == 0
来源：http://uw.lnxyls.cn

[S07] C：数组遍历求和
来源：http://ku.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ga.asd995.cn

[S08] C：动态内存分配与释放
来源：http://ni.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ki.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://ds.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jc.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://pa.hahajie.cn

int *p = &a;  *p = 5;
来源：http://dj.9csxet.cn

[S11] C：逐行读文件
来源：http://li.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://dy.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tx.nszjky.cn

fclose(f);
来源：http://kv.yuntaijiaju.cn

[S12] C：写文件
来源：http://kl.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xd.gzmigu.cn

[S13] C：宏定义
来源：http://na.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ou.yuntaijiaju.cn

[S14] C：枚举
来源：http://gd.huanxung.cn

enum Color { RED, GREEN, BLUE };
来源：http://md.jctech888.com.cn

[S15] C：类型转换
来源：http://ac.haigaiapp.cn

(double) a / b
来源：http://cu.chemitech.net.cn

[S16] C：位操作置位
来源：http://ad.lnxyls.cn

x |= (1 << 3);
来源：http://fe.huanxung.cn

[S17] C：安全拼接字符串
来源：http://hv.bjjhwx.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lk.gzmigu.cn

[S18] C：命令行参数
来源：http://qo.huixiangedu.cn

int main(int argc, char **argv)
来源：http://ht.yuexingan06.cn

[S19] C：快速排序
来源：http://ru.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cc.bookmarksfly.cn

[S20] C：二分查找
来源：http://vu.yuntaijiaju.cn


<!-- 参考信息 -->