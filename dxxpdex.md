代发 wailian999

[Q33] 多列分组
来源：http://it.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gj.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://xa.muxihuayi.cn

SELECT * FROM (
来源：http://jd.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://el.huanxung.cn

) t WHERE rn = 1;
来源：http://vp.huanxung.cn

[Q35] 内连接
来源：http://gp.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aa.chemitech.net.cn

[Q36] 左连接
来源：http://ck.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ou.asd995.cn

[Q37] 右连接
来源：http://kc.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ph.gzmigu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bq.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://th.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://vj.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kv.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://od.521024.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qn.bookmarksfly.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fd.bookmarksfly.cn

[Q41] 多表连接
来源：http://pb.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jy.asd995.cn

JOIN users u ON u.id = o.user_id
来源：http://pz.chemitech.net.cn

JOIN products p ON p.id = o.product_id;
来源：http://uu.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://sn.huanxung.cn

SELECT u.name, o.amount FROM users u
来源：http://ef.chemitech.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bv.shxzukj.cn

[Q43] 标量子查询
来源：http://af.chemitech.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ar.hahajie.cn

[Q44] IN 子查询
来源：http://cl.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yb.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://pn.nicolike.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dm.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://uv.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hh.yuexingan06.cn

[Q47] 与平均值比较
来源：http://dr.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qr.szxytkj.cn

[Q48] CTE 公用表表达式
来源：http://qs.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://id.muxihuayi.cn

SELECT * FROM t WHERE c > 5;
来源：http://ej.wgjwhj.cn

[Q49] 更新单行
来源：http://nj.huixinmuqiang.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ko.hahajie.cn

[Q50] 批量更新
来源：http://wl.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mp.jctech888.com.cn

[Q51] 用子查询更新
来源：http://oz.yuntaijiaju.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hf.521024.cn

[Q52] 删除指定行
来源：http://ov.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://wl.9csxet.cn

[Q53] 按条件删除
来源：http://gl.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cg.chemitech.net.cn

[Q54] 清空表
来源：http://tb.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://at.nicolike.cn

[Q55] 排名（并列占位）
来源：http://nv.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pu.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://wu.jctech888.com.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zw.gzmigu.cn

[Q57] 行号
来源：http://av.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gz.shxzukj.cn

[Q58] 累计求和
来源：http://nb.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nt.bjjhwx.cn

[Q59] 分组内累计
来源：http://ma.yuntaijiaju.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qr.521024.cn

[Q60] 取上一行 / 下一行
来源：http://fd.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ha.lnxyls.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yp.newstarts.cn

[Q61] 移动平均
来源：http://qq.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nd.yuexingan06.cn

[Q62] 分组占比
来源：http://ko.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wh.nszjky.cn

[Q63] 开启事务
来源：http://zm.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://an.muxihuayi.cn

[Q64] 提交事务
来源：http://tl.9csxet.cn

COMMIT;
来源：http://ab.huixiangedu.cn

[Q65] 回滚事务
来源：http://zj.panjiajie.cn

ROLLBACK;
来源：http://kk.szxytkj.cn

[Q66] 行锁查询
来源：http://pf.szxytkj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ci.wgjwhj.cn

[Q67] 设置隔离级别
来源：http://qh.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bi.szsharing.cn

[Q68] 保存点
来源：http://hm.szsharing.cn

SAVEPOINT sp1;
来源：http://nx.yuexingan06.cn

ROLLBACK TO sp1;
来源：http://bj.9csxet.cn

[Q69] 查看执行计划
来源：http://gj.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zg.bjjhwx.cn

[Q70] 更新统计信息
来源：http://rb.asd995.cn

ANALYZE TABLE users;
来源：http://fs.muxihuayi.cn

[Q71] 查看建表语句
来源：http://zq.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cf.521024.cn

[Q72] 查看索引
来源：http://mk.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://lx.yuexingan06.cn

[Q73] 查看表状态
来源：http://et.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jk.szxytkj.cn

[Q74] 强制使用索引
来源：http://fp.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hc.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://mr.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jv.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zh.haigaiapp.cn

[Q76] 按天统计
来源：http://xm.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://du.gzmigu.cn

[Q77] 时间加减
来源：http://dm.nicolike.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gh.bjjhwx.cn

[Q78] 当前时间
来源：http://st.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://em.szxytkj.cn

[Q79] 字符串拼接
来源：http://im.jctech888.com.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lv.bjjhwx.cn

[Q80] 字符串截取
来源：http://ac.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mt.hahajie.cn

[Q81] 字符串替换
来源：http://ck.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gg.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://tv.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ut.huixiangedu.cn

[Q83] 大小写转换
来源：http://xe.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lz.newstarts.cn

[Q84] 去除首尾空格
来源：http://xn.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://fa.shxzukj.cn

