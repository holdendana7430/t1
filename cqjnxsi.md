代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jd.bjjhwx.cn

[Q11] 一次插入多行
来源：http://am.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ry.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://nv.shxzskj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gu.asd995.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ft.huixiangedu.cn

[Q13] 忽略重复插入
来源：http://wv.panjiajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vt.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://yt.lnxyls.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ir.jianghongdianzi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ch.shxzukj.cn

[Q15] 查询全部
来源：http://pd.szxytkj.cn

SELECT * FROM users;
来源：http://cs.hnjuh.cn

[Q16] 查询指定列
来源：http://rk.nicolike.cn

SELECT id, name FROM users;
来源：http://iy.huixinmuqiang.cn

[Q17] 条件查询
来源：http://se.bjjhwx.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ic.nszjky.cn

[Q18] 模糊匹配
来源：http://kg.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sp.newstarts.cn

[Q19] 范围查询
来源：http://em.yuexingan06.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ih.yuntaijiaju.cn

[Q20] IN 列表
来源：http://dz.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://um.hnjuh.cn

[Q21] 空值判断
来源：http://zc.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://po.bookmarksfly.cn

[Q22] 排序
来源：http://hr.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ff.lnxyls.cn

[Q23] 分页
来源：http://zd.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gt.chemitech.net.cn

[Q24] 去重
来源：http://du.szsharing.cn

SELECT DISTINCT city FROM users;
来源：http://kn.nicolike.cn

[Q25] 只取前 N 条
来源：http://zs.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bh.gzmigu.cn

[Q26] 计数
来源：http://ax.newstarts.cn

SELECT COUNT(*) FROM users;
来源：http://ee.gzmigu.cn

[Q27] 条件计数
来源：http://kt.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ml.shxzukj.cn

[Q28] 求和与平均
来源：http://kv.asd995.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ao.hahajie.cn

[Q29] 最大最小值
来源：http://al.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ff.newstarts.cn

[Q30] 分组统计
来源：http://tg.hahajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://je.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://ay.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fs.jctech888.com.cn

[Q32] 分组拼接字符串
来源：http://hc.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qq.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fm.colortex.cn

[Q33] 多列分组
来源：http://ic.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ph.huixiangedu.cn

[Q34] 每组取第一条
来源：http://ld.szsharing.cn

SELECT * FROM (
来源：http://zn.szsharing.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zp.chemitech.net.cn

) t WHERE rn = 1;
来源：http://em.wgjwhj.cn

[Q35] 内连接
来源：http://tm.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ww.hnjuh.cn

[Q36] 左连接
来源：http://xx.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ar.bjjhwx.cn

[Q37] 右连接
来源：http://uy.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zy.yuntaijiaju.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cy.lnxyls.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ay.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://dt.jianghongdianzi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qk.asd995.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://it.9csxet.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wy.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wq.panjiajie.cn

[Q41] 多表连接
来源：http://yj.szsharing.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://co.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://hj.jianghongdianzi.cn

JOIN products p ON p.id = o.product_id;
来源：http://ud.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://wd.gzmigu.cn

SELECT u.name, o.amount FROM users u
来源：http://cw.panjiajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bt.huanxung.cn

[Q43] 标量子查询
来源：http://bu.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://av.haigaiapp.cn

[Q44] IN 子查询
来源：http://cf.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hl.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://af.wgjwhj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gp.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mh.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ht.nicolike.cn

[Q47] 与平均值比较
来源：http://je.hahajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://td.asd995.cn

[Q48] CTE 公用表表达式
来源：http://mr.jctech888.com.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dn.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://sl.jctech888.com.cn

[Q49] 更新单行
来源：http://ta.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ee.muxihuayi.cn

[Q50] 批量更新
来源：http://hx.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bf.shxzskj.cn

[Q51] 用子查询更新
来源：http://bt.muxihuayi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xi.hnjuh.cn

[Q52] 删除指定行
来源：http://st.panjiajie.cn

DELETE FROM users WHERE id = 10;
来源：http://vc.haigaiapp.cn

[Q53] 按条件删除
来源：http://tm.gzmigu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lj.bookmarksfly.cn

[Q54] 清空表
来源：http://ra.haigaiapp.cn

TRUNCATE TABLE logs;
来源：http://ly.wgjwhj.cn

[Q55] 排名（并列占位）
来源：http://wh.lnxyls.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dl.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://be.jctech888.com.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xy.9csxet.cn

[Q57] 行号
来源：http://lc.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cd.colortex.cn

[Q58] 累计求和
来源：http://rp.muxihuayi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nt.nicolike.cn

[Q59] 分组内累计
来源：http://yl.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rq.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://gs.gzmigu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zl.haigaiapp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lz.9csxet.cn

