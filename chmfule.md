代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://ai.huanxung.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ga.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tw.521024.cn

[Q15] 查询全部
来源：http://ne.panjiajie.cn

SELECT * FROM users;
来源：http://vh.huanxung.cn

[Q16] 查询指定列
来源：http://jl.huixinmuqiang.cn

SELECT id, name FROM users;
来源：http://oz.bjjhwx.cn

[Q17] 条件查询
来源：http://lh.panjiajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qn.shxzskj.cn

[Q18] 模糊匹配
来源：http://mk.huanxung.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://le.521024.cn

[Q19] 范围查询
来源：http://ed.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vt.521024.cn

[Q20] IN 列表
来源：http://rx.chemitech.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sd.hnjuh.cn

[Q21] 空值判断
来源：http://dy.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://uy.panjiajie.cn

[Q22] 排序
来源：http://vr.huixinmuqiang.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lo.yuexingan06.cn

[Q23] 分页
来源：http://jh.muxihuayi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gb.newstarts.cn

[Q24] 去重
来源：http://ws.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://zs.newstarts.cn

[Q25] 只取前 N 条
来源：http://ce.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qs.jianghongdianzi.cn

[Q26] 计数
来源：http://xs.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://qo.shxzukj.cn

[Q27] 条件计数
来源：http://ii.chemitech.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ms.wgjwhj.cn

[Q28] 求和与平均
来源：http://ao.yuexingan06.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://np.shxzskj.cn

[Q29] 最大最小值
来源：http://dh.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ws.huixinmuqiang.cn

[Q30] 分组统计
来源：http://or.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iw.huixiangedu.cn

[Q31] 分组后过滤
来源：http://du.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://re.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://gu.521024.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jc.shxzskj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ik.shxzukj.cn

[Q33] 多列分组
来源：http://jh.wgjwhj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kr.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://iz.shxzskj.cn

SELECT * FROM (
来源：http://zl.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vd.huanxung.cn

) t WHERE rn = 1;
来源：http://me.hahajie.cn

[Q35] 内连接
来源：http://hg.lnxyls.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xf.lnxyls.cn

[Q36] 左连接
来源：http://dq.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gk.gzmigu.cn

[Q37] 右连接
来源：http://re.panjiajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ki.shxzskj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vr.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lv.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://lk.jianghongdianzi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dm.shtwfgs.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dw.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rb.szxytkj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gs.yuntaijiaju.cn

[Q41] 多表连接
来源：http://fg.hahajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cz.shxzskj.cn

JOIN users u ON u.id = o.user_id
来源：http://kk.bookmarksfly.cn

JOIN products p ON p.id = o.product_id;
来源：http://nx.muxihuayi.cn

[Q42] 连接条件附加过滤
来源：http://ma.nicolike.cn

SELECT u.name, o.amount FROM users u
来源：http://wf.gzmigu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zr.szxytkj.cn

[Q43] 标量子查询
来源：http://wt.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://su.szxytkj.cn

[Q44] IN 子查询
来源：http://id.szxytkj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://km.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://yg.panjiajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://np.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yl.jianghongdianzi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fp.shtwfgs.cn

[Q47] 与平均值比较
来源：http://zf.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vn.szxytkj.cn

[Q48] CTE 公用表表达式
来源：http://uf.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hl.shxzukj.cn

SELECT * FROM t WHERE c > 5;
来源：http://ou.gzmigu.cn

[Q49] 更新单行
来源：http://xs.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://il.newstarts.cn

[Q50] 批量更新
来源：http://ox.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bw.panjiajie.cn

[Q51] 用子查询更新
来源：http://ef.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://np.yuntaijiaju.cn

[Q52] 删除指定行
来源：http://tk.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://zn.yuntaijiaju.cn

[Q53] 按条件删除
来源：http://pw.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://su.szxytkj.cn

[Q54] 清空表
来源：http://ox.wgjwhj.cn

TRUNCATE TABLE logs;
来源：http://zu.muxihuayi.cn

[Q55] 排名（并列占位）
来源：http://hv.jianghongdianzi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gb.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://ho.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qi.nszjky.cn

[Q57] 行号
来源：http://ek.jctech888.com.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ox.jianghongdianzi.cn

[Q58] 累计求和
来源：http://dn.huanxung.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gw.jianghongdianzi.cn

[Q59] 分组内累计
来源：http://on.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wm.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://sc.chemitech.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://na.haigaiapp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ho.hahajie.cn

