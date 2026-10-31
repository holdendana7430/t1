代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://wu.shtwfgs.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ew.szsharing.cn

[Q13] 忽略重复插入
来源：http://qj.huixinmuqiang.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kr.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://tq.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pt.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://py.nicolike.cn

[Q15] 查询全部
来源：http://dm.panjiajie.cn

SELECT * FROM users;
来源：http://ml.hnjuh.cn

[Q16] 查询指定列
来源：http://mk.shxzukj.cn

SELECT id, name FROM users;
来源：http://ww.newstarts.cn

[Q17] 条件查询
来源：http://vu.hahajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ca.gzmigu.cn

[Q18] 模糊匹配
来源：http://es.hnjuh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ln.hahajie.cn

[Q19] 范围查询
来源：http://ar.chemitech.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jd.shxzskj.cn

[Q20] IN 列表
来源：http://jw.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kt.huixinmuqiang.cn

[Q21] 空值判断
来源：http://nu.huixinmuqiang.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://go.yuexingan06.cn

[Q22] 排序
来源：http://rg.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qg.asd995.cn

[Q23] 分页
来源：http://jd.newstarts.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fq.huixiangedu.cn

[Q24] 去重
来源：http://jj.newstarts.cn

SELECT DISTINCT city FROM users;
来源：http://th.newstarts.cn

[Q25] 只取前 N 条
来源：http://rc.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ij.asd995.cn

[Q26] 计数
来源：http://ul.gzmigu.cn

SELECT COUNT(*) FROM users;
来源：http://og.colortex.cn

[Q27] 条件计数
来源：http://tv.muxihuayi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sa.lnxyls.cn

[Q28] 求和与平均
来源：http://il.yuntaijiaju.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hc.huixiangedu.cn

[Q29] 最大最小值
来源：http://es.nszjky.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tm.huixiangedu.cn

[Q30] 分组统计
来源：http://ap.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://at.nicolike.cn

[Q31] 分组后过滤
来源：http://wd.jianghongdianzi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wl.chemitech.net.cn

[Q32] 分组拼接字符串
来源：http://vo.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ja.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bz.panjiajie.cn

[Q33] 多列分组
来源：http://bs.wgjwhj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tt.shxzskj.cn

[Q34] 每组取第一条
来源：http://oa.9csxet.cn

SELECT * FROM (
来源：http://th.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lb.chemitech.net.cn

) t WHERE rn = 1;
来源：http://wi.shxzukj.cn

[Q35] 内连接
来源：http://jv.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://db.521024.cn

[Q36] 左连接
来源：http://wp.521024.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hs.shxzukj.cn

[Q37] 右连接
来源：http://kt.bookmarksfly.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hq.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ib.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lw.asd995.cn

[Q39] 自连接（查上下级）
来源：http://su.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yf.nicolike.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://on.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bf.szxytkj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bh.hahajie.cn

[Q41] 多表连接
来源：http://vp.chemitech.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://oh.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://ks.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://on.jctech888.com.cn

[Q42] 连接条件附加过滤
来源：http://ix.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://rj.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vk.jctech888.com.cn

[Q43] 标量子查询
来源：http://ij.yuntaijiaju.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nn.shxzukj.cn

[Q44] IN 子查询
来源：http://ks.newstarts.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vp.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://dz.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qd.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vm.szxytkj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ui.shxzskj.cn

[Q47] 与平均值比较
来源：http://mt.jctech888.com.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kr.newstarts.cn

[Q48] CTE 公用表表达式
来源：http://qu.hnjuh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://el.shxzskj.cn

SELECT * FROM t WHERE c > 5;
来源：http://cu.shxzukj.cn

[Q49] 更新单行
来源：http://wh.chemitech.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xp.nicolike.cn

[Q50] 批量更新
来源：http://iy.bookmarksfly.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gu.hnjuh.cn

[Q51] 用子查询更新
来源：http://kl.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qe.szsharing.cn

[Q52] 删除指定行
来源：http://nb.panjiajie.cn

DELETE FROM users WHERE id = 10;
来源：http://ht.9csxet.cn

[Q53] 按条件删除
来源：http://ie.szxytkj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tj.shtwfgs.cn

[Q54] 清空表
来源：http://hm.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://ym.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://hv.lnxyls.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hu.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://yv.hnjuh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xd.huixiangedu.cn

[Q57] 行号
来源：http://wj.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gj.yuntaijiaju.cn

[Q58] 累计求和
来源：http://fa.yuntaijiaju.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ni.haigaiapp.cn

[Q59] 分组内累计
来源：http://dl.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://du.bookmarksfly.cn

