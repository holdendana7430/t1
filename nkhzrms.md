代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qq.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://iu.nszjky.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ex.wgjwhj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sq.521024.cn

[Q33] 多列分组
来源：http://md.gzmigu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kx.chemitech.net.cn

[Q34] 每组取第一条
来源：http://by.yuntaijiaju.cn

SELECT * FROM (
来源：http://mo.9csxet.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ul.yuexingan06.cn

) t WHERE rn = 1;
来源：http://oh.panjiajie.cn

[Q35] 内连接
来源：http://on.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pv.haigaiapp.cn

[Q36] 左连接
来源：http://xi.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kl.nicolike.cn

[Q37] 右连接
来源：http://zx.yuexingan06.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://me.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yg.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ql.shxzskj.cn

[Q39] 自连接（查上下级）
来源：http://nc.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wl.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ub.panjiajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sa.huanxung.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ty.huixiangedu.cn

[Q41] 多表连接
来源：http://vk.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wy.huixiangedu.cn

JOIN users u ON u.id = o.user_id
来源：http://oz.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://ny.shtwfgs.cn

[Q42] 连接条件附加过滤
来源：http://oo.asd995.cn

SELECT u.name, o.amount FROM users u
来源：http://dx.bookmarksfly.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wi.hahajie.cn

[Q43] 标量子查询
来源：http://si.chemitech.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tr.lnxyls.cn

[Q44] IN 子查询
来源：http://yu.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nj.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://lw.huixinmuqiang.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zt.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://oe.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pq.szxytkj.cn

[Q47] 与平均值比较
来源：http://bt.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sh.jctech888.com.cn

[Q48] CTE 公用表表达式
来源：http://nt.szsharing.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qf.bjjhwx.cn

SELECT * FROM t WHERE c > 5;
来源：http://di.asd995.cn

[Q49] 更新单行
来源：http://iv.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nt.lnxyls.cn

[Q50] 批量更新
来源：http://dk.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xo.haigaiapp.cn

[Q51] 用子查询更新
来源：http://gw.9csxet.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oh.muxihuayi.cn

[Q52] 删除指定行
来源：http://pa.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://rl.chemitech.net.cn

[Q53] 按条件删除
来源：http://qk.wgjwhj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ik.panjiajie.cn

[Q54] 清空表
来源：http://xi.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://zv.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://kv.yuntaijiaju.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oi.yuexingan06.cn

[Q56] 密集排名（并列不占位）
来源：http://et.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ls.wgjwhj.cn

[Q57] 行号
来源：http://uu.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jg.colortex.cn

[Q58] 累计求和
来源：http://zm.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://en.shxzukj.cn

[Q59] 分组内累计
来源：http://gc.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hx.haigaiapp.cn

[Q60] 取上一行 / 下一行
来源：http://if.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://eg.nszjky.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sv.haigaiapp.cn

[Q61] 移动平均
来源：http://lz.521024.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gh.gzmigu.cn

[Q62] 分组占比
来源：http://np.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ln.shxzukj.cn

[Q63] 开启事务
来源：http://ba.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://co.jctech888.com.cn

[Q64] 提交事务
来源：http://wl.szxytkj.cn

COMMIT;
来源：http://lg.shxzskj.cn

[Q65] 回滚事务
来源：http://cx.asd995.cn

ROLLBACK;
来源：http://yj.panjiajie.cn

[Q66] 行锁查询
来源：http://fj.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vx.gzmigu.cn

[Q67] 设置隔离级别
来源：http://mt.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://la.hahajie.cn

[Q68] 保存点
来源：http://je.haigaiapp.cn

SAVEPOINT sp1;
来源：http://ri.lnxyls.cn

ROLLBACK TO sp1;
来源：http://ic.hnjuh.cn

[Q69] 查看执行计划
来源：http://xh.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ru.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://sl.shxzukj.cn

ANALYZE TABLE users;
来源：http://bb.shxzskj.cn

[Q71] 查看建表语句
来源：http://tu.gzmigu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rp.shxzukj.cn

[Q72] 查看索引
来源：http://cy.521024.cn

SHOW INDEX FROM users;
来源：http://zg.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://ct.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pg.shtwfgs.cn

[Q74] 强制使用索引
来源：http://oj.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ch.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://wx.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vy.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://do.huixiangedu.cn

[Q76] 按天统计
来源：http://pr.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mt.bookmarksfly.cn

[Q77] 时间加减
来源：http://ib.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yp.huixinmuqiang.cn

[Q78] 当前时间
来源：http://jd.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nu.bjjhwx.cn

