代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://bp.hnjuh.cn

[Q22] 排序
来源：http://nt.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ae.hnjuh.cn

[Q23] 分页
来源：http://ie.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zn.chemitech.net.cn

[Q24] 去重
来源：http://rg.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://ra.gzmigu.cn

[Q25] 只取前 N 条
来源：http://ot.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ab.hahajie.cn

[Q26] 计数
来源：http://tq.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://gy.szsharing.cn

[Q27] 条件计数
来源：http://ew.bjjhwx.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jm.lnxyls.cn

[Q28] 求和与平均
来源：http://mw.jctech888.com.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iu.szxytkj.cn

[Q29] 最大最小值
来源：http://ur.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gc.yuexingan06.cn

[Q30] 分组统计
来源：http://pd.lnxyls.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sg.shxzukj.cn

[Q31] 分组后过滤
来源：http://mn.hnjuh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mb.szsharing.cn

[Q32] 分组拼接字符串
来源：http://oc.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wc.huixiangedu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mo.newstarts.cn

[Q33] 多列分组
来源：http://zg.521024.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kj.lnxyls.cn

[Q34] 每组取第一条
来源：http://me.szxytkj.cn

SELECT * FROM (
来源：http://bb.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qe.muxihuayi.cn

) t WHERE rn = 1;
来源：http://wl.newstarts.cn

[Q35] 内连接
来源：http://pi.wgjwhj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ov.chemitech.net.cn

[Q36] 左连接
来源：http://mw.panjiajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rw.yuntaijiaju.cn

[Q37] 右连接
来源：http://ax.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vz.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://to.hnjuh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vd.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://oi.jianghongdianzi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bj.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lt.jianghongdianzi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rx.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zl.muxihuayi.cn

[Q41] 多表连接
来源：http://nw.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yh.chemitech.net.cn

JOIN users u ON u.id = o.user_id
来源：http://xo.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://ut.gzmigu.cn

[Q42] 连接条件附加过滤
来源：http://ax.chemitech.net.cn

SELECT u.name, o.amount FROM users u
来源：http://nd.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vi.shxzukj.cn

[Q43] 标量子查询
来源：http://rc.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jo.bjjhwx.cn

[Q44] IN 子查询
来源：http://fc.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://li.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://jk.newstarts.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ni.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://te.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xc.shxzskj.cn

[Q47] 与平均值比较
来源：http://yb.nicolike.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kj.nszjky.cn

[Q48] CTE 公用表表达式
来源：http://mv.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ub.chemitech.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://xs.hahajie.cn

[Q49] 更新单行
来源：http://cs.bookmarksfly.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://no.panjiajie.cn

[Q50] 批量更新
来源：http://cl.nszjky.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ou.yuexingan06.cn

[Q51] 用子查询更新
来源：http://dk.521024.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ku.asd995.cn

[Q52] 删除指定行
来源：http://zm.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://jn.hnjuh.cn

[Q53] 按条件删除
来源：http://qf.9csxet.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dz.9csxet.cn

[Q54] 清空表
来源：http://qu.asd995.cn

TRUNCATE TABLE logs;
来源：http://hm.hnjuh.cn

[Q55] 排名（并列占位）
来源：http://cl.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kl.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://zv.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qo.hnjuh.cn

[Q57] 行号
来源：http://ki.muxihuayi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pa.huixinmuqiang.cn

[Q58] 累计求和
来源：http://xi.nicolike.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rn.huixinmuqiang.cn

[Q59] 分组内累计
来源：http://ym.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hm.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://mu.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tl.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ue.yuexingan06.cn

[Q61] 移动平均
来源：http://yg.haigaiapp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xv.huixiangedu.cn

[Q62] 分组占比
来源：http://xb.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gb.huixiangedu.cn

[Q63] 开启事务
来源：http://di.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cv.jianghongdianzi.cn

[Q64] 提交事务
来源：http://nd.chemitech.net.cn

COMMIT;
来源：http://uv.bjjhwx.cn

[Q65] 回滚事务
来源：http://da.jianghongdianzi.cn

ROLLBACK;
来源：http://zk.bookmarksfly.cn

[Q66] 行锁查询
来源：http://uf.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://us.9csxet.cn

[Q67] 设置隔离级别
来源：http://be.huixiangedu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fe.nicolike.cn

[Q68] 保存点
来源：http://qt.shtwfgs.cn

SAVEPOINT sp1;
来源：http://dw.nszjky.cn

ROLLBACK TO sp1;
来源：http://lj.jctech888.com.cn

[Q69] 查看执行计划
来源：http://ip.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lw.huanxung.cn

