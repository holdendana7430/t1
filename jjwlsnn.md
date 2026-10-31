代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bv.wgjwhj.cn

[Q20] IN 列表
来源：http://xp.jctech888.com.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mo.hnjuh.cn

[Q21] 空值判断
来源：http://am.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wj.bookmarksfly.cn

[Q22] 排序
来源：http://ba.nszjky.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yk.hnjuh.cn

[Q23] 分页
来源：http://tb.huixinmuqiang.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yp.hnjuh.cn

[Q24] 去重
来源：http://kf.bookmarksfly.cn

SELECT DISTINCT city FROM users;
来源：http://uc.huanxung.cn

[Q25] 只取前 N 条
来源：http://ja.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sk.shtwfgs.cn

[Q26] 计数
来源：http://ng.newstarts.cn

SELECT COUNT(*) FROM users;
来源：http://sb.newstarts.cn

[Q27] 条件计数
来源：http://bh.yuexingan06.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mk.colortex.cn

[Q28] 求和与平均
来源：http://ox.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tr.hahajie.cn

[Q29] 最大最小值
来源：http://sa.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cb.huixinmuqiang.cn

[Q30] 分组统计
来源：http://bv.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ne.huixinmuqiang.cn

[Q31] 分组后过滤
来源：http://zy.bjjhwx.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fo.haigaiapp.cn

[Q32] 分组拼接字符串
来源：http://dw.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lf.bookmarksfly.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qu.shxzukj.cn

[Q33] 多列分组
来源：http://af.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fj.haigaiapp.cn

[Q34] 每组取第一条
来源：http://sm.asd995.cn

SELECT * FROM (
来源：http://ws.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://aj.huanxung.cn

) t WHERE rn = 1;
来源：http://ov.szsharing.cn

[Q35] 内连接
来源：http://cc.newstarts.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fz.huixiangedu.cn

[Q36] 左连接
来源：http://qa.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lh.colortex.cn

[Q37] 右连接
来源：http://pf.lnxyls.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://os.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lk.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ac.jctech888.com.cn

[Q39] 自连接（查上下级）
来源：http://kt.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nf.muxihuayi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vd.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pz.nicolike.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ud.muxihuayi.cn

[Q41] 多表连接
来源：http://el.shxzskj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ap.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://fd.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://zf.szsharing.cn

[Q42] 连接条件附加过滤
来源：http://ck.521024.cn

SELECT u.name, o.amount FROM users u
来源：http://op.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xl.shxzukj.cn

[Q43] 标量子查询
来源：http://qb.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sl.shtwfgs.cn

[Q44] IN 子查询
来源：http://zh.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://of.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://kp.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jl.nszjky.cn

[Q46] NOT EXISTS 判断不存在
来源：http://eg.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://og.521024.cn

[Q47] 与平均值比较
来源：http://fc.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ds.nszjky.cn

[Q48] CTE 公用表表达式
来源：http://tg.newstarts.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mv.colortex.cn

SELECT * FROM t WHERE c > 5;
来源：http://hz.haigaiapp.cn

[Q49] 更新单行
来源：http://bp.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sx.shtwfgs.cn

[Q50] 批量更新
来源：http://zh.panjiajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xk.hahajie.cn

[Q51] 用子查询更新
来源：http://co.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cd.shxzskj.cn

[Q52] 删除指定行
来源：http://oq.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://xt.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://bi.szxytkj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vp.panjiajie.cn

[Q54] 清空表
来源：http://mf.nicolike.cn

TRUNCATE TABLE logs;
来源：http://xx.huanxung.cn

[Q55] 排名（并列占位）
来源：http://ad.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cy.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://kv.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cd.yuntaijiaju.cn

[Q57] 行号
来源：http://ap.gzmigu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://al.asd995.cn

[Q58] 累计求和
来源：http://pg.shxzukj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zo.bjjhwx.cn

[Q59] 分组内累计
来源：http://ty.chemitech.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nw.hnjuh.cn

[Q60] 取上一行 / 下一行
来源：http://cj.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rf.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tq.hahajie.cn

[Q61] 移动平均
来源：http://hr.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mj.gzmigu.cn

[Q62] 分组占比
来源：http://rb.newstarts.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cb.hahajie.cn

[Q63] 开启事务
来源：http://nk.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bv.hahajie.cn

[Q64] 提交事务
来源：http://nq.szxytkj.cn

COMMIT;
来源：http://tj.9csxet.cn

[Q65] 回滚事务
来源：http://wa.bjjhwx.cn

ROLLBACK;
来源：http://le.szsharing.cn

