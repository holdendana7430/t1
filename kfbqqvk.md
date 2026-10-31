代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wh.jianghongdianzi.cn

[Q24] 去重
来源：http://sz.bookmarksfly.cn

SELECT DISTINCT city FROM users;
来源：http://cz.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://fp.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oj.hnjuh.cn

[Q26] 计数
来源：http://wv.shxzskj.cn

SELECT COUNT(*) FROM users;
来源：http://qs.asd995.cn

[Q27] 条件计数
来源：http://in.haigaiapp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gr.haigaiapp.cn

[Q28] 求和与平均
来源：http://ut.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sq.colortex.cn

[Q29] 最大最小值
来源：http://md.shxzskj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gd.gzmigu.cn

[Q30] 分组统计
来源：http://mn.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yl.shxzskj.cn

[Q31] 分组后过滤
来源：http://jg.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cn.huixinmuqiang.cn

[Q32] 分组拼接字符串
来源：http://yq.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vr.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bu.hahajie.cn

[Q33] 多列分组
来源：http://ww.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qs.colortex.cn

[Q34] 每组取第一条
来源：http://gd.9csxet.cn

SELECT * FROM (
来源：http://mu.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wy.yuexingan06.cn

) t WHERE rn = 1;
来源：http://ml.nszjky.cn

[Q35] 内连接
来源：http://qg.bjjhwx.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xe.jianghongdianzi.cn

[Q36] 左连接
来源：http://ps.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uf.nszjky.cn

[Q37] 右连接
来源：http://ta.nszjky.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ze.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rp.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kv.panjiajie.cn

[Q39] 自连接（查上下级）
来源：http://hm.yuexingan06.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://be.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://te.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zn.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hh.szxytkj.cn

[Q41] 多表连接
来源：http://rb.nicolike.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dl.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://hp.jianghongdianzi.cn

JOIN products p ON p.id = o.product_id;
来源：http://bg.szxytkj.cn

[Q42] 连接条件附加过滤
来源：http://je.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://ky.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nm.hnjuh.cn

[Q43] 标量子查询
来源：http://dr.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fo.haigaiapp.cn

[Q44] IN 子查询
来源：http://jd.521024.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qx.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://ay.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bm.bjjhwx.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jl.colortex.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ti.newstarts.cn

[Q47] 与平均值比较
来源：http://gx.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mz.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://cm.521024.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vf.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://rg.lnxyls.cn

[Q49] 更新单行
来源：http://wb.asd995.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dx.bookmarksfly.cn

[Q50] 批量更新
来源：http://ui.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://md.521024.cn

[Q51] 用子查询更新
来源：http://gq.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vj.shxzskj.cn

[Q52] 删除指定行
来源：http://oe.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://xx.haigaiapp.cn

[Q53] 按条件删除
来源：http://lj.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xb.panjiajie.cn

[Q54] 清空表
来源：http://lp.wgjwhj.cn

TRUNCATE TABLE logs;
来源：http://dv.colortex.cn

[Q55] 排名（并列占位）
来源：http://yo.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rv.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://gv.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xh.yuexingan06.cn

[Q57] 行号
来源：http://fr.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qw.huanxung.cn

[Q58] 累计求和
来源：http://gw.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://on.haigaiapp.cn

[Q59] 分组内累计
来源：http://ux.hahajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rn.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://cd.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://be.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ju.huanxung.cn

[Q61] 移动平均
来源：http://gm.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sa.lnxyls.cn

[Q62] 分组占比
来源：http://yr.haigaiapp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mt.szxytkj.cn

[Q63] 开启事务
来源：http://mw.colortex.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dq.huixiangedu.cn

[Q64] 提交事务
来源：http://dk.asd995.cn

COMMIT;
来源：http://ys.hnjuh.cn

[Q65] 回滚事务
来源：http://hy.yuexingan06.cn

ROLLBACK;
来源：http://md.szsharing.cn

[Q66] 行锁查询
来源：http://fe.9csxet.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xn.shxzukj.cn

[Q67] 设置隔离级别
来源：http://pe.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lt.colortex.cn

[Q68] 保存点
来源：http://ym.newstarts.cn

SAVEPOINT sp1;
来源：http://ca.newstarts.cn

ROLLBACK TO sp1;
来源：http://yd.panjiajie.cn

