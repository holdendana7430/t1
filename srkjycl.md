代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://xk.bookmarksfly.cn

[Q30] 分组统计
来源：http://ev.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yg.521024.cn

[Q31] 分组后过滤
来源：http://jx.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gu.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://cb.521024.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ev.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ad.huixinmuqiang.cn

[Q33] 多列分组
来源：http://vj.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zo.colortex.cn

[Q34] 每组取第一条
来源：http://so.521024.cn

SELECT * FROM (
来源：http://dw.gzmigu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zy.lnxyls.cn

) t WHERE rn = 1;
来源：http://yb.shtwfgs.cn

[Q35] 内连接
来源：http://zm.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sl.521024.cn

[Q36] 左连接
来源：http://ak.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zk.bookmarksfly.cn

[Q37] 右连接
来源：http://ty.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jx.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nf.shxzskj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qj.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://cs.szsharing.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dg.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nk.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ik.huanxung.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fd.bookmarksfly.cn

[Q41] 多表连接
来源：http://jn.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://iq.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://vl.szsharing.cn

JOIN products p ON p.id = o.product_id;
来源：http://yb.huixiangedu.cn

[Q42] 连接条件附加过滤
来源：http://ew.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://kw.gzmigu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rw.jctech888.com.cn

[Q43] 标量子查询
来源：http://yy.yuntaijiaju.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ku.wgjwhj.cn

[Q44] IN 子查询
来源：http://bb.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hk.huixiangedu.cn

[Q45] EXISTS 判断存在
来源：http://kx.bjjhwx.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wn.nszjky.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hy.shxzukj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://na.huanxung.cn

[Q47] 与平均值比较
来源：http://ke.yuntaijiaju.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pf.yuexingan06.cn

[Q48] CTE 公用表表达式
来源：http://ty.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://en.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://ls.szsharing.cn

[Q49] 更新单行
来源：http://ip.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cw.chemitech.net.cn

[Q50] 批量更新
来源：http://nx.panjiajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wk.lnxyls.cn

[Q51] 用子查询更新
来源：http://ht.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://be.huixiangedu.cn

[Q52] 删除指定行
来源：http://hg.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://zv.panjiajie.cn

[Q53] 按条件删除
来源：http://ff.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wc.szsharing.cn

[Q54] 清空表
来源：http://ci.colortex.cn

TRUNCATE TABLE logs;
来源：http://su.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://lg.lnxyls.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rm.shtwfgs.cn

[Q56] 密集排名（并列不占位）
来源：http://dm.shtwfgs.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ls.521024.cn

[Q57] 行号
来源：http://iu.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xe.nicolike.cn

[Q58] 累计求和
来源：http://sb.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qt.jctech888.com.cn

[Q59] 分组内累计
来源：http://sg.newstarts.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://af.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://ex.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pl.haigaiapp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pe.jctech888.com.cn

[Q61] 移动平均
来源：http://zi.nszjky.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jc.shxzskj.cn

[Q62] 分组占比
来源：http://fi.jianghongdianzi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://up.jianghongdianzi.cn

[Q63] 开启事务
来源：http://im.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gn.jctech888.com.cn

[Q64] 提交事务
来源：http://my.yuntaijiaju.cn

COMMIT;
来源：http://ie.szxytkj.cn

[Q65] 回滚事务
来源：http://cr.huanxung.cn

ROLLBACK;
来源：http://dx.asd995.cn

[Q66] 行锁查询
来源：http://bz.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ox.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://iy.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tl.hnjuh.cn

[Q68] 保存点
来源：http://eq.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://ly.shtwfgs.cn

ROLLBACK TO sp1;
来源：http://yf.yuexingan06.cn

[Q69] 查看执行计划
来源：http://wh.yuexingan06.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qs.jianghongdianzi.cn

[Q70] 更新统计信息
来源：http://yw.szxytkj.cn

ANALYZE TABLE users;
来源：http://hk.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://va.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jl.newstarts.cn

[Q72] 查看索引
来源：http://kn.gzmigu.cn

SHOW INDEX FROM users;
来源：http://wd.521024.cn

[Q73] 查看表状态
来源：http://va.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nr.jianghongdianzi.cn

[Q74] 强制使用索引
来源：http://sq.bookmarksfly.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://aq.nicolike.cn

[Q75] 日期格式化
来源：http://ql.nicolike.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dx.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uv.9csxet.cn

[Q76] 按天统计
来源：http://qz.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://so.9csxet.cn

[Q77] 时间加减
来源：http://ub.9csxet.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://th.hnjuh.cn

[Q78] 当前时间
来源：http://dh.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zm.huixiangedu.cn

