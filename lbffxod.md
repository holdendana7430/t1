代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://fx.hahajie.cn

[Q07] 删除表
来源：http://fq.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://od.newstarts.cn

[Q08] 创建普通索引
来源：http://di.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xv.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://pi.jctech888.com.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ql.shxzskj.cn

[Q10] 插入单行
来源：http://bl.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ne.lnxyls.cn

[Q11] 一次插入多行
来源：http://km.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bx.521024.cn

[Q12] 插入后取自增 ID
来源：http://bd.wgjwhj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wb.hahajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://iv.chemitech.net.cn

[Q13] 忽略重复插入
来源：http://vy.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://id.lnxyls.cn

[Q14] 存在则更新（upsert）
来源：http://yd.muxihuayi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tx.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mb.huixiangedu.cn

[Q15] 查询全部
来源：http://up.chemitech.net.cn

SELECT * FROM users;
来源：http://hd.szsharing.cn

[Q16] 查询指定列
来源：http://fk.chemitech.net.cn

SELECT id, name FROM users;
来源：http://jf.shxzukj.cn

[Q17] 条件查询
来源：http://jp.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://am.newstarts.cn

[Q18] 模糊匹配
来源：http://xk.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ml.bookmarksfly.cn

[Q19] 范围查询
来源：http://wd.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fr.yuntaijiaju.cn

[Q20] IN 列表
来源：http://uu.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://th.gzmigu.cn

[Q21] 空值判断
来源：http://qb.panjiajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zz.hahajie.cn

[Q22] 排序
来源：http://un.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ut.szsharing.cn

[Q23] 分页
来源：http://tm.huixiangedu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ks.bjjhwx.cn

[Q24] 去重
来源：http://kn.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://cw.szsharing.cn

[Q25] 只取前 N 条
来源：http://qc.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vy.jctech888.com.cn

[Q26] 计数
来源：http://oe.szsharing.cn

SELECT COUNT(*) FROM users;
来源：http://fn.szxytkj.cn

[Q27] 条件计数
来源：http://xi.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vp.szsharing.cn

[Q28] 求和与平均
来源：http://vd.hnjuh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://up.chemitech.net.cn

[Q29] 最大最小值
来源：http://uk.hahajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://en.szsharing.cn

[Q30] 分组统计
来源：http://lf.newstarts.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://to.shxzskj.cn

[Q31] 分组后过滤
来源：http://pi.521024.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mb.nszjky.cn

[Q32] 分组拼接字符串
来源：http://zl.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ya.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ea.lnxyls.cn

[Q33] 多列分组
来源：http://pn.huixiangedu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mn.muxihuayi.cn

[Q34] 每组取第一条
来源：http://hi.szxytkj.cn

SELECT * FROM (
来源：http://fi.521024.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oq.shtwfgs.cn

) t WHERE rn = 1;
来源：http://hk.9csxet.cn

[Q35] 内连接
来源：http://dk.huanxung.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ar.lnxyls.cn

[Q36] 左连接
来源：http://kf.panjiajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ti.shxzskj.cn

[Q37] 右连接
来源：http://zq.szsharing.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://db.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qb.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ri.nszjky.cn

[Q39] 自连接（查上下级）
来源：http://kt.jianghongdianzi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rs.muxihuayi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ah.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ea.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bv.huixinmuqiang.cn

[Q41] 多表连接
来源：http://yf.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tf.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://bt.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://gt.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://yk.huixiangedu.cn

SELECT u.name, o.amount FROM users u
来源：http://is.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ux.panjiajie.cn

[Q43] 标量子查询
来源：http://zh.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ff.shxzskj.cn

[Q44] IN 子查询
来源：http://ov.shxzskj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wz.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://lp.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dx.hahajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jq.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://em.hahajie.cn

[Q47] 与平均值比较
来源：http://dh.colortex.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sp.521024.cn

[Q48] CTE 公用表表达式
来源：http://xj.asd995.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bl.jctech888.com.cn

SELECT * FROM t WHERE c > 5;
来源：http://iw.9csxet.cn

[Q49] 更新单行
来源：http://uf.shxzskj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ri.wgjwhj.cn

[Q50] 批量更新
来源：http://pg.colortex.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nr.shtwfgs.cn

[Q51] 用子查询更新
来源：http://kt.szxytkj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ey.hnjuh.cn

[Q52] 删除指定行
来源：http://id.huixiangedu.cn

DELETE FROM users WHERE id = 10;
来源：http://fk.muxihuayi.cn

