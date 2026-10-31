代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zc.hahajie.cn

[Q32] 分组拼接字符串
来源：http://bz.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xk.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xp.nszjky.cn

[Q33] 多列分组
来源：http://sc.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dr.521024.cn

[Q34] 每组取第一条
来源：http://ns.shxzukj.cn

SELECT * FROM (
来源：http://cd.panjiajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ph.bookmarksfly.cn

) t WHERE rn = 1;
来源：http://gw.wgjwhj.cn

[Q35] 内连接
来源：http://ip.szsharing.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pd.9csxet.cn

[Q36] 左连接
来源：http://at.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ws.shxzskj.cn

[Q37] 右连接
来源：http://fk.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tl.huanxung.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nb.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jv.asd995.cn

[Q39] 自连接（查上下级）
来源：http://rh.bookmarksfly.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vl.huixiangedu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ee.huixinmuqiang.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ju.yuntaijiaju.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nj.gzmigu.cn

[Q41] 多表连接
来源：http://at.shxzukj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gd.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://dd.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://hf.colortex.cn

[Q42] 连接条件附加过滤
来源：http://vd.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://wl.muxihuayi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zq.9csxet.cn

[Q43] 标量子查询
来源：http://cs.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ef.panjiajie.cn

[Q44] IN 子查询
来源：http://hg.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tb.bookmarksfly.cn

[Q45] EXISTS 判断存在
来源：http://fx.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://il.chemitech.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ao.haigaiapp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ji.gzmigu.cn

[Q47] 与平均值比较
来源：http://ty.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jf.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://ld.huixiangedu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cl.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://dn.bookmarksfly.cn

[Q49] 更新单行
来源：http://tm.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ft.asd995.cn

[Q50] 批量更新
来源：http://bv.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bb.huixiangedu.cn

[Q51] 用子查询更新
来源：http://dm.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sn.chemitech.net.cn

[Q52] 删除指定行
来源：http://om.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://ny.bjjhwx.cn

[Q53] 按条件删除
来源：http://si.asd995.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rn.jctech888.com.cn

[Q54] 清空表
来源：http://ti.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://ib.shtwfgs.cn

[Q55] 排名（并列占位）
来源：http://sl.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ly.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://xz.bjjhwx.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mf.chemitech.net.cn

[Q57] 行号
来源：http://cg.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xc.shxzukj.cn

[Q58] 累计求和
来源：http://qa.nicolike.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pb.szsharing.cn

[Q59] 分组内累计
来源：http://si.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sa.521024.cn

[Q60] 取上一行 / 下一行
来源：http://si.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wy.shtwfgs.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://de.huixinmuqiang.cn

[Q61] 移动平均
来源：http://bw.lnxyls.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qt.colortex.cn

[Q62] 分组占比
来源：http://wa.hnjuh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fr.asd995.cn

[Q63] 开启事务
来源：http://kj.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bz.lnxyls.cn

[Q64] 提交事务
来源：http://cz.gzmigu.cn

COMMIT;
来源：http://fc.szsharing.cn

[Q65] 回滚事务
来源：http://xq.lnxyls.cn

ROLLBACK;
来源：http://kc.asd995.cn

[Q66] 行锁查询
来源：http://ud.colortex.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pm.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://cv.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mm.colortex.cn

[Q68] 保存点
来源：http://pg.panjiajie.cn

SAVEPOINT sp1;
来源：http://jk.hnjuh.cn

ROLLBACK TO sp1;
来源：http://ry.gzmigu.cn

[Q69] 查看执行计划
来源：http://pe.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ph.hahajie.cn

[Q70] 更新统计信息
来源：http://gm.lnxyls.cn

ANALYZE TABLE users;
来源：http://hl.newstarts.cn

[Q71] 查看建表语句
来源：http://nr.nszjky.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jg.yuexingan06.cn

[Q72] 查看索引
来源：http://ng.haigaiapp.cn

SHOW INDEX FROM users;
来源：http://yb.jianghongdianzi.cn

[Q73] 查看表状态
来源：http://an.shxzskj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qv.hnjuh.cn

[Q74] 强制使用索引
来源：http://wv.jianghongdianzi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jz.shxzskj.cn

[Q75] 日期格式化
来源：http://gv.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://id.bjjhwx.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eq.huixinmuqiang.cn

[Q76] 按天统计
来源：http://kx.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uo.haigaiapp.cn

[Q77] 时间加减
来源：http://sv.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fz.yuexingan06.cn

[Q78] 当前时间
来源：http://jd.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lr.521024.cn

[Q79] 字符串拼接
来源：http://as.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gg.nicolike.cn

[Q80] 字符串截取
来源：http://rr.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dd.521024.cn

