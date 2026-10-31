代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://if.jianghongdianzi.cn

[Q09] 创建唯一索引
来源：http://ot.huixiangedu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ez.yuexingan06.cn

[Q10] 插入单行
来源：http://hr.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ic.muxihuayi.cn

[Q11] 一次插入多行
来源：http://gv.panjiajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://re.bookmarksfly.cn

[Q12] 插入后取自增 ID
来源：http://ar.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wd.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xz.nicolike.cn

[Q13] 忽略重复插入
来源：http://lq.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ht.gzmigu.cn

[Q14] 存在则更新（upsert）
来源：http://vo.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ri.wgjwhj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uu.hahajie.cn

[Q15] 查询全部
来源：http://vj.jianghongdianzi.cn

SELECT * FROM users;
来源：http://gx.gzmigu.cn

[Q16] 查询指定列
来源：http://wy.9csxet.cn

SELECT id, name FROM users;
来源：http://od.asd995.cn

[Q17] 条件查询
来源：http://gg.jctech888.com.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qe.newstarts.cn

[Q18] 模糊匹配
来源：http://qa.hnjuh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://im.jctech888.com.cn

[Q19] 范围查询
来源：http://cg.shtwfgs.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wb.lnxyls.cn

[Q20] IN 列表
来源：http://qu.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vy.bjjhwx.cn

[Q21] 空值判断
来源：http://uu.jianghongdianzi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ba.gzmigu.cn

[Q22] 排序
来源：http://db.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yh.asd995.cn

[Q23] 分页
来源：http://du.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iu.huixinmuqiang.cn

[Q24] 去重
来源：http://rb.szsharing.cn

SELECT DISTINCT city FROM users;
来源：http://um.huixiangedu.cn

[Q25] 只取前 N 条
来源：http://bs.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nu.wgjwhj.cn

[Q26] 计数
来源：http://jn.colortex.cn

SELECT COUNT(*) FROM users;
来源：http://za.bjjhwx.cn

[Q27] 条件计数
来源：http://cy.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://th.hahajie.cn

[Q28] 求和与平均
来源：http://vq.yuexingan06.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cu.lnxyls.cn

[Q29] 最大最小值
来源：http://au.jianghongdianzi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jw.panjiajie.cn

[Q30] 分组统计
来源：http://wm.szsharing.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gk.nszjky.cn

[Q31] 分组后过滤
来源：http://cy.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ns.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://fd.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sz.huixinmuqiang.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ma.yuexingan06.cn

[Q33] 多列分组
来源：http://wp.shtwfgs.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tq.szsharing.cn

[Q34] 每组取第一条
来源：http://yf.hnjuh.cn

SELECT * FROM (
来源：http://eq.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://we.hnjuh.cn

) t WHERE rn = 1;
来源：http://nt.jctech888.com.cn

[Q35] 内连接
来源：http://tz.hnjuh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yl.newstarts.cn

[Q36] 左连接
来源：http://te.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://os.yuntaijiaju.cn

[Q37] 右连接
来源：http://kc.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xb.gzmigu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wz.haigaiapp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ps.yuntaijiaju.cn

[Q39] 自连接（查上下级）
来源：http://vn.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pv.chemitech.net.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yv.newstarts.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zp.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vh.asd995.cn

[Q41] 多表连接
来源：http://pg.nszjky.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qg.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://eh.muxihuayi.cn

JOIN products p ON p.id = o.product_id;
来源：http://xx.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://lg.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://nz.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://td.521024.cn

[Q43] 标量子查询
来源：http://by.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ai.huixiangedu.cn

[Q44] IN 子查询
来源：http://jk.shxzskj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zj.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://wa.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jx.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xp.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iz.shxzskj.cn

[Q47] 与平均值比较
来源：http://yl.nicolike.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lp.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://ej.asd995.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tr.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://bu.panjiajie.cn

[Q49] 更新单行
来源：http://rs.bookmarksfly.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ro.jianghongdianzi.cn

[Q50] 批量更新
来源：http://vp.chemitech.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://px.haigaiapp.cn

[Q51] 用子查询更新
来源：http://ww.asd995.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dl.asd995.cn

[Q52] 删除指定行
来源：http://gs.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://on.521024.cn

[Q53] 按条件删除
来源：http://kw.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nt.huixiangedu.cn

[Q54] 清空表
来源：http://je.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://ys.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://kl.panjiajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ai.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://ea.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rz.jctech888.com.cn