[Q61] 移动平均
来源：http://an.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tm.huixinmuqiang.cn

[Q62] 分组占比
来源：http://zh.colortex.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://if.521024.cn

[Q63] 开启事务
来源：http://wt.wgjwhj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wt.huanxung.cn

[Q64] 提交事务
来源：http://lq.shxzskj.cn

COMMIT;
来源：http://cv.gzmigu.cn

[Q65] 回滚事务
来源：http://lj.muxihuayi.cn

ROLLBACK;
来源：http://cz.bookmarksfly.cn

[Q66] 行锁查询
来源：http://nn.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rb.szxytkj.cn

[Q67] 设置隔离级别
来源：http://gc.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ao.jctech888.com.cn

[Q68] 保存点
来源：http://pm.szsharing.cn

SAVEPOINT sp1;
来源：http://ek.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://eu.shtwfgs.cn

[Q69] 查看执行计划
来源：http://pd.wgjwhj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yt.chemitech.net.cn

[Q70] 更新统计信息
来源：http://zi.asd995.cn

ANALYZE TABLE users;
来源：http://ny.asd995.cn

[Q71] 查看建表语句
来源：http://kb.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rt.hnjuh.cn

[Q72] 查看索引
来源：http://su.nszjky.cn

SHOW INDEX FROM users;
来源：http://ux.jianghongdianzi.cn

[Q73] 查看表状态
来源：http://za.jctech888.com.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ir.jianghongdianzi.cn

[Q74] 强制使用索引
来源：http://mv.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zl.nszjky.cn

[Q75] 日期格式化
来源：http://lb.jctech888.com.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://av.bjjhwx.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bz.huanxung.cn

[Q76] 按天统计
来源：http://qo.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sz.panjiajie.cn

[Q77] 时间加减
来源：http://eb.huixinmuqiang.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ch.521024.cn

[Q78] 当前时间
来源：http://eq.lnxyls.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wo.jctech888.com.cn

[Q79] 字符串拼接
来源：http://id.nszjky.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fc.shtwfgs.cn

[Q80] 字符串截取
来源：http://ug.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vd.yuexingan06.cn

[Q81] 字符串替换
来源：http://yi.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wi.jctech888.com.cn

[Q82] 字符长度与字节长度
来源：http://vi.yuntaijiaju.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bf.hahajie.cn

[Q83] 大小写转换
来源：http://xo.yuexingan06.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zj.panjiajie.cn

[Q84] 去除首尾空格
来源：http://jo.shxzukj.cn

SELECT TRIM(name) FROM users;
来源：http://af.gzmigu.cn

[Q85] 数值取整
来源：http://vf.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mk.521024.cn

[Q86] 读取 JSON 字段
来源：http://qb.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://uj.wgjwhj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fz.lnxyls.cn

[Q88] 行转列（条件聚合）
来源：http://ii.szsharing.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wj.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ep.colortex.cn

[Q89] 判断表是否存在
来源：http://fl.muxihuayi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yx.shtwfgs.cn

[Q90] 生成序号列
来源：http://eh.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dm.hnjuh.cn

================================================================================
来源：http://hh.muxihuayi.cn

R. Bash 专题
来源：http://wm.panjiajie.cn

================================================================================
来源：http://ho.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://oc.jctech888.com.cn

#!/usr/bin/env bash
来源：http://zv.huixinmuqiang.cn

set -euo pipefail
来源：http://su.nicolike.cn

[R02] 变量赋值与使用
来源：http://sl.panjiajie.cn

name="Tom"; echo "$name"
来源：http://yc.hahajie.cn

[R03] 只读变量
来源：http://ay.panjiajie.cn

readonly PI=3.14
来源：http://jv.yuexingan06.cn

[R04] 位置参数
来源：http://lc.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qc.asd995.cn

[R05] 参数默认值
来源：http://fg.yuexingan06.cn

name="${1:-default}"
来源：http://oy.nszjky.cn

[R06] 判断命令是否存在
来源：http://hv.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ik.muxihuayi.cn

[R07] if 判断文件
来源：http://ch.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rc.shtwfgs.cn

[R08] 数值比较
来源：http://of.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sp.huixiangedu.cn

[R09] 字符串比较
来源：http://uo.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cd.shtwfgs.cn

[R10] 正则匹配
来源：http://su.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lx.newstarts.cn

[R11] case 多分支
来源：http://dv.shxzukj.cn

case "$1" in
来源：http://dt.huixiangedu.cn

start) echo "启动" ;;
来源：http://yl.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://pk.muxihuayi.cn

*)     echo "未知命令" ;;
来源：http://qd.hnjuh.cn

