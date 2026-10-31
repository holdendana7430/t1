代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://dm.jianghongdianzi.cn

[Q30] 分组统计
来源：http://wj.jianghongdianzi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://oq.szxytkj.cn

[Q31] 分组后过滤
来源：http://uc.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jz.wgjwhj.cn

[Q32] 分组拼接字符串
来源：http://ti.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://al.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fi.shxzukj.cn

[Q33] 多列分组
来源：http://xu.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yf.9csxet.cn

[Q34] 每组取第一条
来源：http://cd.huanxung.cn

SELECT * FROM (
来源：http://tm.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ls.bjjhwx.cn

) t WHERE rn = 1;
来源：http://sm.nszjky.cn

[Q35] 内连接
来源：http://av.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wh.nszjky.cn

[Q36] 左连接
来源：http://nb.muxihuayi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wf.huixinmuqiang.cn

[Q37] 右连接
来源：http://ow.szsharing.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vq.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cs.521024.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qu.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://qt.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://id.chemitech.net.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jy.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ut.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lv.521024.cn

[Q41] 多表连接
来源：http://jl.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://om.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://ui.nicolike.cn

JOIN products p ON p.id = o.product_id;
来源：http://go.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://an.gzmigu.cn

SELECT u.name, o.amount FROM users u
来源：http://hg.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://aj.521024.cn

[Q43] 标量子查询
来源：http://qx.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://by.newstarts.cn

[Q44] IN 子查询
来源：http://vf.gzmigu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rg.521024.cn

[Q45] EXISTS 判断存在
来源：http://bb.lnxyls.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yf.wgjwhj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yl.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yf.gzmigu.cn

[Q47] 与平均值比较
来源：http://nc.haigaiapp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ly.nicolike.cn

[Q48] CTE 公用表表达式
来源：http://yu.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://og.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://dl.huixinmuqiang.cn

[Q49] 更新单行
来源：http://um.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oj.szsharing.cn

[Q50] 批量更新
来源：http://um.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sl.jianghongdianzi.cn

[Q51] 用子查询更新
来源：http://kd.szsharing.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iq.shxzskj.cn

[Q52] 删除指定行
来源：http://dj.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://zc.nicolike.cn

[Q53] 按条件删除
来源：http://xa.haigaiapp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wq.bookmarksfly.cn

[Q54] 清空表
来源：http://mj.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://us.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://wa.muxihuayi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wh.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://ou.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dc.bjjhwx.cn

[Q57] 行号
来源：http://dm.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ln.shtwfgs.cn

[Q58] 累计求和
来源：http://qr.gzmigu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bo.chemitech.net.cn

[Q59] 分组内累计
来源：http://it.9csxet.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xz.panjiajie.cn

[Q60] 取上一行 / 下一行
来源：http://hc.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xt.jctech888.com.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mc.lnxyls.cn

[Q61] 移动平均
来源：http://ol.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sn.521024.cn

[Q62] 分组占比
来源：http://mm.yuntaijiaju.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://od.jianghongdianzi.cn

[Q63] 开启事务
来源：http://yb.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://np.szxytkj.cn

[Q64] 提交事务
来源：http://ms.huanxung.cn

COMMIT;
来源：http://ai.colortex.cn

[Q65] 回滚事务
来源：http://ml.huanxung.cn

ROLLBACK;
来源：http://ln.muxihuayi.cn

[Q66] 行锁查询
来源：http://zm.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sm.muxihuayi.cn

[Q67] 设置隔离级别
来源：http://wd.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://be.jianghongdianzi.cn

[Q68] 保存点
来源：http://xj.gzmigu.cn

SAVEPOINT sp1;
来源：http://dn.muxihuayi.cn

ROLLBACK TO sp1;
来源：http://hv.shxzskj.cn

[Q69] 查看执行计划
来源：http://bf.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xe.gzmigu.cn

[Q70] 更新统计信息
来源：http://yb.shtwfgs.cn

ANALYZE TABLE users;
来源：http://ak.shxzskj.cn

[Q71] 查看建表语句
来源：http://cm.wgjwhj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rl.lnxyls.cn

[Q72] 查看索引
来源：http://zz.szsharing.cn

SHOW INDEX FROM users;
来源：http://pp.huixiangedu.cn

[Q73] 查看表状态
来源：http://zk.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mt.jianghongdianzi.cn

[Q74] 强制使用索引
来源：http://xg.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xr.nszjky.cn

[Q75] 日期格式化
来源：http://xa.yuntaijiaju.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pa.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dy.muxihuayi.cn

[Q76] 按天统计
来源：http://er.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://am.haigaiapp.cn

[Q77] 时间加减
来源：http://cl.shtwfgs.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bs.shxzukj.cn

