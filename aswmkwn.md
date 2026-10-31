代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lw.panjiajie.cn

[Q26] 计数
来源：http://oc.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://ng.hnjuh.cn

[Q27] 条件计数
来源：http://mj.jctech888.com.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ak.muxihuayi.cn

[Q28] 求和与平均
来源：http://ac.lnxyls.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zk.panjiajie.cn

[Q29] 最大最小值
来源：http://gd.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qr.newstarts.cn

[Q30] 分组统计
来源：http://yl.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://no.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://lf.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kn.chemitech.net.cn

[Q32] 分组拼接字符串
来源：http://mr.hahajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ut.nszjky.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yv.jctech888.com.cn

[Q33] 多列分组
来源：http://el.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jl.nszjky.cn

[Q34] 每组取第一条
来源：http://py.newstarts.cn

SELECT * FROM (
来源：http://dq.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pr.hnjuh.cn

) t WHERE rn = 1;
来源：http://ux.szsharing.cn

[Q35] 内连接
来源：http://cf.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://if.newstarts.cn

[Q36] 左连接
来源：http://my.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://md.gzmigu.cn

[Q37] 右连接
来源：http://ub.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vx.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tf.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://py.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://lt.9csxet.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ql.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vn.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://og.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mx.bjjhwx.cn

[Q41] 多表连接
来源：http://nd.asd995.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mg.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://vg.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://uj.shxzukj.cn

[Q42] 连接条件附加过滤
来源：http://vy.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://et.gzmigu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xa.asd995.cn

[Q43] 标量子查询
来源：http://mj.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yv.shtwfgs.cn

[Q44] IN 子查询
来源：http://zs.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vs.521024.cn

[Q45] EXISTS 判断存在
来源：http://gy.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zn.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pc.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lx.szxytkj.cn

[Q47] 与平均值比较
来源：http://mi.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lx.yuexingan06.cn

[Q48] CTE 公用表表达式
来源：http://sp.newstarts.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ds.colortex.cn

SELECT * FROM t WHERE c > 5;
来源：http://dk.shxzskj.cn

[Q49] 更新单行
来源：http://cv.shtwfgs.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hh.chemitech.net.cn

[Q50] 批量更新
来源：http://lg.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rv.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://du.szsharing.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mr.panjiajie.cn

[Q52] 删除指定行
来源：http://vn.nszjky.cn

DELETE FROM users WHERE id = 10;
来源：http://io.shtwfgs.cn

[Q53] 按条件删除
来源：http://uv.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sa.haigaiapp.cn

[Q54] 清空表
来源：http://yl.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://ni.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://wz.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bo.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://wr.hnjuh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uk.shxzukj.cn

[Q57] 行号
来源：http://ht.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wk.yuntaijiaju.cn

[Q58] 累计求和
来源：http://ne.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://us.nszjky.cn

[Q59] 分组内累计
来源：http://ju.huanxung.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://so.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://iu.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qo.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sv.yuntaijiaju.cn

[Q61] 移动平均
来源：http://jw.colortex.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fk.521024.cn

[Q62] 分组占比
来源：http://ms.shtwfgs.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fm.asd995.cn

[Q63] 开启事务
来源：http://jq.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kg.colortex.cn

[Q64] 提交事务
来源：http://sq.gzmigu.cn

COMMIT;
来源：http://wz.huanxung.cn

[Q65] 回滚事务
来源：http://wi.szxytkj.cn

ROLLBACK;
来源：http://ks.shxzskj.cn

[Q66] 行锁查询
来源：http://nz.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iv.huanxung.cn

[Q67] 设置隔离级别
来源：http://lo.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mx.521024.cn

[Q68] 保存点
来源：http://ir.shxzskj.cn

SAVEPOINT sp1;
来源：http://kg.huanxung.cn

ROLLBACK TO sp1;
来源：http://eh.jctech888.com.cn

[Q69] 查看执行计划
来源：http://ti.nicolike.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yb.szsharing.cn

[Q70] 更新统计信息
来源：http://lu.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://gj.shtwfgs.cn

[Q71] 查看建表语句
来源：http://fh.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kl.wgjwhj.cn

[Q72] 查看索引
来源：http://hi.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://gt.gzmigu.cn

[Q73] 查看表状态
来源：http://bn.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ex.newstarts.cn

[Q74] 强制使用索引
来源：http://ec.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yh.huixiangedu.cn