[Q57] 行号
来源：http://jo.nicolike.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://no.shxzukj.cn

[Q58] 累计求和
来源：http://sh.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qh.szsharing.cn

[Q59] 分组内累计
来源：http://kj.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pb.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://qo.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qs.yuntaijiaju.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bd.huixiangedu.cn

[Q61] 移动平均
来源：http://bi.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.nicolike.cn

[Q62] 分组占比
来源：http://zl.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wm.szxytkj.cn

[Q63] 开启事务
来源：http://yw.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gh.bookmarksfly.cn

[Q64] 提交事务
来源：http://kl.nicolike.cn

COMMIT;
来源：http://yw.gzmigu.cn

[Q65] 回滚事务
来源：http://yz.muxihuayi.cn

ROLLBACK;
来源：http://he.lnxyls.cn

[Q66] 行锁查询
来源：http://tx.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bu.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://mq.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oa.nszjky.cn

[Q68] 保存点
来源：http://ef.colortex.cn

SAVEPOINT sp1;
来源：http://rc.szsharing.cn

ROLLBACK TO sp1;
来源：http://ec.wgjwhj.cn

[Q69] 查看执行计划
来源：http://qr.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lr.chemitech.net.cn

[Q70] 更新统计信息
来源：http://km.bookmarksfly.cn

ANALYZE TABLE users;
来源：http://ci.hnjuh.cn

[Q71] 查看建表语句
来源：http://gv.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hi.hahajie.cn

[Q72] 查看索引
来源：http://ze.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://xl.newstarts.cn

[Q73] 查看表状态
来源：http://bq.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uc.yuexingan06.cn

[Q74] 强制使用索引
来源：http://gb.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fr.521024.cn

[Q75] 日期格式化
来源：http://yd.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://iv.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://af.jianghongdianzi.cn

[Q76] 按天统计
来源：http://gv.colortex.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hw.shxzukj.cn

[Q77] 时间加减
来源：http://vl.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ec.chemitech.net.cn

[Q78] 当前时间
来源：http://em.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hp.wgjwhj.cn

[Q79] 字符串拼接
来源：http://sm.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kl.bookmarksfly.cn

[Q80] 字符串截取
来源：http://pd.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ih.9csxet.cn

[Q81] 字符串替换
来源：http://hm.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yz.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://tw.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jw.bjjhwx.cn

[Q83] 大小写转换
来源：http://fs.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gx.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://yp.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://hm.jianghongdianzi.cn

[Q85] 数值取整
来源：http://yz.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ou.yuntaijiaju.cn

[Q86] 读取 JSON 字段
来源：http://ly.nicolike.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uw.newstarts.cn

[Q87] JSON 字段做条件
来源：http://rx.wgjwhj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ix.9csxet.cn

[Q88] 行转列（条件聚合）
来源：http://fo.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://us.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uq.nszjky.cn

[Q89] 判断表是否存在
来源：http://hh.szsharing.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ek.haigaiapp.cn

[Q90] 生成序号列
来源：http://lt.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gq.jianghongdianzi.cn

================================================================================
来源：http://cw.lnxyls.cn

R. Bash 专题
来源：http://ix.muxihuayi.cn

================================================================================
来源：http://dm.nszjky.cn

[R01] shebang 与严格模式
来源：http://gh.chemitech.net.cn

#!/usr/bin/env bash
来源：http://gs.szsharing.cn

set -euo pipefail
来源：http://ri.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://fn.nicolike.cn

name="Tom"; echo "$name"
来源：http://mr.yuntaijiaju.cn

[R03] 只读变量
来源：http://qq.shxzskj.cn

readonly PI=3.14
来源：http://gi.jianghongdianzi.cn

[R04] 位置参数
来源：http://ai.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ne.szxytkj.cn

[R05] 参数默认值
来源：http://ib.chemitech.net.cn

name="${1:-default}"
来源：http://ms.huixinmuqiang.cn

[R06] 判断命令是否存在
来源：http://pj.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ch.huixiangedu.cn

[R07] if 判断文件
来源：http://aa.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ou.wgjwhj.cn

[R08] 数值比较
来源：http://wd.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://iv.szsharing.cn

[R09] 字符串比较
来源：http://lt.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ym.521024.cn

[R10] 正则匹配
来源：http://yo.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ju.colortex.cn

[R11] case 多分支
来源：http://gj.521024.cn

case "$1" in
来源：http://ho.chemitech.net.cn

