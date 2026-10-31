代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wo.colortex.cn

[Q26] 计数
来源：http://sx.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://ux.muxihuayi.cn

[Q27] 条件计数
来源：http://fa.shtwfgs.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fu.521024.cn

[Q28] 求和与平均
来源：http://lk.lnxyls.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uv.huixiangedu.cn

[Q29] 最大最小值
来源：http://ra.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qb.huixinmuqiang.cn

[Q30] 分组统计
来源：http://ve.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gi.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://tl.bjjhwx.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uw.yuntaijiaju.cn

[Q32] 分组拼接字符串
来源：http://yo.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://li.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nj.521024.cn

[Q33] 多列分组
来源：http://ib.gzmigu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ac.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://up.lnxyls.cn

SELECT * FROM (
来源：http://to.nszjky.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://df.chemitech.net.cn

) t WHERE rn = 1;
来源：http://ra.jianghongdianzi.cn

[Q35] 内连接
来源：http://bu.szsharing.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wu.panjiajie.cn

[Q36] 左连接
来源：http://zn.9csxet.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nw.hnjuh.cn

[Q37] 右连接
来源：http://pt.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://up.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yg.9csxet.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ro.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://ju.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://uq.shtwfgs.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yl.colortex.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hb.huanxung.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bs.hnjuh.cn

[Q41] 多表连接
来源：http://on.gzmigu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ql.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://eb.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://mn.szsharing.cn

[Q42] 连接条件附加过滤
来源：http://qs.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://mi.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hl.colortex.cn

[Q43] 标量子查询
来源：http://kl.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://za.muxihuayi.cn

[Q44] IN 子查询
来源：http://nn.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fo.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://gx.bjjhwx.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qj.nszjky.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ca.panjiajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://je.shtwfgs.cn

[Q47] 与平均值比较
来源：http://tb.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hy.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://gy.jctech888.com.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ie.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://tb.yuexingan06.cn

[Q49] 更新单行
来源：http://zr.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vz.shxzukj.cn

[Q50] 批量更新
来源：http://pa.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gc.yuexingan06.cn

[Q51] 用子查询更新
来源：http://ui.yuntaijiaju.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dk.asd995.cn

[Q52] 删除指定行
来源：http://ko.gzmigu.cn

DELETE FROM users WHERE id = 10;
来源：http://ge.wgjwhj.cn

[Q53] 按条件删除
来源：http://xv.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lx.colortex.cn

[Q54] 清空表
来源：http://qg.shxzukj.cn

TRUNCATE TABLE logs;
来源：http://ry.wgjwhj.cn

[Q55] 排名（并列占位）
来源：http://sx.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wt.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://kq.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ag.huanxung.cn

[Q57] 行号
来源：http://pd.jctech888.com.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ez.yuexingan06.cn

[Q58] 累计求和
来源：http://lu.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zv.bookmarksfly.cn

[Q59] 分组内累计
来源：http://uh.panjiajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pb.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://nf.nicolike.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://md.yuntaijiaju.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ne.yuexingan06.cn

[Q61] 移动平均
来源：http://jd.521024.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lq.jianghongdianzi.cn

[Q62] 分组占比
来源：http://rj.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ab.huixiangedu.cn

[Q63] 开启事务
来源：http://an.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fd.yuntaijiaju.cn

[Q64] 提交事务
来源：http://ek.panjiajie.cn

COMMIT;
来源：http://fh.szxytkj.cn

[Q65] 回滚事务
来源：http://yp.szsharing.cn

ROLLBACK;
来源：http://ah.colortex.cn

[Q66] 行锁查询
来源：http://kz.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fr.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://zd.haigaiapp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ud.yuexingan06.cn

[Q68] 保存点
来源：http://dd.chemitech.net.cn

SAVEPOINT sp1;
来源：http://no.panjiajie.cn

ROLLBACK TO sp1;
来源：http://pu.nszjky.cn

[Q69] 查看执行计划
来源：http://ou.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gb.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://qb.shtwfgs.cn

ANALYZE TABLE users;
来源：http://ve.bjjhwx.cn

[Q71] 查看建表语句
来源：http://ed.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lp.haigaiapp.cn

[Q72] 查看索引
来源：http://hr.huanxung.cn

SHOW INDEX FROM users;
来源：http://tb.wgjwhj.cn

[Q73] 查看表状态
来源：http://bc.bookmarksfly.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xh.bookmarksfly.cn

[Q74] 强制使用索引
来源：http://sv.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sl.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://ap.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rt.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fz.newstarts.cn

[Q76] 按天统计
来源：http://om.szxytkj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rp.nszjky.cn

[Q77] 时间加减
来源：http://vz.yuexingan06.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ge.521024.cn