[Q75] 日期格式化
来源：http://qg.newstarts.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zd.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rh.shxzskj.cn

[Q76] 按天统计
来源：http://qt.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hk.hahajie.cn

[Q77] 时间加减
来源：http://sf.wgjwhj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qp.jctech888.com.cn

[Q78] 当前时间
来源：http://ep.jctech888.com.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rl.lnxyls.cn

[Q79] 字符串拼接
来源：http://oc.bookmarksfly.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rt.nszjky.cn

[Q80] 字符串截取
来源：http://fa.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sq.chemitech.net.cn

[Q81] 字符串替换
来源：http://nv.bjjhwx.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wk.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://md.szsharing.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ch.haigaiapp.cn

[Q83] 大小写转换
来源：http://nl.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qr.jianghongdianzi.cn

[Q84] 去除首尾空格
来源：http://oa.521024.cn

SELECT TRIM(name) FROM users;
来源：http://mf.haigaiapp.cn

[Q85] 数值取整
来源：http://zk.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vq.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://zs.wgjwhj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gv.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://pz.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ox.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://dr.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ld.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ma.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://ha.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fz.huanxung.cn

[Q90] 生成序号列
来源：http://zy.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vx.lnxyls.cn

================================================================================
来源：http://hx.yuexingan06.cn

R. Bash 专题
来源：http://jk.muxihuayi.cn

================================================================================
来源：http://qu.newstarts.cn

[R01] shebang 与严格模式
来源：http://kp.nszjky.cn

#!/usr/bin/env bash
来源：http://cm.gzmigu.cn

set -euo pipefail
来源：http://zp.szsharing.cn

[R02] 变量赋值与使用
来源：http://zo.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://di.colortex.cn

[R03] 只读变量
来源：http://kc.hahajie.cn

readonly PI=3.14
来源：http://cg.szsharing.cn

[R04] 位置参数
来源：http://yu.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xc.nszjky.cn

[R05] 参数默认值
来源：http://cf.chemitech.net.cn

name="${1:-default}"
来源：http://tb.gzmigu.cn

[R06] 判断命令是否存在
来源：http://xi.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yx.chemitech.net.cn

[R07] if 判断文件
来源：http://ma.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lf.gzmigu.cn

[R08] 数值比较
来源：http://xc.panjiajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wk.hahajie.cn

[R09] 字符串比较
来源：http://yt.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bi.yuntaijiaju.cn

[R10] 正则匹配
来源：http://ml.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nz.yuexingan06.cn

[R11] case 多分支
来源：http://bz.wgjwhj.cn

case "$1" in
来源：http://kr.shtwfgs.cn

start) echo "启动" ;;
来源：http://jp.hnjuh.cn

stop)  echo "停止" ;;
来源：http://pv.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://fy.haigaiapp.cn

esac
来源：http://jw.521024.cn

[R12] for 遍历文件
来源：http://wq.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://tg.shxzskj.cn

[R13] for 计数循环
来源：http://gr.huanxung.cn

for i in {1..10}; do echo "$i"; done
来源：http://tr.asd995.cn

[R14] C 风格 for
来源：http://yd.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pt.9csxet.cn

[R15] while 逐行读文件
来源：http://le.huanxung.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sh.521024.cn

[R16] until 等待条件
来源：http://pw.jctech888.com.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pd.chemitech.net.cn

[R17] 数组定义与取值
来源：http://dn.lnxyls.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ua.huixinmuqiang.cn

[R18] 遍历数组
来源：http://qf.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gt.wgjwhj.cn

[R19] 数组长度
来源：http://fe.panjiajie.cn

echo "${#arr[@]}"
来源：http://kl.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://kf.hahajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bg.wgjwhj.cn

[R21] 字符串长度
来源：http://hp.hahajie.cn

echo "${#s}"
来源：http://ka.hnjuh.cn

[R22] 截取子串
来源：http://uy.9csxet.cn

echo "${s:0:5}"
来源：http://bu.hahajie.cn

[R23] 字符串替换
来源：http://bf.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sr.bookmarksfly.cn

[R24] 大小写转换
来源：http://xk.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zk.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://hq.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fn.szxytkj.cn

[R26] 命令替换
来源：http://wp.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://vp.huanxung.cn

[R27] 算术展开
来源：http://gj.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://dw.bjjhwx.cn