[Q79] 字符串拼接
来源：http://lo.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mt.yuexingan06.cn

[Q80] 字符串截取
来源：http://ex.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ex.521024.cn

[Q81] 字符串替换
来源：http://se.szsharing.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wi.bookmarksfly.cn

[Q82] 字符长度与字节长度
来源：http://ct.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://px.szxytkj.cn

[Q83] 大小写转换
来源：http://io.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kj.colortex.cn

[Q84] 去除首尾空格
来源：http://sb.colortex.cn

SELECT TRIM(name) FROM users;
来源：http://ej.521024.cn

[Q85] 数值取整
来源：http://mh.bookmarksfly.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wa.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://er.bjjhwx.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xi.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://wk.yuexingan06.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wc.chemitech.net.cn

[Q88] 行转列（条件聚合）
来源：http://ns.newstarts.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lk.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ga.shxzskj.cn

[Q89] 判断表是否存在
来源：http://nm.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zy.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://gk.huanxung.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yuexingan06.cn

================================================================================
来源：http://ag.huixinmuqiang.cn

R. Bash 专题
来源：http://xc.gzmigu.cn

================================================================================
来源：http://ci.shxzskj.cn

[R01] shebang 与严格模式
来源：http://rs.haigaiapp.cn

#!/usr/bin/env bash
来源：http://uv.jctech888.com.cn

set -euo pipefail
来源：http://ax.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://ym.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://qi.newstarts.cn

[R03] 只读变量
来源：http://rl.panjiajie.cn

readonly PI=3.14
来源：http://zd.yuntaijiaju.cn

[R04] 位置参数
来源：http://jl.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bh.haigaiapp.cn

[R05] 参数默认值
来源：http://jt.bjjhwx.cn

name="${1:-default}"
来源：http://ex.panjiajie.cn

[R06] 判断命令是否存在
来源：http://sn.gzmigu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cw.lnxyls.cn

[R07] if 判断文件
来源：http://bp.hahajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ep.hahajie.cn

[R08] 数值比较
来源：http://py.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sh.shxzukj.cn

[R09] 字符串比较
来源：http://ms.bookmarksfly.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://db.shtwfgs.cn

[R10] 正则匹配
来源：http://os.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kx.jianghongdianzi.cn

[R11] case 多分支
来源：http://oc.huixinmuqiang.cn

case "$1" in
来源：http://bp.huixinmuqiang.cn

start) echo "启动" ;;
来源：http://th.521024.cn

stop)  echo "停止" ;;
来源：http://da.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://su.huanxung.cn

esac
来源：http://fh.521024.cn

[R12] for 遍历文件
来源：http://yz.9csxet.cn

for f in *.txt; do echo "$f"; done
来源：http://sb.colortex.cn

[R13] for 计数循环
来源：http://wu.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://lv.hnjuh.cn

[R14] C 风格 for
来源：http://bh.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gx.asd995.cn

[R15] while 逐行读文件
来源：http://lo.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ec.huixinmuqiang.cn

[R16] until 等待条件
来源：http://iu.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ms.nicolike.cn

[R17] 数组定义与取值
来源：http://qf.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ex.hahajie.cn

[R18] 遍历数组
来源：http://jl.nicolike.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hn.muxihuayi.cn

[R19] 数组长度
来源：http://oi.9csxet.cn

echo "${#arr[@]}"
来源：http://xm.panjiajie.cn

[R20] 关联数组（字典）
来源：http://we.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pv.newstarts.cn

[R21] 字符串长度
来源：http://qx.hnjuh.cn

echo "${#s}"
来源：http://ct.hnjuh.cn

[R22] 截取子串
来源：http://eo.panjiajie.cn

echo "${s:0:5}"
来源：http://mf.hnjuh.cn

[R23] 字符串替换
来源：http://so.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zb.chemitech.net.cn

[R24] 大小写转换
来源：http://ot.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ud.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://jy.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pj.bookmarksfly.cn

[R26] 命令替换
来源：http://yb.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://bn.521024.cn

[R27] 算术展开
来源：http://jj.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://uc.shxzukj.cn

[R28] 浮点运算
来源：http://zh.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://nn.lnxyls.cn

[R29] 定义函数
来源：http://zv.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gz.lnxyls.cn

[R30] 函数返回状态码
来源：http://hy.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://eo.huixinmuqiang.cn

[R31] 局部变量
来源：http://bn.bjjhwx.cn

f() { local x=1; echo "$x"; }
来源：http://vw.szxytkj.cn

[R32] 参数个数校验
来源：http://ko.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ma.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://xy.hnjuh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rj.panjiajie.cn