[Q85] 数值取整
来源：http://ft.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fp.nszjky.cn

[Q86] 读取 JSON 字段
来源：http://qf.shxzskj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qx.asd995.cn

[Q87] JSON 字段做条件
来源：http://km.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ei.9csxet.cn

[Q88] 行转列（条件聚合）
来源：http://ie.asd995.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bd.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jn.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://zk.jctech888.com.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://in.muxihuayi.cn

[Q90] 生成序号列
来源：http://al.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qr.yuexingan06.cn

================================================================================
来源：http://dc.szxytkj.cn

R. Bash 专题
来源：http://hw.shxzskj.cn

================================================================================
来源：http://sm.gzmigu.cn

[R01] shebang 与严格模式
来源：http://dc.panjiajie.cn

#!/usr/bin/env bash
来源：http://qi.shxzukj.cn

set -euo pipefail
来源：http://cp.hahajie.cn

[R02] 变量赋值与使用
来源：http://qb.lnxyls.cn

name="Tom"; echo "$name"
来源：http://pz.yuntaijiaju.cn

[R03] 只读变量
来源：http://ag.lnxyls.cn

readonly PI=3.14
来源：http://bd.haigaiapp.cn

[R04] 位置参数
来源：http://ae.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mh.chemitech.net.cn

[R05] 参数默认值
来源：http://yb.521024.cn

name="${1:-default}"
来源：http://iz.521024.cn

[R06] 判断命令是否存在
来源：http://pq.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sx.wgjwhj.cn

[R07] if 判断文件
来源：http://um.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ba.jctech888.com.cn

[R08] 数值比较
来源：http://ra.nszjky.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://km.chemitech.net.cn

[R09] 字符串比较
来源：http://mm.szxytkj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kt.9csxet.cn

[R10] 正则匹配
来源：http://ci.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qg.shtwfgs.cn

[R11] case 多分支
来源：http://ws.szxytkj.cn

case "$1" in
来源：http://xf.9csxet.cn

start) echo "启动" ;;
来源：http://tj.shtwfgs.cn

stop)  echo "停止" ;;
来源：http://bj.szxytkj.cn

*)     echo "未知命令" ;;
来源：http://bc.lnxyls.cn

esac
来源：http://dp.asd995.cn

[R12] for 遍历文件
来源：http://jg.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://vw.colortex.cn

[R13] for 计数循环
来源：http://hu.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://rk.chemitech.net.cn

[R14] C 风格 for
来源：http://rs.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kl.bjjhwx.cn

[R15] while 逐行读文件
来源：http://rm.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sb.muxihuayi.cn

[R16] until 等待条件
来源：http://ig.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jh.colortex.cn

[R17] 数组定义与取值
来源：http://pz.jianghongdianzi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://df.chemitech.net.cn

[R18] 遍历数组
来源：http://jh.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xc.shxzukj.cn

[R19] 数组长度
来源：http://gw.hnjuh.cn

echo "${#arr[@]}"
来源：http://we.nicolike.cn

[R20] 关联数组（字典）
来源：http://pt.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oa.nicolike.cn

[R21] 字符串长度
来源：http://sw.lnxyls.cn

echo "${#s}"
来源：http://zs.bookmarksfly.cn

[R22] 截取子串
来源：http://qc.newstarts.cn

echo "${s:0:5}"
来源：http://db.huixinmuqiang.cn

[R23] 字符串替换
来源：http://nw.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bt.yuntaijiaju.cn

[R24] 大小写转换
来源：http://dp.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bl.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://ei.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lt.szsharing.cn

[R26] 命令替换
来源：http://xs.521024.cn

now=$(date +%F); echo "$now"
来源：http://eo.gzmigu.cn

[R27] 算术展开
来源：http://as.huixinmuqiang.cn

echo $((1 + 2 * 3))
来源：http://xc.huixinmuqiang.cn

[R28] 浮点运算
来源：http://ug.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://mu.yuexingan06.cn

[R29] 定义函数
来源：http://zr.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gg.shxzukj.cn

[R30] 函数返回状态码
来源：http://bl.lnxyls.cn

f() { return 0; }; f || echo "失败了"
来源：http://yn.huixiangedu.cn

[R31] 局部变量
来源：http://pf.bjjhwx.cn

f() { local x=1; echo "$x"; }
来源：http://jh.gzmigu.cn

[R32] 参数个数校验
来源：http://gx.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bk.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://kl.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qz.muxihuayi.cn

[R34] 退出时清理
来源：http://qm.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qj.shtwfgs.cn

[R35] 后台执行并等待
来源：http://hz.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uo.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://fv.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wp.asd995.cn

[R37] 把输出赋给变量
来源：http://uk.asd995.cn

