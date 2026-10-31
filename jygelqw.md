代发 wailian999

SELECT * FROM users;
来源：http://th.9csxet.cn

[Q16] 查询指定列
来源：http://iv.muxihuayi.cn

SELECT id, name FROM users;
来源：http://ld.chemitech.net.cn

[Q17] 条件查询
来源：http://my.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xw.hnjuh.cn

[Q18] 模糊匹配
来源：http://cw.hnjuh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nt.jctech888.com.cn

[Q19] 范围查询
来源：http://wr.huixiangedu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ba.huixinmuqiang.cn

[Q20] IN 列表
来源：http://xu.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qn.haigaiapp.cn

[Q21] 空值判断
来源：http://nh.szsharing.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://du.muxihuayi.cn

[Q22] 排序
来源：http://lc.szsharing.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bk.jianghongdianzi.cn

[Q23] 分页
来源：http://fr.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cd.shxzskj.cn

[Q24] 去重
来源：http://co.521024.cn

SELECT DISTINCT city FROM users;
来源：http://gf.newstarts.cn

[Q25] 只取前 N 条
来源：http://cu.bjjhwx.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fi.gzmigu.cn

[Q26] 计数
来源：http://hu.newstarts.cn

SELECT COUNT(*) FROM users;
来源：http://iu.huixinmuqiang.cn

[Q27] 条件计数
来源：http://ng.yuntaijiaju.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ts.szxytkj.cn

[Q28] 求和与平均
来源：http://dr.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rk.hahajie.cn

[Q29] 最大最小值
来源：http://oj.wgjwhj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ng.newstarts.cn

[Q30] 分组统计
来源：http://ja.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hs.lnxyls.cn

[Q31] 分组后过滤
来源：http://kq.hnjuh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://te.hahajie.cn

[Q32] 分组拼接字符串
来源：http://qy.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zn.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ix.chemitech.net.cn

[Q33] 多列分组
来源：http://yb.huixiangedu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zw.huixiangedu.cn

[Q34] 每组取第一条
来源：http://ng.chemitech.net.cn

SELECT * FROM (
来源：http://dv.521024.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qr.panjiajie.cn

) t WHERE rn = 1;
来源：http://ol.hnjuh.cn

[Q35] 内连接
来源：http://tj.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gn.haigaiapp.cn

[Q36] 左连接
来源：http://gu.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xe.shxzukj.cn

[Q37] 右连接
来源：http://zx.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://je.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://om.9csxet.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pu.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://iu.shxzskj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://te.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ru.521024.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hd.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lz.huixinmuqiang.cn

[Q41] 多表连接
来源：http://sl.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sv.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://tk.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://nj.muxihuayi.cn

[Q42] 连接条件附加过滤
来源：http://ik.nszjky.cn

SELECT u.name, o.amount FROM users u
来源：http://pn.panjiajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pp.asd995.cn

[Q43] 标量子查询
来源：http://ir.chemitech.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wd.newstarts.cn

[Q44] IN 子查询
来源：http://ed.bjjhwx.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mq.asd995.cn

[Q45] EXISTS 判断存在
来源：http://fd.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://io.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ir.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ad.gzmigu.cn

[Q47] 与平均值比较
来源：http://ij.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wg.shtwfgs.cn

[Q48] CTE 公用表表达式
来源：http://to.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qz.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://gt.haigaiapp.cn

[Q49] 更新单行
来源：http://dn.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zo.haigaiapp.cn

[Q50] 批量更新
来源：http://ve.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sx.huixiangedu.cn

[Q51] 用子查询更新
来源：http://ko.szxytkj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ih.nicolike.cn

[Q52] 删除指定行
来源：http://hx.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://ar.shxzukj.cn

[Q53] 按条件删除
来源：http://vm.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ps.bookmarksfly.cn

[Q54] 清空表
来源：http://eb.jctech888.com.cn

TRUNCATE TABLE logs;
来源：http://nw.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://bk.muxihuayi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hd.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://if.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://td.jctech888.com.cn

[Q57] 行号
来源：http://ba.9csxet.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ho.9csxet.cn

[Q58] 累计求和
来源：http://zx.nszjky.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://op.shxzukj.cn

[Q59] 分组内累计
来源：http://ne.yuntaijiaju.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kd.jctech888.com.cn

[Q60] 取上一行 / 下一行
来源：http://kr.wgjwhj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ul.lnxyls.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dn.muxihuayi.cn

[Q61] 移动平均
来源：http://fn.gzmigu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mg.wgjwhj.cn

[Q62] 分组占比
来源：http://rx.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dx.szsharing.cn

[Q63] 开启事务
来源：http://aj.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mb.huixinmuqiang.cn

[Q64] 提交事务
来源：http://fl.shxzskj.cn

