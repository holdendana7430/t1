代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vn.szxytkj.cn

[Q26] 计数
来源：http://mj.colortex.cn

SELECT COUNT(*) FROM users;
来源：http://gm.shtwfgs.cn

[Q27] 条件计数
来源：http://nt.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zu.hnjuh.cn

[Q28] 求和与平均
来源：http://ru.newstarts.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xy.9csxet.cn

[Q29] 最大最小值
来源：http://jc.yuexingan06.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yf.gzmigu.cn

[Q30] 分组统计
来源：http://mz.yuntaijiaju.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kc.shtwfgs.cn

[Q31] 分组后过滤
来源：http://nb.haigaiapp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ir.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://if.hahajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://do.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sn.shxzskj.cn

[Q33] 多列分组
来源：http://gy.9csxet.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mi.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://rk.lnxyls.cn

SELECT * FROM (
来源：http://ln.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fu.nicolike.cn

) t WHERE rn = 1;
来源：http://bc.jctech888.com.cn

[Q35] 内连接
来源：http://dj.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://iw.9csxet.cn

[Q36] 左连接
来源：http://tq.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uk.hnjuh.cn

[Q37] 右连接
来源：http://dq.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qs.nicolike.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xs.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lq.jianghongdianzi.cn

[Q39] 自连接（查上下级）
来源：http://xn.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ga.yuntaijiaju.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dd.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tc.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tj.yuexingan06.cn

[Q41] 多表连接
来源：http://rq.chemitech.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://aj.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://kv.szxytkj.cn

JOIN products p ON p.id = o.product_id;
来源：http://mb.hnjuh.cn

[Q42] 连接条件附加过滤
来源：http://ir.panjiajie.cn

SELECT u.name, o.amount FROM users u
来源：http://cy.bookmarksfly.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fn.huixinmuqiang.cn

[Q43] 标量子查询
来源：http://iq.hahajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mk.521024.cn

[Q44] IN 子查询
来源：http://zc.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qo.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://sd.bjjhwx.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zi.521024.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zv.shxzskj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oc.newstarts.cn

[Q47] 与平均值比较
来源：http://uw.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://br.521024.cn

[Q48] CTE 公用表表达式
来源：http://ot.hnjuh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://le.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://kq.colortex.cn

[Q49] 更新单行
来源：http://kr.gzmigu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yo.yuexingan06.cn

[Q50] 批量更新
来源：http://cv.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dw.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://le.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zd.huanxung.cn

[Q52] 删除指定行
来源：http://ft.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://hp.wgjwhj.cn

[Q53] 按条件删除
来源：http://lg.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ca.hahajie.cn

[Q54] 清空表
来源：http://ec.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://ag.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://sp.panjiajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sm.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://df.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://md.asd995.cn

[Q57] 行号
来源：http://oz.muxihuayi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qt.huanxung.cn

[Q58] 累计求和
来源：http://zp.lnxyls.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mi.szsharing.cn

[Q59] 分组内累计
来源：http://lt.yuntaijiaju.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ad.jctech888.com.cn

[Q60] 取上一行 / 下一行
来源：http://db.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ea.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dk.muxihuayi.cn

[Q61] 移动平均
来源：http://go.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cd.521024.cn

[Q62] 分组占比
来源：http://di.haigaiapp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://un.yuexingan06.cn

[Q63] 开启事务
来源：http://cv.nszjky.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lf.muxihuayi.cn

[Q64] 提交事务
来源：http://rq.nszjky.cn

COMMIT;
来源：http://eh.9csxet.cn

[Q65] 回滚事务
来源：http://tz.yuntaijiaju.cn

ROLLBACK;
来源：http://uc.nicolike.cn

[Q66] 行锁查询
来源：http://yv.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wi.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://ra.gzmigu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wq.yuntaijiaju.cn

[Q68] 保存点
来源：http://hi.lnxyls.cn

SAVEPOINT sp1;
来源：http://yu.9csxet.cn

ROLLBACK TO sp1;
来源：http://jx.colortex.cn

[Q69] 查看执行计划
来源：http://et.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://is.chemitech.net.cn

[Q70] 更新统计信息
来源：http://rd.muxihuayi.cn

ANALYZE TABLE users;
来源：http://sn.yuexingan06.cn

[Q71] 查看建表语句
来源：http://jr.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cv.gzmigu.cn

[Q72] 查看索引
来源：http://ko.shxzukj.cn

SHOW INDEX FROM users;
来源：http://mc.bjjhwx.cn

[Q73] 查看表状态
来源：http://cr.shxzskj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yc.wgjwhj.cn

