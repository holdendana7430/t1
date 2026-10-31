代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://ap.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://ue.jctech888.com.cn

JOIN products p ON p.id = o.product_id;
来源：http://od.shxzskj.cn

[Q42] 连接条件附加过滤
来源：http://nd.hnjuh.cn

SELECT u.name, o.amount FROM users u
来源：http://kz.shxzukj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fc.yuntaijiaju.cn

[Q43] 标量子查询
来源：http://xn.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iv.521024.cn

[Q44] IN 子查询
来源：http://mw.bjjhwx.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ae.asd995.cn

[Q45] EXISTS 判断存在
来源：http://hr.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vb.521024.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vl.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wh.szxytkj.cn

[Q47] 与平均值比较
来源：http://zt.nicolike.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fk.jianghongdianzi.cn

[Q48] CTE 公用表表达式
来源：http://ap.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cq.jianghongdianzi.cn

SELECT * FROM t WHERE c > 5;
来源：http://qg.szsharing.cn

[Q49] 更新单行
来源：http://us.asd995.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pm.hnjuh.cn

[Q50] 批量更新
来源：http://ju.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uq.nicolike.cn

[Q51] 用子查询更新
来源：http://un.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jo.huixiangedu.cn

[Q52] 删除指定行
来源：http://yy.huanxung.cn

DELETE FROM users WHERE id = 10;
来源：http://tr.shxzukj.cn

[Q53] 按条件删除
来源：http://or.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hc.muxihuayi.cn

[Q54] 清空表
来源：http://hy.asd995.cn

TRUNCATE TABLE logs;
来源：http://ug.asd995.cn

[Q55] 排名（并列占位）
来源：http://or.hnjuh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zp.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://kf.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bc.jianghongdianzi.cn

[Q57] 行号
来源：http://zh.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wn.9csxet.cn

[Q58] 累计求和
来源：http://cg.shxzskj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cq.521024.cn

[Q59] 分组内累计
来源：http://wp.colortex.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hg.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://xv.yuexingan06.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mp.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ot.jctech888.com.cn

[Q61] 移动平均
来源：http://pp.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bn.shtwfgs.cn

[Q62] 分组占比
来源：http://bt.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fu.nszjky.cn

[Q63] 开启事务
来源：http://az.yuexingan06.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uu.haigaiapp.cn

[Q64] 提交事务
来源：http://xq.nszjky.cn

COMMIT;
来源：http://vq.nicolike.cn

[Q65] 回滚事务
来源：http://og.shxzukj.cn

ROLLBACK;
来源：http://iz.9csxet.cn

[Q66] 行锁查询
来源：http://hg.muxihuayi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zz.9csxet.cn

[Q67] 设置隔离级别
来源：http://pt.gzmigu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://om.szsharing.cn

[Q68] 保存点
来源：http://ga.shxzskj.cn

SAVEPOINT sp1;
来源：http://hs.huanxung.cn

ROLLBACK TO sp1;
来源：http://gi.shtwfgs.cn

[Q69] 查看执行计划
来源：http://uw.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qi.shxzskj.cn

[Q70] 更新统计信息
来源：http://et.shxzukj.cn

ANALYZE TABLE users;
来源：http://wc.nszjky.cn

[Q71] 查看建表语句
来源：http://xq.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zk.nszjky.cn

[Q72] 查看索引
来源：http://ab.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://xf.muxihuayi.cn

[Q73] 查看表状态
来源：http://dq.jctech888.com.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rj.shxzskj.cn

[Q74] 强制使用索引
来源：http://fl.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yr.bjjhwx.cn

[Q75] 日期格式化
来源：http://yq.nicolike.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ps.muxihuayi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ot.lnxyls.cn

[Q76] 按天统计
来源：http://kx.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rb.newstarts.cn

[Q77] 时间加减
来源：http://wz.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yy.lnxyls.cn

[Q78] 当前时间
来源：http://in.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ko.szsharing.cn

[Q79] 字符串拼接
来源：http://co.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ly.nicolike.cn

[Q80] 字符串截取
来源：http://ge.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ys.shxzukj.cn

[Q81] 字符串替换
来源：http://ly.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://au.chemitech.net.cn

[Q82] 字符长度与字节长度
来源：http://xy.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lk.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://fv.huanxung.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jy.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://vc.yuexingan06.cn

SELECT TRIM(name) FROM users;
来源：http://sp.huixiangedu.cn

[Q85] 数值取整
来源：http://ry.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ux.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://fx.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bi.bjjhwx.cn

[Q87] JSON 字段做条件
来源：http://bc.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wt.hahajie.cn

[Q88] 行转列（条件聚合）
来源：http://gh.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ko.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vu.szsharing.cn

[Q89] 判断表是否存在
来源：http://vj.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hv.shxzskj.cn