[Q61] 移动平均
来源：http://td.lnxyls.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zm.chemitech.net.cn

[Q62] 分组占比
来源：http://ue.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://if.shxzskj.cn

[Q63] 开启事务
来源：http://yw.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vn.yuntaijiaju.cn

[Q64] 提交事务
来源：http://eg.huixiangedu.cn

COMMIT;
来源：http://qj.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://so.szsharing.cn

ROLLBACK;
来源：http://bs.huixiangedu.cn

[Q66] 行锁查询
来源：http://qr.hahajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wo.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://ra.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dm.haigaiapp.cn

[Q68] 保存点
来源：http://hv.wgjwhj.cn

SAVEPOINT sp1;
来源：http://ft.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://et.nicolike.cn

[Q69] 查看执行计划
来源：http://ty.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vv.yuexingan06.cn

[Q70] 更新统计信息
来源：http://ka.huixiangedu.cn

ANALYZE TABLE users;
来源：http://zh.chemitech.net.cn

[Q71] 查看建表语句
来源：http://dl.panjiajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oa.yuntaijiaju.cn

[Q72] 查看索引
来源：http://fi.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://nr.jctech888.com.cn

[Q73] 查看表状态
来源：http://wx.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jo.shtwfgs.cn

[Q74] 强制使用索引
来源：http://zm.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ml.haigaiapp.cn

[Q75] 日期格式化
来源：http://ze.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jo.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yb.jctech888.com.cn

[Q76] 按天统计
来源：http://jg.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pf.huixiangedu.cn

[Q77] 时间加减
来源：http://or.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fh.nicolike.cn

[Q78] 当前时间
来源：http://ew.shxzskj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nj.lnxyls.cn

[Q79] 字符串拼接
来源：http://jo.wgjwhj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ns.muxihuayi.cn

[Q80] 字符串截取
来源：http://jm.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tx.nszjky.cn

[Q81] 字符串替换
来源：http://lf.9csxet.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iq.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://lh.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://of.huixiangedu.cn

[Q83] 大小写转换
来源：http://hf.huanxung.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nu.521024.cn

[Q84] 去除首尾空格
来源：http://xg.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://ks.szsharing.cn

[Q85] 数值取整
来源：http://ty.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rt.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://yt.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://em.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://zc.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zo.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://wf.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ze.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gu.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://ph.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kc.yuexingan06.cn

[Q90] 生成序号列
来源：http://pr.muxihuayi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qt.9csxet.cn

================================================================================
来源：http://ez.muxihuayi.cn

R. Bash 专题
来源：http://mb.wgjwhj.cn

================================================================================
来源：http://nu.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://qp.chemitech.net.cn

#!/usr/bin/env bash
来源：http://el.wgjwhj.cn

set -euo pipefail
来源：http://is.panjiajie.cn

[R02] 变量赋值与使用
来源：http://ts.9csxet.cn

name="Tom"; echo "$name"
来源：http://ep.yuexingan06.cn

[R03] 只读变量
来源：http://ys.jianghongdianzi.cn

readonly PI=3.14
来源：http://hq.bookmarksfly.cn

[R04] 位置参数
来源：http://kd.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cj.nszjky.cn

[R05] 参数默认值
来源：http://gb.wgjwhj.cn

name="${1:-default}"
来源：http://bj.panjiajie.cn

[R06] 判断命令是否存在
来源：http://oa.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://io.521024.cn

[R07] if 判断文件
来源：http://ql.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tw.muxihuayi.cn

[R08] 数值比较
来源：http://ri.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zf.huanxung.cn

[R09] 字符串比较
来源：http://jp.lnxyls.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ch.huixiangedu.cn

[R10] 正则匹配
来源：http://zh.panjiajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wr.bookmarksfly.cn

[R11] case 多分支
来源：http://gf.yuexingan06.cn

case "$1" in
来源：http://dv.shtwfgs.cn

start) echo "启动" ;;
来源：http://fm.panjiajie.cn

stop)  echo "停止" ;;
来源：http://fo.yuntaijiaju.cn

*)     echo "未知命令" ;;
来源：http://rd.hnjuh.cn

esac
来源：http://jr.asd995.cn

[R12] for 遍历文件
来源：http://ac.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://nj.hnjuh.cn

[R13] for 计数循环
来源：http://zd.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://zh.szsharing.cn

[R14] C 风格 for
来源：http://sg.jianghongdianzi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zb.colortex.cn

[R15] while 逐行读文件
来源：http://us.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fc.wgjwhj.cn