[R34] 退出时清理
来源：http://fp.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lj.shxzukj.cn

[R35] 后台执行并等待
来源：http://aq.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kn.jianghongdianzi.cn

[R36] 并发执行多个任务
来源：http://mv.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://av.nszjky.cn

[R37] 把输出赋给变量
来源：http://bl.shxzskj.cn

files=$(ls -1)
来源：http://rd.jianghongdianzi.cn

[R38] 管道串联
来源：http://jl.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://dm.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://fr.lnxyls.cn

cmd > out.log 2>&1
来源：http://uo.chemitech.net.cn

[R40] 追加写日志
来源：http://wd.nszjky.cn

echo "log" >> out.log
来源：http://gq.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://lz.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://dj.hnjuh.cn

[R42] 输入重定向
来源：http://te.shxzukj.cn

wc -l < a.txt
来源：http://mc.521024.cn

[R43] 按名字查找文件
来源：http://yv.newstarts.cn

find . -name "*.log" -type f
来源：http://ry.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://bo.yuexingan06.cn

find . -mtime -7 -type f
来源：http://iv.bookmarksfly.cn

[R45] 批量删除
来源：http://iy.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://yp.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://xn.shtwfgs.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nj.huixiangedu.cn

[R47] sed 单行替换
来源：http://xo.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bd.szxytkj.cn

[R48] awk 取指定列
来源：http://li.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://lu.asd995.cn

[R49] awk 带条件
来源：http://lo.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pq.bjjhwx.cn

[R50] awk 求和
来源：http://lp.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ly.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://pd.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://la.lnxyls.cn

[R52] 统计行数
来源：http://nj.nszjky.cn

wc -l a.txt
来源：http://wn.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://ua.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://up.nszjky.cn

[R54] 比较两个文件
来源：http://go.panjiajie.cn

diff a.txt b.txt
来源：http://ab.hahajie.cn

[R55] 压缩与解压
来源：http://ik.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xj.shxzukj.cn

[R56] 远程拷贝
来源：http://iv.lnxyls.cn

scp file user@host:/path/
来源：http://yc.521024.cn

[R57] 远程执行命令
来源：http://nz.yuntaijiaju.cn

ssh user@host 'uptime'
来源：http://mr.szsharing.cn

[R58] 下载文件
来源：http://zm.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ih.haigaiapp.cn

[R59] 发 POST JSON
来源：http://ye.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qq.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://nc.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dx.hahajie.cn

[R61] 磁盘占用
来源：http://io.haigaiapp.cn

df -h;  du -sh *
来源：http://lc.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://yk.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://yj.nicolike.cn

[R63] 内存与进程
来源：http://nw.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://kx.bookmarksfly.cn

[R64] 结束进程
来源：http://bf.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://fx.nicolike.cn

[R65] 查看端口占用
来源：http://ld.huixinmuqiang.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fq.panjiajie.cn

[R66] 定时任务
来源：http://ht.szxytkj.cn

crontab -e;  crontab -l
来源：http://yk.nszjky.cn

[R67] 生成随机十六进制串
来源：http://yw.shtwfgs.cn

openssl rand -hex 16
来源：http://wg.newstarts.cn

[R68] 计算文件校验值
来源：http://pe.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wv.haigaiapp.cn

[R69] 生成随机密码
来源：http://tj.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://ni.haigaiapp.cn

[R70] 时间戳与互转
来源：http://rj.huixiangedu.cn

date +%s;  date -d @1700000000
来源：http://kb.colortex.cn

[R71] 日期格式化
来源：http://at.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uj.huixinmuqiang.cn

[R72] 等待端口就绪
来源：http://de.newstarts.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bs.szsharing.cn

[R73] 分割大日志
来源：http://il.jctech888.com.cn

split -l 1000 big.log part_
来源：http://nv.9csxet.cn

[R74] 批量重命名
来源：http://kd.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xv.huanxung.cn

[R75] 导出环境变量
来源：http://zg.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://pv.nicolike.cn

[R76] 使用临时文件
来源：http://bo.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sr.muxihuayi.cn

[R77] 读取用户输入
来源：http://pc.wgjwhj.cn

read -rp "请输入: " ans
来源：http://ij.szxytkj.cn

[R78] 交互式菜单
来源：http://kq.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cn.shtwfgs.cn

[R79] 解析命令行选项
来源：http://ll.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kc.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://cf.yuexingan06.cn

time ./run.sh
来源：http://st.asd995.cn

================================================================================
来源：http://iw.lnxyls.cn


<!-- 参考信息 -->