[Q60] 取上一行 / 下一行
来源：http://bl.yuexingan06.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://no.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rm.bookmarksfly.cn

[Q61] 移动平均
来源：http://hl.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ko.bookmarksfly.cn

[Q62] 分组占比
来源：http://jz.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://de.shxzukj.cn

[Q63] 开启事务
来源：http://qs.nicolike.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://eq.gzmigu.cn

[Q64] 提交事务
来源：http://df.lnxyls.cn

COMMIT;
来源：http://my.huanxung.cn

[Q65] 回滚事务
来源：http://uv.521024.cn

ROLLBACK;
来源：http://xn.jianghongdianzi.cn

[Q66] 行锁查询
来源：http://hj.gzmigu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xt.shxzukj.cn

[Q67] 设置隔离级别
来源：http://cr.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vn.yuntaijiaju.cn

[Q68] 保存点
来源：http://vh.wgjwhj.cn

SAVEPOINT sp1;
来源：http://hj.gzmigu.cn

ROLLBACK TO sp1;
来源：http://pc.newstarts.cn

[Q69] 查看执行计划
来源：http://ne.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wz.szsharing.cn

[Q70] 更新统计信息
来源：http://ji.bookmarksfly.cn

ANALYZE TABLE users;
来源：http://xo.nszjky.cn

[Q71] 查看建表语句
来源：http://yi.haigaiapp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zu.gzmigu.cn

[Q72] 查看索引
来源：http://ds.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://nj.colortex.cn

[Q73] 查看表状态
来源：http://sn.gzmigu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uo.colortex.cn

[Q74] 强制使用索引
来源：http://mj.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ik.muxihuayi.cn

[Q75] 日期格式化
来源：http://os.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kx.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xx.9csxet.cn

[Q76] 按天统计
来源：http://sm.nszjky.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://af.chemitech.net.cn

[Q77] 时间加减
来源：http://yy.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mm.shtwfgs.cn

[Q78] 当前时间
来源：http://dn.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ic.chemitech.net.cn

[Q79] 字符串拼接
来源：http://et.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ij.lnxyls.cn

[Q80] 字符串截取
来源：http://xe.panjiajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gk.hahajie.cn

[Q81] 字符串替换
来源：http://yu.9csxet.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zt.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://is.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://md.nszjky.cn

[Q83] 大小写转换
来源：http://qi.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gl.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://ao.nicolike.cn

SELECT TRIM(name) FROM users;
来源：http://ry.gzmigu.cn

[Q85] 数值取整
来源：http://yb.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dc.jianghongdianzi.cn

[Q86] 读取 JSON 字段
来源：http://ve.nszjky.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ub.nicolike.cn

[Q87] JSON 字段做条件
来源：http://qd.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zq.muxihuayi.cn

[Q88] 行转列（条件聚合）
来源：http://zg.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kl.wgjwhj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pp.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://pp.szsharing.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vl.panjiajie.cn

[Q90] 生成序号列
来源：http://ff.szsharing.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bh.huanxung.cn

================================================================================
来源：http://ub.colortex.cn

R. Bash 专题
来源：http://gb.haigaiapp.cn

================================================================================
来源：http://xm.huanxung.cn

[R01] shebang 与严格模式
来源：http://ox.szsharing.cn

#!/usr/bin/env bash
来源：http://rh.hahajie.cn

set -euo pipefail
来源：http://vc.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://gp.9csxet.cn

name="Tom"; echo "$name"
来源：http://qn.muxihuayi.cn

[R03] 只读变量
来源：http://ku.haigaiapp.cn

readonly PI=3.14
来源：http://vj.yuntaijiaju.cn

[R04] 位置参数
来源：http://mu.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yv.nszjky.cn

[R05] 参数默认值
来源：http://ho.9csxet.cn

name="${1:-default}"
来源：http://ts.szxytkj.cn

[R06] 判断命令是否存在
来源：http://st.jctech888.com.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ey.panjiajie.cn

[R07] if 判断文件
来源：http://af.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jq.asd995.cn

[R08] 数值比较
来源：http://fp.huanxung.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kp.colortex.cn

[R09] 字符串比较
来源：http://eu.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nk.szsharing.cn

[R10] 正则匹配
来源：http://dz.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ll.hahajie.cn

[R11] case 多分支
来源：http://gc.bjjhwx.cn

case "$1" in
来源：http://ta.lnxyls.cn

start) echo "启动" ;;
来源：http://ec.nicolike.cn

stop)  echo "停止" ;;
来源：http://pa.szsharing.cn

*)     echo "未知命令" ;;
来源：http://cw.huixinmuqiang.cn

esac
来源：http://ui.521024.cn

[R12] for 遍历文件
来源：http://xc.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://wo.huixiangedu.cn