[R16] until 等待条件
来源：http://bx.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gf.haigaiapp.cn

[R17] 数组定义与取值
来源：http://ox.hahajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gy.shtwfgs.cn

[R18] 遍历数组
来源：http://uo.newstarts.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yd.wgjwhj.cn

[R19] 数组长度
来源：http://sg.hnjuh.cn

echo "${#arr[@]}"
来源：http://wq.gzmigu.cn

[R20] 关联数组（字典）
来源：http://uu.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hd.wgjwhj.cn

[R21] 字符串长度
来源：http://oj.jctech888.com.cn

echo "${#s}"
来源：http://ek.huixiangedu.cn

[R22] 截取子串
来源：http://dw.nicolike.cn

echo "${s:0:5}"
来源：http://xn.gzmigu.cn

[R23] 字符串替换
来源：http://oh.huixinmuqiang.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gg.chemitech.net.cn

[R24] 大小写转换
来源：http://zh.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yj.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://jm.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gu.panjiajie.cn

[R26] 命令替换
来源：http://nx.asd995.cn

now=$(date +%F); echo "$now"
来源：http://as.hahajie.cn

[R27] 算术展开
来源：http://ab.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://bt.shtwfgs.cn

[R28] 浮点运算
来源：http://jy.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://rr.asd995.cn

[R29] 定义函数
来源：http://oi.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xn.panjiajie.cn

[R30] 函数返回状态码
来源：http://mf.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://uk.colortex.cn

[R31] 局部变量
来源：http://hw.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://hk.chemitech.net.cn

[R32] 参数个数校验
来源：http://cx.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mg.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://ac.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bp.bjjhwx.cn

[R34] 退出时清理
来源：http://wg.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ar.9csxet.cn

[R35] 后台执行并等待
来源：http://cx.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://js.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://ef.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gw.newstarts.cn

[R37] 把输出赋给变量
来源：http://zs.gzmigu.cn

files=$(ls -1)
来源：http://yq.shxzskj.cn

[R38] 管道串联
来源：http://yh.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://mw.colortex.cn

[R39] 重定向标准输出与错误
来源：http://ak.colortex.cn

cmd > out.log 2>&1
来源：http://wa.colortex.cn

[R40] 追加写日志
来源：http://na.newstarts.cn

echo "log" >> out.log
来源：http://dl.nicolike.cn

[R41] 丢弃输出
来源：http://he.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://qr.colortex.cn

[R42] 输入重定向
来源：http://vt.szsharing.cn

wc -l < a.txt
来源：http://bp.nszjky.cn

[R43] 按名字查找文件
来源：http://fx.nszjky.cn

find . -name "*.log" -type f
来源：http://fm.shxzskj.cn

[R44] 按修改时间查找
来源：http://oe.hahajie.cn

find . -mtime -7 -type f
来源：http://xq.nszjky.cn

[R45] 批量删除
来源：http://pr.nicolike.cn

find . -name "*.tmp" -delete
来源：http://bo.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://lf.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ab.colortex.cn

[R47] sed 单行替换
来源：http://js.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kc.lnxyls.cn

[R48] awk 取指定列
来源：http://qk.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://fv.521024.cn

[R49] awk 带条件
来源：http://xu.asd995.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xv.nicolike.cn

[R50] awk 求和
来源：http://il.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bm.9csxet.cn

[R51] 排序去重取前几
来源：http://lr.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fx.521024.cn

[R52] 统计行数
来源：http://cy.szxytkj.cn

wc -l a.txt
来源：http://aw.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://kt.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zw.bjjhwx.cn

[R54] 比较两个文件
来源：http://pd.colortex.cn

diff a.txt b.txt
来源：http://yg.shtwfgs.cn

[R55] 压缩与解压
来源：http://zj.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bq.colortex.cn

[R56] 远程拷贝
来源：http://vo.huanxung.cn

scp file user@host:/path/
来源：http://zc.haigaiapp.cn

[R57] 远程执行命令
来源：http://me.lnxyls.cn

ssh user@host 'uptime'
来源：http://cu.gzmigu.cn

[R58] 下载文件
来源：http://hr.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fk.bjjhwx.cn

[R59] 发 POST JSON
来源：http://ig.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ew.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://wp.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yv.hahajie.cn

[R61] 磁盘占用
来源：http://ik.bjjhwx.cn

df -h;  du -sh *
来源：http://fc.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://pk.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://wr.shxzukj.cn

[R63] 内存与进程
来源：http://cl.wgjwhj.cn


<!-- 参考信息 -->