代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ni.shtwfgs.cn

[Q26] 计数
来源：http://jl.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://lu.szsharing.cn

[Q27] 条件计数
来源：http://ac.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fg.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://sp.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ii.colortex.cn

[Q29] 最大最小值
来源：http://ri.szsharing.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dk.wgjwhj.cn

[Q30] 分组统计
来源：http://wm.jctech888.com.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tj.szxytkj.cn

[Q31] 分组后过滤
来源：http://eo.asd995.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vo.huixinmuqiang.cn

[Q32] 分组拼接字符串
来源：http://xz.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://te.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mj.yuexingan06.cn

[Q33] 多列分组
来源：http://dz.shxzskj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xi.jctech888.com.cn

[Q34] 每组取第一条
来源：http://hf.haigaiapp.cn

SELECT * FROM (
来源：http://py.muxihuayi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://le.szsharing.cn

) t WHERE rn = 1;
来源：http://qc.yuexingan06.cn

[Q35] 内连接
来源：http://gu.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mx.shxzukj.cn

[Q36] 左连接
来源：http://gd.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hn.nicolike.cn

[Q37] 右连接
来源：http://ft.shxzskj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gj.gzmigu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vc.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sj.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://ej.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jw.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pq.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://co.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vm.hnjuh.cn

[Q41] 多表连接
来源：http://wy.szsharing.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://em.yuexingan06.cn

JOIN users u ON u.id = o.user_id
来源：http://yb.colortex.cn

JOIN products p ON p.id = o.product_id;
来源：http://wp.newstarts.cn

[Q42] 连接条件附加过滤
来源：http://gs.huanxung.cn

SELECT u.name, o.amount FROM users u
来源：http://sa.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qh.huixinmuqiang.cn

[Q43] 标量子查询
来源：http://li.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oo.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://bu.gzmigu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zr.lnxyls.cn

[Q45] EXISTS 判断存在
来源：http://rt.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qb.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ez.huixinmuqiang.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bb.lnxyls.cn

[Q47] 与平均值比较
来源：http://pi.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xi.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://tz.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wb.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://oa.hahajie.cn

[Q49] 更新单行
来源：http://cp.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://do.newstarts.cn

[Q50] 批量更新
来源：http://xi.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fv.gzmigu.cn

[Q51] 用子查询更新
来源：http://he.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fs.muxihuayi.cn

[Q52] 删除指定行
来源：http://zy.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://sr.bookmarksfly.cn

[Q53] 按条件删除
来源：http://on.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qf.haigaiapp.cn

[Q54] 清空表
来源：http://pt.shxzskj.cn

TRUNCATE TABLE logs;
来源：http://nw.newstarts.cn

[Q55] 排名（并列占位）
来源：http://vj.yuntaijiaju.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jk.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://vj.bookmarksfly.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oa.shxzskj.cn

[Q57] 行号
来源：http://qn.9csxet.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xg.521024.cn

[Q58] 累计求和
来源：http://om.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gy.hnjuh.cn

[Q59] 分组内累计
来源：http://vq.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pi.jctech888.com.cn

[Q60] 取上一行 / 下一行
来源：http://dz.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jz.panjiajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bc.lnxyls.cn

[Q61] 移动平均
来源：http://qe.521024.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gp.bjjhwx.cn

[Q62] 分组占比
来源：http://nc.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ww.haigaiapp.cn

[Q63] 开启事务
来源：http://ru.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gp.shtwfgs.cn

[Q64] 提交事务
来源：http://vg.huanxung.cn

COMMIT;
来源：http://fj.jctech888.com.cn

[Q65] 回滚事务
来源：http://rt.colortex.cn

ROLLBACK;
来源：http://ml.wgjwhj.cn

[Q66] 行锁查询
来源：http://bw.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ys.shxzukj.cn

[Q67] 设置隔离级别
来源：http://sa.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bu.hnjuh.cn

[Q68] 保存点
来源：http://rg.9csxet.cn

SAVEPOINT sp1;
来源：http://yo.lnxyls.cn

ROLLBACK TO sp1;
来源：http://iw.asd995.cn

[Q69] 查看执行计划
来源：http://zf.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yq.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://re.jianghongdianzi.cn

ANALYZE TABLE users;
来源：http://wt.panjiajie.cn

[Q71] 查看建表语句
来源：http://le.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cs.huixinmuqiang.cn

[Q72] 查看索引
来源：http://yn.gzmigu.cn

SHOW INDEX FROM users;
来源：http://ws.panjiajie.cn

[Q73] 查看表状态
来源：http://iz.lnxyls.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qu.huanxung.cn

