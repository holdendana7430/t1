代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://eh.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xk.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ex.lnxyls.cn

[Q15] 查询全部
来源：http://fl.huixiangedu.cn

SELECT * FROM users;
来源：http://xx.nszjky.cn

[Q16] 查询指定列
来源：http://vs.hahajie.cn

SELECT id, name FROM users;
来源：http://lt.yuexingan06.cn

[Q17] 条件查询
来源：http://ot.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oj.nicolike.cn

[Q18] 模糊匹配
来源：http://nb.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zt.jctech888.com.cn

[Q19] 范围查询
来源：http://bq.newstarts.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ug.wgjwhj.cn

[Q20] IN 列表
来源：http://oy.szxytkj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ht.bookmarksfly.cn

[Q21] 空值判断
来源：http://kl.colortex.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pv.bookmarksfly.cn

[Q22] 排序
来源：http://kw.jianghongdianzi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zn.yuexingan06.cn

[Q23] 分页
来源：http://fq.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zw.hahajie.cn

[Q24] 去重
来源：http://mk.gzmigu.cn

SELECT DISTINCT city FROM users;
来源：http://bq.nicolike.cn

[Q25] 只取前 N 条
来源：http://hc.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wg.huixiangedu.cn

[Q26] 计数
来源：http://tv.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://iz.nicolike.cn

[Q27] 条件计数
来源：http://vq.szxytkj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gu.hahajie.cn

[Q28] 求和与平均
来源：http://zr.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gi.yuexingan06.cn

[Q29] 最大最小值
来源：http://pe.muxihuayi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://oe.jianghongdianzi.cn

[Q30] 分组统计
来源：http://pf.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ag.lnxyls.cn

[Q31] 分组后过滤
来源：http://zs.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://df.521024.cn

[Q32] 分组拼接字符串
来源：http://ir.jctech888.com.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ud.bookmarksfly.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jl.bookmarksfly.cn

[Q33] 多列分组
来源：http://on.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://op.chemitech.net.cn

[Q34] 每组取第一条
来源：http://cb.panjiajie.cn

SELECT * FROM (
来源：http://uz.haigaiapp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pt.gzmigu.cn

) t WHERE rn = 1;
来源：http://ql.bookmarksfly.cn

[Q35] 内连接
来源：http://pt.nicolike.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cm.asd995.cn

[Q36] 左连接
来源：http://lm.wgjwhj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://aj.huixiangedu.cn

[Q37] 右连接
来源：http://ol.hahajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pk.chemitech.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zn.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://av.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://fi.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lz.huixiangedu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bm.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sx.shxzskj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iz.521024.cn

[Q41] 多表连接
来源：http://wo.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pz.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://ci.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://cl.521024.cn

[Q42] 连接条件附加过滤
来源：http://be.chemitech.net.cn

SELECT u.name, o.amount FROM users u
来源：http://oj.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ws.jianghongdianzi.cn

[Q43] 标量子查询
来源：http://ql.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xk.hahajie.cn

[Q44] IN 子查询
来源：http://dw.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ml.colortex.cn

[Q45] EXISTS 判断存在
来源：http://bu.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mq.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ve.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wc.wgjwhj.cn

[Q47] 与平均值比较
来源：http://uz.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hs.newstarts.cn

[Q48] CTE 公用表表达式
来源：http://ep.newstarts.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ub.huanxung.cn

SELECT * FROM t WHERE c > 5;
来源：http://ol.haigaiapp.cn

[Q49] 更新单行
来源：http://ju.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qs.9csxet.cn

[Q50] 批量更新
来源：http://ah.muxihuayi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bz.wgjwhj.cn

[Q51] 用子查询更新
来源：http://hu.huixiangedu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qt.jianghongdianzi.cn

[Q52] 删除指定行
来源：http://ln.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://kr.yuexingan06.cn

[Q53] 按条件删除
来源：http://us.szsharing.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pg.nszjky.cn

[Q54] 清空表
来源：http://zz.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://bs.asd995.cn

[Q55] 排名（并列占位）
来源：http://uv.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jc.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://al.hahajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ph.newstarts.cn

[Q57] 行号
来源：http://rz.jianghongdianzi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ht.chemitech.net.cn

[Q58] 累计求和
来源：http://qa.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gb.muxihuayi.cn

[Q59] 分组内累计
来源：http://ak.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ry.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://ef.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://el.haigaiapp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sc.huixiangedu.cn

[Q61] 移动平均
来源：http://py.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xr.muxihuayi.cn

[Q62] 分组占比
来源：http://mq.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ub.yuntaijiaju.cn