[Q78] 当前时间
来源：http://jh.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qe.huanxung.cn

[Q79] 字符串拼接
来源：http://pq.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ri.nszjky.cn

[Q80] 字符串截取
来源：http://dp.gzmigu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ph.szsharing.cn

[Q81] 字符串替换
来源：http://ut.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rd.shxzukj.cn

[Q82] 字符长度与字节长度
来源：http://kc.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xr.asd995.cn

[Q83] 大小写转换
来源：http://vd.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gp.hnjuh.cn

[Q84] 去除首尾空格
来源：http://vp.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://td.jctech888.com.cn

[Q85] 数值取整
来源：http://rq.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wi.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://rb.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sb.521024.cn

[Q87] JSON 字段做条件
来源：http://so.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hi.jianghongdianzi.cn

[Q88] 行转列（条件聚合）
来源：http://yd.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hh.nszjky.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oo.asd995.cn

[Q89] 判断表是否存在
来源：http://ll.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eu.asd995.cn

[Q90] 生成序号列
来源：http://se.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pd.shtwfgs.cn

================================================================================
来源：http://vs.jianghongdianzi.cn

R. Bash 专题
来源：http://lt.bjjhwx.cn

================================================================================
来源：http://lz.szxytkj.cn

[R01] shebang 与严格模式
来源：http://gk.jctech888.com.cn

#!/usr/bin/env bash
来源：http://ui.colortex.cn

set -euo pipefail
来源：http://ie.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://wk.shxzskj.cn

name="Tom"; echo "$name"
来源：http://kj.muxihuayi.cn

[R03] 只读变量
来源：http://ze.haigaiapp.cn

readonly PI=3.14
来源：http://nl.lnxyls.cn

[R04] 位置参数
来源：http://cn.chemitech.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fv.gzmigu.cn

[R05] 参数默认值
来源：http://re.szsharing.cn

name="${1:-default}"
来源：http://fm.newstarts.cn

[R06] 判断命令是否存在
来源：http://po.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sl.szxytkj.cn

[R07] if 判断文件
来源：http://oa.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aq.shxzukj.cn

[R08] 数值比较
来源：http://ib.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://um.shtwfgs.cn

[R09] 字符串比较
来源：http://ai.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://co.jctech888.com.cn

[R10] 正则匹配
来源：http://pm.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pv.hahajie.cn

[R11] case 多分支
来源：http://tb.hahajie.cn

case "$1" in
来源：http://qs.nicolike.cn

start) echo "启动" ;;
来源：http://zj.hahajie.cn

stop)  echo "停止" ;;
来源：http://hb.hahajie.cn

*)     echo "未知命令" ;;
来源：http://pk.asd995.cn

esac
来源：http://mf.hnjuh.cn

[R12] for 遍历文件
来源：http://hb.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://ww.9csxet.cn

[R13] for 计数循环
来源：http://yy.huanxung.cn

for i in {1..10}; do echo "$i"; done
来源：http://tu.wgjwhj.cn

[R14] C 风格 for
来源：http://fq.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pt.newstarts.cn

[R15] while 逐行读文件
来源：http://lc.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xk.hahajie.cn

[R16] until 等待条件
来源：http://fx.521024.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jk.szxytkj.cn

[R17] 数组定义与取值
来源：http://fv.muxihuayi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cl.jctech888.com.cn

[R18] 遍历数组
来源：http://ls.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ra.jianghongdianzi.cn

[R19] 数组长度
来源：http://zp.gzmigu.cn

echo "${#arr[@]}"
来源：http://rf.hnjuh.cn

[R20] 关联数组（字典）
来源：http://hl.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://km.521024.cn

[R21] 字符串长度
来源：http://fk.yuntaijiaju.cn

echo "${#s}"
来源：http://oo.shxzskj.cn

[R22] 截取子串
来源：http://ol.asd995.cn

echo "${s:0:5}"
来源：http://bx.yuexingan06.cn

[R23] 字符串替换
来源：http://hu.521024.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sm.gzmigu.cn

[R24] 大小写转换
来源：http://tq.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nx.521024.cn

[R25] 去后缀 / 去前缀
来源：http://zk.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tp.521024.cn

[R26] 命令替换
来源：http://ii.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://ys.szsharing.cn

[R27] 算术展开
来源：http://yg.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://zu.asd995.cn

[R28] 浮点运算
来源：http://xh.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://ac.colortex.cn

[R29] 定义函数
来源：http://uv.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ij.jctech888.com.cn

[R30] 函数返回状态码
来源：http://cf.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://du.chemitech.net.cn

[R31] 局部变量
来源：http://mq.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://tj.hahajie.cn

[R32] 参数个数校验
来源：http://oc.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ls.panjiajie.cn