[Q53] 按条件删除
来源：http://og.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ub.bjjhwx.cn

[Q54] 清空表
来源：http://sg.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://am.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://uf.gzmigu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vo.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://lf.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kg.hnjuh.cn

[Q57] 行号
来源：http://dm.jctech888.com.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wi.huixinmuqiang.cn

[Q58] 累计求和
来源：http://wz.jctech888.com.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kk.newstarts.cn

[Q59] 分组内累计
来源：http://tm.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cf.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://bm.jctech888.com.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yh.yuntaijiaju.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ot.jianghongdianzi.cn

[Q61] 移动平均
来源：http://he.lnxyls.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rp.gzmigu.cn

[Q62] 分组占比
来源：http://yg.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uu.wgjwhj.cn

[Q63] 开启事务
来源：http://wo.lnxyls.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ae.hnjuh.cn

[Q64] 提交事务
来源：http://pb.shxzukj.cn

COMMIT;
来源：http://tr.hahajie.cn

[Q65] 回滚事务
来源：http://sf.shxzukj.cn

ROLLBACK;
来源：http://mh.yuntaijiaju.cn

[Q66] 行锁查询
来源：http://wv.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sy.szsharing.cn

[Q67] 设置隔离级别
来源：http://lf.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://co.panjiajie.cn

[Q68] 保存点
来源：http://gx.gzmigu.cn

SAVEPOINT sp1;
来源：http://hp.asd995.cn

ROLLBACK TO sp1;
来源：http://rd.haigaiapp.cn

[Q69] 查看执行计划
来源：http://ik.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gp.yuexingan06.cn

[Q70] 更新统计信息
来源：http://th.bookmarksfly.cn

ANALYZE TABLE users;
来源：http://lv.nszjky.cn

[Q71] 查看建表语句
来源：http://oc.yuntaijiaju.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lk.521024.cn

[Q72] 查看索引
来源：http://nm.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://or.colortex.cn

[Q73] 查看表状态
来源：http://sp.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ik.newstarts.cn

[Q74] 强制使用索引
来源：http://hr.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hr.newstarts.cn

[Q75] 日期格式化
来源：http://kj.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gr.muxihuayi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uk.yuexingan06.cn

[Q76] 按天统计
来源：http://ch.szxytkj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://in.jctech888.com.cn

[Q77] 时间加减
来源：http://fj.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rx.yuexingan06.cn

[Q78] 当前时间
来源：http://nc.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uz.nszjky.cn

[Q79] 字符串拼接
来源：http://uw.shtwfgs.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ts.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://ey.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://us.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://pd.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yv.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://xs.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fs.shtwfgs.cn

[Q83] 大小写转换
来源：http://hw.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cg.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://jv.huixiangedu.cn

SELECT TRIM(name) FROM users;
来源：http://bm.bookmarksfly.cn

[Q85] 数值取整
来源：http://ph.yuntaijiaju.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xx.huixinmuqiang.cn

[Q86] 读取 JSON 字段
来源：http://rz.gzmigu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ma.huixiangedu.cn

[Q87] JSON 字段做条件
来源：http://jn.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://we.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://dk.521024.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nr.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cz.shxzskj.cn

[Q89] 判断表是否存在
来源：http://iq.jctech888.com.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rg.bookmarksfly.cn

[Q90] 生成序号列
来源：http://hv.huanxung.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yt.colortex.cn

================================================================================
来源：http://ln.panjiajie.cn

R. Bash 专题
来源：http://wd.nszjky.cn

================================================================================
来源：http://rv.hahajie.cn

[R01] shebang 与严格模式
来源：http://qy.yuexingan06.cn

#!/usr/bin/env bash
来源：http://hn.haigaiapp.cn

set -euo pipefail
来源：http://jz.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://pj.gzmigu.cn

name="Tom"; echo "$name"
来源：http://du.colortex.cn

[R03] 只读变量
来源：http://xx.panjiajie.cn

readonly PI=3.14
来源：http://pm.huixiangedu.cn

[R04] 位置参数
来源：http://ip.bookmarksfly.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ec.huixinmuqiang.cn

[R05] 参数默认值
来源：http://pl.muxihuayi.cn

name="${1:-default}"
来源：http://tq.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://qq.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://th.haigaiapp.cn

[R07] if 判断文件
来源：http://ys.521024.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pl.yuntaijiaju.cn

[R08] 数值比较
来源：http://jl.hahajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jp.wgjwhj.cn

[R09] 字符串比较
来源：http://eo.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ak.nszjky.cn

[R10] 正则匹配
来源：http://ow.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://km.bookmarksfly.cn