[Q63] 开启事务
来源：http://fa.yuntaijiaju.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ve.bjjhwx.cn

[Q64] 提交事务
来源：http://fc.shxzukj.cn

COMMIT;
来源：http://au.hnjuh.cn

[Q65] 回滚事务
来源：http://ty.newstarts.cn

ROLLBACK;
来源：http://hr.hahajie.cn

[Q66] 行锁查询
来源：http://da.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tn.nicolike.cn

[Q67] 设置隔离级别
来源：http://he.szxytkj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wq.huixinmuqiang.cn

[Q68] 保存点
来源：http://dv.wgjwhj.cn

SAVEPOINT sp1;
来源：http://fa.wgjwhj.cn

ROLLBACK TO sp1;
来源：http://vf.bjjhwx.cn

[Q69] 查看执行计划
来源：http://sb.yuntaijiaju.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ys.shxzskj.cn

[Q70] 更新统计信息
来源：http://fm.nszjky.cn

ANALYZE TABLE users;
来源：http://jo.jctech888.com.cn

[Q71] 查看建表语句
来源：http://ys.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lg.hahajie.cn

[Q72] 查看索引
来源：http://dc.lnxyls.cn

SHOW INDEX FROM users;
来源：http://rj.jianghongdianzi.cn

[Q73] 查看表状态
来源：http://sn.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ha.szxytkj.cn

[Q74] 强制使用索引
来源：http://ye.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fh.hahajie.cn

[Q75] 日期格式化
来源：http://ts.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vx.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zl.huixinmuqiang.cn

[Q76] 按天统计
来源：http://ep.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://km.bjjhwx.cn

[Q77] 时间加减
来源：http://ts.shtwfgs.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tg.haigaiapp.cn

[Q78] 当前时间
来源：http://bd.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xu.nicolike.cn

[Q79] 字符串拼接
来源：http://gd.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qw.wgjwhj.cn

[Q80] 字符串截取
来源：http://wa.shtwfgs.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://va.shxzskj.cn

[Q81] 字符串替换
来源：http://ud.nszjky.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sl.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://ta.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gd.wgjwhj.cn

[Q83] 大小写转换
来源：http://sz.szsharing.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zi.huixinmuqiang.cn

[Q84] 去除首尾空格
来源：http://ae.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://cp.muxihuayi.cn

[Q85] 数值取整
来源：http://lj.shtwfgs.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ha.521024.cn

[Q86] 读取 JSON 字段
来源：http://lj.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ct.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://ku.huixiangedu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nw.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://do.521024.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fi.shxzskj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vk.yuntaijiaju.cn

[Q89] 判断表是否存在
来源：http://cj.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ci.colortex.cn

[Q90] 生成序号列
来源：http://ud.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ss.yuntaijiaju.cn

================================================================================
来源：http://tz.bookmarksfly.cn

R. Bash 专题
来源：http://qw.9csxet.cn

================================================================================
来源：http://fe.hahajie.cn

[R01] shebang 与严格模式
来源：http://zs.jctech888.com.cn

#!/usr/bin/env bash
来源：http://eu.szsharing.cn

set -euo pipefail
来源：http://ls.521024.cn

[R02] 变量赋值与使用
来源：http://dw.huanxung.cn

name="Tom"; echo "$name"
来源：http://wp.wgjwhj.cn

[R03] 只读变量
来源：http://sw.szxytkj.cn

readonly PI=3.14
来源：http://ac.shtwfgs.cn

[R04] 位置参数
来源：http://ou.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sv.hahajie.cn

[R05] 参数默认值
来源：http://ly.jianghongdianzi.cn

name="${1:-default}"
来源：http://sr.521024.cn

[R06] 判断命令是否存在
来源：http://xk.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ji.hahajie.cn

[R07] if 判断文件
来源：http://lr.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dy.haigaiapp.cn

[R08] 数值比较
来源：http://vk.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yo.shxzukj.cn

[R09] 字符串比较
来源：http://oa.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wk.jianghongdianzi.cn

[R10] 正则匹配
来源：http://xv.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pu.huixiangedu.cn

[R11] case 多分支
来源：http://qf.newstarts.cn

case "$1" in
来源：http://lx.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://jk.nszjky.cn

stop)  echo "停止" ;;
来源：http://cw.nszjky.cn

*)     echo "未知命令" ;;
来源：http://qp.lnxyls.cn

esac
来源：http://ow.shxzukj.cn

[R12] for 遍历文件
来源：http://dk.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://qd.colortex.cn

[R13] for 计数循环
来源：http://yr.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://ow.asd995.cn