esac
来源：http://hd.shtwfgs.cn

[R12] for 遍历文件
来源：http://wq.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://na.hahajie.cn

[R13] for 计数循环
来源：http://mz.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://kk.wgjwhj.cn

[R14] C 风格 for
来源：http://qt.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://do.huixiangedu.cn

[R15] while 逐行读文件
来源：http://ij.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ja.shxzskj.cn

[R16] until 等待条件
来源：http://ry.newstarts.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ty.hahajie.cn

[R17] 数组定义与取值
来源：http://wz.bjjhwx.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zr.jctech888.com.cn

[R18] 遍历数组
来源：http://fb.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://so.521024.cn

[R19] 数组长度
来源：http://uf.jianghongdianzi.cn

echo "${#arr[@]}"
来源：http://ay.nszjky.cn

[R20] 关联数组（字典）
来源：http://td.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zt.nicolike.cn

[R21] 字符串长度
来源：http://bx.wgjwhj.cn

echo "${#s}"
来源：http://jy.9csxet.cn

[R22] 截取子串
来源：http://qi.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://vd.bookmarksfly.cn

[R23] 字符串替换
来源：http://jl.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vg.bjjhwx.cn

[R24] 大小写转换
来源：http://ov.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://em.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://zh.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rk.huanxung.cn

[R26] 命令替换
来源：http://lx.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://fm.shxzukj.cn

[R27] 算术展开
来源：http://me.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://rm.szsharing.cn

[R28] 浮点运算
来源：http://et.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://og.hahajie.cn

[R29] 定义函数
来源：http://yc.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iq.szxytkj.cn

[R30] 函数返回状态码
来源：http://xe.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://iv.yuntaijiaju.cn

[R31] 局部变量
来源：http://si.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://py.panjiajie.cn

[R32] 参数个数校验
来源：http://hp.chemitech.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qu.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://qu.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ca.9csxet.cn

[R34] 退出时清理
来源：http://ih.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bb.9csxet.cn

[R35] 后台执行并等待
来源：http://xr.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://my.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://kb.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bv.lnxyls.cn

[R37] 把输出赋给变量
来源：http://wg.jianghongdianzi.cn

files=$(ls -1)
来源：http://tr.9csxet.cn

[R38] 管道串联
来源：http://lb.szxytkj.cn

cat a.txt | grep -i error | wc -l
来源：http://tf.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://al.nszjky.cn

cmd > out.log 2>&1
来源：http://iy.haigaiapp.cn

[R40] 追加写日志
来源：http://bo.gzmigu.cn

echo "log" >> out.log
来源：http://em.hnjuh.cn

[R41] 丢弃输出
来源：http://pg.jctech888.com.cn

cmd >/dev/null 2>&1
来源：http://ht.huixiangedu.cn

[R42] 输入重定向
来源：http://nd.bookmarksfly.cn

wc -l < a.txt
来源：http://to.9csxet.cn

[R43] 按名字查找文件
来源：http://ib.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://gd.hahajie.cn

[R44] 按修改时间查找
来源：http://zq.panjiajie.cn

find . -mtime -7 -type f
来源：http://gd.hahajie.cn

[R45] 批量删除
来源：http://uk.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://ve.panjiajie.cn

[R46] 递归替换文件内容
来源：http://xs.muxihuayi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mg.huixiangedu.cn

[R47] sed 单行替换
来源：http://eg.9csxet.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ph.newstarts.cn

[R48] awk 取指定列
来源：http://al.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://ry.hahajie.cn

[R49] awk 带条件
来源：http://qr.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://md.hahajie.cn

[R50] awk 求和
来源：http://lz.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hn.nszjky.cn

[R51] 排序去重取前几
来源：http://ps.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cv.shtwfgs.cn

[R52] 统计行数
来源：http://oa.panjiajie.cn

wc -l a.txt
来源：http://xn.shxzskj.cn

[R53] 查看文件头与实时尾
来源：http://fh.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hn.huixiangedu.cn

[R54] 比较两个文件
来源：http://el.panjiajie.cn

diff a.txt b.txt
来源：http://ui.bjjhwx.cn

[R55] 压缩与解压
来源：http://ti.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xd.wgjwhj.cn

[R56] 远程拷贝
来源：http://au.wgjwhj.cn

scp file user@host:/path/
来源：http://tn.shxzukj.cn

[R57] 远程执行命令
来源：http://da.hnjuh.cn

ssh user@host 'uptime'
来源：http://pk.szxytkj.cn

[R58] 下载文件
来源：http://pe.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ds.szsharing.cn

[R59] 发 POST JSON
来源：http://qs.9csxet.cn


<!-- 参考信息 -->