[Q90] 生成序号列
来源：http://bw.muxihuayi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oj.huanxung.cn

================================================================================
来源：http://ee.yuntaijiaju.cn

R. Bash 专题
来源：http://ab.jianghongdianzi.cn

================================================================================
来源：http://al.shxzskj.cn

[R01] shebang 与严格模式
来源：http://ey.muxihuayi.cn

#!/usr/bin/env bash
来源：http://xm.chemitech.net.cn

set -euo pipefail
来源：http://gg.9csxet.cn

[R02] 变量赋值与使用
来源：http://kh.newstarts.cn

name="Tom"; echo "$name"
来源：http://bo.yuexingan06.cn

[R03] 只读变量
来源：http://zb.bookmarksfly.cn

readonly PI=3.14
来源：http://es.lnxyls.cn

[R04] 位置参数
来源：http://qp.colortex.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ul.huanxung.cn

[R05] 参数默认值
来源：http://tn.gzmigu.cn

name="${1:-default}"
来源：http://gh.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://ra.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sq.muxihuayi.cn

[R07] if 判断文件
来源：http://bk.bjjhwx.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ia.huanxung.cn

[R08] 数值比较
来源：http://uc.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ws.chemitech.net.cn

[R09] 字符串比较
来源：http://fa.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hv.9csxet.cn

[R10] 正则匹配
来源：http://gn.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dn.haigaiapp.cn

[R11] case 多分支
来源：http://qg.yuexingan06.cn

case "$1" in
来源：http://ru.jctech888.com.cn

start) echo "启动" ;;
来源：http://ed.hnjuh.cn

stop)  echo "停止" ;;
来源：http://tx.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://zh.szsharing.cn

esac
来源：http://yu.lnxyls.cn

[R12] for 遍历文件
来源：http://uq.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://gp.huixinmuqiang.cn

[R13] for 计数循环
来源：http://dz.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://fi.gzmigu.cn

[R14] C 风格 for
来源：http://fn.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gj.nicolike.cn

[R15] while 逐行读文件
来源：http://yv.huixiangedu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ol.szxytkj.cn

[R16] until 等待条件
来源：http://yl.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dq.huanxung.cn

[R17] 数组定义与取值
来源：http://fp.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yc.szxytkj.cn

[R18] 遍历数组
来源：http://mh.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ci.shxzskj.cn

[R19] 数组长度
来源：http://pk.gzmigu.cn

echo "${#arr[@]}"
来源：http://ph.9csxet.cn

[R20] 关联数组（字典）
来源：http://cx.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nk.nszjky.cn

[R21] 字符串长度
来源：http://hh.hahajie.cn

echo "${#s}"
来源：http://pm.gzmigu.cn

[R22] 截取子串
来源：http://qp.jctech888.com.cn

echo "${s:0:5}"
来源：http://zn.huixinmuqiang.cn

[R23] 字符串替换
来源：http://lj.szxytkj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uu.9csxet.cn

[R24] 大小写转换
来源：http://un.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://eg.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://ri.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dg.9csxet.cn

[R26] 命令替换
来源：http://pq.colortex.cn

now=$(date +%F); echo "$now"
来源：http://fy.yuexingan06.cn

[R27] 算术展开
来源：http://kr.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://my.huanxung.cn

[R28] 浮点运算
来源：http://ur.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://dt.shxzskj.cn

[R29] 定义函数
来源：http://hp.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://na.shtwfgs.cn

[R30] 函数返回状态码
来源：http://yo.shxzskj.cn

f() { return 0; }; f || echo "失败了"
来源：http://hr.9csxet.cn

[R31] 局部变量
来源：http://lz.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://po.shxzukj.cn

[R32] 参数个数校验
来源：http://kl.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hg.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://fy.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hx.lnxyls.cn

[R34] 退出时清理
来源：http://zo.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xf.shtwfgs.cn

[R35] 后台执行并等待
来源：http://ny.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wq.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://te.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hk.huixinmuqiang.cn

[R37] 把输出赋给变量
来源：http://lk.jctech888.com.cn

files=$(ls -1)
来源：http://gu.yuntaijiaju.cn

[R38] 管道串联
来源：http://ev.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://ze.colortex.cn

[R39] 重定向标准输出与错误
来源：http://jj.gzmigu.cn

cmd > out.log 2>&1
来源：http://kr.muxihuayi.cn

[R40] 追加写日志
来源：http://gz.chemitech.net.cn

echo "log" >> out.log
来源：http://zq.gzmigu.cn

[R41] 丢弃输出
来源：http://cd.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://uz.lnxyls.cn

[R42] 输入重定向
来源：http://qm.wgjwhj.cn

wc -l < a.txt
来源：http://qn.muxihuayi.cn