[R14] C 风格 for
来源：http://ho.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wz.jctech888.com.cn

[R15] while 逐行读文件
来源：http://ex.bjjhwx.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mi.shtwfgs.cn

[R16] until 等待条件
来源：http://hz.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ll.huixinmuqiang.cn

[R17] 数组定义与取值
来源：http://py.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zr.hnjuh.cn

[R18] 遍历数组
来源：http://np.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ub.huixiangedu.cn

[R19] 数组长度
来源：http://gr.shxzskj.cn

echo "${#arr[@]}"
来源：http://jg.gzmigu.cn

[R20] 关联数组（字典）
来源：http://aq.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nl.521024.cn

[R21] 字符串长度
来源：http://vs.nicolike.cn

echo "${#s}"
来源：http://ee.panjiajie.cn

[R22] 截取子串
来源：http://gi.hnjuh.cn

echo "${s:0:5}"
来源：http://km.bookmarksfly.cn

[R23] 字符串替换
来源：http://rg.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zc.gzmigu.cn

[R24] 大小写转换
来源：http://ec.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ys.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://fg.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://el.shtwfgs.cn

[R26] 命令替换
来源：http://sn.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://yz.9csxet.cn

[R27] 算术展开
来源：http://db.asd995.cn

echo $((1 + 2 * 3))
来源：http://wx.lnxyls.cn

[R28] 浮点运算
来源：http://ol.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://cs.yuntaijiaju.cn

[R29] 定义函数
来源：http://nv.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wn.asd995.cn

[R30] 函数返回状态码
来源：http://dr.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://pk.chemitech.net.cn

[R31] 局部变量
来源：http://ie.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://xo.hnjuh.cn

[R32] 参数个数校验
来源：http://rw.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://te.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://is.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rb.lnxyls.cn

[R34] 退出时清理
来源：http://kq.9csxet.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fg.shxzukj.cn

[R35] 后台执行并等待
来源：http://hc.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jw.gzmigu.cn

[R36] 并发执行多个任务
来源：http://qc.wgjwhj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eq.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://sf.jianghongdianzi.cn

files=$(ls -1)
来源：http://go.hahajie.cn

[R38] 管道串联
来源：http://jz.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://bf.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://ea.chemitech.net.cn

cmd > out.log 2>&1
来源：http://ej.nszjky.cn

[R40] 追加写日志
来源：http://lz.521024.cn

echo "log" >> out.log
来源：http://ye.bjjhwx.cn

[R41] 丢弃输出
来源：http://rf.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://jx.gzmigu.cn

[R42] 输入重定向
来源：http://pg.huixinmuqiang.cn

wc -l < a.txt
来源：http://cp.asd995.cn

[R43] 按名字查找文件
来源：http://kp.hnjuh.cn

find . -name "*.log" -type f
来源：http://vo.newstarts.cn

[R44] 按修改时间查找
来源：http://dl.nszjky.cn

find . -mtime -7 -type f
来源：http://xg.shxzskj.cn

[R45] 批量删除
来源：http://au.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://sn.szxytkj.cn

[R46] 递归替换文件内容
来源：http://cn.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gc.asd995.cn

[R47] sed 单行替换
来源：http://ea.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mi.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://oe.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://fk.bjjhwx.cn

[R49] awk 带条件
来源：http://nb.wgjwhj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jo.gzmigu.cn

[R50] awk 求和
来源：http://nr.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ym.panjiajie.cn

[R51] 排序去重取前几
来源：http://to.yuexingan06.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ux.hahajie.cn

[R52] 统计行数
来源：http://ig.jianghongdianzi.cn

wc -l a.txt
来源：http://ck.huanxung.cn

[R53] 查看文件头与实时尾
来源：http://ll.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yf.haigaiapp.cn

[R54] 比较两个文件
来源：http://mk.shxzskj.cn

diff a.txt b.txt
来源：http://wk.szsharing.cn

[R55] 压缩与解压
来源：http://ie.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zs.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://fr.yuexingan06.cn

scp file user@host:/path/
来源：http://aw.newstarts.cn

[R57] 远程执行命令
来源：http://se.521024.cn

ssh user@host 'uptime'
来源：http://zr.hahajie.cn

[R58] 下载文件
来源：http://ea.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fz.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://ru.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xy.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://vu.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://of.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://tj.yuexingan06.cn

df -h;  du -sh *
来源：http://mg.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://zd.521024.cn

du -ah . | sort -rh | head -10
来源：http://pf.shxzskj.cn

[R63] 内存与进程
来源：http://cf.chemitech.net.cn


<!-- 参考信息 -->