[Q69] 查看执行计划
来源：http://fg.newstarts.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ol.asd995.cn

[Q70] 更新统计信息
来源：http://tz.newstarts.cn

ANALYZE TABLE users;
来源：http://vz.szsharing.cn

[Q71] 查看建表语句
来源：http://ho.huanxung.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gs.lnxyls.cn

[Q72] 查看索引
来源：http://id.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://my.bookmarksfly.cn

[Q73] 查看表状态
来源：http://tg.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yd.szsharing.cn

[Q74] 强制使用索引
来源：http://qe.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hr.colortex.cn

[Q75] 日期格式化
来源：http://ay.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wr.jianghongdianzi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://my.jianghongdianzi.cn

[Q76] 按天统计
来源：http://gd.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rp.bookmarksfly.cn

[Q77] 时间加减
来源：http://ns.521024.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ba.bookmarksfly.cn

[Q78] 当前时间
来源：http://bb.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fe.szsharing.cn

[Q79] 字符串拼接
来源：http://pf.huanxung.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tx.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://tb.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fi.szsharing.cn

[Q81] 字符串替换
来源：http://bn.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tn.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://fu.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qi.chemitech.net.cn

[Q83] 大小写转换
来源：http://id.asd995.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wc.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://gv.nicolike.cn

SELECT TRIM(name) FROM users;
来源：http://xv.nszjky.cn

[Q85] 数值取整
来源：http://ik.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rf.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://vc.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bh.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://vj.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zg.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://yn.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cm.asd995.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oq.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://nf.yuntaijiaju.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yr.shxzskj.cn

[Q90] 生成序号列
来源：http://ak.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zc.asd995.cn

================================================================================
来源：http://fh.muxihuayi.cn

R. Bash 专题
来源：http://tz.huixinmuqiang.cn

================================================================================
来源：http://jo.szxytkj.cn

[R01] shebang 与严格模式
来源：http://ef.521024.cn

#!/usr/bin/env bash
来源：http://tl.nszjky.cn

set -euo pipefail
来源：http://nx.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://fp.asd995.cn

name="Tom"; echo "$name"
来源：http://he.yuexingan06.cn

[R03] 只读变量
来源：http://wn.yuexingan06.cn

readonly PI=3.14
来源：http://gp.yuexingan06.cn

[R04] 位置参数
来源：http://qw.bjjhwx.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wu.yuexingan06.cn

[R05] 参数默认值
来源：http://ns.huanxung.cn

name="${1:-default}"
来源：http://ss.shxzukj.cn

[R06] 判断命令是否存在
来源：http://vx.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ug.shtwfgs.cn

[R07] if 判断文件
来源：http://ui.nszjky.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zz.jianghongdianzi.cn

[R08] 数值比较
来源：http://gq.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zk.szsharing.cn

[R09] 字符串比较
来源：http://vn.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ga.nszjky.cn

[R10] 正则匹配
来源：http://cb.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cd.yuntaijiaju.cn

[R11] case 多分支
来源：http://tp.huanxung.cn

case "$1" in
来源：http://vx.szsharing.cn

start) echo "启动" ;;
来源：http://co.szxytkj.cn

stop)  echo "停止" ;;
来源：http://lw.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://do.colortex.cn

esac
来源：http://gi.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://jw.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://or.huixiangedu.cn

[R13] for 计数循环
来源：http://wa.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://xl.asd995.cn

[R14] C 风格 for
来源：http://rs.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://br.hahajie.cn

[R15] while 逐行读文件
来源：http://wu.asd995.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qe.nicolike.cn

[R16] until 等待条件
来源：http://np.yuexingan06.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wa.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://je.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ka.huanxung.cn

[R18] 遍历数组
来源：http://yj.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oy.newstarts.cn

[R19] 数组长度
来源：http://sv.panjiajie.cn

echo "${#arr[@]}"
来源：http://gc.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://li.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tq.9csxet.cn

[R21] 字符串长度
来源：http://bx.panjiajie.cn

echo "${#s}"
来源：http://sd.haigaiapp.cn

[R22] 截取子串
来源：http://za.jctech888.com.cn

echo "${s:0:5}"
来源：http://zu.yuexingan06.cn

[R23] 字符串替换
来源：http://cu.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bq.huixiangedu.cn

[R24] 大小写转换
来源：http://nk.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rp.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://fb.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ao.szsharing.cn