[Q74] 强制使用索引
来源：http://yr.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dd.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://ir.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ls.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ut.chemitech.net.cn

[Q76] 按天统计
来源：http://sl.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lu.bjjhwx.cn

[Q77] 时间加减
来源：http://xv.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cg.nicolike.cn

[Q78] 当前时间
来源：http://ns.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ub.newstarts.cn

[Q79] 字符串拼接
来源：http://mc.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ld.gzmigu.cn

[Q80] 字符串截取
来源：http://zu.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://or.bjjhwx.cn

[Q81] 字符串替换
来源：http://hh.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zz.bookmarksfly.cn

[Q82] 字符长度与字节长度
来源：http://jq.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tb.521024.cn

[Q83] 大小写转换
来源：http://uo.huanxung.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://iz.9csxet.cn

[Q84] 去除首尾空格
来源：http://jg.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://dw.szsharing.cn

[Q85] 数值取整
来源：http://cr.chemitech.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ay.hnjuh.cn

[Q86] 读取 JSON 字段
来源：http://zl.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ps.haigaiapp.cn

[Q87] JSON 字段做条件
来源：http://nw.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cv.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://zr.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uj.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pw.bjjhwx.cn

[Q89] 判断表是否存在
来源：http://kz.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ge.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://kc.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vb.huanxung.cn

================================================================================
来源：http://ry.shtwfgs.cn

R. Bash 专题
来源：http://pd.nicolike.cn

================================================================================
来源：http://mm.hahajie.cn

[R01] shebang 与严格模式
来源：http://wg.shxzukj.cn

#!/usr/bin/env bash
来源：http://yw.bookmarksfly.cn

set -euo pipefail
来源：http://eb.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://eg.yuntaijiaju.cn

name="Tom"; echo "$name"
来源：http://zk.wgjwhj.cn

[R03] 只读变量
来源：http://nq.haigaiapp.cn

readonly PI=3.14
来源：http://ns.newstarts.cn

[R04] 位置参数
来源：http://kk.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eb.szsharing.cn

[R05] 参数默认值
来源：http://yx.521024.cn

name="${1:-default}"
来源：http://uo.hnjuh.cn

[R06] 判断命令是否存在
来源：http://is.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pc.yuntaijiaju.cn

[R07] if 判断文件
来源：http://zo.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mv.lnxyls.cn

[R08] 数值比较
来源：http://yz.huanxung.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cj.nicolike.cn

[R09] 字符串比较
来源：http://np.lnxyls.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shxzukj.cn

[R10] 正则匹配
来源：http://hl.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://im.huixiangedu.cn

[R11] case 多分支
来源：http://jj.huixiangedu.cn

case "$1" in
来源：http://mx.huanxung.cn

start) echo "启动" ;;
来源：http://dq.huixiangedu.cn

stop)  echo "停止" ;;
来源：http://kp.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://mb.jctech888.com.cn

esac
来源：http://nh.haigaiapp.cn

[R12] for 遍历文件
来源：http://es.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://jk.huixinmuqiang.cn

[R13] for 计数循环
来源：http://iq.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://ef.gzmigu.cn

[R14] C 风格 for
来源：http://jm.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wj.shtwfgs.cn

[R15] while 逐行读文件
来源：http://mu.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wx.muxihuayi.cn

[R16] until 等待条件
来源：http://jb.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dc.yuntaijiaju.cn

[R17] 数组定义与取值
来源：http://xc.bjjhwx.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ie.szsharing.cn

[R18] 遍历数组
来源：http://qg.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ii.muxihuayi.cn

[R19] 数组长度
来源：http://gt.nszjky.cn

echo "${#arr[@]}"
来源：http://yw.panjiajie.cn

[R20] 关联数组（字典）
来源：http://iq.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sd.huixiangedu.cn

[R21] 字符串长度
来源：http://yz.bookmarksfly.cn

echo "${#s}"
来源：http://iy.huixiangedu.cn

[R22] 截取子串
来源：http://na.panjiajie.cn

echo "${s:0:5}"
来源：http://it.muxihuayi.cn

[R23] 字符串替换
来源：http://lz.chemitech.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qs.lnxyls.cn

[R24] 大小写转换
来源：http://rs.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hv.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://yj.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://la.panjiajie.cn

[R26] 命令替换
来源：http://rp.colortex.cn

now=$(date +%F); echo "$now"
来源：http://cd.newstarts.cn

[R27] 算术展开
来源：http://us.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://cu.yuexingan06.cn

[R28] 浮点运算
来源：http://ig.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://of.521024.cn

