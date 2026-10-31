代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://ca.muxihuayi.cn

[Q22] 排序
来源：http://ph.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zq.bookmarksfly.cn

[Q23] 分页
来源：http://ij.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oy.hahajie.cn

[Q24] 去重
来源：http://jo.yuntaijiaju.cn

SELECT DISTINCT city FROM users;
来源：http://yz.szsharing.cn

[Q25] 只取前 N 条
来源：http://eg.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uw.nicolike.cn

[Q26] 计数
来源：http://gb.yuexingan06.cn

SELECT COUNT(*) FROM users;
来源：http://eo.hnjuh.cn

[Q27] 条件计数
来源：http://xs.yuntaijiaju.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fp.huanxung.cn

[Q28] 求和与平均
来源：http://mq.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://op.newstarts.cn

[Q29] 最大最小值
来源：http://em.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hw.wgjwhj.cn

[Q30] 分组统计
来源：http://bw.shxzukj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://oo.szxytkj.cn

[Q31] 分组后过滤
来源：http://hk.newstarts.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xk.521024.cn

[Q32] 分组拼接字符串
来源：http://ec.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dw.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ih.bookmarksfly.cn

[Q33] 多列分组
来源：http://qr.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oj.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://kq.wgjwhj.cn

SELECT * FROM (
来源：http://fc.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ve.szxytkj.cn

) t WHERE rn = 1;
来源：http://gc.jctech888.com.cn

[Q35] 内连接
来源：http://bc.wgjwhj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ia.wgjwhj.cn

[Q36] 左连接
来源：http://ob.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ve.bookmarksfly.cn

[Q37] 右连接
来源：http://yy.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xe.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bv.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nr.shxzskj.cn

[Q39] 自连接（查上下级）
来源：http://or.yuntaijiaju.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ru.muxihuayi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bq.bjjhwx.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kc.nicolike.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tx.nicolike.cn

[Q41] 多表连接
来源：http://pk.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rx.panjiajie.cn

JOIN users u ON u.id = o.user_id
来源：http://vj.yuexingan06.cn

JOIN products p ON p.id = o.product_id;
来源：http://tl.521024.cn

[Q42] 连接条件附加过滤
来源：http://mz.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://mh.wgjwhj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ii.bookmarksfly.cn

[Q43] 标量子查询
来源：http://fn.newstarts.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oz.panjiajie.cn

[Q44] IN 子查询
来源：http://wm.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qx.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://dy.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://df.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sf.shxzskj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jk.huixinmuqiang.cn

[Q47] 与平均值比较
来源：http://hk.hahajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zo.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://dr.szsharing.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cr.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://oi.haigaiapp.cn

[Q49] 更新单行
来源：http://bb.9csxet.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hy.panjiajie.cn

[Q50] 批量更新
来源：http://qd.panjiajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gv.szsharing.cn

[Q51] 用子查询更新
来源：http://or.wgjwhj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vr.chemitech.net.cn

[Q52] 删除指定行
来源：http://zc.huixiangedu.cn

DELETE FROM users WHERE id = 10;
来源：http://bv.shxzukj.cn

[Q53] 按条件删除
来源：http://ki.newstarts.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lx.bookmarksfly.cn

[Q54] 清空表
来源：http://jq.haigaiapp.cn

TRUNCATE TABLE logs;
来源：http://bo.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://eo.shxzskj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pk.szxytkj.cn

[Q56] 密集排名（并列不占位）
来源：http://ut.asd995.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qw.colortex.cn

[Q57] 行号
来源：http://bd.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xn.521024.cn

[Q58] 累计求和
来源：http://uo.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ra.chemitech.net.cn

[Q59] 分组内累计
来源：http://uy.shxzskj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hx.gzmigu.cn

[Q60] 取上一行 / 下一行
来源：http://vm.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rm.lnxyls.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bf.haigaiapp.cn

[Q61] 移动平均
来源：http://ws.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nh.panjiajie.cn

[Q62] 分组占比
来源：http://pc.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gj.shxzskj.cn

[Q63] 开启事务
来源：http://dl.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cv.shtwfgs.cn

[Q64] 提交事务
来源：http://bd.muxihuayi.cn

COMMIT;
来源：http://ah.bjjhwx.cn

[Q65] 回滚事务
来源：http://nd.szsharing.cn

ROLLBACK;
来源：http://yu.521024.cn

[Q66] 行锁查询
来源：http://qr.lnxyls.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ql.huanxung.cn

[Q67] 设置隔离级别
来源：http://xq.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://no.shtwfgs.cn

