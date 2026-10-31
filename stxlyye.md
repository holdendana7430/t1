代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ud.asd995.cn

[Q11] 一次插入多行
来源：http://tc.szxytkj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sj.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://no.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sl.bjjhwx.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fj.521024.cn

[Q13] 忽略重复插入
来源：http://ra.521024.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wm.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://bk.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oh.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yd.hahajie.cn

[Q15] 查询全部
来源：http://ic.muxihuayi.cn

SELECT * FROM users;
来源：http://sk.colortex.cn

[Q16] 查询指定列
来源：http://yg.asd995.cn

SELECT id, name FROM users;
来源：http://zj.lnxyls.cn

[Q17] 条件查询
来源：http://oh.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ye.jctech888.com.cn

[Q18] 模糊匹配
来源：http://cz.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://df.shxzskj.cn

[Q19] 范围查询
来源：http://zh.huixiangedu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gs.bjjhwx.cn

[Q20] IN 列表
来源：http://sl.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yz.huanxung.cn

[Q21] 空值判断
来源：http://ah.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bq.szxytkj.cn

[Q22] 排序
来源：http://ff.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lu.chemitech.net.cn

[Q23] 分页
来源：http://kq.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ix.yuexingan06.cn

[Q24] 去重
来源：http://tv.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://fc.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://uv.bjjhwx.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eh.colortex.cn

[Q26] 计数
来源：http://fn.9csxet.cn

SELECT COUNT(*) FROM users;
来源：http://up.shxzukj.cn

[Q27] 条件计数
来源：http://pi.muxihuayi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ka.shxzskj.cn

[Q28] 求和与平均
来源：http://ur.szxytkj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nq.bookmarksfly.cn

[Q29] 最大最小值
来源：http://zf.szsharing.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lh.jctech888.com.cn

[Q30] 分组统计
来源：http://ea.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xy.wgjwhj.cn

[Q31] 分组后过滤
来源：http://du.bookmarksfly.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://km.huixinmuqiang.cn

[Q32] 分组拼接字符串
来源：http://ww.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qr.yuexingan06.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://od.hnjuh.cn

[Q33] 多列分组
来源：http://ua.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dy.haigaiapp.cn

[Q34] 每组取第一条
来源：http://zd.szxytkj.cn

