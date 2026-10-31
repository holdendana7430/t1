代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xm.shxzskj.cn

[Q11] 一次插入多行
来源：http://bo.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dh.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://ks.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jm.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xi.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://le.bjjhwx.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dk.huanxung.cn

[Q14] 存在则更新（upsert）
来源：http://ty.bookmarksfly.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://db.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cu.nicolike.cn

[Q15] 查询全部
来源：http://uz.lnxyls.cn

SELECT * FROM users;
来源：http://yh.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://ew.hahajie.cn

SELECT id, name FROM users;
来源：http://vj.521024.cn

[Q17] 条件查询
来源：http://ms.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cs.huixiangedu.cn

[Q18] 模糊匹配
来源：http://lf.lnxyls.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uk.jianghongdianzi.cn

[Q19] 范围查询
来源：http://xb.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ot.lnxyls.cn

[Q20] IN 列表
来源：http://oz.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ti.nicolike.cn

[Q21] 空值判断
来源：http://jx.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vk.newstarts.cn

[Q22] 排序
来源：http://ke.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ko.lnxyls.cn

[Q23] 分页
来源：http://at.jctech888.com.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ox.9csxet.cn

[Q24] 去重
来源：http://xo.szxytkj.cn

SELECT DISTINCT city FROM users;
来源：http://ny.panjiajie.cn

[Q25] 只取前 N 条
来源：http://wi.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zu.jctech888.com.cn

[Q26] 计数
来源：http://zn.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://pv.hnjuh.cn

[Q27] 条件计数
来源：http://yw.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ah.muxihuayi.cn

[Q28] 求和与平均
来源：http://wj.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zl.521024.cn

[Q29] 最大最小值
来源：http://vv.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bd.yuexingan06.cn

[Q30] 分组统计
来源：http://lx.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vv.nszjky.cn

[Q31] 分组后过滤
来源：http://yp.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yf.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://sz.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rx.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ud.lnxyls.cn

[Q33] 多列分组
来源：http://hz.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ah.chemitech.net.cn

[Q34] 每组取第一条
来源：http://pc.shxzukj.cn

SELECT * FROM (
来源：http://bk.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xu.shxzskj.cn

) t WHERE rn = 1;
来源：http://wo.wgjwhj.cn

[Q35] 内连接
来源：http://hp.lnxyls.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cd.hnjuh.cn

[Q36] 左连接
来源：http://dj.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hs.yuntaijiaju.cn

[Q37] 右连接
来源：http://iu.bjjhwx.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mk.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://if.asd995.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zw.nicolike.cn

[Q39] 自连接（查上下级）
来源：http://dv.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qf.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sv.wgjwhj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rr.chemitech.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cn.shtwfgs.cn

[Q41] 多表连接
来源：http://bn.shxzskj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ig.asd995.cn

JOIN users u ON u.id = o.user_id
来源：http://ko.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://wh.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://bl.jctech888.com.cn

SELECT u.name, o.amount FROM users u
来源：http://hk.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mu.chemitech.net.cn

[Q43] 标量子查询
来源：http://eg.jianghongdianzi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ka.521024.cn

[Q44] IN 子查询
来源：http://sq.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fi.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://hl.bookmarksfly.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ax.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pe.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gd.nicolike.cn

[Q47] 与平均值比较
来源：http://qd.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qe.gzmigu.cn

[Q48] CTE 公用表表达式
来源：http://xy.hnjuh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fv.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://is.wgjwhj.cn

[Q49] 更新单行
来源：http://mm.yuntaijiaju.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nk.lnxyls.cn

[Q50] 批量更新
来源：http://et.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hn.jctech888.com.cn

[Q51] 用子查询更新
来源：http://kz.muxihuayi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oo.nszjky.cn

[Q52] 删除指定行
来源：http://rp.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://dh.yuexingan06.cn

[Q53] 按条件删除
来源：http://df.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wl.gzmigu.cn

[Q54] 清空表
来源：http://po.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://wi.huanxung.cn

[Q55] 排名（并列占位）
来源：http://na.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bf.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://bt.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wz.521024.cn

[Q57] 行号
来源：http://ug.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://op.yuexingan06.cn

[Q58] 累计求和
来源：http://gm.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eg.chemitech.net.cn

[Q59] 分组内累计
来源：http://st.chemitech.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tb.shxzukj.cn

[Q60] 取上一行 / 下一行
来源：http://an.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fx.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gu.hahajie.cn

