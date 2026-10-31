代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sa.haigaiapp.cn

[Q24] 去重
来源：http://si.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://po.wgjwhj.cn

[Q25] 只取前 N 条
来源：http://dw.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fz.yuntaijiaju.cn

[Q26] 计数
来源：http://ko.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://cd.yuntaijiaju.cn

[Q27] 条件计数
来源：http://iy.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hx.asd995.cn

[Q28] 求和与平均
来源：http://we.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jp.yuntaijiaju.cn

[Q29] 最大最小值
来源：http://db.521024.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ur.jctech888.com.cn

[Q30] 分组统计
来源：http://sh.9csxet.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pw.hnjuh.cn

[Q31] 分组后过滤
来源：http://nf.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yy.shtwfgs.cn

[Q32] 分组拼接字符串
来源：http://os.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gq.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uk.wgjwhj.cn

[Q33] 多列分组
来源：http://zv.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pk.panjiajie.cn

[Q34] 每组取第一条
来源：http://nc.gzmigu.cn

SELECT * FROM (
来源：http://qa.521024.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cp.jctech888.com.cn

) t WHERE rn = 1;
来源：http://yr.9csxet.cn

[Q35] 内连接
来源：http://oa.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vy.shxzskj.cn

[Q36] 左连接
来源：http://mv.asd995.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ax.asd995.cn

[Q37] 右连接
来源：http://cf.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vk.9csxet.cn

[Q38] 全外连接（PostgreSQL）
来源：http://an.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://et.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://lm.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sw.yuexingan06.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lx.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ek.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pt.gzmigu.cn

[Q41] 多表连接
来源：http://sj.newstarts.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yz.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://bl.lnxyls.cn

JOIN products p ON p.id = o.product_id;
来源：http://ng.colortex.cn

[Q42] 连接条件附加过滤
来源：http://rz.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://sr.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yd.chemitech.net.cn

[Q43] 标量子查询
来源：http://fh.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hk.colortex.cn

[Q44] IN 子查询
来源：http://iv.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nd.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://mc.nicolike.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ue.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dr.muxihuayi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ks.yuntaijiaju.cn

[Q47] 与平均值比较
来源：http://ot.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gf.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://og.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pi.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://oc.szxytkj.cn

[Q49] 更新单行
来源：http://tz.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tb.521024.cn

[Q50] 批量更新
来源：http://yj.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ev.gzmigu.cn

[Q51] 用子查询更新
来源：http://vi.wgjwhj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sa.hahajie.cn

[Q52] 删除指定行
来源：http://zk.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://zy.yuntaijiaju.cn

[Q53] 按条件删除
来源：http://zo.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tv.szxytkj.cn

[Q54] 清空表
来源：http://tw.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://zu.wgjwhj.cn

[Q55] 排名（并列占位）
来源：http://tp.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dv.nicolike.cn

[Q56] 密集排名（并列不占位）
来源：http://ol.colortex.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gv.yuexingan06.cn

[Q57] 行号
来源：http://jo.521024.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://el.lnxyls.cn

[Q58] 累计求和
来源：http://ko.gzmigu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ag.lnxyls.cn

[Q59] 分组内累计
来源：http://qk.521024.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lw.huixinmuqiang.cn

[Q60] 取上一行 / 下一行
来源：http://uy.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yl.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ac.yuexingan06.cn

[Q61] 移动平均
来源：http://tu.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pc.szxytkj.cn

[Q62] 分组占比
来源：http://mg.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vw.asd995.cn

[Q63] 开启事务
来源：http://rw.lnxyls.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tk.hahajie.cn

[Q64] 提交事务
来源：http://ta.panjiajie.cn

COMMIT;
来源：http://yo.hahajie.cn

[Q65] 回滚事务
来源：http://ry.haigaiapp.cn

ROLLBACK;
来源：http://qk.asd995.cn

[Q66] 行锁查询
来源：http://ya.bjjhwx.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mq.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://uu.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pw.lnxyls.cn

[Q68] 保存点
来源：http://mf.nszjky.cn

SAVEPOINT sp1;
来源：http://wr.colortex.cn

ROLLBACK TO sp1;
来源：http://ya.huanxung.cn

[Q69] 查看执行计划
来源：http://ek.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yo.shtwfgs.cn

[Q70] 更新统计信息
来源：http://sb.lnxyls.cn

ANALYZE TABLE users;
来源：http://mh.newstarts.cn

[Q71] 查看建表语句
来源：http://tm.muxihuayi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uu.bookmarksfly.cn