[Q68] 保存点
来源：http://qo.huanxung.cn

SAVEPOINT sp1;
来源：http://wz.szsharing.cn

ROLLBACK TO sp1;
来源：http://ck.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://nz.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ks.nicolike.cn

[Q70] 更新统计信息
来源：http://tb.asd995.cn

ANALYZE TABLE users;
来源：http://oc.yuexingan06.cn

[Q71] 查看建表语句
来源：http://xq.panjiajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qp.hahajie.cn

[Q72] 查看索引
来源：http://eu.shxzukj.cn

SHOW INDEX FROM users;
来源：http://py.gzmigu.cn

[Q73] 查看表状态
来源：http://ds.asd995.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pg.9csxet.cn

[Q74] 强制使用索引
来源：http://dh.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bg.jctech888.com.cn

[Q75] 日期格式化
来源：http://ko.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yl.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wq.colortex.cn

[Q76] 按天统计
来源：http://hf.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jr.haigaiapp.cn

[Q77] 时间加减
来源：http://ml.jianghongdianzi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xa.hnjuh.cn

[Q78] 当前时间
来源：http://rt.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yi.huanxung.cn

[Q79] 字符串拼接
来源：http://qd.shxzukj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fz.9csxet.cn

[Q80] 字符串截取
来源：http://wq.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cw.wgjwhj.cn

[Q81] 字符串替换
来源：http://ze.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gb.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://vj.9csxet.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fn.gzmigu.cn

[Q83] 大小写转换
来源：http://nr.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hf.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://lp.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://cy.hnjuh.cn

[Q85] 数值取整
来源：http://gx.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://me.colortex.cn

[Q86] 读取 JSON 字段
来源：http://se.bookmarksfly.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yq.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://ca.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xm.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://gi.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pj.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dt.shxzskj.cn

[Q89] 判断表是否存在
来源：http://cn.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vs.huixinmuqiang.cn

[Q90] 生成序号列
来源：http://fv.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yd.lnxyls.cn

================================================================================
来源：http://bv.panjiajie.cn

R. Bash 专题
来源：http://ft.chemitech.net.cn

================================================================================
来源：http://nc.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://zq.haigaiapp.cn

#!/usr/bin/env bash
来源：http://mp.jctech888.com.cn

set -euo pipefail
来源：http://ur.lnxyls.cn

[R02] 变量赋值与使用
来源：http://mf.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://ma.gzmigu.cn

[R03] 只读变量
来源：http://wq.huanxung.cn

readonly PI=3.14
来源：http://bp.nicolike.cn

[R04] 位置参数
来源：http://cl.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://at.bookmarksfly.cn

[R05] 参数默认值
来源：http://zl.asd995.cn

name="${1:-default}"
来源：http://ht.shxzskj.cn

[R06] 判断命令是否存在
来源：http://md.asd995.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wb.gzmigu.cn

[R07] if 判断文件
来源：http://mk.521024.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cg.shtwfgs.cn

[R08] 数值比较
来源：http://he.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://om.nszjky.cn

[R09] 字符串比较
来源：http://te.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kn.yuexingan06.cn

[R10] 正则匹配
来源：http://zs.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ql.huixinmuqiang.cn

[R11] case 多分支
来源：http://uo.huanxung.cn

case "$1" in
来源：http://xr.9csxet.cn

start) echo "启动" ;;
来源：http://sp.newstarts.cn

stop)  echo "停止" ;;
来源：http://oa.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://qd.huanxung.cn

esac
来源：http://tn.chemitech.net.cn

[R12] for 遍历文件
来源：http://oh.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://qp.asd995.cn

[R13] for 计数循环
来源：http://ll.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://od.shtwfgs.cn

[R14] C 风格 for
来源：http://gz.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qi.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://hu.bjjhwx.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lq.newstarts.cn

[R16] until 等待条件
来源：http://jr.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://na.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://hk.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rw.muxihuayi.cn

[R18] 遍历数组
来源：http://gf.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gy.bjjhwx.cn

[R19] 数组长度
来源：http://zv.colortex.cn

echo "${#arr[@]}"
来源：http://wy.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://uw.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cq.chemitech.net.cn

[R21] 字符串长度
来源：http://ta.jctech888.com.cn

echo "${#s}"
来源：http://ra.asd995.cn

[R22] 截取子串
来源：http://yc.wgjwhj.cn

echo "${s:0:5}"
来源：http://zr.gzmigu.cn

[R23] 字符串替换
来源：http://un.bjjhwx.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wh.yuntaijiaju.cn

[R24] 大小写转换
来源：http://ma.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wc.521024.cn