start) echo "启动" ;;
来源：http://wf.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://px.yuntaijiaju.cn

*)     echo "未知命令" ;;
来源：http://vx.haigaiapp.cn

esac
来源：http://fc.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://bf.shtwfgs.cn

for f in *.txt; do echo "$f"; done
来源：http://up.shxzukj.cn

[R13] for 计数循环
来源：http://aj.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://in.huixiangedu.cn

[R14] C 风格 for
来源：http://zr.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ow.nicolike.cn

[R15] while 逐行读文件
来源：http://zn.huixiangedu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rq.huanxung.cn

[R16] until 等待条件
来源：http://li.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kf.huixiangedu.cn

[R17] 数组定义与取值
来源：http://wm.521024.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uf.szxytkj.cn

[R18] 遍历数组
来源：http://sl.hnjuh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bh.muxihuayi.cn

[R19] 数组长度
来源：http://bi.hnjuh.cn

echo "${#arr[@]}"
来源：http://wt.bookmarksfly.cn

[R20] 关联数组（字典）
来源：http://du.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://db.huanxung.cn

[R21] 字符串长度
来源：http://pb.yuexingan06.cn

echo "${#s}"
来源：http://me.panjiajie.cn

[R22] 截取子串
来源：http://gc.hahajie.cn

echo "${s:0:5}"
来源：http://jg.huixinmuqiang.cn

[R23] 字符串替换
来源：http://dn.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://po.colortex.cn

[R24] 大小写转换
来源：http://nd.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ne.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://xh.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ye.huixinmuqiang.cn

[R26] 命令替换
来源：http://pj.huixiangedu.cn

now=$(date +%F); echo "$now"
来源：http://mf.shtwfgs.cn

[R27] 算术展开
来源：http://wp.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://dp.lnxyls.cn

[R28] 浮点运算
来源：http://yk.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://sb.muxihuayi.cn

[R29] 定义函数
来源：http://cz.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pt.hnjuh.cn

[R30] 函数返回状态码
来源：http://ut.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://xm.chemitech.net.cn

[R31] 局部变量
来源：http://az.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://wd.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://ax.huixinmuqiang.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wj.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://wi.hnjuh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yy.hahajie.cn

[R34] 退出时清理
来源：http://az.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://oy.huixiangedu.cn

[R35] 后台执行并等待
来源：http://mf.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ph.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://kc.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dr.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://iy.shxzukj.cn

files=$(ls -1)
来源：http://qd.yuexingan06.cn

[R38] 管道串联
来源：http://ip.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://ar.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://lw.muxihuayi.cn

cmd > out.log 2>&1
来源：http://ui.nszjky.cn

[R40] 追加写日志
来源：http://vh.nszjky.cn

echo "log" >> out.log
来源：http://ry.yuntaijiaju.cn

[R41] 丢弃输出
来源：http://pp.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://iw.jctech888.com.cn

[R42] 输入重定向
来源：http://bi.huixiangedu.cn

wc -l < a.txt
来源：http://om.panjiajie.cn

[R43] 按名字查找文件
来源：http://qv.colortex.cn

find . -name "*.log" -type f
来源：http://oq.nicolike.cn

[R44] 按修改时间查找
来源：http://xz.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://qq.yuexingan06.cn

[R45] 批量删除
来源：http://fd.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://al.colortex.cn

[R46] 递归替换文件内容
来源：http://vk.chemitech.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://td.colortex.cn

[R47] sed 单行替换
来源：http://dt.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://px.bjjhwx.cn

[R48] awk 取指定列
来源：http://pt.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://jl.nszjky.cn

[R49] awk 带条件
来源：http://ry.asd995.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ej.newstarts.cn

[R50] awk 求和
来源：http://ak.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ip.chemitech.net.cn

[R51] 排序去重取前几
来源：http://ak.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gd.lnxyls.cn

[R52] 统计行数
来源：http://je.yuntaijiaju.cn

wc -l a.txt
来源：http://ts.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://hf.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mp.szsharing.cn

[R54] 比较两个文件
来源：http://kq.nszjky.cn

diff a.txt b.txt
来源：http://do.hnjuh.cn

[R55] 压缩与解压
来源：http://ob.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yu.szsharing.cn

[R56] 远程拷贝
来源：http://dk.haigaiapp.cn

scp file user@host:/path/
来源：http://mx.hahajie.cn

[R57] 远程执行命令
来源：http://oi.newstarts.cn


<!-- 参考信息 -->