[R29] 定义函数
来源：http://fk.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vc.colortex.cn

[R30] 函数返回状态码
来源：http://sc.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://rv.521024.cn

[R31] 局部变量
来源：http://wb.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://tc.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://jt.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://om.muxihuayi.cn

[R33] 捕获错误并提示行号
来源：http://qj.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ic.huixiangedu.cn

[R34] 退出时清理
来源：http://cs.9csxet.cn

trap 'rm -f "$tmp"' EXIT
来源：http://er.bjjhwx.cn

[R35] 后台执行并等待
来源：http://ei.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xp.lnxyls.cn

[R36] 并发执行多个任务
来源：http://jl.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xo.huixinmuqiang.cn

[R37] 把输出赋给变量
来源：http://yw.nicolike.cn

files=$(ls -1)
来源：http://hg.nicolike.cn

[R38] 管道串联
来源：http://oh.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://lc.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://cm.shxzukj.cn

cmd > out.log 2>&1
来源：http://cq.haigaiapp.cn

[R40] 追加写日志
来源：http://fu.521024.cn

echo "log" >> out.log
来源：http://pu.asd995.cn

[R41] 丢弃输出
来源：http://nj.szsharing.cn

cmd >/dev/null 2>&1
来源：http://gx.shxzukj.cn

[R42] 输入重定向
来源：http://oz.bookmarksfly.cn

wc -l < a.txt
来源：http://yb.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://wr.yuexingan06.cn

find . -name "*.log" -type f
来源：http://xk.chemitech.net.cn

[R44] 按修改时间查找
来源：http://gu.lnxyls.cn

find . -mtime -7 -type f
来源：http://tf.jctech888.com.cn

[R45] 批量删除
来源：http://fr.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://xr.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://yv.chemitech.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cq.521024.cn

[R47] sed 单行替换
来源：http://id.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lx.asd995.cn

[R48] awk 取指定列
来源：http://rm.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://nn.yuexingan06.cn

[R49] awk 带条件
来源：http://ws.huixiangedu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gr.bookmarksfly.cn

[R50] awk 求和
来源：http://bx.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ep.huixiangedu.cn

[R51] 排序去重取前几
来源：http://xd.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jz.shxzukj.cn

[R52] 统计行数
来源：http://da.colortex.cn

wc -l a.txt
来源：http://jk.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://ya.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://er.lnxyls.cn

[R54] 比较两个文件
来源：http://vu.haigaiapp.cn

diff a.txt b.txt
来源：http://wo.shxzskj.cn

[R55] 压缩与解压
来源：http://jk.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ue.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://mj.hnjuh.cn

scp file user@host:/path/
来源：http://nw.huixiangedu.cn

[R57] 远程执行命令
来源：http://vt.yuexingan06.cn

ssh user@host 'uptime'
来源：http://lv.shxzskj.cn

[R58] 下载文件
来源：http://fv.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kq.shtwfgs.cn

[R59] 发 POST JSON
来源：http://bn.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://au.521024.cn

[R60] 只看 HTTP 状态码
来源：http://mk.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vv.newstarts.cn

[R61] 磁盘占用
来源：http://fj.panjiajie.cn

df -h;  du -sh *
来源：http://xb.nszjky.cn

[R62] 找最占空间的文件
来源：http://ze.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://si.shtwfgs.cn

[R63] 内存与进程
来源：http://ei.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://cy.haigaiapp.cn

[R64] 结束进程
来源：http://nn.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://to.nszjky.cn

[R65] 查看端口占用
来源：http://sy.jctech888.com.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://of.szxytkj.cn

[R66] 定时任务
来源：http://ho.521024.cn

crontab -e;  crontab -l
来源：http://ng.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://cu.muxihuayi.cn

openssl rand -hex 16
来源：http://mt.nszjky.cn

[R68] 计算文件校验值
来源：http://uh.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gp.colortex.cn

[R69] 生成随机密码
来源：http://eo.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://cp.521024.cn

[R70] 时间戳与互转
来源：http://fh.hahajie.cn

date +%s;  date -d @1700000000
来源：http://af.huanxung.cn

[R71] 日期格式化
来源：http://tv.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qu.colortex.cn

[R72] 等待端口就绪
来源：http://my.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://av.jctech888.com.cn

[R73] 分割大日志
来源：http://fx.shtwfgs.cn

split -l 1000 big.log part_
来源：http://ed.szsharing.cn

[R74] 批量重命名
来源：http://ee.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fw.huanxung.cn

[R75] 导出环境变量
来源：http://qf.wgjwhj.cn


<!-- 参考信息 -->