代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ue.gzmigu.cn

[Q26] 计数
来源：http://ss.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://lo.szsharing.cn

[Q27] 条件计数
来源：http://zo.shtwfgs.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ag.asd995.cn

[Q28] 求和与平均
来源：http://qr.haigaiapp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tb.szxytkj.cn

[Q29] 最大最小值
来源：http://jp.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bw.bookmarksfly.cn

[Q30] 分组统计
来源：http://gj.colortex.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://la.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://lb.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://aq.521024.cn

[Q32] 分组拼接字符串
来源：http://ah.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://li.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vr.gzmigu.cn

[Q33] 多列分组
来源：http://kq.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hn.asd995.cn

[Q34] 每组取第一条
来源：http://qx.hnjuh.cn

SELECT * FROM (
来源：http://ui.nszjky.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ok.szxytkj.cn

) t WHERE rn = 1;
来源：http://vh.yuexingan06.cn

[Q35] 内连接
来源：http://ag.szxytkj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ye.nicolike.cn

[Q36] 左连接
来源：http://og.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://il.yuexingan06.cn

[Q37] 右连接
来源：http://tq.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ms.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yk.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uk.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://og.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xg.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://af.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ek.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ow.nicolike.cn

[Q41] 多表连接
来源：http://df.hahajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gh.shtwfgs.cn

JOIN users u ON u.id = o.user_id
来源：http://wa.shxzukj.cn

JOIN products p ON p.id = o.product_id;
来源：http://jv.521024.cn

[Q42] 连接条件附加过滤
来源：http://ue.nszjky.cn

SELECT u.name, o.amount FROM users u
来源：http://ib.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sh.panjiajie.cn

[Q43] 标量子查询
来源：http://tj.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ii.9csxet.cn

[Q44] IN 子查询
来源：http://bp.szxytkj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cq.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://so.gzmigu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lt.asd995.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bg.9csxet.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vs.nszjky.cn

[Q47] 与平均值比较
来源：http://uh.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lu.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://xq.panjiajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ex.nszjky.cn

SELECT * FROM t WHERE c > 5;
来源：http://oa.hahajie.cn

[Q49] 更新单行
来源：http://bn.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gl.bookmarksfly.cn

[Q50] 批量更新
来源：http://tv.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dl.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://ta.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pi.wgjwhj.cn

[Q52] 删除指定行
来源：http://go.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://uc.bjjhwx.cn

[Q53] 按条件删除
来源：http://si.huixiangedu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rb.yuntaijiaju.cn

[Q54] 清空表
来源：http://qp.haigaiapp.cn

TRUNCATE TABLE logs;
来源：http://wh.521024.cn

[Q55] 排名（并列占位）
来源：http://hx.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gt.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://ao.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pq.hahajie.cn

[Q57] 行号
来源：http://fe.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gp.szxytkj.cn

[Q58] 累计求和
来源：http://ay.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oi.huixinmuqiang.cn

[Q59] 分组内累计
来源：http://ef.hahajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ys.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://wm.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ky.szxytkj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qj.asd995.cn

[Q61] 移动平均
来源：http://ow.wgjwhj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ln.wgjwhj.cn

[Q62] 分组占比
来源：http://ok.yuntaijiaju.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ol.muxihuayi.cn

[Q63] 开启事务
来源：http://ru.huanxung.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sw.521024.cn

[Q64] 提交事务
来源：http://ti.hnjuh.cn

COMMIT;
来源：http://ja.muxihuayi.cn

[Q65] 回滚事务
来源：http://sv.9csxet.cn

ROLLBACK;
来源：http://ur.szxytkj.cn

[Q66] 行锁查询
来源：http://de.lnxyls.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bn.gzmigu.cn

[Q67] 设置隔离级别
来源：http://qt.szsharing.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nu.jianghongdianzi.cn

[Q68] 保存点
来源：http://qx.shtwfgs.cn

SAVEPOINT sp1;
来源：http://dr.huanxung.cn

ROLLBACK TO sp1;
来源：http://wh.shtwfgs.cn

[Q69] 查看执行计划
来源：http://op.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vj.muxihuayi.cn

[Q70] 更新统计信息
来源：http://mk.muxihuayi.cn

ANALYZE TABLE users;
来源：http://wh.szxytkj.cn

[Q71] 查看建表语句
来源：http://xn.nicolike.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ew.hnjuh.cn

[Q72] 查看索引
来源：http://ls.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://vc.shxzskj.cn