[Q66] 行锁查询
来源：http://rc.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oo.bjjhwx.cn

[Q67] 设置隔离级别
来源：http://nt.lnxyls.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vg.521024.cn

[Q68] 保存点
来源：http://ho.shtwfgs.cn

SAVEPOINT sp1;
来源：http://oy.jctech888.com.cn

ROLLBACK TO sp1;
来源：http://sy.bjjhwx.cn

[Q69] 查看执行计划
来源：http://wy.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qc.colortex.cn

[Q70] 更新统计信息
来源：http://tx.newstarts.cn

ANALYZE TABLE users;
来源：http://oa.szxytkj.cn

[Q71] 查看建表语句
来源：http://ov.muxihuayi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://up.hahajie.cn

[Q72] 查看索引
来源：http://jm.huanxung.cn

SHOW INDEX FROM users;
来源：http://lf.haigaiapp.cn

[Q73] 查看表状态
来源：http://fs.jctech888.com.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zi.bjjhwx.cn

[Q74] 强制使用索引
来源：http://zo.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wr.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://vw.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zr.muxihuayi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wo.gzmigu.cn

[Q76] 按天统计
来源：http://dy.colortex.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cm.yuntaijiaju.cn

[Q77] 时间加减
来源：http://iq.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ol.gzmigu.cn

[Q78] 当前时间
来源：http://li.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ou.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://kf.jctech888.com.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bq.shtwfgs.cn

[Q80] 字符串截取
来源：http://co.9csxet.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lj.panjiajie.cn

[Q81] 字符串替换
来源：http://bi.shxzskj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rj.panjiajie.cn

[Q82] 字符长度与字节长度
来源：http://gn.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nz.hnjuh.cn

[Q83] 大小写转换
来源：http://tc.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://by.huixinmuqiang.cn

[Q84] 去除首尾空格
来源：http://pd.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://iz.bookmarksfly.cn

[Q85] 数值取整
来源：http://oj.lnxyls.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://af.huixinmuqiang.cn

[Q86] 读取 JSON 字段
来源：http://dy.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kj.colortex.cn

[Q87] JSON 字段做条件
来源：http://rk.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ys.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://ns.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qe.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yu.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://kh.jianghongdianzi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lj.panjiajie.cn

[Q90] 生成序号列
来源：http://dt.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zl.hahajie.cn

================================================================================
来源：http://sv.nszjky.cn

R. Bash 专题
来源：http://di.lnxyls.cn

================================================================================
来源：http://fd.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://vd.haigaiapp.cn

#!/usr/bin/env bash
来源：http://lf.haigaiapp.cn

set -euo pipefail
来源：http://yf.9csxet.cn

[R02] 变量赋值与使用
来源：http://qh.asd995.cn

name="Tom"; echo "$name"
来源：http://kv.gzmigu.cn

[R03] 只读变量
来源：http://vc.gzmigu.cn

readonly PI=3.14
来源：http://jh.chemitech.net.cn

[R04] 位置参数
来源：http://le.panjiajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qs.lnxyls.cn

[R05] 参数默认值
来源：http://mg.newstarts.cn

name="${1:-default}"
来源：http://lz.521024.cn

[R06] 判断命令是否存在
来源：http://ih.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mf.asd995.cn

[R07] if 判断文件
来源：http://rt.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fz.wgjwhj.cn

[R08] 数值比较
来源：http://au.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sv.newstarts.cn

[R09] 字符串比较
来源：http://ve.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kz.szxytkj.cn

[R10] 正则匹配
来源：http://qi.newstarts.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rn.jctech888.com.cn

[R11] case 多分支
来源：http://vu.yuntaijiaju.cn

case "$1" in
来源：http://it.lnxyls.cn

start) echo "启动" ;;
来源：http://ay.szsharing.cn

stop)  echo "停止" ;;
来源：http://fp.szxytkj.cn

*)     echo "未知命令" ;;
来源：http://gu.9csxet.cn

esac
来源：http://nk.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://nl.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://aa.colortex.cn

[R13] for 计数循环
来源：http://av.yuntaijiaju.cn

for i in {1..10}; do echo "$i"; done
来源：http://iy.shxzskj.cn

[R14] C 风格 for
来源：http://wn.9csxet.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://do.nicolike.cn

[R15] while 逐行读文件
来源：http://lu.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jc.shxzskj.cn

[R16] until 等待条件
来源：http://yg.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ct.jianghongdianzi.cn

[R17] 数组定义与取值
来源：http://nb.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qm.jctech888.com.cn

[R18] 遍历数组
来源：http://bi.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dd.huixiangedu.cn