[Q81] 字符串替换
来源：http://vw.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fc.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://el.yuexingan06.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://si.huixiangedu.cn

[Q83] 大小写转换
来源：http://ke.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yz.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://ph.nicolike.cn

SELECT TRIM(name) FROM users;
来源：http://hk.chemitech.net.cn

[Q85] 数值取整
来源：http://xz.jianghongdianzi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tz.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://uj.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ej.shxzukj.cn

[Q87] JSON 字段做条件
来源：http://kw.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kg.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://fc.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bx.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kd.huanxung.cn

[Q89] 判断表是否存在
来源：http://fy.jctech888.com.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qv.huixiangedu.cn

[Q90] 生成序号列
来源：http://si.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://do.521024.cn

================================================================================
来源：http://iz.newstarts.cn

R. Bash 专题
来源：http://mh.panjiajie.cn

================================================================================
来源：http://vh.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://ts.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://ih.shxzskj.cn

set -euo pipefail
来源：http://sr.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://an.asd995.cn

name="Tom"; echo "$name"
来源：http://ld.nicolike.cn

[R03] 只读变量
来源：http://eo.wgjwhj.cn

readonly PI=3.14
来源：http://id.bookmarksfly.cn

[R04] 位置参数
来源：http://mk.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ac.yuntaijiaju.cn

[R05] 参数默认值
来源：http://hl.hahajie.cn

name="${1:-default}"
来源：http://bt.huixinmuqiang.cn

[R06] 判断命令是否存在
来源：http://bl.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uy.colortex.cn

[R07] if 判断文件
来源：http://el.nszjky.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ls.yuexingan06.cn

[R08] 数值比较
来源：http://yk.panjiajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qr.bookmarksfly.cn

[R09] 字符串比较
来源：http://hx.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fl.yuntaijiaju.cn

[R10] 正则匹配
来源：http://gm.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hj.9csxet.cn

[R11] case 多分支
来源：http://gq.shxzskj.cn

case "$1" in
来源：http://tw.huixiangedu.cn

start) echo "启动" ;;
来源：http://br.lnxyls.cn

stop)  echo "停止" ;;
来源：http://id.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://kf.gzmigu.cn

esac
来源：http://qu.newstarts.cn

[R12] for 遍历文件
来源：http://lz.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://nb.hahajie.cn

[R13] for 计数循环
来源：http://bu.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://vx.lnxyls.cn

[R14] C 风格 for
来源：http://hh.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ol.szsharing.cn

[R15] while 逐行读文件
来源：http://gx.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hj.bjjhwx.cn

[R16] until 等待条件
来源：http://eu.nszjky.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jb.muxihuayi.cn

[R17] 数组定义与取值
来源：http://wo.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dj.bjjhwx.cn

[R18] 遍历数组
来源：http://ux.hnjuh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dd.yuntaijiaju.cn

[R19] 数组长度
来源：http://oa.gzmigu.cn

echo "${#arr[@]}"
来源：http://ks.shxzskj.cn

[R20] 关联数组（字典）
来源：http://xq.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gx.wgjwhj.cn

[R21] 字符串长度
来源：http://ib.newstarts.cn

echo "${#s}"
来源：http://by.bjjhwx.cn

[R22] 截取子串
来源：http://br.muxihuayi.cn

echo "${s:0:5}"
来源：http://vh.muxihuayi.cn

[R23] 字符串替换
来源：http://dy.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ee.shxzukj.cn

[R24] 大小写转换
来源：http://iy.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sh.521024.cn

[R25] 去后缀 / 去前缀
来源：http://zb.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cg.haigaiapp.cn

[R26] 命令替换
来源：http://hu.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://va.bjjhwx.cn

[R27] 算术展开
来源：http://pz.colortex.cn

echo $((1 + 2 * 3))
来源：http://pc.nszjky.cn

[R28] 浮点运算
来源：http://kr.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://pj.lnxyls.cn

[R29] 定义函数
来源：http://no.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pv.9csxet.cn

[R30] 函数返回状态码
来源：http://mm.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://vm.hahajie.cn

[R31] 局部变量
来源：http://aq.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://in.nszjky.cn

[R32] 参数个数校验
来源：http://iz.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nm.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://hs.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eb.newstarts.cn

[R34] 退出时清理
来源：http://sn.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gc.gzmigu.cn

[R35] 后台执行并等待
来源：http://aj.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mc.jianghongdianzi.cn

[R36] 并发执行多个任务
来源：http://kn.wgjwhj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vm.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://mw.asd995.cn

files=$(ls -1)
来源：http://ql.jianghongdianzi.cn