[R13] for 计数循环
来源：http://yn.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://pd.chemitech.net.cn

[R14] C 风格 for
来源：http://bt.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gp.chemitech.net.cn

[R15] while 逐行读文件
来源：http://on.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kh.shxzukj.cn

[R16] until 等待条件
来源：http://od.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ys.newstarts.cn

[R17] 数组定义与取值
来源：http://jd.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://io.shxzskj.cn

[R18] 遍历数组
来源：http://bs.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://no.shxzskj.cn

[R19] 数组长度
来源：http://yf.shxzskj.cn

echo "${#arr[@]}"
来源：http://vq.colortex.cn

[R20] 关联数组（字典）
来源：http://eo.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://et.9csxet.cn

[R21] 字符串长度
来源：http://io.lnxyls.cn

echo "${#s}"
来源：http://on.gzmigu.cn

[R22] 截取子串
来源：http://in.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://xa.yuntaijiaju.cn

[R23] 字符串替换
来源：http://tx.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xo.asd995.cn

[R24] 大小写转换
来源：http://tn.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ty.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://cx.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pd.huixiangedu.cn

[R26] 命令替换
来源：http://gl.shxzukj.cn

now=$(date +%F); echo "$now"
来源：http://ei.szxytkj.cn

[R27] 算术展开
来源：http://lf.newstarts.cn

echo $((1 + 2 * 3))
来源：http://hr.yuexingan06.cn

[R28] 浮点运算
来源：http://lg.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://ja.huixinmuqiang.cn

[R29] 定义函数
来源：http://pk.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hp.shtwfgs.cn

[R30] 函数返回状态码
来源：http://vl.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://er.haigaiapp.cn

[R31] 局部变量
来源：http://oe.haigaiapp.cn

f() { local x=1; echo "$x"; }
来源：http://js.yuexingan06.cn

[R32] 参数个数校验
来源：http://fi.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xq.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://hx.huanxung.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sm.muxihuayi.cn

[R34] 退出时清理
来源：http://ru.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://za.wgjwhj.cn

[R35] 后台执行并等待
来源：http://ck.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xl.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://ih.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://od.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://zd.yuexingan06.cn

files=$(ls -1)
来源：http://yw.521024.cn

[R38] 管道串联
来源：http://cb.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://mf.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://ik.nicolike.cn

cmd > out.log 2>&1
来源：http://ex.521024.cn

[R40] 追加写日志
来源：http://la.wgjwhj.cn

echo "log" >> out.log
来源：http://sf.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://ny.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://ri.wgjwhj.cn

[R42] 输入重定向
来源：http://yd.chemitech.net.cn

wc -l < a.txt
来源：http://dw.shxzskj.cn

[R43] 按名字查找文件
来源：http://ny.huanxung.cn

find . -name "*.log" -type f
来源：http://da.huixiangedu.cn

[R44] 按修改时间查找
来源：http://vw.shtwfgs.cn

find . -mtime -7 -type f
来源：http://rr.jianghongdianzi.cn

[R45] 批量删除
来源：http://hd.huanxung.cn

find . -name "*.tmp" -delete
来源：http://he.colortex.cn

[R46] 递归替换文件内容
来源：http://hg.asd995.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cu.bookmarksfly.cn

[R47] sed 单行替换
来源：http://id.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ul.bookmarksfly.cn

[R48] awk 取指定列
来源：http://cs.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://co.asd995.cn

[R49] awk 带条件
来源：http://fx.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jn.nszjky.cn

[R50] awk 求和
来源：http://ak.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ko.newstarts.cn

[R51] 排序去重取前几
来源：http://ha.hnjuh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ap.colortex.cn

[R52] 统计行数
来源：http://hf.panjiajie.cn

wc -l a.txt
来源：http://os.colortex.cn

[R53] 查看文件头与实时尾
来源：http://gc.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kp.muxihuayi.cn

[R54] 比较两个文件
来源：http://al.hahajie.cn

diff a.txt b.txt
来源：http://sv.bookmarksfly.cn

[R55] 压缩与解压
来源：http://hp.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dc.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://zq.yuntaijiaju.cn

scp file user@host:/path/
来源：http://pu.lnxyls.cn

[R57] 远程执行命令
来源：http://mz.shtwfgs.cn

ssh user@host 'uptime'
来源：http://ne.bookmarksfly.cn

[R58] 下载文件
来源：http://kq.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fm.nszjky.cn

[R59] 发 POST JSON
来源：http://wo.yuexingan06.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ut.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://cs.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ol.shxzukj.cn

[R61] 磁盘占用
来源：http://vw.huixinmuqiang.cn


<!-- 参考信息 -->