[Q61] 移动平均
来源：http://rl.bjjhwx.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dr.szsharing.cn

[Q62] 分组占比
来源：http://oz.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nc.nicolike.cn

[Q63] 开启事务
来源：http://it.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lb.yuntaijiaju.cn

[Q64] 提交事务
来源：http://jd.gzmigu.cn

COMMIT;
来源：http://jk.yuntaijiaju.cn

[Q65] 回滚事务
来源：http://rc.yuexingan06.cn

ROLLBACK;
来源：http://sh.gzmigu.cn

[Q66] 行锁查询
来源：http://kl.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oo.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://rk.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gs.newstarts.cn

[Q68] 保存点
来源：http://pc.huanxung.cn

SAVEPOINT sp1;
来源：http://nu.shxzskj.cn

ROLLBACK TO sp1;
来源：http://pi.chemitech.net.cn

[Q69] 查看执行计划
来源：http://ex.lnxyls.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yw.wgjwhj.cn

[Q70] 更新统计信息
来源：http://ne.huixiangedu.cn

ANALYZE TABLE users;
来源：http://pi.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://ot.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sb.szxytkj.cn

[Q72] 查看索引
来源：http://mf.panjiajie.cn

SHOW INDEX FROM users;
来源：http://sw.colortex.cn

[Q73] 查看表状态
来源：http://mc.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kp.lnxyls.cn

[Q74] 强制使用索引
来源：http://kw.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hu.colortex.cn

[Q75] 日期格式化
来源：http://mx.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wj.asd995.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jc.lnxyls.cn

[Q76] 按天统计
来源：http://wm.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qw.lnxyls.cn

[Q77] 时间加减
来源：http://sm.yuexingan06.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://be.asd995.cn

[Q78] 当前时间
来源：http://lw.gzmigu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zv.gzmigu.cn

[Q79] 字符串拼接
来源：http://tw.lnxyls.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uv.bjjhwx.cn

[Q80] 字符串截取
来源：http://sb.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://li.nicolike.cn

[Q81] 字符串替换
来源：http://oy.shxzskj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lt.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://cr.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lz.hahajie.cn

[Q83] 大小写转换
来源：http://rs.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sv.asd995.cn

[Q84] 去除首尾空格
来源：http://vk.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://wt.shtwfgs.cn

[Q85] 数值取整
来源：http://fo.szxytkj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cq.gzmigu.cn

[Q86] 读取 JSON 字段
来源：http://rj.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://il.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://uo.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vr.huixinmuqiang.cn

[Q88] 行转列（条件聚合）
来源：http://ge.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vn.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://by.hahajie.cn

[Q89] 判断表是否存在
来源：http://ii.jianghongdianzi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hd.huixiangedu.cn

[Q90] 生成序号列
来源：http://jb.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jr.chemitech.net.cn

================================================================================
来源：http://wo.szsharing.cn

R. Bash 专题
来源：http://xa.nszjky.cn

================================================================================
来源：http://ak.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://nh.9csxet.cn

#!/usr/bin/env bash
来源：http://qu.shxzskj.cn

set -euo pipefail
来源：http://zl.nicolike.cn

[R02] 变量赋值与使用
来源：http://bi.newstarts.cn

name="Tom"; echo "$name"
来源：http://wx.521024.cn

[R03] 只读变量
来源：http://ua.gzmigu.cn

readonly PI=3.14
来源：http://nf.shtwfgs.cn

[R04] 位置参数
来源：http://hj.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dq.nicolike.cn

[R05] 参数默认值
来源：http://qx.shxzskj.cn

name="${1:-default}"
来源：http://wd.haigaiapp.cn

[R06] 判断命令是否存在
来源：http://re.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://or.shxzskj.cn

[R07] if 判断文件
来源：http://hp.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rg.szsharing.cn

[R08] 数值比较
来源：http://ue.jianghongdianzi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uu.bookmarksfly.cn

[R09] 字符串比较
来源：http://qi.jctech888.com.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jm.szsharing.cn

[R10] 正则匹配
来源：http://ak.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xg.lnxyls.cn

[R11] case 多分支
来源：http://wi.hnjuh.cn

case "$1" in
来源：http://km.shtwfgs.cn

start) echo "启动" ;;
来源：http://qc.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://jt.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://sz.szxytkj.cn

esac
来源：http://ae.panjiajie.cn

[R12] for 遍历文件
来源：http://mw.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://rf.shtwfgs.cn

[R13] for 计数循环
来源：http://va.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://ja.521024.cn