[Q70] 更新统计信息
来源：http://vs.bjjhwx.cn

ANALYZE TABLE users;
来源：http://oo.521024.cn

[Q71] 查看建表语句
来源：http://al.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rs.colortex.cn

[Q72] 查看索引
来源：http://pr.gzmigu.cn

SHOW INDEX FROM users;
来源：http://yy.panjiajie.cn

[Q73] 查看表状态
来源：http://pp.shxzskj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ar.jianghongdianzi.cn

[Q74] 强制使用索引
来源：http://vu.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pj.yuexingan06.cn

[Q75] 日期格式化
来源：http://ox.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uo.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gb.9csxet.cn

[Q76] 按天统计
来源：http://do.shxzukj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ey.jctech888.com.cn

[Q77] 时间加减
来源：http://kp.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vv.szsharing.cn

[Q78] 当前时间
来源：http://ll.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ov.521024.cn

[Q79] 字符串拼接
来源：http://xx.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ae.huanxung.cn

[Q80] 字符串截取
来源：http://pt.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hw.nicolike.cn

[Q81] 字符串替换
来源：http://cx.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gy.yuexingan06.cn

[Q82] 字符长度与字节长度
来源：http://tk.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wd.haigaiapp.cn

[Q83] 大小写转换
来源：http://ta.huixiangedu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kc.nszjky.cn

[Q84] 去除首尾空格
来源：http://iq.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://cn.panjiajie.cn

[Q85] 数值取整
来源：http://nt.lnxyls.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dh.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://oz.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qm.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://pg.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wm.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://xw.panjiajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tz.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lx.chemitech.net.cn

[Q89] 判断表是否存在
来源：http://ok.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ny.colortex.cn

[Q90] 生成序号列
来源：http://yn.huixiangedu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sh.wgjwhj.cn

================================================================================
来源：http://ij.wgjwhj.cn

R. Bash 专题
来源：http://bv.muxihuayi.cn

================================================================================
来源：http://dq.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://ff.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://cg.521024.cn

set -euo pipefail
来源：http://nr.521024.cn

[R02] 变量赋值与使用
来源：http://ds.bookmarksfly.cn

name="Tom"; echo "$name"
来源：http://tn.jctech888.com.cn

[R03] 只读变量
来源：http://fk.shxzskj.cn

readonly PI=3.14
来源：http://yb.521024.cn

[R04] 位置参数
来源：http://qf.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://po.lnxyls.cn

[R05] 参数默认值
来源：http://wn.haigaiapp.cn

name="${1:-default}"
来源：http://pm.szsharing.cn

[R06] 判断命令是否存在
来源：http://ld.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xe.szxytkj.cn

[R07] if 判断文件
来源：http://ss.jianghongdianzi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zb.521024.cn

[R08] 数值比较
来源：http://hm.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xa.jianghongdianzi.cn

[R09] 字符串比较
来源：http://tf.bookmarksfly.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rt.yuntaijiaju.cn

[R10] 正则匹配
来源：http://tl.haigaiapp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sf.jctech888.com.cn

[R11] case 多分支
来源：http://ea.hnjuh.cn

case "$1" in
来源：http://fz.szsharing.cn

start) echo "启动" ;;
来源：http://uj.yuexingan06.cn

stop)  echo "停止" ;;
来源：http://js.gzmigu.cn

*)     echo "未知命令" ;;
来源：http://gb.shxzukj.cn

esac
来源：http://tu.huanxung.cn

[R12] for 遍历文件
来源：http://va.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://ba.huanxung.cn

[R13] for 计数循环
来源：http://zi.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://pu.nszjky.cn

[R14] C 风格 for
来源：http://jo.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://is.shtwfgs.cn

[R15] while 逐行读文件
来源：http://cd.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cu.newstarts.cn

[R16] until 等待条件
来源：http://va.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://of.jianghongdianzi.cn

[R17] 数组定义与取值
来源：http://qh.9csxet.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wv.521024.cn

[R18] 遍历数组
来源：http://gv.bookmarksfly.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nh.yuexingan06.cn

[R19] 数组长度
来源：http://gf.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://qe.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://ws.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ko.shxzukj.cn

[R21] 字符串长度
来源：http://ai.bjjhwx.cn

echo "${#s}"
来源：http://yy.bookmarksfly.cn

[R22] 截取子串
来源：http://wy.bookmarksfly.cn

echo "${s:0:5}"
来源：http://rf.shxzukj.cn

[R23] 字符串替换
来源：http://xv.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hj.shxzskj.cn

[R24] 大小写转换
来源：http://om.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tn.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://bf.colortex.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://so.gzmigu.cn