[R38] 管道串联
来源：http://ad.nicolike.cn

cat a.txt | grep -i error | wc -l
来源：http://zk.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://sq.haigaiapp.cn

cmd > out.log 2>&1
来源：http://um.huixinmuqiang.cn

[R40] 追加写日志
来源：http://wl.yuntaijiaju.cn

echo "log" >> out.log
来源：http://at.haigaiapp.cn

[R41] 丢弃输出
来源：http://uw.521024.cn

cmd >/dev/null 2>&1
来源：http://vt.huixiangedu.cn

[R42] 输入重定向
来源：http://fr.shxzukj.cn

wc -l < a.txt
来源：http://kx.huanxung.cn

[R43] 按名字查找文件
来源：http://qi.521024.cn

find . -name "*.log" -type f
来源：http://lf.newstarts.cn

[R44] 按修改时间查找
来源：http://kh.newstarts.cn

find . -mtime -7 -type f
来源：http://oc.hnjuh.cn

[R45] 批量删除
来源：http://wx.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://oi.yuexingan06.cn

[R46] 递归替换文件内容
来源：http://dz.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ro.shtwfgs.cn

[R47] sed 单行替换
来源：http://hn.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cm.shxzukj.cn

[R48] awk 取指定列
来源：http://go.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://xi.shxzukj.cn

[R49] awk 带条件
来源：http://gp.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hn.colortex.cn

[R50] awk 求和
来源：http://cg.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jg.9csxet.cn

[R51] 排序去重取前几
来源：http://zm.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hi.asd995.cn

[R52] 统计行数
来源：http://yd.9csxet.cn

wc -l a.txt
来源：http://uu.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://wa.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ms.nicolike.cn

[R54] 比较两个文件
来源：http://fj.hahajie.cn

diff a.txt b.txt
来源：http://ka.yuexingan06.cn

[R55] 压缩与解压
来源：http://yf.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yq.newstarts.cn

[R56] 远程拷贝
来源：http://hk.wgjwhj.cn

scp file user@host:/path/
来源：http://ix.chemitech.net.cn

[R57] 远程执行命令
来源：http://mg.yuntaijiaju.cn

ssh user@host 'uptime'
来源：http://js.colortex.cn

[R58] 下载文件
来源：http://ka.hnjuh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ev.9csxet.cn

[R59] 发 POST JSON
来源：http://kr.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uy.nicolike.cn

[R60] 只看 HTTP 状态码
来源：http://jm.muxihuayi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uo.yuexingan06.cn

[R61] 磁盘占用
来源：http://xx.huixinmuqiang.cn

df -h;  du -sh *
来源：http://og.huixinmuqiang.cn

[R62] 找最占空间的文件
来源：http://jo.9csxet.cn

du -ah . | sort -rh | head -10
来源：http://wq.bjjhwx.cn

[R63] 内存与进程
来源：http://cw.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://yq.gzmigu.cn

[R64] 结束进程
来源：http://md.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://yf.wgjwhj.cn

[R65] 查看端口占用
来源：http://gy.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wz.asd995.cn

[R66] 定时任务
来源：http://cz.lnxyls.cn

crontab -e;  crontab -l
来源：http://nb.hahajie.cn

[R67] 生成随机十六进制串
来源：http://iz.chemitech.net.cn

openssl rand -hex 16
来源：http://tc.colortex.cn

[R68] 计算文件校验值
来源：http://ip.gzmigu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mx.chemitech.net.cn

[R69] 生成随机密码
来源：http://yq.huanxung.cn

head -c 16 /dev/urandom | base64
来源：http://zt.nicolike.cn

[R70] 时间戳与互转
来源：http://sm.colortex.cn

date +%s;  date -d @1700000000
来源：http://hs.shxzukj.cn

[R71] 日期格式化
来源：http://hj.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fx.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://xy.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ob.jctech888.com.cn

[R73] 分割大日志
来源：http://cb.huanxung.cn

split -l 1000 big.log part_
来源：http://jl.nicolike.cn

[R74] 批量重命名
来源：http://tr.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ms.szsharing.cn

[R75] 导出环境变量
来源：http://aj.szsharing.cn

export PATH="$HOME/bin:$PATH"
来源：http://fg.jctech888.com.cn

[R76] 使用临时文件
来源：http://uk.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zl.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://nx.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://ag.szxytkj.cn

[R78] 交互式菜单
来源：http://rw.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rv.chemitech.net.cn

[R79] 解析命令行选项
来源：http://zp.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dx.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://ek.bookmarksfly.cn

time ./run.sh
来源：http://ez.huixiangedu.cn

================================================================================
来源：http://ei.colortex.cn


<!-- 参考信息 -->