[Q74] 强制使用索引
来源：http://gj.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zb.shxzskj.cn

[Q75] 日期格式化
来源：http://qc.jctech888.com.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ld.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hi.bjjhwx.cn

[Q76] 按天统计
来源：http://ni.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ez.huixiangedu.cn

[Q77] 时间加减
来源：http://px.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://be.chemitech.net.cn

[Q78] 当前时间
来源：http://xa.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lx.bjjhwx.cn

[Q79] 字符串拼接
来源：http://wi.shxzskj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tn.muxihuayi.cn

[Q80] 字符串截取
来源：http://cx.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rw.panjiajie.cn

[Q81] 字符串替换
来源：http://hp.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://he.jctech888.com.cn

[Q82] 字符长度与字节长度
来源：http://oc.shxzukj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cx.bjjhwx.cn

[Q83] 大小写转换
来源：http://uc.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sk.jianghongdianzi.cn

[Q84] 去除首尾空格
来源：http://mm.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://kz.colortex.cn

[Q85] 数值取整
来源：http://je.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bm.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://wg.chemitech.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yf.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://xn.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nv.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://dh.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tr.szsharing.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://da.shxzukj.cn

[Q89] 判断表是否存在
来源：http://la.muxihuayi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gy.wgjwhj.cn

[Q90] 生成序号列
来源：http://da.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dp.hnjuh.cn

================================================================================
来源：http://ft.panjiajie.cn

R. Bash 专题
来源：http://ay.nszjky.cn

================================================================================
来源：http://ms.hnjuh.cn

[R01] shebang 与严格模式
来源：http://zx.newstarts.cn

#!/usr/bin/env bash
来源：http://kc.gzmigu.cn

set -euo pipefail
来源：http://xj.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://fn.521024.cn

name="Tom"; echo "$name"
来源：http://ve.jianghongdianzi.cn

[R03] 只读变量
来源：http://po.lnxyls.cn

readonly PI=3.14
来源：http://ha.9csxet.cn

[R04] 位置参数
来源：http://tw.bjjhwx.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uj.chemitech.net.cn

[R05] 参数默认值
来源：http://cs.bjjhwx.cn

name="${1:-default}"
来源：http://do.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://jr.jctech888.com.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ih.jianghongdianzi.cn

[R07] if 判断文件
来源：http://mt.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aa.nszjky.cn

[R08] 数值比较
来源：http://ta.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://oy.szsharing.cn

[R09] 字符串比较
来源：http://tz.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://to.huixiangedu.cn

[R10] 正则匹配
来源：http://lm.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xr.9csxet.cn

[R11] case 多分支
来源：http://bx.huixinmuqiang.cn

case "$1" in
来源：http://aq.shtwfgs.cn

start) echo "启动" ;;
来源：http://jb.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://wy.hahajie.cn

*)     echo "未知命令" ;;
来源：http://pu.jctech888.com.cn

esac
来源：http://dq.muxihuayi.cn

[R12] for 遍历文件
来源：http://ie.shxzskj.cn

for f in *.txt; do echo "$f"; done
来源：http://rf.nszjky.cn

[R13] for 计数循环
来源：http://cv.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://ax.huixiangedu.cn

[R14] C 风格 for
来源：http://xb.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ih.yuexingan06.cn

[R15] while 逐行读文件
来源：http://qr.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qg.huixinmuqiang.cn

[R16] until 等待条件
来源：http://xa.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vc.asd995.cn

[R17] 数组定义与取值
来源：http://pa.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bd.nszjky.cn

[R18] 遍历数组
来源：http://ih.9csxet.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pi.huanxung.cn

[R19] 数组长度
来源：http://sr.yuexingan06.cn

echo "${#arr[@]}"
来源：http://xq.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://jc.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rc.yuntaijiaju.cn

[R21] 字符串长度
来源：http://xv.newstarts.cn

echo "${#s}"
来源：http://vo.chemitech.net.cn

[R22] 截取子串
来源：http://bp.muxihuayi.cn

echo "${s:0:5}"
来源：http://sh.newstarts.cn

[R23] 字符串替换
来源：http://je.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cu.haigaiapp.cn

[R24] 大小写转换
来源：http://lt.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hj.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://py.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://er.hnjuh.cn

[R26] 命令替换
来源：http://hp.chemitech.net.cn

now=$(date +%F); echo "$now"
来源：http://ni.wgjwhj.cn

[R27] 算术展开
来源：http://ni.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://rw.9csxet.cn

[R28] 浮点运算
来源：http://md.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://cp.lnxyls.cn

[R29] 定义函数
来源：http://ub.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://is.yuexingan06.cn