[R43] 按名字查找文件
来源：http://bh.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://ew.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://gb.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://fk.huanxung.cn

[R45] 批量删除
来源：http://hd.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://vi.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://cw.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ji.chemitech.net.cn

[R47] sed 单行替换
来源：http://nm.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qj.lnxyls.cn

[R48] awk 取指定列
来源：http://dk.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://op.shxzskj.cn

[R49] awk 带条件
来源：http://qf.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lx.gzmigu.cn

[R50] awk 求和
来源：http://cg.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://de.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://np.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://er.huixinmuqiang.cn

[R52] 统计行数
来源：http://wc.asd995.cn

wc -l a.txt
来源：http://nf.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://hn.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bv.hnjuh.cn

[R54] 比较两个文件
来源：http://gu.huixinmuqiang.cn

diff a.txt b.txt
来源：http://gz.shtwfgs.cn

[R55] 压缩与解压
来源：http://pu.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ya.huixiangedu.cn

[R56] 远程拷贝
来源：http://pa.szsharing.cn

scp file user@host:/path/
来源：http://id.bjjhwx.cn

[R57] 远程执行命令
来源：http://ve.asd995.cn

ssh user@host 'uptime'
来源：http://ku.hnjuh.cn

[R58] 下载文件
来源：http://oe.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pc.szsharing.cn

[R59] 发 POST JSON
来源：http://nl.haigaiapp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bu.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://yx.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://so.panjiajie.cn

[R61] 磁盘占用
来源：http://gs.bookmarksfly.cn

df -h;  du -sh *
来源：http://jv.asd995.cn

[R62] 找最占空间的文件
来源：http://ot.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://ly.colortex.cn

[R63] 内存与进程
来源：http://of.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://tk.haigaiapp.cn

[R64] 结束进程
来源：http://la.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://ax.lnxyls.cn

[R65] 查看端口占用
来源：http://is.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hb.gzmigu.cn

[R66] 定时任务
来源：http://ee.9csxet.cn

crontab -e;  crontab -l
来源：http://tf.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://sa.lnxyls.cn

openssl rand -hex 16
来源：http://yn.shtwfgs.cn

[R68] 计算文件校验值
来源：http://oa.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fc.colortex.cn

[R69] 生成随机密码
来源：http://pw.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://cx.colortex.cn

[R70] 时间戳与互转
来源：http://tj.jianghongdianzi.cn

date +%s;  date -d @1700000000
来源：http://aw.shxzskj.cn

[R71] 日期格式化
来源：http://zt.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tr.chemitech.net.cn

[R72] 等待端口就绪
来源：http://cr.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ij.bookmarksfly.cn

[R73] 分割大日志
来源：http://lb.nicolike.cn

split -l 1000 big.log part_
来源：http://mi.bjjhwx.cn

[R74] 批量重命名
来源：http://eo.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ia.521024.cn

[R75] 导出环境变量
来源：http://nw.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://pm.lnxyls.cn

[R76] 使用临时文件
来源：http://qy.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rr.hnjuh.cn

[R77] 读取用户输入
来源：http://by.shxzskj.cn

read -rp "请输入: " ans
来源：http://iq.huixiangedu.cn

[R78] 交互式菜单
来源：http://no.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qy.521024.cn

[R79] 解析命令行选项
来源：http://vq.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dm.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://es.haigaiapp.cn

time ./run.sh
来源：http://rj.colortex.cn

================================================================================
来源：http://kw.gzmigu.cn

S. C / C++ 专题
来源：http://dw.jctech888.com.cn

================================================================================
来源：http://gw.szxytkj.cn

[S01] C：Hello World
来源：http://mn.521024.cn

#include <stdio.h>
来源：http://zr.newstarts.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ub.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://ev.lnxyls.cn

int a = 10; printf("%d\n", a);
来源：http://ny.shtwfgs.cn

[S03] C：读入整数
来源：http://ex.shxzukj.cn

int x; scanf("%d", &x);
来源：http://rn.9csxet.cn

[S04] C：字符串复制
来源：http://nd.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ah.jianghongdianzi.cn

[S05] C：字符串长度
来源：http://gl.szxytkj.cn

strlen(s)
来源：http://ec.bookmarksfly.cn

[S06] C：字符串比较
来源：http://zo.yuexingan06.cn

strcmp(a, b) == 0
来源：http://rx.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://aq.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wx.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://ea.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ue.asd995.cn

[S09] C：结构体定义与初始化
来源：http://pw.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nv.nszjky.cn

[S10] C：指针与解引用
来源：http://bl.nszjky.cn

int *p = &a;  *p = 5;
来源：http://un.newstarts.cn

[S11] C：逐行读文件
来源：http://lf.huixiangedu.cn


<!-- 参考信息 -->