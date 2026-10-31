代发 wailian999

[Q44] IN 子查询
来源：http://uv.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wa.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://wo.chemitech.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ck.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ks.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pk.nszjky.cn

[Q47] 与平均值比较
来源：http://ma.yuexingan06.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sj.nszjky.cn

[Q48] CTE 公用表表达式
来源：http://ju.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ir.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://wr.shxzskj.cn

[Q49] 更新单行
来源：http://ug.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ra.chemitech.net.cn

[Q50] 批量更新
来源：http://oa.muxihuayi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://om.nicolike.cn

[Q51] 用子查询更新
来源：http://ff.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uy.9csxet.cn

[Q52] 删除指定行
来源：http://mo.muxihuayi.cn

DELETE FROM users WHERE id = 10;
来源：http://to.haigaiapp.cn

[Q53] 按条件删除
来源：http://jy.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sn.chemitech.net.cn

[Q54] 清空表
来源：http://lq.bookmarksfly.cn

TRUNCATE TABLE logs;
来源：http://ky.9csxet.cn

[Q55] 排名（并列占位）
来源：http://fv.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tf.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://by.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ou.huixiangedu.cn

[Q57] 行号
来源：http://zo.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ej.chemitech.net.cn

[Q58] 累计求和
来源：http://xr.huanxung.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sp.panjiajie.cn

[Q59] 分组内累计
来源：http://ys.521024.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ul.lnxyls.cn

[Q60] 取上一行 / 下一行
来源：http://xm.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wb.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hy.521024.cn

[Q61] 移动平均
来源：http://ht.wgjwhj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tp.asd995.cn

[Q62] 分组占比
来源：http://kd.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bc.shxzskj.cn

[Q63] 开启事务
来源：http://he.shxzskj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hl.nszjky.cn

[Q64] 提交事务
来源：http://uh.szsharing.cn

COMMIT;
来源：http://yw.hahajie.cn

[Q65] 回滚事务
来源：http://tj.9csxet.cn

ROLLBACK;
来源：http://bk.asd995.cn

[Q66] 行锁查询
来源：http://nt.asd995.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vn.panjiajie.cn

[Q67] 设置隔离级别
来源：http://bf.lnxyls.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jf.bookmarksfly.cn

[Q68] 保存点
来源：http://ys.shxzskj.cn

SAVEPOINT sp1;
来源：http://ev.gzmigu.cn

ROLLBACK TO sp1;
来源：http://wn.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://jx.panjiajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uq.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://uz.chemitech.net.cn

ANALYZE TABLE users;
来源：http://zg.521024.cn

[Q71] 查看建表语句
来源：http://je.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vy.wgjwhj.cn

[Q72] 查看索引
来源：http://qb.szxytkj.cn

SHOW INDEX FROM users;
来源：http://uq.colortex.cn

[Q73] 查看表状态
来源：http://lh.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://js.yuexingan06.cn

[Q74] 强制使用索引
来源：http://ll.haigaiapp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://iw.panjiajie.cn

[Q75] 日期格式化
来源：http://zt.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fu.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zs.lnxyls.cn

[Q76] 按天统计
来源：http://lm.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ji.huanxung.cn

[Q77] 时间加减
来源：http://on.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ze.lnxyls.cn

[Q78] 当前时间
来源：http://nn.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ta.panjiajie.cn

[Q79] 字符串拼接
来源：http://as.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sg.muxihuayi.cn

[Q80] 字符串截取
来源：http://rm.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yg.hnjuh.cn

[Q81] 字符串替换
来源：http://wg.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://na.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://mr.521024.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gq.bookmarksfly.cn

[Q83] 大小写转换
来源：http://wm.521024.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qc.9csxet.cn

[Q84] 去除首尾空格
来源：http://sj.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://tf.szxytkj.cn

[Q85] 数值取整
来源：http://xi.9csxet.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://as.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://xw.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ar.chemitech.net.cn

[Q87] JSON 字段做条件
来源：http://hi.yuexingan06.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iz.jianghongdianzi.cn

[Q88] 行转列（条件聚合）
来源：http://to.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hn.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wu.muxihuayi.cn

[Q89] 判断表是否存在
来源：http://bv.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ht.haigaiapp.cn

[Q90] 生成序号列
来源：http://nl.muxihuayi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hd.jctech888.com.cn

================================================================================
来源：http://rx.jctech888.com.cn

R. Bash 专题
来源：http://qo.wgjwhj.cn

================================================================================
来源：http://jt.gzmigu.cn

[R01] shebang 与严格模式
来源：http://lh.shtwfgs.cn

#!/usr/bin/env bash
来源：http://uo.yuntaijiaju.cn

set -euo pipefail
来源：http://gw.jianghongdianzi.cn