[R30] 函数返回状态码
来源：http://eu.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://er.jianghongdianzi.cn

[R31] 局部变量
来源：http://fb.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://eu.521024.cn

[R32] 参数个数校验
来源：http://nn.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aa.asd995.cn

[R33] 捕获错误并提示行号
来源：http://bl.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sj.panjiajie.cn

[R34] 退出时清理
来源：http://qg.yuexingan06.cn

trap 'rm -f "$tmp"' EXIT
来源：http://at.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://bx.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sw.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://te.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ip.huanxung.cn

[R37] 把输出赋给变量
来源：http://sa.szxytkj.cn

files=$(ls -1)
来源：http://na.szxytkj.cn

[R38] 管道串联
来源：http://at.hnjuh.cn

cat a.txt | grep -i error | wc -l
来源：http://op.bookmarksfly.cn

[R39] 重定向标准输出与错误
来源：http://zk.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://zu.szsharing.cn

[R40] 追加写日志
来源：http://qb.hahajie.cn

echo "log" >> out.log
来源：http://io.huixiangedu.cn

[R41] 丢弃输出
来源：http://hj.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://wp.colortex.cn

[R42] 输入重定向
来源：http://jj.jianghongdianzi.cn

wc -l < a.txt
来源：http://sp.newstarts.cn

[R43] 按名字查找文件
来源：http://or.hahajie.cn

find . -name "*.log" -type f
来源：http://ch.521024.cn

[R44] 按修改时间查找
来源：http://bq.shxzukj.cn

find . -mtime -7 -type f
来源：http://hl.huixiangedu.cn

[R45] 批量删除
来源：http://jp.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://id.yuntaijiaju.cn

[R46] 递归替换文件内容
来源：http://pq.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://la.chemitech.net.cn

[R47] sed 单行替换
来源：http://ik.bookmarksfly.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jn.hnjuh.cn

[R48] awk 取指定列
来源：http://mo.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://hz.hnjuh.cn

[R49] awk 带条件
来源：http://pj.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hs.jianghongdianzi.cn

[R50] awk 求和
来源：http://hm.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xr.colortex.cn

[R51] 排序去重取前几
来源：http://jp.nszjky.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qy.gzmigu.cn

[R52] 统计行数
来源：http://hi.nszjky.cn

wc -l a.txt
来源：http://kj.521024.cn

[R53] 查看文件头与实时尾
来源：http://rx.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cb.lnxyls.cn

[R54] 比较两个文件
来源：http://ut.nszjky.cn

diff a.txt b.txt
来源：http://wu.newstarts.cn

[R55] 压缩与解压
来源：http://ro.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qz.yuexingan06.cn

[R56] 远程拷贝
来源：http://od.hahajie.cn

scp file user@host:/path/
来源：http://wo.asd995.cn

[R57] 远程执行命令
来源：http://wm.wgjwhj.cn

ssh user@host 'uptime'
来源：http://bf.newstarts.cn

[R58] 下载文件
来源：http://qn.colortex.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://li.asd995.cn

[R59] 发 POST JSON
来源：http://kk.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yr.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://ny.yuexingan06.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mf.asd995.cn

[R61] 磁盘占用
来源：http://cy.shtwfgs.cn

df -h;  du -sh *
来源：http://vr.szsharing.cn

[R62] 找最占空间的文件
来源：http://ag.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://rz.jianghongdianzi.cn

[R63] 内存与进程
来源：http://in.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://yr.shxzukj.cn

[R64] 结束进程
来源：http://zu.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://lv.asd995.cn

[R65] 查看端口占用
来源：http://ju.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eb.szsharing.cn

[R66] 定时任务
来源：http://gt.chemitech.net.cn

crontab -e;  crontab -l
来源：http://rk.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://qr.wgjwhj.cn

openssl rand -hex 16
来源：http://vf.haigaiapp.cn

[R68] 计算文件校验值
来源：http://hq.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lu.panjiajie.cn

[R69] 生成随机密码
来源：http://qi.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://eh.szxytkj.cn

[R70] 时间戳与互转
来源：http://er.huanxung.cn

date +%s;  date -d @1700000000
来源：http://zr.asd995.cn

[R71] 日期格式化
来源：http://oi.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wp.hahajie.cn

[R72] 等待端口就绪
来源：http://sz.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mw.huanxung.cn

[R73] 分割大日志
来源：http://nz.muxihuayi.cn

split -l 1000 big.log part_
来源：http://eb.jctech888.com.cn

[R74] 批量重命名
来源：http://ow.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ac.colortex.cn

[R75] 导出环境变量
来源：http://dg.9csxet.cn


<!-- 参考信息 -->