[Q72] 查看索引
来源：http://hv.shxzskj.cn

SHOW INDEX FROM users;
来源：http://kx.shtwfgs.cn

[Q73] 查看表状态
来源：http://ys.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vl.panjiajie.cn

[Q74] 强制使用索引
来源：http://us.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fz.colortex.cn

[Q75] 日期格式化
来源：http://ed.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qb.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ls.muxihuayi.cn

[Q76] 按天统计
来源：http://sh.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xu.shxzukj.cn

[Q77] 时间加减
来源：http://ca.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rw.huixiangedu.cn

[Q78] 当前时间
来源：http://kg.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ng.nicolike.cn

[Q79] 字符串拼接
来源：http://dg.nszjky.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pt.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://uh.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gc.521024.cn

[Q81] 字符串替换
来源：http://cr.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ad.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://ms.jctech888.com.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yy.haigaiapp.cn

[Q83] 大小写转换
来源：http://nd.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://um.szxytkj.cn

[Q84] 去除首尾空格
来源：http://ra.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://gc.haigaiapp.cn

[Q85] 数值取整
来源：http://co.huixinmuqiang.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rj.521024.cn

[Q86] 读取 JSON 字段
来源：http://xv.bjjhwx.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pz.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://zr.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oe.nicolike.cn

[Q88] 行转列（条件聚合）
来源：http://qj.huanxung.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ta.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nf.nszjky.cn

[Q89] 判断表是否存在
来源：http://rj.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lr.huixiangedu.cn

[Q90] 生成序号列
来源：http://qq.szsharing.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hq.shxzukj.cn

================================================================================
来源：http://ax.shtwfgs.cn

R. Bash 专题
来源：http://fp.yuexingan06.cn

================================================================================
来源：http://xl.colortex.cn

[R01] shebang 与严格模式
来源：http://kk.szxytkj.cn

#!/usr/bin/env bash
来源：http://ab.shxzskj.cn

set -euo pipefail
来源：http://ma.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://ym.bookmarksfly.cn

name="Tom"; echo "$name"
来源：http://dv.9csxet.cn

[R03] 只读变量
来源：http://rp.yuexingan06.cn

readonly PI=3.14
来源：http://lk.newstarts.cn

[R04] 位置参数
来源：http://zq.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mj.shtwfgs.cn

[R05] 参数默认值
来源：http://wq.shtwfgs.cn

name="${1:-default}"
来源：http://pj.521024.cn

[R06] 判断命令是否存在
来源：http://tl.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nk.nicolike.cn

[R07] if 判断文件
来源：http://bz.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fv.colortex.cn

[R08] 数值比较
来源：http://rn.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cz.huixinmuqiang.cn

[R09] 字符串比较
来源：http://el.bookmarksfly.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://al.shtwfgs.cn

[R10] 正则匹配
来源：http://xq.muxihuayi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zs.bookmarksfly.cn

[R11] case 多分支
来源：http://xv.lnxyls.cn

case "$1" in
来源：http://zz.yuexingan06.cn

start) echo "启动" ;;
来源：http://ch.9csxet.cn

stop)  echo "停止" ;;
来源：http://ff.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://lg.wgjwhj.cn

esac
来源：http://ep.9csxet.cn

[R12] for 遍历文件
来源：http://ao.newstarts.cn

for f in *.txt; do echo "$f"; done
来源：http://or.yuexingan06.cn

[R13] for 计数循环
来源：http://sb.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://jd.shtwfgs.cn

[R14] C 风格 for
来源：http://ul.yuntaijiaju.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://we.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://en.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qn.shxzukj.cn

[R16] until 等待条件
来源：http://lc.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mt.521024.cn

[R17] 数组定义与取值
来源：http://rt.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nx.yuntaijiaju.cn

[R18] 遍历数组
来源：http://vy.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ba.huixiangedu.cn

[R19] 数组长度
来源：http://fs.colortex.cn

echo "${#arr[@]}"
来源：http://zi.lnxyls.cn

[R20] 关联数组（字典）
来源：http://uy.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zc.wgjwhj.cn

[R21] 字符串长度
来源：http://gm.szsharing.cn

echo "${#s}"
来源：http://yj.huanxung.cn

[R22] 截取子串
来源：http://nv.szsharing.cn

echo "${s:0:5}"
来源：http://sr.panjiajie.cn

[R23] 字符串替换
来源：http://ck.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cs.521024.cn

[R24] 大小写转换
来源：http://ki.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yd.huixinmuqiang.cn

[R25] 去后缀 / 去前缀
来源：http://dx.wgjwhj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pq.hahajie.cn