[R02] 变量赋值与使用
来源：http://ms.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://nb.newstarts.cn

[R03] 只读变量
来源：http://cx.asd995.cn

readonly PI=3.14
来源：http://di.shxzukj.cn

[R04] 位置参数
来源：http://ky.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://aq.yuexingan06.cn

[R05] 参数默认值
来源：http://jg.huanxung.cn

name="${1:-default}"
来源：http://jh.shxzskj.cn

[R06] 判断命令是否存在
来源：http://un.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kq.bookmarksfly.cn

[R07] if 判断文件
来源：http://ue.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vj.szsharing.cn

[R08] 数值比较
来源：http://ep.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vl.shxzukj.cn

[R09] 字符串比较
来源：http://qs.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rj.shxzukj.cn

[R10] 正则匹配
来源：http://ey.muxihuayi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fy.colortex.cn

[R11] case 多分支
来源：http://kv.huixinmuqiang.cn

case "$1" in
来源：http://ja.nszjky.cn

start) echo "启动" ;;
来源：http://sb.9csxet.cn

stop)  echo "停止" ;;
来源：http://fb.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://cd.huanxung.cn

esac
来源：http://gg.wgjwhj.cn

[R12] for 遍历文件
来源：http://qh.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://gk.bjjhwx.cn

[R13] for 计数循环
来源：http://px.szsharing.cn

for i in {1..10}; do echo "$i"; done
来源：http://ht.bookmarksfly.cn

[R14] C 风格 for
来源：http://di.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vm.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://sb.bjjhwx.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wu.asd995.cn

[R16] until 等待条件
来源：http://qi.shxzskj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qh.jctech888.com.cn

[R17] 数组定义与取值
来源：http://tq.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fy.shxzskj.cn

[R18] 遍历数组
来源：http://nn.szxytkj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fh.bjjhwx.cn

[R19] 数组长度
来源：http://bf.colortex.cn

echo "${#arr[@]}"
来源：http://ui.szsharing.cn

[R20] 关联数组（字典）
来源：http://we.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kc.shxzukj.cn

[R21] 字符串长度
来源：http://wd.jctech888.com.cn

echo "${#s}"
来源：http://td.jianghongdianzi.cn

[R22] 截取子串
来源：http://hn.panjiajie.cn

echo "${s:0:5}"
来源：http://cn.bjjhwx.cn

[R23] 字符串替换
来源：http://tw.newstarts.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vw.huixinmuqiang.cn

[R24] 大小写转换
来源：http://kq.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://il.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://ue.huixiangedu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nh.shtwfgs.cn

[R26] 命令替换
来源：http://ky.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://hi.wgjwhj.cn

[R27] 算术展开
来源：http://ay.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://nl.521024.cn

[R28] 浮点运算
来源：http://tj.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://wo.jianghongdianzi.cn

[R29] 定义函数
来源：http://wc.szxytkj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xb.panjiajie.cn

[R30] 函数返回状态码
来源：http://qo.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://zt.jctech888.com.cn

[R31] 局部变量
来源：http://iw.shxzukj.cn

f() { local x=1; echo "$x"; }
来源：http://vn.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://mu.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gn.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://xv.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ti.huixiangedu.cn

[R34] 退出时清理
来源：http://kn.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://iu.wgjwhj.cn

[R35] 后台执行并等待
来源：http://nu.yuexingan06.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pt.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://xh.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ws.hnjuh.cn

[R37] 把输出赋给变量
来源：http://yd.nicolike.cn

files=$(ls -1)
来源：http://dx.521024.cn

[R38] 管道串联
来源：http://ra.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://yv.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://ew.colortex.cn

cmd > out.log 2>&1
来源：http://gf.521024.cn

[R40] 追加写日志
来源：http://uu.gzmigu.cn

echo "log" >> out.log
来源：http://js.colortex.cn

[R41] 丢弃输出
来源：http://mh.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://ax.bookmarksfly.cn

[R42] 输入重定向
来源：http://it.jianghongdianzi.cn

wc -l < a.txt
来源：http://gq.jctech888.com.cn

[R43] 按名字查找文件
来源：http://mz.gzmigu.cn

find . -name "*.log" -type f
来源：http://kh.szxytkj.cn

[R44] 按修改时间查找
来源：http://pn.asd995.cn

find . -mtime -7 -type f
来源：http://im.panjiajie.cn

[R45] 批量删除
来源：http://na.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://tg.muxihuayi.cn

[R46] 递归替换文件内容
来源：http://mb.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://on.newstarts.cn

[R47] sed 单行替换
来源：http://dg.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fi.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://dj.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://fe.521024.cn

[R49] awk 带条件
来源：http://oe.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rk.yuexingan06.cn

[R50] awk 求和
来源：http://kh.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gs.yuexingan06.cn