[R33] 捕获错误并提示行号
来源：http://nv.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xs.jctech888.com.cn

[R34] 退出时清理
来源：http://pv.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ir.yuexingan06.cn

[R35] 后台执行并等待
来源：http://gf.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mx.colortex.cn

[R36] 并发执行多个任务
来源：http://vp.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ci.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://gk.wgjwhj.cn

files=$(ls -1)
来源：http://qw.nszjky.cn

[R38] 管道串联
来源：http://wj.hnjuh.cn

cat a.txt | grep -i error | wc -l
来源：http://io.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://lc.colortex.cn

cmd > out.log 2>&1
来源：http://fz.szxytkj.cn

[R40] 追加写日志
来源：http://vj.gzmigu.cn

echo "log" >> out.log
来源：http://qy.shxzskj.cn

[R41] 丢弃输出
来源：http://pg.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://le.chemitech.net.cn

[R42] 输入重定向
来源：http://yv.jianghongdianzi.cn

wc -l < a.txt
来源：http://se.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://on.wgjwhj.cn

find . -name "*.log" -type f
来源：http://cb.shxzukj.cn

[R44] 按修改时间查找
来源：http://fv.521024.cn

find . -mtime -7 -type f
来源：http://we.colortex.cn

[R45] 批量删除
来源：http://xb.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://zd.szxytkj.cn

[R46] 递归替换文件内容
来源：http://yv.muxihuayi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mi.asd995.cn

[R47] sed 单行替换
来源：http://az.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ni.newstarts.cn

[R48] awk 取指定列
来源：http://wn.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://ve.szxytkj.cn

[R49] awk 带条件
来源：http://zh.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://me.haigaiapp.cn

[R50] awk 求和
来源：http://wj.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bz.521024.cn

[R51] 排序去重取前几
来源：http://ae.hnjuh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wp.nicolike.cn

[R52] 统计行数
来源：http://ny.lnxyls.cn

wc -l a.txt
来源：http://oy.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://nv.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pi.colortex.cn

[R54] 比较两个文件
来源：http://aj.chemitech.net.cn

diff a.txt b.txt
来源：http://cl.szsharing.cn

[R55] 压缩与解压
来源：http://no.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://aq.huanxung.cn

[R56] 远程拷贝
来源：http://wf.wgjwhj.cn

scp file user@host:/path/
来源：http://lh.shxzukj.cn

[R57] 远程执行命令
来源：http://ms.hahajie.cn

ssh user@host 'uptime'
来源：http://ya.wgjwhj.cn

[R58] 下载文件
来源：http://lf.jianghongdianzi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gl.colortex.cn

[R59] 发 POST JSON
来源：http://tm.521024.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zu.jianghongdianzi.cn

[R60] 只看 HTTP 状态码
来源：http://ez.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wg.szsharing.cn

[R61] 磁盘占用
来源：http://ez.yuexingan06.cn

df -h;  du -sh *
来源：http://qo.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://gt.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://rm.lnxyls.cn

[R63] 内存与进程
来源：http://lh.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://gu.jianghongdianzi.cn

[R64] 结束进程
来源：http://ae.muxihuayi.cn

kill -9 $(pgrep -f app.py)
来源：http://ga.asd995.cn

[R65] 查看端口占用
来源：http://fs.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rj.colortex.cn

[R66] 定时任务
来源：http://pk.haigaiapp.cn

crontab -e;  crontab -l
来源：http://ze.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://xu.nicolike.cn

openssl rand -hex 16
来源：http://ye.nicolike.cn

[R68] 计算文件校验值
来源：http://im.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ch.bookmarksfly.cn

[R69] 生成随机密码
来源：http://oa.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://nf.huanxung.cn

[R70] 时间戳与互转
来源：http://gf.huixinmuqiang.cn

date +%s;  date -d @1700000000
来源：http://wc.huanxung.cn

[R71] 日期格式化
来源：http://lt.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nc.521024.cn

[R72] 等待端口就绪
来源：http://sy.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wv.shxzukj.cn

[R73] 分割大日志
来源：http://mg.jctech888.com.cn

split -l 1000 big.log part_
来源：http://gq.szsharing.cn

[R74] 批量重命名
来源：http://un.newstarts.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://se.jctech888.com.cn

[R75] 导出环境变量
来源：http://dm.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://zv.bookmarksfly.cn

[R76] 使用临时文件
来源：http://rm.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nq.521024.cn

[R77] 读取用户输入
来源：http://go.yuntaijiaju.cn

read -rp "请输入: " ans
来源：http://iw.shxzukj.cn

[R78] 交互式菜单
来源：http://zr.jctech888.com.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mt.nszjky.cn

[R79] 解析命令行选项
来源：http://yw.asd995.cn


<!-- 参考信息 -->