[R26] 命令替换
来源：http://hp.szxytkj.cn

now=$(date +%F); echo "$now"
来源：http://lr.jctech888.com.cn

[R27] 算术展开
来源：http://eo.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://tw.newstarts.cn

[R28] 浮点运算
来源：http://io.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://jw.huixinmuqiang.cn

[R29] 定义函数
来源：http://cy.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dh.bjjhwx.cn

[R30] 函数返回状态码
来源：http://gv.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://sm.nszjky.cn

[R31] 局部变量
来源：http://eg.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://qu.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://fw.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hc.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://lo.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://um.shtwfgs.cn

[R34] 退出时清理
来源：http://wt.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ve.huixiangedu.cn

[R35] 后台执行并等待
来源：http://ht.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://eq.szsharing.cn

[R36] 并发执行多个任务
来源：http://ch.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uu.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://of.shxzukj.cn

files=$(ls -1)
来源：http://qs.shtwfgs.cn

[R38] 管道串联
来源：http://yx.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://ay.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://cp.lnxyls.cn

cmd > out.log 2>&1
来源：http://ca.asd995.cn

[R40] 追加写日志
来源：http://fe.shtwfgs.cn

echo "log" >> out.log
来源：http://rx.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://hm.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://hj.wgjwhj.cn

[R42] 输入重定向
来源：http://pt.nicolike.cn

wc -l < a.txt
来源：http://uk.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://ju.gzmigu.cn

find . -name "*.log" -type f
来源：http://uq.gzmigu.cn

[R44] 按修改时间查找
来源：http://ni.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://dn.jctech888.com.cn

[R45] 批量删除
来源：http://iu.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://uw.521024.cn

[R46] 递归替换文件内容
来源：http://gw.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wd.szsharing.cn

[R47] sed 单行替换
来源：http://sb.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yf.521024.cn

[R48] awk 取指定列
来源：http://va.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://bw.gzmigu.cn

[R49] awk 带条件
来源：http://lu.huixiangedu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ep.jctech888.com.cn

[R50] awk 求和
来源：http://nj.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xk.521024.cn

[R51] 排序去重取前几
来源：http://gz.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pn.colortex.cn

[R52] 统计行数
来源：http://xu.nicolike.cn

wc -l a.txt
来源：http://av.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://ul.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fh.shxzukj.cn

[R54] 比较两个文件
来源：http://el.yuexingan06.cn

diff a.txt b.txt
来源：http://nl.colortex.cn

[R55] 压缩与解压
来源：http://rk.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cb.muxihuayi.cn

[R56] 远程拷贝
来源：http://hp.chemitech.net.cn

scp file user@host:/path/
来源：http://ro.szxytkj.cn

[R57] 远程执行命令
来源：http://bh.colortex.cn

ssh user@host 'uptime'
来源：http://xy.hnjuh.cn

[R58] 下载文件
来源：http://xy.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wg.9csxet.cn

[R59] 发 POST JSON
来源：http://om.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hd.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://ox.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vi.szsharing.cn

[R61] 磁盘占用
来源：http://ga.szxytkj.cn

df -h;  du -sh *
来源：http://kf.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://jb.bjjhwx.cn

du -ah . | sort -rh | head -10
来源：http://wo.yuexingan06.cn

[R63] 内存与进程
来源：http://eg.haigaiapp.cn

free -h;  ps aux | grep nginx
来源：http://vt.shxzskj.cn

[R64] 结束进程
来源：http://bn.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://ru.newstarts.cn

[R65] 查看端口占用
来源：http://ig.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://um.shxzskj.cn

[R66] 定时任务
来源：http://st.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://tt.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://kr.shtwfgs.cn

openssl rand -hex 16
来源：http://je.hahajie.cn

[R68] 计算文件校验值
来源：http://dh.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ki.huixiangedu.cn

[R69] 生成随机密码
来源：http://lm.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://um.shxzukj.cn

[R70] 时间戳与互转
来源：http://xz.huanxung.cn

date +%s;  date -d @1700000000
来源：http://bc.nicolike.cn

[R71] 日期格式化
来源：http://lv.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pf.9csxet.cn

[R72] 等待端口就绪
来源：http://kv.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rc.muxihuayi.cn

[R73] 分割大日志
来源：http://og.9csxet.cn


<!-- 参考信息 -->