[R51] 排序去重取前几
来源：http://ut.haigaiapp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fa.colortex.cn

[R52] 统计行数
来源：http://id.wgjwhj.cn

wc -l a.txt
来源：http://xs.yuntaijiaju.cn

[R53] 查看文件头与实时尾
来源：http://vd.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lo.muxihuayi.cn

[R54] 比较两个文件
来源：http://ae.chemitech.net.cn

diff a.txt b.txt
来源：http://fc.newstarts.cn

[R55] 压缩与解压
来源：http://fm.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wj.newstarts.cn

[R56] 远程拷贝
来源：http://rb.huixiangedu.cn

scp file user@host:/path/
来源：http://ll.shxzukj.cn

[R57] 远程执行命令
来源：http://lr.yuntaijiaju.cn

ssh user@host 'uptime'
来源：http://pj.nszjky.cn

[R58] 下载文件
来源：http://kf.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ds.gzmigu.cn

[R59] 发 POST JSON
来源：http://ou.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kj.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://ds.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wo.wgjwhj.cn

[R61] 磁盘占用
来源：http://yq.wgjwhj.cn

df -h;  du -sh *
来源：http://mk.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://qw.bookmarksfly.cn

du -ah . | sort -rh | head -10
来源：http://kf.shtwfgs.cn

[R63] 内存与进程
来源：http://tu.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://un.bookmarksfly.cn

[R64] 结束进程
来源：http://uf.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://ky.gzmigu.cn

[R65] 查看端口占用
来源：http://rh.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ef.9csxet.cn

[R66] 定时任务
来源：http://os.muxihuayi.cn

crontab -e;  crontab -l
来源：http://ws.huanxung.cn

[R67] 生成随机十六进制串
来源：http://lt.shtwfgs.cn

openssl rand -hex 16
来源：http://do.chemitech.net.cn

[R68] 计算文件校验值
来源：http://ui.hnjuh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tm.panjiajie.cn

[R69] 生成随机密码
来源：http://oe.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://qy.newstarts.cn

[R70] 时间戳与互转
来源：http://vm.huixinmuqiang.cn

date +%s;  date -d @1700000000
来源：http://qy.colortex.cn

[R71] 日期格式化
来源：http://sd.bjjhwx.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dn.nszjky.cn

[R72] 等待端口就绪
来源：http://sc.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://eh.lnxyls.cn

[R73] 分割大日志
来源：http://mx.hahajie.cn

split -l 1000 big.log part_
来源：http://da.shxzukj.cn

[R74] 批量重命名
来源：http://tk.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ib.bookmarksfly.cn

[R75] 导出环境变量
来源：http://iv.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://oa.shtwfgs.cn

[R76] 使用临时文件
来源：http://yt.szxytkj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ej.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://tn.shxzukj.cn

read -rp "请输入: " ans
来源：http://uo.panjiajie.cn

[R78] 交互式菜单
来源：http://sc.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jt.haigaiapp.cn

[R79] 解析命令行选项
来源：http://ia.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://go.asd995.cn

[R80] 查看脚本执行耗时
来源：http://jh.panjiajie.cn

time ./run.sh
来源：http://yc.yuntaijiaju.cn

================================================================================
来源：http://ns.huixinmuqiang.cn

S. C / C++ 专题
来源：http://dm.wgjwhj.cn

================================================================================
来源：http://dt.chemitech.net.cn

[S01] C：Hello World
来源：http://lh.szxytkj.cn

#include <stdio.h>
来源：http://xx.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ex.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://tw.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://ks.bookmarksfly.cn

[S03] C：读入整数
来源：http://fe.lnxyls.cn

int x; scanf("%d", &x);
来源：http://ri.shxzukj.cn

[S04] C：字符串复制
来源：http://bc.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gi.asd995.cn

[S05] C：字符串长度
来源：http://tc.shxzukj.cn

strlen(s)
来源：http://gp.muxihuayi.cn

[S06] C：字符串比较
来源：http://ec.nszjky.cn

strcmp(a, b) == 0
来源：http://xe.shxzukj.cn

[S07] C：数组遍历求和
来源：http://ce.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jx.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://cw.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cf.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://cv.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mz.nicolike.cn

[S10] C：指针与解引用
来源：http://ot.nszjky.cn

int *p = &a;  *p = 5;
来源：http://st.wgjwhj.cn

[S11] C：逐行读文件
来源：http://jf.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://jk.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wu.newstarts.cn

fclose(f);
来源：http://mm.colortex.cn

[S12] C：写文件
来源：http://hx.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kd.gzmigu.cn

[S13] C：宏定义
来源：http://eg.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ei.wgjwhj.cn

[S14] C：枚举
来源：http://xo.yuntaijiaju.cn


<!-- 参考信息 -->