COMMIT;
来源：http://oc.szsharing.cn

[Q65] 回滚事务
来源：http://gh.shtwfgs.cn

ROLLBACK;
来源：http://fh.panjiajie.cn

[Q66] 行锁查询
来源：http://px.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zv.hnjuh.cn

[Q67] 设置隔离级别
来源：http://mb.huixiangedu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rc.panjiajie.cn

[Q68] 保存点
来源：http://lq.szxytkj.cn

SAVEPOINT sp1;
来源：http://ra.huixinmuqiang.cn

ROLLBACK TO sp1;
来源：http://jk.huanxung.cn

[Q69] 查看执行计划
来源：http://mj.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rs.muxihuayi.cn

[Q70] 更新统计信息
来源：http://ru.lnxyls.cn

ANALYZE TABLE users;
来源：http://eu.colortex.cn

[Q71] 查看建表语句
来源：http://ab.szxytkj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mh.yuntaijiaju.cn

[Q72] 查看索引
来源：http://xs.gzmigu.cn

SHOW INDEX FROM users;
来源：http://cv.hnjuh.cn

[Q73] 查看表状态
来源：http://wh.gzmigu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yc.shxzskj.cn

[Q74] 强制使用索引
来源：http://wb.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://aa.huanxung.cn

[Q75] 日期格式化
来源：http://ry.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://no.colortex.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qi.haigaiapp.cn

[Q76] 按天统计
来源：http://vt.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cr.huixiangedu.cn

[Q77] 时间加减
来源：http://ff.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dr.hnjuh.cn

[Q78] 当前时间
来源：http://mw.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pw.shxzskj.cn

[Q79] 字符串拼接
来源：http://lc.hnjuh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ni.huixiangedu.cn

[Q80] 字符串截取
来源：http://mm.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zi.panjiajie.cn

[Q81] 字符串替换
来源：http://fw.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vc.muxihuayi.cn

[Q82] 字符长度与字节长度
来源：http://qk.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ku.bookmarksfly.cn

[Q83] 大小写转换
来源：http://iv.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kc.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://yg.bookmarksfly.cn

SELECT TRIM(name) FROM users;
来源：http://qd.huixiangedu.cn

[Q85] 数值取整
来源：http://gh.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://on.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://eh.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mk.newstarts.cn

[Q87] JSON 字段做条件
来源：http://pf.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mg.lnxyls.cn

[Q88] 行转列（条件聚合）
来源：http://xf.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mg.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://da.newstarts.cn

[Q89] 判断表是否存在
来源：http://zc.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sv.bjjhwx.cn

[Q90] 生成序号列
来源：http://zt.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nu.shxzukj.cn

================================================================================
来源：http://fz.szsharing.cn

R. Bash 专题
来源：http://fz.jianghongdianzi.cn

================================================================================
来源：http://hm.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://gb.wgjwhj.cn

#!/usr/bin/env bash
来源：http://my.hahajie.cn

set -euo pipefail
来源：http://rg.bjjhwx.cn

[R02] 变量赋值与使用
来源：http://hz.szsharing.cn

name="Tom"; echo "$name"
来源：http://wu.jianghongdianzi.cn

[R03] 只读变量
来源：http://dl.bjjhwx.cn

readonly PI=3.14
来源：http://si.gzmigu.cn

[R04] 位置参数
来源：http://mr.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zi.asd995.cn

[R05] 参数默认值
来源：http://it.wgjwhj.cn

name="${1:-default}"
来源：http://ad.gzmigu.cn

[R06] 判断命令是否存在
来源：http://mv.yuexingan06.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xv.bjjhwx.cn

[R07] if 判断文件
来源：http://cb.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gf.jianghongdianzi.cn

[R08] 数值比较
来源：http://ba.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bj.521024.cn

[R09] 字符串比较
来源：http://ji.szxytkj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gl.huixinmuqiang.cn

[R10] 正则匹配
来源：http://hx.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kw.yuntaijiaju.cn

[R11] case 多分支
来源：http://wj.jianghongdianzi.cn

case "$1" in
来源：http://it.yuexingan06.cn

start) echo "启动" ;;
来源：http://hw.asd995.cn

stop)  echo "停止" ;;
来源：http://bv.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://so.panjiajie.cn

esac
来源：http://lg.shxzskj.cn

[R12] for 遍历文件
来源：http://bi.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://bh.gzmigu.cn

[R13] for 计数循环
来源：http://bk.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://yj.panjiajie.cn

[R14] C 风格 for
来源：http://qt.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ua.bjjhwx.cn

[R15] while 逐行读文件
来源：http://hj.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xs.lnxyls.cn

[R16] until 等待条件
来源：http://bk.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ky.hnjuh.cn