[R25] 去后缀 / 去前缀
来源：http://vz.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://og.muxihuayi.cn

[R26] 命令替换
来源：http://nx.yuntaijiaju.cn

now=$(date +%F); echo "$now"
来源：http://zc.newstarts.cn

[R27] 算术展开
来源：http://kp.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://ys.huixiangedu.cn

[R28] 浮点运算
来源：http://ld.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://mq.shxzskj.cn

[R29] 定义函数
来源：http://rc.jctech888.com.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yb.yuntaijiaju.cn

[R30] 函数返回状态码
来源：http://np.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://sv.panjiajie.cn

[R31] 局部变量
来源：http://pn.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://lp.newstarts.cn

[R32] 参数个数校验
来源：http://fi.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rn.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://yz.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uf.yuexingan06.cn

[R34] 退出时清理
来源：http://xn.chemitech.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://de.colortex.cn

[R35] 后台执行并等待
来源：http://is.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qm.asd995.cn

[R36] 并发执行多个任务
来源：http://ht.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://na.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://tj.wgjwhj.cn

files=$(ls -1)
来源：http://pt.nszjky.cn

[R38] 管道串联
来源：http://nk.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://ai.bookmarksfly.cn

[R39] 重定向标准输出与错误
来源：http://ja.szsharing.cn

cmd > out.log 2>&1
来源：http://ht.yuntaijiaju.cn

[R40] 追加写日志
来源：http://nv.lnxyls.cn

echo "log" >> out.log
来源：http://ih.hahajie.cn

[R41] 丢弃输出
来源：http://ee.shxzskj.cn

cmd >/dev/null 2>&1
来源：http://fp.shxzukj.cn

[R42] 输入重定向
来源：http://am.yuntaijiaju.cn

wc -l < a.txt
来源：http://pq.yuntaijiaju.cn

[R43] 按名字查找文件
来源：http://ov.huanxung.cn

find . -name "*.log" -type f
来源：http://ud.wgjwhj.cn

[R44] 按修改时间查找
来源：http://do.haigaiapp.cn

find . -mtime -7 -type f
来源：http://ru.haigaiapp.cn

[R45] 批量删除
来源：http://cb.szsharing.cn

find . -name "*.tmp" -delete
来源：http://kd.colortex.cn

[R46] 递归替换文件内容
来源：http://ci.shtwfgs.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dc.jctech888.com.cn

[R47] sed 单行替换
来源：http://yv.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://my.szxytkj.cn

[R48] awk 取指定列
来源：http://um.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://wd.hnjuh.cn

[R49] awk 带条件
来源：http://lt.shxzskj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://by.panjiajie.cn

[R50] awk 求和
来源：http://iq.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ro.lnxyls.cn

[R51] 排序去重取前几
来源：http://ws.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gk.9csxet.cn

[R52] 统计行数
来源：http://hj.chemitech.net.cn

wc -l a.txt
来源：http://kw.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://cr.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://al.wgjwhj.cn

[R54] 比较两个文件
来源：http://vl.nicolike.cn

diff a.txt b.txt
来源：http://lb.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://au.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gr.9csxet.cn

[R56] 远程拷贝
来源：http://qr.hahajie.cn

scp file user@host:/path/
来源：http://zx.colortex.cn

[R57] 远程执行命令
来源：http://fm.521024.cn

ssh user@host 'uptime'
来源：http://ep.hnjuh.cn

[R58] 下载文件
来源：http://sh.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uo.szxytkj.cn

[R59] 发 POST JSON
来源：http://hy.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gv.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://en.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://os.lnxyls.cn

[R61] 磁盘占用
来源：http://vt.huixinmuqiang.cn

df -h;  du -sh *
来源：http://di.szxytkj.cn

[R62] 找最占空间的文件
来源：http://co.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://aa.asd995.cn

[R63] 内存与进程
来源：http://ps.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://cu.wgjwhj.cn

[R64] 结束进程
来源：http://xm.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://gz.jctech888.com.cn

[R65] 查看端口占用
来源：http://gq.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kg.yuntaijiaju.cn

[R66] 定时任务
来源：http://by.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://nb.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://rn.panjiajie.cn

openssl rand -hex 16
来源：http://lg.bjjhwx.cn

[R68] 计算文件校验值
来源：http://us.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tt.wgjwhj.cn

[R69] 生成随机密码
来源：http://sa.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://az.huanxung.cn

[R70] 时间戳与互转
来源：http://lb.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://hr.hnjuh.cn

[R71] 日期格式化
来源：http://za.jianghongdianzi.cn


<!-- 参考信息 -->