[R19] 数组长度
来源：http://zk.shxzskj.cn

echo "${#arr[@]}"
来源：http://yo.shxzukj.cn

[R20] 关联数组（字典）
来源：http://tn.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fv.yuntaijiaju.cn

[R21] 字符串长度
来源：http://lt.szxytkj.cn

echo "${#s}"
来源：http://bm.colortex.cn

[R22] 截取子串
来源：http://vv.huanxung.cn

echo "${s:0:5}"
来源：http://nc.newstarts.cn

[R23] 字符串替换
来源：http://qp.asd995.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wp.muxihuayi.cn

[R24] 大小写转换
来源：http://dy.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ge.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://bx.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cl.hahajie.cn

[R26] 命令替换
来源：http://ol.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://pj.haigaiapp.cn

[R27] 算术展开
来源：http://fe.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://ov.chemitech.net.cn

[R28] 浮点运算
来源：http://oj.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://cd.9csxet.cn

[R29] 定义函数
来源：http://yn.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ou.szxytkj.cn

[R30] 函数返回状态码
来源：http://pf.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://yu.colortex.cn

[R31] 局部变量
来源：http://fg.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://zu.nicolike.cn

[R32] 参数个数校验
来源：http://fi.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qx.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://bi.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://og.shxzskj.cn

[R34] 退出时清理
来源：http://ok.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bg.szsharing.cn

[R35] 后台执行并等待
来源：http://nc.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lc.huixinmuqiang.cn

[R36] 并发执行多个任务
来源：http://ig.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ui.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://sm.nicolike.cn

files=$(ls -1)
来源：http://wx.nicolike.cn

[R38] 管道串联
来源：http://kp.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://yu.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://vj.chemitech.net.cn

cmd > out.log 2>&1
来源：http://og.jianghongdianzi.cn

[R40] 追加写日志
来源：http://jj.chemitech.net.cn

echo "log" >> out.log
来源：http://be.nicolike.cn

[R41] 丢弃输出
来源：http://xa.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://ws.lnxyls.cn

[R42] 输入重定向
来源：http://ld.jctech888.com.cn

wc -l < a.txt
来源：http://rf.lnxyls.cn

[R43] 按名字查找文件
来源：http://jk.gzmigu.cn

find . -name "*.log" -type f
来源：http://tp.asd995.cn

[R44] 按修改时间查找
来源：http://wt.gzmigu.cn

find . -mtime -7 -type f
来源：http://pp.chemitech.net.cn

[R45] 批量删除
来源：http://vm.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://vl.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://vf.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pa.huixiangedu.cn

[R47] sed 单行替换
来源：http://cr.panjiajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cq.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://nf.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://nz.hahajie.cn

[R49] awk 带条件
来源：http://bj.muxihuayi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dx.hnjuh.cn

[R50] awk 求和
来源：http://yl.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dn.jctech888.com.cn

[R51] 排序去重取前几
来源：http://kl.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ez.bookmarksfly.cn

[R52] 统计行数
来源：http://iz.chemitech.net.cn

wc -l a.txt
来源：http://qf.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://ve.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hk.newstarts.cn

[R54] 比较两个文件
来源：http://ty.shxzukj.cn

diff a.txt b.txt
来源：http://qn.hahajie.cn

[R55] 压缩与解压
来源：http://st.shxzukj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wv.yuexingan06.cn

[R56] 远程拷贝
来源：http://cw.hahajie.cn

scp file user@host:/path/
来源：http://xf.newstarts.cn

[R57] 远程执行命令
来源：http://ae.newstarts.cn

ssh user@host 'uptime'
来源：http://ac.nszjky.cn

[R58] 下载文件
来源：http://ln.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pm.panjiajie.cn

[R59] 发 POST JSON
来源：http://wb.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rn.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://as.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lo.wgjwhj.cn

[R61] 磁盘占用
来源：http://df.huixiangedu.cn

df -h;  du -sh *
来源：http://fy.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://nz.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://xc.bjjhwx.cn

[R63] 内存与进程
来源：http://vr.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://ci.shxzukj.cn

[R64] 结束进程
来源：http://hu.haigaiapp.cn

kill -9 $(pgrep -f app.py)
来源：http://kz.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://tc.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bh.szxytkj.cn

[R66] 定时任务
来源：http://nk.szsharing.cn

crontab -e;  crontab -l
来源：http://dq.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://iu.521024.cn

openssl rand -hex 16
来源：http://ij.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://pd.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uq.haigaiapp.cn

[R69] 生成随机密码
来源：http://uj.huixiangedu.cn


<!-- 参考信息 -->