[Q79] 字符串拼接
来源：http://pm.bookmarksfly.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ab.szsharing.cn

[Q80] 字符串截取
来源：http://ue.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ac.nicolike.cn

[Q81] 字符串替换
来源：http://lp.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nd.bookmarksfly.cn

[Q82] 字符长度与字节长度
来源：http://fp.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ui.shtwfgs.cn

[Q83] 大小写转换
来源：http://tk.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://br.gzmigu.cn

[Q84] 去除首尾空格
来源：http://iy.521024.cn

SELECT TRIM(name) FROM users;
来源：http://jb.yuntaijiaju.cn

[Q85] 数值取整
来源：http://sj.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mf.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://ry.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ca.newstarts.cn

[Q87] JSON 字段做条件
来源：http://wj.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qx.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://wq.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ci.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cj.9csxet.cn

[Q89] 判断表是否存在
来源：http://dd.szsharing.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ni.chemitech.net.cn

[Q90] 生成序号列
来源：http://ri.muxihuayi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hh.hnjuh.cn

================================================================================
来源：http://ml.huanxung.cn

R. Bash 专题
来源：http://ix.wgjwhj.cn

================================================================================
来源：http://ck.9csxet.cn

[R01] shebang 与严格模式
来源：http://zw.huixinmuqiang.cn

#!/usr/bin/env bash
来源：http://lp.521024.cn

set -euo pipefail
来源：http://fs.colortex.cn

[R02] 变量赋值与使用
来源：http://ze.bookmarksfly.cn

name="Tom"; echo "$name"
来源：http://vn.bookmarksfly.cn

[R03] 只读变量
来源：http://we.bookmarksfly.cn

readonly PI=3.14
来源：http://ps.nicolike.cn

[R04] 位置参数
来源：http://if.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://if.nicolike.cn

[R05] 参数默认值
来源：http://fa.yuntaijiaju.cn

name="${1:-default}"
来源：http://er.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://if.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qw.521024.cn

[R07] if 判断文件
来源：http://fe.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://da.wgjwhj.cn

[R08] 数值比较
来源：http://wk.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zn.muxihuayi.cn

[R09] 字符串比较
来源：http://fk.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fw.panjiajie.cn

[R10] 正则匹配
来源：http://ts.lnxyls.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mz.szxytkj.cn

[R11] case 多分支
来源：http://rp.chemitech.net.cn

case "$1" in
来源：http://pz.asd995.cn

start) echo "启动" ;;
来源：http://ed.panjiajie.cn

stop)  echo "停止" ;;
来源：http://bh.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://rx.gzmigu.cn

esac
来源：http://ft.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://qp.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://pi.jianghongdianzi.cn

[R13] for 计数循环
来源：http://lp.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://sp.colortex.cn

[R14] C 风格 for
来源：http://vm.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uc.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://vb.huanxung.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lw.newstarts.cn

[R16] until 等待条件
来源：http://mn.newstarts.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bs.521024.cn

[R17] 数组定义与取值
来源：http://yg.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cn.huanxung.cn

[R18] 遍历数组
来源：http://pg.9csxet.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bz.lnxyls.cn

[R19] 数组长度
来源：http://wm.muxihuayi.cn

echo "${#arr[@]}"
来源：http://ox.colortex.cn

[R20] 关联数组（字典）
来源：http://ir.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mm.panjiajie.cn

[R21] 字符串长度
来源：http://kg.haigaiapp.cn

echo "${#s}"
来源：http://ks.9csxet.cn

[R22] 截取子串
来源：http://uz.haigaiapp.cn

echo "${s:0:5}"
来源：http://aa.panjiajie.cn

[R23] 字符串替换
来源：http://bz.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eu.yuexingan06.cn

[R24] 大小写转换
来源：http://fh.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://du.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://pe.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qo.szxytkj.cn

[R26] 命令替换
来源：http://fy.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://ic.bookmarksfly.cn

[R27] 算术展开
来源：http://rs.9csxet.cn

echo $((1 + 2 * 3))
来源：http://np.shxzskj.cn

[R28] 浮点运算
来源：http://eo.nszjky.cn

echo "scale=2; 10/3" | bc
来源：http://gt.asd995.cn

[R29] 定义函数
来源：http://ke.yuntaijiaju.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ek.hahajie.cn

[R30] 函数返回状态码
来源：http://hh.9csxet.cn

f() { return 0; }; f || echo "失败了"
来源：http://iu.wgjwhj.cn

[R31] 局部变量
来源：http://ln.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://tn.shxzukj.cn

[R32] 参数个数校验
来源：http://qo.huixinmuqiang.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iw.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://is.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zo.colortex.cn