[R26] 命令替换
来源：http://fm.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://rg.9csxet.cn

[R27] 算术展开
来源：http://dz.gzmigu.cn

echo $((1 + 2 * 3))
来源：http://ve.9csxet.cn

[R28] 浮点运算
来源：http://ac.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://nf.panjiajie.cn

[R29] 定义函数
来源：http://wx.shxzskj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zr.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://bu.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://er.huixiangedu.cn

[R31] 局部变量
来源：http://uh.hahajie.cn

f() { local x=1; echo "$x"; }
来源：http://ti.szsharing.cn

[R32] 参数个数校验
来源：http://zc.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ri.asd995.cn

[R33] 捕获错误并提示行号
来源：http://vo.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ke.bookmarksfly.cn

[R34] 退出时清理
来源：http://lc.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ve.lnxyls.cn

[R35] 后台执行并等待
来源：http://ci.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rf.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://xh.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jt.shxzskj.cn

[R37] 把输出赋给变量
来源：http://qi.nszjky.cn

files=$(ls -1)
来源：http://oc.huixiangedu.cn

[R38] 管道串联
来源：http://vb.nszjky.cn

cat a.txt | grep -i error | wc -l
来源：http://ry.jctech888.com.cn

[R39] 重定向标准输出与错误
来源：http://pu.bjjhwx.cn

cmd > out.log 2>&1
来源：http://pi.huixiangedu.cn

[R40] 追加写日志
来源：http://wk.hahajie.cn

echo "log" >> out.log
来源：http://ud.nicolike.cn

[R41] 丢弃输出
来源：http://cx.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://sw.panjiajie.cn

[R42] 输入重定向
来源：http://qn.nicolike.cn

wc -l < a.txt
来源：http://im.haigaiapp.cn

[R43] 按名字查找文件
来源：http://nv.shtwfgs.cn

find . -name "*.log" -type f
来源：http://sz.hnjuh.cn

[R44] 按修改时间查找
来源：http://fb.gzmigu.cn

find . -mtime -7 -type f
来源：http://ba.gzmigu.cn

[R45] 批量删除
来源：http://xd.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://oo.hahajie.cn

[R46] 递归替换文件内容
来源：http://lq.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sy.shxzukj.cn

[R47] sed 单行替换
来源：http://lf.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ol.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://yj.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://mx.muxihuayi.cn

[R49] awk 带条件
来源：http://pw.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ui.panjiajie.cn

[R50] awk 求和
来源：http://rc.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uq.asd995.cn

[R51] 排序去重取前几
来源：http://us.gzmigu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sp.yuexingan06.cn

[R52] 统计行数
来源：http://bb.haigaiapp.cn

wc -l a.txt
来源：http://si.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://am.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vb.shxzukj.cn

[R54] 比较两个文件
来源：http://tv.szsharing.cn

diff a.txt b.txt
来源：http://oy.colortex.cn

[R55] 压缩与解压
来源：http://ce.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://po.newstarts.cn

[R56] 远程拷贝
来源：http://qo.huixinmuqiang.cn

scp file user@host:/path/
来源：http://ad.muxihuayi.cn

[R57] 远程执行命令
来源：http://pe.bjjhwx.cn

ssh user@host 'uptime'
来源：http://ll.chemitech.net.cn

[R58] 下载文件
来源：http://so.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://na.newstarts.cn

[R59] 发 POST JSON
来源：http://tb.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://we.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://qu.muxihuayi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gk.szsharing.cn

[R61] 磁盘占用
来源：http://si.huixiangedu.cn

df -h;  du -sh *
来源：http://qp.gzmigu.cn

[R62] 找最占空间的文件
来源：http://nr.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://zb.lnxyls.cn

[R63] 内存与进程
来源：http://vd.newstarts.cn

free -h;  ps aux | grep nginx
来源：http://al.panjiajie.cn

[R64] 结束进程
来源：http://ij.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://pg.panjiajie.cn

[R65] 查看端口占用
来源：http://os.nicolike.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mj.hahajie.cn

[R66] 定时任务
来源：http://ql.huanxung.cn

crontab -e;  crontab -l
来源：http://bn.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://cu.gzmigu.cn

openssl rand -hex 16
来源：http://xr.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://yn.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://oy.shtwfgs.cn

[R69] 生成随机密码
来源：http://pc.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://xm.chemitech.net.cn

[R70] 时间戳与互转
来源：http://xd.colortex.cn

date +%s;  date -d @1700000000
来源：http://bc.haigaiapp.cn

[R71] 日期格式化
来源：http://mq.szsharing.cn


<!-- 参考信息 -->