[Q78] 当前时间
来源：http://ou.panjiajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ws.jianghongdianzi.cn

[Q79] 字符串拼接
来源：http://tb.gzmigu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zt.wgjwhj.cn

[Q80] 字符串截取
来源：http://ev.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uu.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://au.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ju.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://lq.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ce.wgjwhj.cn

[Q83] 大小写转换
来源：http://uk.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ba.jctech888.com.cn

[Q84] 去除首尾空格
来源：http://hm.haigaiapp.cn

SELECT TRIM(name) FROM users;
来源：http://ai.jctech888.com.cn

[Q85] 数值取整
来源：http://im.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ft.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://kf.9csxet.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pv.9csxet.cn

[Q87] JSON 字段做条件
来源：http://fu.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://if.huixinmuqiang.cn

[Q88] 行转列（条件聚合）
来源：http://jc.newstarts.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fj.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ck.nicolike.cn

[Q89] 判断表是否存在
来源：http://xs.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://py.bookmarksfly.cn

[Q90] 生成序号列
来源：http://gb.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gr.huanxung.cn

================================================================================
来源：http://qk.szxytkj.cn

R. Bash 专题
来源：http://ve.hahajie.cn

================================================================================
来源：http://nl.haigaiapp.cn

[R01] shebang 与严格模式
来源：http://xw.huixinmuqiang.cn

#!/usr/bin/env bash
来源：http://ul.jianghongdianzi.cn

set -euo pipefail
来源：http://tp.nszjky.cn

[R02] 变量赋值与使用
来源：http://rx.nicolike.cn

name="Tom"; echo "$name"
来源：http://cb.nszjky.cn

[R03] 只读变量
来源：http://um.lnxyls.cn

readonly PI=3.14
来源：http://fe.bookmarksfly.cn

[R04] 位置参数
来源：http://pb.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ys.gzmigu.cn

[R05] 参数默认值
来源：http://ni.muxihuayi.cn

name="${1:-default}"
来源：http://ut.panjiajie.cn

[R06] 判断命令是否存在
来源：http://ej.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ba.huanxung.cn

[R07] if 判断文件
来源：http://qm.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://um.bookmarksfly.cn

[R08] 数值比较
来源：http://dp.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ar.shxzukj.cn

[R09] 字符串比较
来源：http://ei.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://my.wgjwhj.cn

[R10] 正则匹配
来源：http://zo.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ze.shxzukj.cn

[R11] case 多分支
来源：http://lo.nicolike.cn

case "$1" in
来源：http://rq.huanxung.cn

start) echo "启动" ;;
来源：http://ep.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://vm.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://cm.huanxung.cn

esac
来源：http://qo.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://pr.newstarts.cn

for f in *.txt; do echo "$f"; done
来源：http://ic.asd995.cn

[R13] for 计数循环
来源：http://wh.yuntaijiaju.cn

for i in {1..10}; do echo "$i"; done
来源：http://pi.hnjuh.cn

[R14] C 风格 for
来源：http://pa.huixiangedu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vg.szsharing.cn

[R15] while 逐行读文件
来源：http://it.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qy.hnjuh.cn

[R16] until 等待条件
来源：http://gg.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cv.asd995.cn

[R17] 数组定义与取值
来源：http://yf.shtwfgs.cn

arr=(a b c); echo "${arr[0]}"
来源：http://js.szxytkj.cn

[R18] 遍历数组
来源：http://jy.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pt.yuexingan06.cn

[R19] 数组长度
来源：http://sf.bjjhwx.cn

echo "${#arr[@]}"
来源：http://gi.shtwfgs.cn

[R20] 关联数组（字典）
来源：http://bk.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://za.yuntaijiaju.cn

[R21] 字符串长度
来源：http://oa.haigaiapp.cn

echo "${#s}"
来源：http://jc.shxzskj.cn

[R22] 截取子串
来源：http://xm.shtwfgs.cn

echo "${s:0:5}"
来源：http://qt.521024.cn

[R23] 字符串替换
来源：http://fa.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://re.yuexingan06.cn

[R24] 大小写转换
来源：http://by.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sa.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://tu.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cr.colortex.cn

[R26] 命令替换
来源：http://iu.huixiangedu.cn

now=$(date +%F); echo "$now"
来源：http://jg.chemitech.net.cn

[R27] 算术展开
来源：http://or.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://xf.lnxyls.cn

[R28] 浮点运算
来源：http://kn.521024.cn

echo "scale=2; 10/3" | bc
来源：http://ng.bjjhwx.cn

[R29] 定义函数
来源：http://fh.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jj.huanxung.cn

[R30] 函数返回状态码
来源：http://ur.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://by.521024.cn