[Q73] 查看表状态
来源：http://ea.huixiangedu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ow.haigaiapp.cn

[Q74] 强制使用索引
来源：http://qs.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://av.panjiajie.cn

[Q75] 日期格式化
来源：http://ga.szsharing.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://je.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xh.szxytkj.cn

[Q76] 按天统计
来源：http://xi.yuntaijiaju.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xg.huanxung.cn

[Q77] 时间加减
来源：http://oh.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://db.nicolike.cn

[Q78] 当前时间
来源：http://zc.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ns.hnjuh.cn

[Q79] 字符串拼接
来源：http://yb.haigaiapp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dr.haigaiapp.cn

[Q80] 字符串截取
来源：http://tx.asd995.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ko.lnxyls.cn

[Q81] 字符串替换
来源：http://tp.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ew.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://uv.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hm.szsharing.cn

[Q83] 大小写转换
来源：http://fi.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uq.newstarts.cn

[Q84] 去除首尾空格
来源：http://gy.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://vk.newstarts.cn

[Q85] 数值取整
来源：http://ar.521024.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eq.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://gj.nszjky.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kf.yuexingan06.cn

[Q87] JSON 字段做条件
来源：http://ow.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kg.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://os.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mp.shxzskj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pu.szsharing.cn

[Q89] 判断表是否存在
来源：http://yn.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rx.hahajie.cn

[Q90] 生成序号列
来源：http://il.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ve.shxzukj.cn

================================================================================
来源：http://nj.shxzskj.cn

R. Bash 专题
来源：http://am.huixiangedu.cn

================================================================================
来源：http://ql.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://jb.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://ro.bjjhwx.cn

set -euo pipefail
来源：http://zz.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://yk.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://rg.jianghongdianzi.cn

[R03] 只读变量
来源：http://cu.newstarts.cn

readonly PI=3.14
来源：http://rd.nszjky.cn

[R04] 位置参数
来源：http://dz.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ex.9csxet.cn

[R05] 参数默认值
来源：http://og.9csxet.cn

name="${1:-default}"
来源：http://xu.yuexingan06.cn

[R06] 判断命令是否存在
来源：http://fk.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://py.9csxet.cn

[R07] if 判断文件
来源：http://mx.521024.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://md.szsharing.cn

[R08] 数值比较
来源：http://ba.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zw.9csxet.cn

[R09] 字符串比较
来源：http://zz.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ib.asd995.cn

[R10] 正则匹配
来源：http://sf.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oz.521024.cn

[R11] case 多分支
来源：http://nb.lnxyls.cn

case "$1" in
来源：http://yy.nicolike.cn

start) echo "启动" ;;
来源：http://zn.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://vz.nicolike.cn

*)     echo "未知命令" ;;
来源：http://za.muxihuayi.cn

esac
来源：http://zu.nszjky.cn

[R12] for 遍历文件
来源：http://zs.shtwfgs.cn

for f in *.txt; do echo "$f"; done
来源：http://jy.bookmarksfly.cn

[R13] for 计数循环
来源：http://vq.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://zf.yuexingan06.cn

[R14] C 风格 for
来源：http://jz.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rs.yuexingan06.cn

[R15] while 逐行读文件
来源：http://ip.huanxung.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kg.huixinmuqiang.cn

[R16] until 等待条件
来源：http://sx.haigaiapp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://in.panjiajie.cn

[R17] 数组定义与取值
来源：http://cd.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kz.nszjky.cn

[R18] 遍历数组
来源：http://fk.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gh.hahajie.cn

[R19] 数组长度
来源：http://si.yuexingan06.cn

echo "${#arr[@]}"
来源：http://gt.szsharing.cn

[R20] 关联数组（字典）
来源：http://cz.bookmarksfly.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gc.bookmarksfly.cn

[R21] 字符串长度
来源：http://yh.yuntaijiaju.cn

echo "${#s}"
来源：http://vb.panjiajie.cn

[R22] 截取子串
来源：http://rv.521024.cn

echo "${s:0:5}"
来源：http://ow.hahajie.cn

[R23] 字符串替换
来源：http://el.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rh.wgjwhj.cn

[R24] 大小写转换
来源：http://lp.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gf.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://xv.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ii.haigaiapp.cn

[R26] 命令替换
来源：http://vx.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://hz.gzmigu.cn

[R27] 算术展开
来源：http://ov.9csxet.cn

echo $((1 + 2 * 3))
来源：http://xl.chemitech.net.cn

[R28] 浮点运算
来源：http://hh.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://he.chemitech.net.cn