[R11] case 多分支
来源：http://ie.jianghongdianzi.cn

case "$1" in
来源：http://qj.hnjuh.cn

start) echo "启动" ;;
来源：http://lz.szsharing.cn

stop)  echo "停止" ;;
来源：http://dq.asd995.cn

*)     echo "未知命令" ;;
来源：http://su.szsharing.cn

esac
来源：http://zz.lnxyls.cn

[R12] for 遍历文件
来源：http://aa.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://zl.bookmarksfly.cn

[R13] for 计数循环
来源：http://um.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://tt.szxytkj.cn

[R14] C 风格 for
来源：http://jf.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ta.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://xh.yuexingan06.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yz.nicolike.cn

[R16] until 等待条件
来源：http://ni.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://en.yuntaijiaju.cn

[R17] 数组定义与取值
来源：http://jz.hahajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zn.szsharing.cn

[R18] 遍历数组
来源：http://uo.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qc.panjiajie.cn

[R19] 数组长度
来源：http://wr.shxzukj.cn

echo "${#arr[@]}"
来源：http://iy.wgjwhj.cn

[R20] 关联数组（字典）
来源：http://dn.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cv.9csxet.cn

[R21] 字符串长度
来源：http://of.szxytkj.cn

echo "${#s}"
来源：http://ev.jctech888.com.cn

[R22] 截取子串
来源：http://hz.shxzukj.cn

echo "${s:0:5}"
来源：http://el.wgjwhj.cn

[R23] 字符串替换
来源：http://cw.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uj.9csxet.cn

[R24] 大小写转换
来源：http://os.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mv.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://xe.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hj.jctech888.com.cn

[R26] 命令替换
来源：http://yd.colortex.cn

now=$(date +%F); echo "$now"
来源：http://aj.huanxung.cn

[R27] 算术展开
来源：http://jh.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://os.nszjky.cn

[R28] 浮点运算
来源：http://ha.521024.cn

echo "scale=2; 10/3" | bc
来源：http://tx.haigaiapp.cn

[R29] 定义函数
来源：http://cj.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oa.hahajie.cn

[R30] 函数返回状态码
来源：http://zr.521024.cn

f() { return 0; }; f || echo "失败了"
来源：http://ol.szxytkj.cn

[R31] 局部变量
来源：http://ay.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://gn.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://rm.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zn.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://hr.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ex.shtwfgs.cn

[R34] 退出时清理
来源：http://ip.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xn.bjjhwx.cn

[R35] 后台执行并等待
来源：http://wz.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qi.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://xi.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ep.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://sa.hnjuh.cn

files=$(ls -1)
来源：http://bc.haigaiapp.cn

[R38] 管道串联
来源：http://cl.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://xn.panjiajie.cn

[R39] 重定向标准输出与错误
来源：http://fk.huixiangedu.cn

cmd > out.log 2>&1
来源：http://qz.nszjky.cn

[R40] 追加写日志
来源：http://nl.hnjuh.cn

echo "log" >> out.log
来源：http://my.bookmarksfly.cn

[R41] 丢弃输出
来源：http://oz.colortex.cn

cmd >/dev/null 2>&1
来源：http://yq.lnxyls.cn

[R42] 输入重定向
来源：http://ck.shtwfgs.cn

wc -l < a.txt
来源：http://ff.newstarts.cn

[R43] 按名字查找文件
来源：http://fd.huixiangedu.cn

find . -name "*.log" -type f
来源：http://zl.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://ak.lnxyls.cn

find . -mtime -7 -type f
来源：http://vd.jianghongdianzi.cn

[R45] 批量删除
来源：http://zh.hahajie.cn

find . -name "*.tmp" -delete
来源：http://bz.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://cn.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ln.yuexingan06.cn

[R47] sed 单行替换
来源：http://fd.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cl.colortex.cn

[R48] awk 取指定列
来源：http://zt.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://bz.jctech888.com.cn

[R49] awk 带条件
来源：http://yq.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ap.hahajie.cn

[R50] awk 求和
来源：http://qu.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mx.huanxung.cn

[R51] 排序去重取前几
来源：http://ts.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xz.nicolike.cn

[R52] 统计行数
来源：http://hy.asd995.cn

wc -l a.txt
来源：http://rh.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://ua.gzmigu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mf.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://ug.huixinmuqiang.cn

diff a.txt b.txt
来源：http://dp.nszjky.cn

[R55] 压缩与解压
来源：http://ur.shxzskj.cn


<!-- 参考信息 -->