[R26] 命令替换
来源：http://qe.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://ic.asd995.cn

[R27] 算术展开
来源：http://hw.colortex.cn

echo $((1 + 2 * 3))
来源：http://hb.asd995.cn

[R28] 浮点运算
来源：http://rq.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://ut.lnxyls.cn

[R29] 定义函数
来源：http://sk.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zb.colortex.cn

[R30] 函数返回状态码
来源：http://qr.wgjwhj.cn

f() { return 0; }; f || echo "失败了"
来源：http://gw.jianghongdianzi.cn

[R31] 局部变量
来源：http://sr.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://gc.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://mw.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ba.yuntaijiaju.cn

[R33] 捕获错误并提示行号
来源：http://km.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vb.huixinmuqiang.cn

[R34] 退出时清理
来源：http://ih.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sj.huanxung.cn

[R35] 后台执行并等待
来源：http://pi.jianghongdianzi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pa.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://tz.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://af.lnxyls.cn

[R37] 把输出赋给变量
来源：http://tq.521024.cn

files=$(ls -1)
来源：http://zf.haigaiapp.cn

[R38] 管道串联
来源：http://kx.lnxyls.cn

cat a.txt | grep -i error | wc -l
来源：http://me.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://iu.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://wz.wgjwhj.cn

[R40] 追加写日志
来源：http://tw.huanxung.cn

echo "log" >> out.log
来源：http://rt.nszjky.cn

[R41] 丢弃输出
来源：http://xm.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://en.muxihuayi.cn

[R42] 输入重定向
来源：http://ij.huanxung.cn

wc -l < a.txt
来源：http://dk.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://nj.colortex.cn

find . -name "*.log" -type f
来源：http://wz.shxzukj.cn

[R44] 按修改时间查找
来源：http://fo.newstarts.cn

find . -mtime -7 -type f
来源：http://vc.wgjwhj.cn

[R45] 批量删除
来源：http://xu.nszjky.cn

find . -name "*.tmp" -delete
来源：http://ev.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://sy.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bk.huixiangedu.cn

[R47] sed 单行替换
来源：http://jz.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dh.muxihuayi.cn

[R48] awk 取指定列
来源：http://va.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://xv.shtwfgs.cn

[R49] awk 带条件
来源：http://bp.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tb.521024.cn

[R50] awk 求和
来源：http://ma.bookmarksfly.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wz.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://ii.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fy.bjjhwx.cn

[R52] 统计行数
来源：http://qy.gzmigu.cn

wc -l a.txt
来源：http://jv.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://le.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ju.yuexingan06.cn

[R54] 比较两个文件
来源：http://cl.szsharing.cn

diff a.txt b.txt
来源：http://tz.chemitech.net.cn

[R55] 压缩与解压
来源：http://jp.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nj.nicolike.cn

[R56] 远程拷贝
来源：http://ke.shtwfgs.cn

scp file user@host:/path/
来源：http://qi.shxzukj.cn

[R57] 远程执行命令
来源：http://ia.jctech888.com.cn

ssh user@host 'uptime'
来源：http://ms.521024.cn

[R58] 下载文件
来源：http://va.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lb.shxzskj.cn

[R59] 发 POST JSON
来源：http://mj.panjiajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rt.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://ep.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ai.szsharing.cn

[R61] 磁盘占用
来源：http://ot.wgjwhj.cn

df -h;  du -sh *
来源：http://ba.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://dt.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://hi.9csxet.cn

[R63] 内存与进程
来源：http://we.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://te.shtwfgs.cn

[R64] 结束进程
来源：http://gz.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://cy.nszjky.cn

[R65] 查看端口占用
来源：http://sx.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xu.nicolike.cn

[R66] 定时任务
来源：http://qx.szxytkj.cn

crontab -e;  crontab -l
来源：http://ji.huanxung.cn

[R67] 生成随机十六进制串
来源：http://yd.huixinmuqiang.cn

openssl rand -hex 16
来源：http://fo.asd995.cn

[R68] 计算文件校验值
来源：http://tp.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rh.nicolike.cn

[R69] 生成随机密码
来源：http://fg.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://wz.colortex.cn

[R70] 时间戳与互转
来源：http://ji.colortex.cn

date +%s;  date -d @1700000000
来源：http://ub.wgjwhj.cn

[R71] 日期格式化
来源：http://dt.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zh.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://dn.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kf.jctech888.com.cn

[R73] 分割大日志
来源：http://hi.szsharing.cn


<!-- 参考信息 -->