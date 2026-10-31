代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://wa.chemitech.net.cn

[Q07] 删除表
来源：http://us.yuexingan06.cn

DROP TABLE IF EXISTS orders;
来源：http://it.newstarts.cn

[Q08] 创建普通索引
来源：http://rc.szsharing.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tl.lnxyls.cn

[Q09] 创建唯一索引
来源：http://tw.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zu.muxihuayi.cn

[Q10] 插入单行
来源：http://zh.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kb.bjjhwx.cn

[Q11] 一次插入多行
来源：http://vy.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ii.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://zz.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qn.bjjhwx.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ub.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://cb.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ny.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://lv.huixiangedu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bv.asd995.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ai.gzmigu.cn

[Q15] 查询全部
来源：http://aq.huixinmuqiang.cn

SELECT * FROM users;
来源：http://ie.huixiangedu.cn

[Q16] 查询指定列
来源：http://hx.shxzskj.cn

SELECT id, name FROM users;
来源：http://pg.hnjuh.cn

[Q17] 条件查询
来源：http://et.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pd.nszjky.cn

[Q18] 模糊匹配
来源：http://xs.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yf.bjjhwx.cn

[Q19] 范围查询
来源：http://bc.shxzskj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oe.bjjhwx.cn

[Q20] IN 列表
来源：http://ee.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://df.bookmarksfly.cn

[Q21] 空值判断
来源：http://mg.huanxung.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pp.521024.cn

[Q22] 排序
来源：http://in.asd995.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rz.haigaiapp.cn

[Q23] 分页
来源：http://ir.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ja.colortex.cn

[Q24] 去重
来源：http://sp.hahajie.cn

SELECT DISTINCT city FROM users;
来源：http://yf.9csxet.cn

[Q25] 只取前 N 条
来源：http://jy.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://th.shxzukj.cn

[Q26] 计数
来源：http://py.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://yj.521024.cn

[Q27] 条件计数
来源：http://du.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ed.gzmigu.cn

[Q28] 求和与平均
来源：http://lb.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oh.jianghongdianzi.cn

[Q29] 最大最小值
来源：http://er.nszjky.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ty.muxihuayi.cn

[Q30] 分组统计
来源：http://bm.muxihuayi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nq.521024.cn

[Q31] 分组后过滤
来源：http://wu.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kk.nszjky.cn

[Q32] 分组拼接字符串
来源：http://cg.huixinmuqiang.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rs.bjjhwx.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://za.jctech888.com.cn

[Q33] 多列分组
来源：http://kt.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ar.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://uk.shtwfgs.cn

SELECT * FROM (
来源：http://zy.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ey.hnjuh.cn

) t WHERE rn = 1;
来源：http://ib.szxytkj.cn

[Q35] 内连接
来源：http://vs.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pk.huixiangedu.cn

[Q36] 左连接
来源：http://nn.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nn.haigaiapp.cn

[Q37] 右连接
来源：http://vk.nicolike.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wx.chemitech.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wq.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vv.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://jd.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gr.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ed.panjiajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ou.shxzskj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gy.asd995.cn

[Q41] 多表连接
来源：http://tt.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xk.haigaiapp.cn

JOIN users u ON u.id = o.user_id
来源：http://uy.bookmarksfly.cn

JOIN products p ON p.id = o.product_id;
来源：http://qc.yuexingan06.cn

[Q42] 连接条件附加过滤
来源：http://ad.521024.cn

SELECT u.name, o.amount FROM users u
来源：http://lh.bookmarksfly.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ux.jctech888.com.cn

[Q43] 标量子查询
来源：http://ye.asd995.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jy.panjiajie.cn

[Q44] IN 子查询
来源：http://eh.bjjhwx.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ua.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://fv.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dm.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wf.bookmarksfly.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kv.shxzskj.cn

[Q47] 与平均值比较
来源：http://ha.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wt.yuexingan06.cn

[Q48] CTE 公用表表达式
来源：http://nh.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://it.hnjuh.cn

SELECT * FROM t WHERE c > 5;
来源：http://an.jctech888.com.cn

[Q49] 更新单行
来源：http://hu.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://id.521024.cn

[Q50] 批量更新
来源：http://gf.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ni.haigaiapp.cn

[Q51] 用子查询更新
来源：http://ni.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ys.jctech888.com.cn

[Q52] 删除指定行
来源：http://ot.haigaiapp.cn

DELETE FROM users WHERE id = 10;
来源：http://ym.huixinmuqiang.cn

[Q53] 按条件删除
来源：http://xd.jianghongdianzi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://us.521024.cn