[R31] 局部变量
来源：http://uh.bjjhwx.cn

f() { local x=1; echo "$x"; }
来源：http://kj.chemitech.net.cn

[R32] 参数个数校验
来源：http://lq.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ml.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://tx.gzmigu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tb.panjiajie.cn

[R34] 退出时清理
来源：http://pt.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ls.nicolike.cn

[R35] 后台执行并等待
来源：http://re.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://el.szxytkj.cn

[R36] 并发执行多个任务
来源：http://eu.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jo.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://jp.shtwfgs.cn

files=$(ls -1)
来源：http://rw.yuntaijiaju.cn

[R38] 管道串联
来源：http://ce.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://rf.jctech888.com.cn

[R39] 重定向标准输出与错误
来源：http://wa.haigaiapp.cn

cmd > out.log 2>&1
来源：http://jj.haigaiapp.cn

[R40] 追加写日志
来源：http://qa.hnjuh.cn

echo "log" >> out.log
来源：http://yr.szsharing.cn

[R41] 丢弃输出
来源：http://vj.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://fr.muxihuayi.cn

[R42] 输入重定向
来源：http://ht.newstarts.cn

wc -l < a.txt
来源：http://vy.hnjuh.cn

[R43] 按名字查找文件
来源：http://cv.muxihuayi.cn

find . -name "*.log" -type f
来源：http://gf.hnjuh.cn

[R44] 按修改时间查找
来源：http://lo.szsharing.cn

find . -mtime -7 -type f
来源：http://eq.9csxet.cn

[R45] 批量删除
来源：http://tl.nicolike.cn

find . -name "*.tmp" -delete
来源：http://el.nszjky.cn

[R46] 递归替换文件内容
来源：http://bp.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zr.gzmigu.cn

[R47] sed 单行替换
来源：http://ho.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ps.hnjuh.cn

[R48] awk 取指定列
来源：http://xd.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://kt.szxytkj.cn

[R49] awk 带条件
来源：http://tg.huixiangedu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qk.asd995.cn

[R50] awk 求和
来源：http://tf.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yw.9csxet.cn

[R51] 排序去重取前几
来源：http://eh.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cm.yuexingan06.cn

[R52] 统计行数
来源：http://uu.shxzskj.cn

wc -l a.txt
来源：http://vi.hahajie.cn

[R53] 查看文件头与实时尾
来源：http://em.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jk.shxzskj.cn

[R54] 比较两个文件
来源：http://vx.nszjky.cn

diff a.txt b.txt
来源：http://mh.lnxyls.cn

[R55] 压缩与解压
来源：http://zz.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cj.hahajie.cn

[R56] 远程拷贝
来源：http://sy.huanxung.cn

scp file user@host:/path/
来源：http://st.muxihuayi.cn

[R57] 远程执行命令
来源：http://qe.huanxung.cn

ssh user@host 'uptime'
来源：http://ng.panjiajie.cn

[R58] 下载文件
来源：http://zf.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rz.lnxyls.cn

[R59] 发 POST JSON
来源：http://xb.panjiajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rv.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://bt.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mk.wgjwhj.cn

[R61] 磁盘占用
来源：http://hn.huixiangedu.cn

df -h;  du -sh *
来源：http://mi.newstarts.cn

[R62] 找最占空间的文件
来源：http://rg.lnxyls.cn

du -ah . | sort -rh | head -10
来源：http://ch.newstarts.cn

[R63] 内存与进程
来源：http://cx.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://pa.chemitech.net.cn

[R64] 结束进程
来源：http://bf.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://pi.nicolike.cn

[R65] 查看端口占用
来源：http://fd.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jz.szxytkj.cn

[R66] 定时任务
来源：http://bs.huanxung.cn

crontab -e;  crontab -l
来源：http://fg.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://jd.chemitech.net.cn

openssl rand -hex 16
来源：http://wt.9csxet.cn

[R68] 计算文件校验值
来源：http://tf.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xx.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://sj.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://kl.shxzukj.cn

[R70] 时间戳与互转
来源：http://mc.yuntaijiaju.cn

date +%s;  date -d @1700000000
来源：http://vd.jctech888.com.cn

[R71] 日期格式化
来源：http://yl.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qk.bjjhwx.cn

[R72] 等待端口就绪
来源：http://op.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ar.shxzukj.cn

[R73] 分割大日志
来源：http://ux.colortex.cn

split -l 1000 big.log part_
来源：http://ia.shxzukj.cn

[R74] 批量重命名
来源：http://ck.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zp.wgjwhj.cn

[R75] 导出环境变量
来源：http://ks.gzmigu.cn


<!-- 参考信息 -->