[R29] 定义函数
来源：http://jg.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zc.nszjky.cn

[R30] 函数返回状态码
来源：http://xp.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://uq.szxytkj.cn

[R31] 局部变量
来源：http://zr.hahajie.cn

f() { local x=1; echo "$x"; }
来源：http://kv.9csxet.cn

[R32] 参数个数校验
来源：http://vy.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xf.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://kr.panjiajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tk.asd995.cn

[R34] 退出时清理
来源：http://bw.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ln.9csxet.cn

[R35] 后台执行并等待
来源：http://hk.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qt.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://mi.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ik.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://yj.9csxet.cn

files=$(ls -1)
来源：http://zd.chemitech.net.cn

[R38] 管道串联
来源：http://ci.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://ql.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://sp.nszjky.cn

cmd > out.log 2>&1
来源：http://pf.jianghongdianzi.cn

[R40] 追加写日志
来源：http://qc.chemitech.net.cn

echo "log" >> out.log
来源：http://vz.huixiangedu.cn

[R41] 丢弃输出
来源：http://gi.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://me.szxytkj.cn

[R42] 输入重定向
来源：http://zb.bookmarksfly.cn

wc -l < a.txt
来源：http://uq.nszjky.cn

[R43] 按名字查找文件
来源：http://ao.chemitech.net.cn

find . -name "*.log" -type f
来源：http://mz.muxihuayi.cn

[R44] 按修改时间查找
来源：http://mh.yuexingan06.cn

find . -mtime -7 -type f
来源：http://iu.bjjhwx.cn

[R45] 批量删除
来源：http://xt.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://we.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://en.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kz.huanxung.cn

[R47] sed 单行替换
来源：http://zw.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://if.chemitech.net.cn

[R48] awk 取指定列
来源：http://xi.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://jv.newstarts.cn

[R49] awk 带条件
来源：http://it.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ll.wgjwhj.cn

[R50] awk 求和
来源：http://pk.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://il.wgjwhj.cn

[R51] 排序去重取前几
来源：http://gj.hnjuh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hn.huanxung.cn

[R52] 统计行数
来源：http://xj.yuexingan06.cn

wc -l a.txt
来源：http://ii.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://rc.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zk.yuexingan06.cn

[R54] 比较两个文件
来源：http://wy.huanxung.cn

diff a.txt b.txt
来源：http://ss.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://en.szxytkj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mp.wgjwhj.cn

[R56] 远程拷贝
来源：http://sv.muxihuayi.cn

scp file user@host:/path/
来源：http://eg.nicolike.cn

[R57] 远程执行命令
来源：http://wz.muxihuayi.cn

ssh user@host 'uptime'
来源：http://we.yuexingan06.cn

[R58] 下载文件
来源：http://jw.colortex.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vp.yuexingan06.cn

[R59] 发 POST JSON
来源：http://wo.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vn.jctech888.com.cn

[R60] 只看 HTTP 状态码
来源：http://wu.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uh.colortex.cn

[R61] 磁盘占用
来源：http://dg.yuntaijiaju.cn

df -h;  du -sh *
来源：http://px.9csxet.cn

[R62] 找最占空间的文件
来源：http://yd.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://re.nszjky.cn

[R63] 内存与进程
来源：http://rz.jctech888.com.cn

free -h;  ps aux | grep nginx
来源：http://md.hnjuh.cn

[R64] 结束进程
来源：http://xs.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://cx.panjiajie.cn

[R65] 查看端口占用
来源：http://og.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rw.yuntaijiaju.cn

[R66] 定时任务
来源：http://gu.asd995.cn

crontab -e;  crontab -l
来源：http://hf.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://cb.colortex.cn

openssl rand -hex 16
来源：http://vx.szsharing.cn

[R68] 计算文件校验值
来源：http://fv.521024.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ue.colortex.cn

[R69] 生成随机密码
来源：http://sm.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://vx.huanxung.cn

[R70] 时间戳与互转
来源：http://hh.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://mq.shtwfgs.cn

[R71] 日期格式化
来源：http://kq.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eu.yuexingan06.cn

[R72] 等待端口就绪
来源：http://nn.newstarts.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tn.yuntaijiaju.cn

[R73] 分割大日志
来源：http://ir.colortex.cn

split -l 1000 big.log part_
来源：http://tt.szxytkj.cn

[R74] 批量重命名
来源：http://ty.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xh.hnjuh.cn

[R75] 导出环境变量
来源：http://qe.lnxyls.cn


<!-- 参考信息 -->