[Q54] 清空表
来源：http://ij.nicolike.cn

TRUNCATE TABLE logs;
来源：http://fz.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://jc.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ik.asd995.cn

[Q56] 密集排名（并列不占位）
来源：http://sx.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bq.hnjuh.cn

[Q57] 行号
来源：http://kk.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zg.haigaiapp.cn

[Q58] 累计求和
来源：http://wl.newstarts.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ov.bookmarksfly.cn

[Q59] 分组内累计
来源：http://jq.panjiajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ip.shtwfgs.cn

[Q60] 取上一行 / 下一行
来源：http://ii.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rc.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sw.huanxung.cn

[Q61] 移动平均
来源：http://hs.huanxung.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rz.nicolike.cn

[Q62] 分组占比
来源：http://ct.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ao.colortex.cn

[Q63] 开启事务
来源：http://vh.wgjwhj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bu.shxzskj.cn

[Q64] 提交事务
来源：http://bw.9csxet.cn

COMMIT;
来源：http://rb.bookmarksfly.cn

[Q65] 回滚事务
来源：http://dq.muxihuayi.cn

ROLLBACK;
来源：http://ty.bjjhwx.cn

[Q66] 行锁查询
来源：http://zd.haigaiapp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zs.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://rc.nszjky.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ro.hahajie.cn

[Q68] 保存点
来源：http://sw.521024.cn

SAVEPOINT sp1;
来源：http://lt.shtwfgs.cn

ROLLBACK TO sp1;
来源：http://eo.521024.cn

[Q69] 查看执行计划
来源：http://qv.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pg.asd995.cn

[Q70] 更新统计信息
来源：http://jn.chemitech.net.cn

ANALYZE TABLE users;
来源：http://ye.shxzskj.cn

[Q71] 查看建表语句
来源：http://nn.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zw.bjjhwx.cn

[Q72] 查看索引
来源：http://ux.szsharing.cn

SHOW INDEX FROM users;
来源：http://rk.jianghongdianzi.cn

[Q73] 查看表状态
来源：http://ga.huixiangedu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wi.nicolike.cn

[Q74] 强制使用索引
来源：http://qs.haigaiapp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hi.shxzskj.cn

[Q75] 日期格式化
来源：http://ew.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tn.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ix.hahajie.cn

[Q76] 按天统计
来源：http://uu.newstarts.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kb.yuntaijiaju.cn

[Q77] 时间加减
来源：http://pe.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dg.jctech888.com.cn

[Q78] 当前时间
来源：http://nn.jianghongdianzi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ne.wgjwhj.cn

[Q79] 字符串拼接
来源：http://bu.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ox.colortex.cn

[Q80] 字符串截取
来源：http://ig.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qn.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://pv.huixiangedu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wu.9csxet.cn

[Q82] 字符长度与字节长度
来源：http://vz.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cf.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://nc.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xv.9csxet.cn

[Q84] 去除首尾空格
来源：http://qk.jianghongdianzi.cn

SELECT TRIM(name) FROM users;
来源：http://qi.hahajie.cn

[Q85] 数值取整
来源：http://qj.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nb.hnjuh.cn

[Q86] 读取 JSON 字段
来源：http://zy.muxihuayi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://km.newstarts.cn

[Q87] JSON 字段做条件
来源：http://km.bookmarksfly.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pp.lnxyls.cn

[Q88] 行转列（条件聚合）
来源：http://ww.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ha.shxzskj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oa.szsharing.cn

[Q89] 判断表是否存在
来源：http://ak.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://de.muxihuayi.cn

[Q90] 生成序号列
来源：http://ll.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tn.9csxet.cn

================================================================================
来源：http://fi.szxytkj.cn

R. Bash 专题
来源：http://vd.yuexingan06.cn

================================================================================
来源：http://jz.colortex.cn

[R01] shebang 与严格模式
来源：http://tr.jctech888.com.cn

#!/usr/bin/env bash
来源：http://qm.521024.cn

set -euo pipefail
来源：http://yo.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://bm.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://bn.shxzukj.cn

[R03] 只读变量
来源：http://jd.shxzukj.cn

readonly PI=3.14
来源：http://nt.colortex.cn

[R04] 位置参数
来源：http://wo.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uc.nicolike.cn

[R05] 参数默认值
来源：http://tz.panjiajie.cn

name="${1:-default}"
来源：http://jv.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://zi.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qh.shxzukj.cn

[R07] if 判断文件
来源：http://tt.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qy.jianghongdianzi.cn

[R08] 数值比较
来源：http://ly.gzmigu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bb.panjiajie.cn