SELECT * FROM (
来源：http://ut.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://su.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://cv.yuexingan06.cn

[Q35] 内连接
来源：http://ew.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lp.hnjuh.cn

[Q36] 左连接
来源：http://ck.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hl.huixiangedu.cn

[Q37] 右连接
来源：http://rm.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kr.shxzskj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ol.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ia.yuntaijiaju.cn

[Q39] 自连接（查上下级）
来源：http://hw.jianghongdianzi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cj.huixinmuqiang.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ep.muxihuayi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wa.colortex.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://og.nszjky.cn

[Q41] 多表连接
来源：http://ti.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ko.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://um.bookmarksfly.cn

JOIN products p ON p.id = o.product_id;
来源：http://bh.newstarts.cn

[Q42] 连接条件附加过滤
来源：http://ac.9csxet.cn

SELECT u.name, o.amount FROM users u
来源：http://cn.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ep.szsharing.cn

[Q43] 标量子查询
来源：http://dy.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xz.muxihuayi.cn

[Q44] IN 子查询
来源：http://ur.nszjky.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mm.bookmarksfly.cn

[Q45] EXISTS 判断存在
来源：http://zr.gzmigu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://co.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gx.colortex.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pl.jctech888.com.cn

[Q47] 与平均值比较
来源：http://fv.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kk.nicolike.cn

[Q48] CTE 公用表表达式
来源：http://qn.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yv.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://nm.szsharing.cn

[Q49] 更新单行
来源：http://dk.szxytkj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bx.jctech888.com.cn

[Q50] 批量更新
来源：http://qg.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tx.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://hb.chemitech.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bb.yuntaijiaju.cn

[Q52] 删除指定行
来源：http://bk.muxihuayi.cn

DELETE FROM users WHERE id = 10;
来源：http://hq.nszjky.cn

[Q53] 按条件删除
来源：http://aj.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sq.wgjwhj.cn

[Q54] 清空表
来源：http://xy.newstarts.cn

TRUNCATE TABLE logs;
来源：http://re.haigaiapp.cn

[Q55] 排名（并列占位）
来源：http://ra.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vv.szxytkj.cn

[Q56] 密集排名（并列不占位）
来源：http://ve.colortex.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://un.yuexingan06.cn

[Q57] 行号
来源：http://aa.nicolike.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ty.asd995.cn

[Q58] 累计求和
来源：http://cy.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hu.nicolike.cn

[Q59] 分组内累计
来源：http://sx.colortex.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jh.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://ti.yuntaijiaju.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xc.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ey.yuexingan06.cn

[Q61] 移动平均
来源：http://zt.haigaiapp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ga.jianghongdianzi.cn

[Q62] 分组占比
来源：http://nw.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://te.jianghongdianzi.cn

[Q63] 开启事务
来源：http://zb.shxzskj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wj.9csxet.cn

[Q64] 提交事务
来源：http://ri.szxytkj.cn

COMMIT;
来源：http://gh.bjjhwx.cn

[Q65] 回滚事务
来源：http://tg.jctech888.com.cn

ROLLBACK;
来源：http://yp.shtwfgs.cn

[Q66] 行锁查询
来源：http://pt.huanxung.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wp.muxihuayi.cn

[Q67] 设置隔离级别
来源：http://bt.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ya.huixiangedu.cn

[Q68] 保存点
来源：http://jg.9csxet.cn

SAVEPOINT sp1;
来源：http://vl.huixiangedu.cn

ROLLBACK TO sp1;
来源：http://op.nszjky.cn

[Q69] 查看执行计划
来源：http://ac.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hm.panjiajie.cn

[Q70] 更新统计信息
来源：http://wy.huanxung.cn

ANALYZE TABLE users;
来源：http://el.nicolike.cn

[Q71] 查看建表语句
来源：http://ek.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qp.colortex.cn

[Q72] 查看索引
来源：http://fa.521024.cn

SHOW INDEX FROM users;
来源：http://qs.colortex.cn

[Q73] 查看表状态
来源：http://gb.shxzskj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ki.jctech888.com.cn

[Q74] 强制使用索引
来源：http://mo.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ig.szxytkj.cn

[Q75] 日期格式化
来源：http://tl.chemitech.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xv.muxihuayi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dl.hahajie.cn

[Q76] 按天统计
来源：http://mw.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ad.shtwfgs.cn

[Q77] 时间加减
来源：http://qw.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mm.yuntaijiaju.cn

[Q78] 当前时间
来源：http://gj.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bx.chemitech.net.cn

[Q79] 字符串拼接
来源：http://xg.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zk.huanxung.cn

[Q80] 字符串截取
来源：http://hc.muxihuayi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vz.panjiajie.cn

[Q81] 字符串替换
来源：http://rx.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uy.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://en.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jt.shxzskj.cn

[Q83] 大小写转换
来源：http://an.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nn.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://zi.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://vp.chemitech.net.cn

[Q85] 数值取整
来源：http://nl.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tv.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://rq.9csxet.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cv.haigaiapp.cn

[Q87] JSON 字段做条件
来源：http://nh.gzmigu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ys.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://fb.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hy.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://si.gzmigu.cn

[Q89] 判断表是否存在
来源：http://zv.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dn.newstarts.cn

[Q90] 生成序号列
来源：http://ye.szsharing.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ch.muxihuayi.cn

================================================================================
来源：http://nl.lnxyls.cn

R. Bash 专题
来源：http://rz.haigaiapp.cn

================================================================================
来源：http://me.lnxyls.cn

[R01] shebang 与严格模式
来源：http://se.nicolike.cn

#!/usr/bin/env bash
来源：http://jk.9csxet.cn

set -euo pipefail
来源：http://vl.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://gf.haigaiapp.cn

name="Tom"; echo "$name"
来源：http://vi.yuexingan06.cn

[R03] 只读变量
来源：http://bt.jctech888.com.cn

readonly PI=3.14
来源：http://zw.nicolike.cn

[R04] 位置参数
来源：http://vq.shxzukj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cp.bookmarksfly.cn

[R05] 参数默认值
来源：http://lb.hnjuh.cn

name="${1:-default}"
来源：http://wz.hnjuh.cn

[R06] 判断命令是否存在
来源：http://vw.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eg.chemitech.net.cn

[R07] if 判断文件
来源：http://cq.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iz.panjiajie.cn

[R08] 数值比较
来源：http://na.panjiajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hn.panjiajie.cn

[R09] 字符串比较
来源：http://sf.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fs.bookmarksfly.cn

[R10] 正则匹配
来源：http://es.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ki.jianghongdianzi.cn

[R11] case 多分支
来源：http://lm.chemitech.net.cn

case "$1" in
来源：http://dy.jctech888.com.cn

start) echo "启动" ;;
来源：http://pw.shtwfgs.cn