[R17] 数组定义与取值
来源：http://wn.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ex.szxytkj.cn

[R18] 遍历数组
来源：http://wy.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xu.hnjuh.cn

[R19] 数组长度
来源：http://tj.chemitech.net.cn

echo "${#arr[@]}"
来源：http://cb.panjiajie.cn

[R20] 关联数组（字典）
来源：http://bx.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qy.nicolike.cn

[R21] 字符串长度
来源：http://qu.gzmigu.cn

echo "${#s}"
来源：http://xc.asd995.cn

[R22] 截取子串
来源：http://ku.muxihuayi.cn

echo "${s:0:5}"
来源：http://ct.nicolike.cn

[R23] 字符串替换
来源：http://gr.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jm.lnxyls.cn

[R24] 大小写转换
来源：http://oi.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yw.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://nk.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pe.bookmarksfly.cn

[R26] 命令替换
来源：http://ej.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://ch.yuntaijiaju.cn

[R27] 算术展开
来源：http://hj.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://fq.haigaiapp.cn

[R28] 浮点运算
来源：http://ru.521024.cn

echo "scale=2; 10/3" | bc
来源：http://xj.shxzukj.cn

[R29] 定义函数
来源：http://eq.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cg.hahajie.cn

[R30] 函数返回状态码
来源：http://pm.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://do.newstarts.cn

[R31] 局部变量
来源：http://zw.shxzukj.cn

f() { local x=1; echo "$x"; }
来源：http://tz.nicolike.cn

[R32] 参数个数校验
来源：http://rv.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cb.colortex.cn

[R33] 捕获错误并提示行号
来源：http://un.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ry.521024.cn

[R34] 退出时清理
来源：http://hr.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jg.9csxet.cn

[R35] 后台执行并等待
来源：http://rq.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nz.shxzskj.cn

[R36] 并发执行多个任务
来源：http://in.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vf.newstarts.cn

[R37] 把输出赋给变量
来源：http://aw.hnjuh.cn

files=$(ls -1)
来源：http://hf.bookmarksfly.cn

[R38] 管道串联
来源：http://mq.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://uv.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://sk.bjjhwx.cn

cmd > out.log 2>&1
来源：http://id.9csxet.cn

[R40] 追加写日志
来源：http://qf.panjiajie.cn

echo "log" >> out.log
来源：http://ui.yuntaijiaju.cn

[R41] 丢弃输出
来源：http://dq.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://ne.jianghongdianzi.cn

[R42] 输入重定向
来源：http://sm.bjjhwx.cn

wc -l < a.txt
来源：http://vv.hnjuh.cn

[R43] 按名字查找文件
来源：http://vt.szsharing.cn

find . -name "*.log" -type f
来源：http://hp.hnjuh.cn

[R44] 按修改时间查找
来源：http://xe.nicolike.cn

find . -mtime -7 -type f
来源：http://mb.szsharing.cn

[R45] 批量删除
来源：http://zh.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://kz.gzmigu.cn

[R46] 递归替换文件内容
来源：http://wd.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pa.bjjhwx.cn

[R47] sed 单行替换
来源：http://su.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://al.haigaiapp.cn

[R48] awk 取指定列
来源：http://uo.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://gf.colortex.cn

[R49] awk 带条件
来源：http://ny.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xn.nicolike.cn

[R50] awk 求和
来源：http://ln.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bv.haigaiapp.cn

[R51] 排序去重取前几
来源：http://ah.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ux.szxytkj.cn

[R52] 统计行数
来源：http://zs.panjiajie.cn

wc -l a.txt
来源：http://zl.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://vv.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tg.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://ag.shtwfgs.cn

diff a.txt b.txt
来源：http://nl.hahajie.cn

[R55] 压缩与解压
来源：http://dl.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qe.chemitech.net.cn

[R56] 远程拷贝
来源：http://yq.wgjwhj.cn

scp file user@host:/path/
来源：http://rt.lnxyls.cn

[R57] 远程执行命令
来源：http://mo.bjjhwx.cn

ssh user@host 'uptime'
来源：http://fy.gzmigu.cn

[R58] 下载文件
来源：http://pa.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wm.szsharing.cn

[R59] 发 POST JSON
来源：http://fk.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nk.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://zt.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xm.hnjuh.cn

[R61] 磁盘占用
来源：http://am.lnxyls.cn

df -h;  du -sh *
来源：http://fq.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://jb.chemitech.net.cn

du -ah . | sort -rh | head -10
来源：http://io.nszjky.cn

[R63] 内存与进程
来源：http://qk.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://ly.muxihuayi.cn

[R64] 结束进程
来源：http://ut.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://tt.wgjwhj.cn

[R65] 查看端口占用
来源：http://gp.huixiangedu.cn


<!-- 参考信息 -->