files=$(ls -1)
来源：http://ro.gzmigu.cn

[R38] 管道串联
来源：http://bj.huixiangedu.cn

cat a.txt | grep -i error | wc -l
来源：http://jz.haigaiapp.cn

[R39] 重定向标准输出与错误
来源：http://pv.nszjky.cn

cmd > out.log 2>&1
来源：http://vf.muxihuayi.cn

[R40] 追加写日志
来源：http://xq.bookmarksfly.cn

echo "log" >> out.log
来源：http://qt.panjiajie.cn

[R41] 丢弃输出
来源：http://hq.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://pg.nicolike.cn

[R42] 输入重定向
来源：http://jv.shxzukj.cn

wc -l < a.txt
来源：http://dt.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://we.yuexingan06.cn

find . -name "*.log" -type f
来源：http://ow.yuexingan06.cn

[R44] 按修改时间查找
来源：http://wz.bjjhwx.cn

find . -mtime -7 -type f
来源：http://os.shxzskj.cn

[R45] 批量删除
来源：http://rk.huanxung.cn

find . -name "*.tmp" -delete
来源：http://yf.szsharing.cn

[R46] 递归替换文件内容
来源：http://oq.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hp.jctech888.com.cn

[R47] sed 单行替换
来源：http://xp.shxzskj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://do.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://jl.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://da.bjjhwx.cn

[R49] awk 带条件
来源：http://la.chemitech.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://df.panjiajie.cn

[R50] awk 求和
来源：http://nv.colortex.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zy.haigaiapp.cn

[R51] 排序去重取前几
来源：http://ig.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ee.shxzukj.cn

[R52] 统计行数
来源：http://bg.szsharing.cn

wc -l a.txt
来源：http://ib.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://bv.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ph.nszjky.cn

[R54] 比较两个文件
来源：http://cy.shxzukj.cn

diff a.txt b.txt
来源：http://ci.jctech888.com.cn

[R55] 压缩与解压
来源：http://sj.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hm.nicolike.cn

[R56] 远程拷贝
来源：http://oi.gzmigu.cn

scp file user@host:/path/
来源：http://tf.yuexingan06.cn

[R57] 远程执行命令
来源：http://xs.newstarts.cn

ssh user@host 'uptime'
来源：http://vz.panjiajie.cn

[R58] 下载文件
来源：http://yw.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lk.muxihuayi.cn

[R59] 发 POST JSON
来源：http://oo.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://un.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://pe.hnjuh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oc.szxytkj.cn

[R61] 磁盘占用
来源：http://vp.muxihuayi.cn

df -h;  du -sh *
来源：http://ua.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://ev.colortex.cn

du -ah . | sort -rh | head -10
来源：http://at.chemitech.net.cn

[R63] 内存与进程
来源：http://ji.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://zc.szsharing.cn

[R64] 结束进程
来源：http://rl.nicolike.cn

kill -9 $(pgrep -f app.py)
来源：http://st.gzmigu.cn

[R65] 查看端口占用
来源：http://gd.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nw.huixiangedu.cn

[R66] 定时任务
来源：http://qo.panjiajie.cn

crontab -e;  crontab -l
来源：http://qh.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://ef.bjjhwx.cn

openssl rand -hex 16
来源：http://kp.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://vz.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://no.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://bu.colortex.cn

head -c 16 /dev/urandom | base64
来源：http://uj.nicolike.cn

[R70] 时间戳与互转
来源：http://ry.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://oy.huixiangedu.cn

[R71] 日期格式化
来源：http://ps.jianghongdianzi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ku.huanxung.cn

[R72] 等待端口就绪
来源：http://de.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ow.muxihuayi.cn

[R73] 分割大日志
来源：http://lg.szxytkj.cn

split -l 1000 big.log part_
来源：http://jv.newstarts.cn

[R74] 批量重命名
来源：http://vv.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qw.bookmarksfly.cn

[R75] 导出环境变量
来源：http://mu.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://jt.panjiajie.cn

[R76] 使用临时文件
来源：http://op.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rl.asd995.cn

[R77] 读取用户输入
来源：http://vr.lnxyls.cn

read -rp "请输入: " ans
来源：http://nw.haigaiapp.cn

[R78] 交互式菜单
来源：http://bq.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kj.521024.cn

[R79] 解析命令行选项
来源：http://il.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://we.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://ku.521024.cn

time ./run.sh
来源：http://jp.bjjhwx.cn

================================================================================
来源：http://pa.panjiajie.cn

S. C / C++ 专题
来源：http://kd.wgjwhj.cn

================================================================================
来源：http://bq.haigaiapp.cn

[S01] C：Hello World
来源：http://sx.jctech888.com.cn

#include <stdio.h>
来源：http://oh.szsharing.cn


<!-- 参考信息 -->