stop)  echo "停止" ;;
来源：http://yp.nicolike.cn

*)     echo "未知命令" ;;
来源：http://ar.wgjwhj.cn

esac
来源：http://rw.szxytkj.cn

[R12] for 遍历文件
来源：http://na.shxzskj.cn

for f in *.txt; do echo "$f"; done
来源：http://lt.hnjuh.cn

[R13] for 计数循环
来源：http://qi.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://rr.shtwfgs.cn

[R14] C 风格 for
来源：http://nu.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lw.lnxyls.cn

[R15] while 逐行读文件
来源：http://wp.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sv.panjiajie.cn

[R16] until 等待条件
来源：http://ny.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wj.yuntaijiaju.cn

[R17] 数组定义与取值
来源：http://nt.shtwfgs.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dh.521024.cn

[R18] 遍历数组
来源：http://ng.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ko.yuexingan06.cn

[R19] 数组长度
来源：http://fu.jianghongdianzi.cn

echo "${#arr[@]}"
来源：http://kw.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://ja.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zu.huanxung.cn

[R21] 字符串长度
来源：http://id.yuntaijiaju.cn

echo "${#s}"
来源：http://cj.9csxet.cn

[R22] 截取子串
来源：http://et.huixiangedu.cn

echo "${s:0:5}"
来源：http://ao.huanxung.cn

[R23] 字符串替换
来源：http://rh.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fe.huanxung.cn

[R24] 大小写转换
来源：http://mb.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ol.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://zv.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hr.yuexingan06.cn

[R26] 命令替换
来源：http://it.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://zi.hahajie.cn

[R27] 算术展开
来源：http://da.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://ot.nicolike.cn

[R28] 浮点运算
来源：http://za.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://mb.muxihuayi.cn

[R29] 定义函数
来源：http://fb.yuexingan06.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wd.huixiangedu.cn

[R30] 函数返回状态码
来源：http://bx.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://js.hahajie.cn

[R31] 局部变量
来源：http://ei.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://sp.shtwfgs.cn

[R32] 参数个数校验
来源：http://zl.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xv.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://wr.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vj.hnjuh.cn

[R34] 退出时清理
来源：http://bw.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uj.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://xi.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tz.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://ro.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zw.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://ht.521024.cn

files=$(ls -1)
来源：http://ro.huixinmuqiang.cn

[R38] 管道串联
来源：http://lz.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://zr.shtwfgs.cn

[R39] 重定向标准输出与错误
来源：http://sh.9csxet.cn

cmd > out.log 2>&1
来源：http://nc.newstarts.cn

[R40] 追加写日志
来源：http://kf.shxzukj.cn

echo "log" >> out.log
来源：http://fh.nszjky.cn

[R41] 丢弃输出
来源：http://uk.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://ye.szxytkj.cn

[R42] 输入重定向
来源：http://gm.szsharing.cn

wc -l < a.txt
来源：http://gl.bjjhwx.cn

[R43] 按名字查找文件
来源：http://vk.nicolike.cn

find . -name "*.log" -type f
来源：http://yo.muxihuayi.cn

[R44] 按修改时间查找
来源：http://om.muxihuayi.cn

find . -mtime -7 -type f
来源：http://ml.yuntaijiaju.cn

[R45] 批量删除
来源：http://ni.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://jt.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://id.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ha.haigaiapp.cn

[R47] sed 单行替换
来源：http://fg.9csxet.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sw.shtwfgs.cn

[R48] awk 取指定列
来源：http://te.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://jp.shtwfgs.cn

[R49] awk 带条件
来源：http://cc.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ku.hahajie.cn

[R50] awk 求和
来源：http://vm.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ei.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://lt.nszjky.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mo.shtwfgs.cn

[R52] 统计行数
来源：http://dz.huixinmuqiang.cn

wc -l a.txt
来源：http://dp.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://ws.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hl.szxytkj.cn

[R54] 比较两个文件
来源：http://mu.wgjwhj.cn

diff a.txt b.txt
来源：http://tr.wgjwhj.cn

[R55] 压缩与解压
来源：http://tj.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ig.hahajie.cn

[R56] 远程拷贝
来源：http://fg.nicolike.cn

scp file user@host:/path/
来源：http://db.hahajie.cn

[R57] 远程执行命令
来源：http://lf.bookmarksfly.cn

ssh user@host 'uptime'
来源：http://yr.bjjhwx.cn

[R58] 下载文件
来源：http://jh.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://du.9csxet.cn

[R59] 发 POST JSON
来源：http://av.shtwfgs.cn


<!-- 参考信息 -->