[R28] 浮点运算
来源：http://wz.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://rt.lnxyls.cn

[R29] 定义函数
来源：http://bs.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nc.shxzukj.cn

[R30] 函数返回状态码
来源：http://an.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://jr.szsharing.cn

[R31] 局部变量
来源：http://yq.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://gk.chemitech.net.cn

[R32] 参数个数校验
来源：http://hz.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vb.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://ny.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iz.szsharing.cn

[R34] 退出时清理
来源：http://jw.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ry.chemitech.net.cn

[R35] 后台执行并等待
来源：http://qg.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kx.lnxyls.cn

[R36] 并发执行多个任务
来源：http://or.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jx.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://nf.9csxet.cn

files=$(ls -1)
来源：http://bd.nszjky.cn

[R38] 管道串联
来源：http://qm.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://zn.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://km.shtwfgs.cn

cmd > out.log 2>&1
来源：http://fr.asd995.cn

[R40] 追加写日志
来源：http://hl.521024.cn

echo "log" >> out.log
来源：http://hf.shxzukj.cn

[R41] 丢弃输出
来源：http://kf.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://zs.szxytkj.cn

[R42] 输入重定向
来源：http://hj.szxytkj.cn

wc -l < a.txt
来源：http://qm.shtwfgs.cn

[R43] 按名字查找文件
来源：http://jv.newstarts.cn

find . -name "*.log" -type f
来源：http://ht.hahajie.cn

[R44] 按修改时间查找
来源：http://ln.yuexingan06.cn

find . -mtime -7 -type f
来源：http://cd.yuexingan06.cn

[R45] 批量删除
来源：http://ks.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://na.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://fo.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gr.nszjky.cn

[R47] sed 单行替换
来源：http://nx.shxzukj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://uz.hahajie.cn

[R48] awk 取指定列
来源：http://nk.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://uo.shxzukj.cn

[R49] awk 带条件
来源：http://dz.jianghongdianzi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kd.yuntaijiaju.cn

[R50] awk 求和
来源：http://tz.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ta.haigaiapp.cn

[R51] 排序去重取前几
来源：http://ub.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ol.szsharing.cn

[R52] 统计行数
来源：http://kv.asd995.cn

wc -l a.txt
来源：http://dn.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://qu.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bc.newstarts.cn

[R54] 比较两个文件
来源：http://kr.gzmigu.cn

diff a.txt b.txt
来源：http://oc.9csxet.cn

[R55] 压缩与解压
来源：http://yr.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gb.bookmarksfly.cn

[R56] 远程拷贝
来源：http://st.521024.cn

scp file user@host:/path/
来源：http://bz.huanxung.cn

[R57] 远程执行命令
来源：http://mc.jctech888.com.cn

ssh user@host 'uptime'
来源：http://xm.szxytkj.cn

[R58] 下载文件
来源：http://cp.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ej.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://qs.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://be.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://vp.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tr.szsharing.cn

[R61] 磁盘占用
来源：http://yx.huixiangedu.cn

df -h;  du -sh *
来源：http://hm.colortex.cn

[R62] 找最占空间的文件
来源：http://eu.9csxet.cn

du -ah . | sort -rh | head -10
来源：http://gb.huanxung.cn

[R63] 内存与进程
来源：http://wm.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://cv.nszjky.cn

[R64] 结束进程
来源：http://kr.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://kl.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://gu.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://um.colortex.cn

[R66] 定时任务
来源：http://jj.shxzukj.cn

crontab -e;  crontab -l
来源：http://uo.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://cl.szsharing.cn

openssl rand -hex 16
来源：http://nl.gzmigu.cn

[R68] 计算文件校验值
来源：http://gi.521024.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wz.gzmigu.cn

[R69] 生成随机密码
来源：http://ll.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://yn.colortex.cn

[R70] 时间戳与互转
来源：http://us.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://xa.bjjhwx.cn

[R71] 日期格式化
来源：http://av.nszjky.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wh.huixinmuqiang.cn

[R72] 等待端口就绪
来源：http://im.yuexingan06.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oj.muxihuayi.cn

[R73] 分割大日志
来源：http://hp.szxytkj.cn

split -l 1000 big.log part_
来源：http://ru.nszjky.cn

[R74] 批量重命名
来源：http://bl.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jl.shtwfgs.cn

[R75] 导出环境变量
来源：http://et.yuntaijiaju.cn


<!-- 参考信息 -->