[R34] 退出时清理
来源：http://pv.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dm.colortex.cn

[R35] 后台执行并等待
来源：http://jh.yuexingan06.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uz.gzmigu.cn

[R36] 并发执行多个任务
来源：http://po.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ws.szxytkj.cn

[R37] 把输出赋给变量
来源：http://tn.gzmigu.cn

files=$(ls -1)
来源：http://bd.jianghongdianzi.cn

[R38] 管道串联
来源：http://vx.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://yt.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://rt.huanxung.cn

cmd > out.log 2>&1
来源：http://ng.asd995.cn

[R40] 追加写日志
来源：http://vb.jianghongdianzi.cn

echo "log" >> out.log
来源：http://dq.panjiajie.cn

[R41] 丢弃输出
来源：http://ii.newstarts.cn

cmd >/dev/null 2>&1
来源：http://qz.shxzskj.cn

[R42] 输入重定向
来源：http://qz.9csxet.cn

wc -l < a.txt
来源：http://zq.bjjhwx.cn

[R43] 按名字查找文件
来源：http://ks.huanxung.cn

find . -name "*.log" -type f
来源：http://ch.asd995.cn

[R44] 按修改时间查找
来源：http://bo.jctech888.com.cn

find . -mtime -7 -type f
来源：http://ud.huixiangedu.cn

[R45] 批量删除
来源：http://ws.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://xu.huanxung.cn

[R46] 递归替换文件内容
来源：http://uu.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ac.hnjuh.cn

[R47] sed 单行替换
来源：http://ta.shxzskj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://se.szxytkj.cn

[R48] awk 取指定列
来源：http://rs.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://qf.hahajie.cn

[R49] awk 带条件
来源：http://xp.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ia.shtwfgs.cn

[R50] awk 求和
来源：http://sj.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wt.hahajie.cn

[R51] 排序去重取前几
来源：http://bj.nszjky.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ux.asd995.cn

[R52] 统计行数
来源：http://qq.nszjky.cn

wc -l a.txt
来源：http://op.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://ac.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ae.hnjuh.cn

[R54] 比较两个文件
来源：http://zt.colortex.cn

diff a.txt b.txt
来源：http://fs.hnjuh.cn

[R55] 压缩与解压
来源：http://zr.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://my.shxzskj.cn

[R56] 远程拷贝
来源：http://sr.lnxyls.cn

scp file user@host:/path/
来源：http://gp.huanxung.cn

[R57] 远程执行命令
来源：http://br.jianghongdianzi.cn

ssh user@host 'uptime'
来源：http://zt.muxihuayi.cn

[R58] 下载文件
来源：http://pw.colortex.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xk.wgjwhj.cn

[R59] 发 POST JSON
来源：http://xu.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iw.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://xv.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ej.bjjhwx.cn

[R61] 磁盘占用
来源：http://ah.muxihuayi.cn

df -h;  du -sh *
来源：http://yb.9csxet.cn

[R62] 找最占空间的文件
来源：http://vu.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://hi.hahajie.cn

[R63] 内存与进程
来源：http://hb.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://zv.gzmigu.cn

[R64] 结束进程
来源：http://sq.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://lu.newstarts.cn

[R65] 查看端口占用
来源：http://ck.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nw.szsharing.cn

[R66] 定时任务
来源：http://ce.newstarts.cn

crontab -e;  crontab -l
来源：http://ny.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://em.jianghongdianzi.cn

openssl rand -hex 16
来源：http://wn.9csxet.cn

[R68] 计算文件校验值
来源：http://xi.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lv.wgjwhj.cn

[R69] 生成随机密码
来源：http://lu.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://ku.nicolike.cn

[R70] 时间戳与互转
来源：http://am.nszjky.cn

date +%s;  date -d @1700000000
来源：http://ld.chemitech.net.cn

[R71] 日期格式化
来源：http://bg.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nc.hahajie.cn

[R72] 等待端口就绪
来源：http://ph.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ho.colortex.cn

[R73] 分割大日志
来源：http://tt.521024.cn

split -l 1000 big.log part_
来源：http://gh.asd995.cn

[R74] 批量重命名
来源：http://ur.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bp.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://sf.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://ji.chemitech.net.cn

[R76] 使用临时文件
来源：http://zs.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yg.szxytkj.cn

[R77] 读取用户输入
来源：http://rx.shxzukj.cn

read -rp "请输入: " ans
来源：http://pb.hahajie.cn

[R78] 交互式菜单
来源：http://zi.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sa.jianghongdianzi.cn

[R79] 解析命令行选项
来源：http://lg.shxzukj.cn


<!-- 参考信息 -->