[R14] C 风格 for
来源：http://oi.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ro.huanxung.cn

[R15] while 逐行读文件
来源：http://wd.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://of.521024.cn

[R16] until 等待条件
来源：http://wh.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gl.yuntaijiaju.cn

[R17] 数组定义与取值
来源：http://if.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yi.haigaiapp.cn

[R18] 遍历数组
来源：http://jt.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bv.colortex.cn

[R19] 数组长度
来源：http://bo.jianghongdianzi.cn

echo "${#arr[@]}"
来源：http://lf.nicolike.cn

[R20] 关联数组（字典）
来源：http://dv.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qw.panjiajie.cn

[R21] 字符串长度
来源：http://jd.nszjky.cn

echo "${#s}"
来源：http://cu.chemitech.net.cn

[R22] 截取子串
来源：http://pj.muxihuayi.cn

echo "${s:0:5}"
来源：http://pe.shxzskj.cn

[R23] 字符串替换
来源：http://zy.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hn.gzmigu.cn

[R24] 大小写转换
来源：http://no.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xw.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://op.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://or.shtwfgs.cn

[R26] 命令替换
来源：http://xw.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://ud.muxihuayi.cn

[R27] 算术展开
来源：http://es.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://nl.yuntaijiaju.cn

[R28] 浮点运算
来源：http://xb.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://cw.nicolike.cn

[R29] 定义函数
来源：http://sh.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://if.lnxyls.cn

[R30] 函数返回状态码
来源：http://aa.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://wy.jianghongdianzi.cn

[R31] 局部变量
来源：http://xg.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://wb.jctech888.com.cn

[R32] 参数个数校验
来源：http://kh.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ix.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://cc.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mn.yuntaijiaju.cn

[R34] 退出时清理
来源：http://md.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://no.colortex.cn

[R35] 后台执行并等待
来源：http://zs.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://eq.jianghongdianzi.cn

[R36] 并发执行多个任务
来源：http://hy.nszjky.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://po.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://jm.wgjwhj.cn

files=$(ls -1)
来源：http://no.wgjwhj.cn

[R38] 管道串联
来源：http://hl.szxytkj.cn

cat a.txt | grep -i error | wc -l
来源：http://ig.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://js.9csxet.cn

cmd > out.log 2>&1
来源：http://sp.hnjuh.cn

[R40] 追加写日志
来源：http://rm.szxytkj.cn

echo "log" >> out.log
来源：http://sl.521024.cn

[R41] 丢弃输出
来源：http://if.colortex.cn

cmd >/dev/null 2>&1
来源：http://xi.shxzskj.cn

[R42] 输入重定向
来源：http://ra.asd995.cn

wc -l < a.txt
来源：http://ki.muxihuayi.cn

[R43] 按名字查找文件
来源：http://zm.lnxyls.cn

find . -name "*.log" -type f
来源：http://bj.wgjwhj.cn

[R44] 按修改时间查找
来源：http://mr.wgjwhj.cn

find . -mtime -7 -type f
来源：http://ct.nicolike.cn

[R45] 批量删除
来源：http://vx.9csxet.cn

find . -name "*.tmp" -delete
来源：http://ih.newstarts.cn

[R46] 递归替换文件内容
来源：http://rz.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://df.huixiangedu.cn

[R47] sed 单行替换
来源：http://wd.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ic.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://nl.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://au.bjjhwx.cn

[R49] awk 带条件
来源：http://fe.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dq.521024.cn

[R50] awk 求和
来源：http://gd.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://de.muxihuayi.cn

[R51] 排序去重取前几
来源：http://wu.huixiangedu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zc.521024.cn

[R52] 统计行数
来源：http://vo.huixiangedu.cn

wc -l a.txt
来源：http://il.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://us.colortex.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tu.shtwfgs.cn

[R54] 比较两个文件
来源：http://cs.gzmigu.cn

diff a.txt b.txt
来源：http://al.muxihuayi.cn

[R55] 压缩与解压
来源：http://tl.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fg.lnxyls.cn

[R56] 远程拷贝
来源：http://hp.bjjhwx.cn

scp file user@host:/path/
来源：http://ky.newstarts.cn

[R57] 远程执行命令
来源：http://mv.colortex.cn

ssh user@host 'uptime'
来源：http://fa.jianghongdianzi.cn

[R58] 下载文件
来源：http://ai.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uv.haigaiapp.cn

[R59] 发 POST JSON
来源：http://xl.colortex.cn


<!-- 参考信息 -->