[R09] 字符串比较
来源：http://pm.lnxyls.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yq.gzmigu.cn

[R10] 正则匹配
来源：http://fi.yuexingan06.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sw.haigaiapp.cn

[R11] case 多分支
来源：http://bi.huanxung.cn

case "$1" in
来源：http://pl.chemitech.net.cn

start) echo "启动" ;;
来源：http://gk.colortex.cn

stop)  echo "停止" ;;
来源：http://nj.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://jl.chemitech.net.cn

esac
来源：http://un.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://zg.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://fv.muxihuayi.cn

[R13] for 计数循环
来源：http://gl.szxytkj.cn

for i in {1..10}; do echo "$i"; done
来源：http://sb.shtwfgs.cn

[R14] C 风格 for
来源：http://kc.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qz.nszjky.cn

[R15] while 逐行读文件
来源：http://qv.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ct.wgjwhj.cn

[R16] until 等待条件
来源：http://va.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xv.asd995.cn

[R17] 数组定义与取值
来源：http://yl.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qy.newstarts.cn

[R18] 遍历数组
来源：http://ms.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wr.jianghongdianzi.cn

[R19] 数组长度
来源：http://ab.huanxung.cn

echo "${#arr[@]}"
来源：http://re.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://mi.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mt.panjiajie.cn

[R21] 字符串长度
来源：http://wf.nszjky.cn

echo "${#s}"
来源：http://rf.newstarts.cn

[R22] 截取子串
来源：http://go.yuexingan06.cn

echo "${s:0:5}"
来源：http://hz.yuntaijiaju.cn

[R23] 字符串替换
来源：http://my.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pz.chemitech.net.cn

[R24] 大小写转换
来源：http://ui.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://na.panjiajie.cn

[R25] 去后缀 / 去前缀
来源：http://jo.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kf.hnjuh.cn

[R26] 命令替换
来源：http://yv.szxytkj.cn

now=$(date +%F); echo "$now"
来源：http://mt.haigaiapp.cn

[R27] 算术展开
来源：http://lf.yuntaijiaju.cn

echo $((1 + 2 * 3))
来源：http://mb.hahajie.cn

[R28] 浮点运算
来源：http://np.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://sy.bjjhwx.cn

[R29] 定义函数
来源：http://wv.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hf.muxihuayi.cn

[R30] 函数返回状态码
来源：http://wj.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://qp.nszjky.cn

[R31] 局部变量
来源：http://hh.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://qn.shxzukj.cn

[R32] 参数个数校验
来源：http://vh.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sm.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://id.gzmigu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zk.nicolike.cn

[R34] 退出时清理
来源：http://nh.yuexingan06.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ex.huixiangedu.cn

[R35] 后台执行并等待
来源：http://li.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gt.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://rd.shxzukj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uk.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://xk.muxihuayi.cn

files=$(ls -1)
来源：http://nw.521024.cn

[R38] 管道串联
来源：http://fg.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://lv.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://cq.jctech888.com.cn

cmd > out.log 2>&1
来源：http://mw.huixiangedu.cn

[R40] 追加写日志
来源：http://eg.huixinmuqiang.cn

echo "log" >> out.log
来源：http://qf.nicolike.cn

[R41] 丢弃输出
来源：http://wv.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://bh.hnjuh.cn

[R42] 输入重定向
来源：http://fl.szsharing.cn

wc -l < a.txt
来源：http://ww.jctech888.com.cn

[R43] 按名字查找文件
来源：http://cz.lnxyls.cn

find . -name "*.log" -type f
来源：http://jt.yuexingan06.cn

[R44] 按修改时间查找
来源：http://ua.haigaiapp.cn

find . -mtime -7 -type f
来源：http://il.colortex.cn

[R45] 批量删除
来源：http://wl.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://cb.szsharing.cn

[R46] 递归替换文件内容
来源：http://kn.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ls.yuexingan06.cn

[R47] sed 单行替换
来源：http://uf.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://uf.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://zw.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://vx.9csxet.cn

[R49] awk 带条件
来源：http://am.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aq.huixinmuqiang.cn

[R50] awk 求和
来源：http://dh.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rn.yuexingan06.cn

[R51] 排序去重取前几
来源：http://ya.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mk.panjiajie.cn

[R52] 统计行数
来源：http://mp.nszjky.cn

wc -l a.txt
来源：http://zb.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://hs.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ab.lnxyls.cn

[R54] 比较两个文件
来源：http://gq.shtwfgs.cn

diff a.txt b.txt
来源：http://td.bookmarksfly.cn

[R55] 压缩与解压
来源：http://lm.bookmarksfly.cn


<!-- 参考信息 -->