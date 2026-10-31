代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rw.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://ab.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vz.hahajie.cn

[Q29] 最大最小值
来源：http://ny.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://na.gzmigu.cn

[Q30] 分组统计
来源：http://uv.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://po.colortex.cn

[Q31] 分组后过滤
来源：http://wd.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ym.hahajie.cn

[Q32] 分组拼接字符串
来源：http://ds.nszjky.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fl.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pr.szsharing.cn

[Q33] 多列分组
来源：http://ek.hahajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://va.shtwfgs.cn

[Q34] 每组取第一条
来源：http://ci.hahajie.cn

SELECT * FROM (
来源：http://uk.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tw.haigaiapp.cn

) t WHERE rn = 1;
来源：http://jy.panjiajie.cn

[Q35] 内连接
来源：http://sx.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ps.colortex.cn

[Q36] 左连接
来源：http://rn.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hm.shxzukj.cn

[Q37] 右连接
来源：http://ib.nicolike.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yp.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gy.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ae.hnjuh.cn

[Q39] 自连接（查上下级）
来源：http://zk.521024.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nj.jianghongdianzi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hb.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tu.nicolike.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kx.szsharing.cn

[Q41] 多表连接
来源：http://mk.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kl.huanxung.cn

JOIN users u ON u.id = o.user_id
来源：http://ot.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://wv.lnxyls.cn

[Q42] 连接条件附加过滤
来源：http://ko.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://ie.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vz.gzmigu.cn

[Q43] 标量子查询
来源：http://ri.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lm.muxihuayi.cn

[Q44] IN 子查询
来源：http://hm.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://av.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://kh.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bf.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xf.bookmarksfly.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://as.huixiangedu.cn

[Q47] 与平均值比较
来源：http://ny.jianghongdianzi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ur.gzmigu.cn

[Q48] CTE 公用表表达式
来源：http://rm.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ac.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://sl.lnxyls.cn

[Q49] 更新单行
来源：http://uj.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eb.huixinmuqiang.cn

[Q50] 批量更新
来源：http://bp.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yc.lnxyls.cn

[Q51] 用子查询更新
来源：http://js.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qj.szxytkj.cn

[Q52] 删除指定行
来源：http://bi.huanxung.cn

DELETE FROM users WHERE id = 10;
来源：http://rz.521024.cn

[Q53] 按条件删除
来源：http://pt.haigaiapp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qp.asd995.cn

[Q54] 清空表
来源：http://tz.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://ms.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://pq.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lz.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://wo.bookmarksfly.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ih.yuexingan06.cn

[Q57] 行号
来源：http://ee.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gc.nicolike.cn

[Q58] 累计求和
来源：http://fe.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cj.gzmigu.cn

[Q59] 分组内累计
来源：http://uv.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ei.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://ef.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fu.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://du.chemitech.net.cn

[Q61] 移动平均
来源：http://sx.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ml.szsharing.cn

[Q62] 分组占比
来源：http://cw.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hd.szsharing.cn

[Q63] 开启事务
来源：http://bx.huanxung.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lw.yuntaijiaju.cn

[Q64] 提交事务
来源：http://ej.jctech888.com.cn

COMMIT;
来源：http://om.yuexingan06.cn

[Q65] 回滚事务
来源：http://ul.szsharing.cn

ROLLBACK;
来源：http://gv.huanxung.cn

[Q66] 行锁查询
来源：http://hu.muxihuayi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rr.jctech888.com.cn

[Q67] 设置隔离级别
来源：http://gg.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://br.9csxet.cn

[Q68] 保存点
来源：http://wg.nszjky.cn

SAVEPOINT sp1;
来源：http://ia.huanxung.cn

ROLLBACK TO sp1;
来源：http://bg.gzmigu.cn

[Q69] 查看执行计划
来源：http://ff.lnxyls.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fi.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://jq.colortex.cn

ANALYZE TABLE users;
来源：http://bw.yuexingan06.cn

[Q71] 查看建表语句
来源：http://yp.bjjhwx.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://el.newstarts.cn

[Q72] 查看索引
来源：http://yt.521024.cn

SHOW INDEX FROM users;
来源：http://cm.panjiajie.cn

[Q73] 查看表状态
来源：http://on.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://np.yuexingan06.cn

[Q74] 强制使用索引
来源：http://zh.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lo.shxzskj.cn

[Q75] 日期格式化
来源：http://ta.hahajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vx.huanxung.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zu.jianghongdianzi.cn

[Q76] 按天统计
来源：http://bf.huixinmuqiang.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wb.asd995.cn

[Q77] 时间加减
来源：http://px.hahajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dx.nicolike.cn

[Q78] 当前时间
来源：http://bt.muxihuayi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://et.lnxyls.cn

[Q79] 字符串拼接
来源：http://hy.shxzskj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ze.shtwfgs.cn

[Q80] 字符串截取
来源：http://jb.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qe.wgjwhj.cn

[Q81] 字符串替换
来源：http://cd.jctech888.com.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zw.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://eq.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ks.hnjuh.cn

[Q83] 大小写转换
来源：http://mo.huixiangedu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://db.szsharing.cn

[Q84] 去除首尾空格
来源：http://nk.jctech888.com.cn

SELECT TRIM(name) FROM users;
来源：http://lh.yuexingan06.cn

[Q85] 数值取整
来源：http://hq.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ub.9csxet.cn

[Q86] 读取 JSON 字段
来源：http://iu.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lb.huixinmuqiang.cn

[Q87] JSON 字段做条件
来源：http://ix.wgjwhj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iy.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://fo.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nu.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vr.hnjuh.cn

[Q89] 判断表是否存在
来源：http://ka.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ya.yuexingan06.cn

[Q90] 生成序号列
来源：http://gj.chemitech.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ot.shtwfgs.cn

================================================================================
来源：http://zo.yuntaijiaju.cn

R. Bash 专题
来源：http://zx.lnxyls.cn

================================================================================
来源：http://kk.hnjuh.cn

[R01] shebang 与严格模式
来源：http://qu.gzmigu.cn

#!/usr/bin/env bash
来源：http://mv.muxihuayi.cn

set -euo pipefail
来源：http://md.wgjwhj.cn

[R02] 变量赋值与使用
来源：http://oh.gzmigu.cn

name="Tom"; echo "$name"
来源：http://hs.panjiajie.cn

[R03] 只读变量
来源：http://dk.bookmarksfly.cn

readonly PI=3.14
来源：http://kr.wgjwhj.cn

[R04] 位置参数
来源：http://rx.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://al.huixinmuqiang.cn

[R05] 参数默认值
来源：http://if.huixiangedu.cn

name="${1:-default}"
来源：http://jy.huixinmuqiang.cn

[R06] 判断命令是否存在
来源：http://hp.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lu.chemitech.net.cn

[R07] if 判断文件
来源：http://nz.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://un.shtwfgs.cn

[R08] 数值比较
来源：http://zs.nszjky.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bf.szsharing.cn

[R09] 字符串比较
来源：http://mu.shtwfgs.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ra.shxzskj.cn

[R10] 正则匹配
来源：http://uh.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rq.jianghongdianzi.cn

[R11] case 多分支
来源：http://wg.muxihuayi.cn

case "$1" in
来源：http://iu.colortex.cn

start) echo "启动" ;;
来源：http://pr.521024.cn

stop)  echo "停止" ;;
来源：http://fa.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://cz.gzmigu.cn

esac
来源：http://om.wgjwhj.cn

[R12] for 遍历文件
来源：http://ns.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://td.yuexingan06.cn

[R13] for 计数循环
来源：http://do.szxytkj.cn

for i in {1..10}; do echo "$i"; done
来源：http://eh.colortex.cn

[R14] C 风格 for
来源：http://gi.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yd.jianghongdianzi.cn

[R15] while 逐行读文件
来源：http://pp.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eu.521024.cn

[R16] until 等待条件
来源：http://bz.nszjky.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tg.huixinmuqiang.cn

[R17] 数组定义与取值
来源：http://zu.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qh.newstarts.cn

[R18] 遍历数组
来源：http://lo.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pp.huixiangedu.cn

[R19] 数组长度
来源：http://jt.nszjky.cn

echo "${#arr[@]}"
来源：http://sr.colortex.cn

[R20] 关联数组（字典）
来源：http://nu.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kw.yuntaijiaju.cn

[R21] 字符串长度
来源：http://ix.huixiangedu.cn

echo "${#s}"
来源：http://ja.asd995.cn

[R22] 截取子串
来源：http://fe.szxytkj.cn

echo "${s:0:5}"
来源：http://ij.521024.cn

[R23] 字符串替换
来源：http://fa.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qe.nszjky.cn

[R24] 大小写转换
来源：http://zi.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qa.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://ju.huanxung.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bi.9csxet.cn

[R26] 命令替换
来源：http://fl.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://uo.panjiajie.cn

[R27] 算术展开
来源：http://tj.colortex.cn

echo $((1 + 2 * 3))
来源：http://jn.wgjwhj.cn

[R28] 浮点运算
来源：http://gu.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://nt.haigaiapp.cn

[R29] 定义函数
来源：http://uq.jctech888.com.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tz.haigaiapp.cn

[R30] 函数返回状态码
来源：http://gp.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://nn.jianghongdianzi.cn

[R31] 局部变量
来源：http://nq.huanxung.cn

f() { local x=1; echo "$x"; }
来源：http://xm.asd995.cn

[R32] 参数个数校验
来源：http://ys.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mn.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://mv.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qm.newstarts.cn

[R34] 退出时清理
来源：http://mx.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nc.nicolike.cn

[R35] 后台执行并等待
来源：http://ou.gzmigu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://iv.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://sv.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ce.bjjhwx.cn

[R37] 把输出赋给变量
来源：http://nl.huixiangedu.cn

files=$(ls -1)
来源：http://ax.newstarts.cn

[R38] 管道串联
来源：http://lk.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://by.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://zo.nicolike.cn

cmd > out.log 2>&1
来源：http://mk.asd995.cn

[R40] 追加写日志
来源：http://br.colortex.cn

echo "log" >> out.log
来源：http://qe.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://ex.nszjky.cn

cmd >/dev/null 2>&1
来源：http://ia.bookmarksfly.cn

[R42] 输入重定向
来源：http://wz.521024.cn

wc -l < a.txt
来源：http://eu.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://km.asd995.cn

find . -name "*.log" -type f
来源：http://zp.muxihuayi.cn

[R44] 按修改时间查找
来源：http://hw.shxzukj.cn

find . -mtime -7 -type f
来源：http://sg.chemitech.net.cn

[R45] 批量删除
来源：http://qd.colortex.cn

find . -name "*.tmp" -delete
来源：http://ej.asd995.cn

[R46] 递归替换文件内容
来源：http://fz.nszjky.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mf.szxytkj.cn

[R47] sed 单行替换
来源：http://ew.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fp.shtwfgs.cn

[R48] awk 取指定列
来源：http://cp.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://fy.muxihuayi.cn

[R49] awk 带条件
来源：http://rq.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ik.panjiajie.cn

[R50] awk 求和
来源：http://rp.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tg.asd995.cn

[R51] 排序去重取前几
来源：http://oe.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://iw.newstarts.cn

[R52] 统计行数
来源：http://ic.colortex.cn

wc -l a.txt
来源：http://fw.hahajie.cn

[R53] 查看文件头与实时尾
来源：http://xr.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mm.gzmigu.cn

[R54] 比较两个文件
来源：http://xa.bookmarksfly.cn

diff a.txt b.txt
来源：http://vz.yuexingan06.cn

[R55] 压缩与解压
来源：http://wp.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ax.muxihuayi.cn

[R56] 远程拷贝
来源：http://us.szxytkj.cn

scp file user@host:/path/
来源：http://mb.huanxung.cn

[R57] 远程执行命令
来源：http://nu.nicolike.cn

ssh user@host 'uptime'
来源：http://fy.nicolike.cn

[R58] 下载文件
来源：http://yh.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rl.gzmigu.cn

[R59] 发 POST JSON
来源：http://wg.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ly.colortex.cn

[R60] 只看 HTTP 状态码
来源：http://ns.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pv.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://yo.bookmarksfly.cn

df -h;  du -sh *
来源：http://iw.panjiajie.cn

[R62] 找最占空间的文件
来源：http://vl.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://jk.yuexingan06.cn

[R63] 内存与进程
来源：http://st.haigaiapp.cn

free -h;  ps aux | grep nginx
来源：http://kp.nszjky.cn

[R64] 结束进程
来源：http://xk.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://ej.bjjhwx.cn

[R65] 查看端口占用
来源：http://qx.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zm.chemitech.net.cn

[R66] 定时任务
来源：http://xs.521024.cn

crontab -e;  crontab -l
来源：http://il.haigaiapp.cn

[R67] 生成随机十六进制串
来源：http://mf.bookmarksfly.cn

openssl rand -hex 16
来源：http://oe.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://sr.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rq.shxzukj.cn

[R69] 生成随机密码
来源：http://nq.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://ad.newstarts.cn

[R70] 时间戳与互转
来源：http://gb.panjiajie.cn

date +%s;  date -d @1700000000
来源：http://km.gzmigu.cn

[R71] 日期格式化
来源：http://kq.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://te.9csxet.cn

[R72] 等待端口就绪
来源：http://qh.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rg.shxzskj.cn

[R73] 分割大日志
来源：http://sk.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://ks.521024.cn

[R74] 批量重命名
来源：http://rz.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ra.9csxet.cn

[R75] 导出环境变量
来源：http://lg.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://yr.panjiajie.cn

[R76] 使用临时文件
来源：http://gu.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wi.521024.cn

[R77] 读取用户输入
来源：http://ve.hahajie.cn


<!-- 参考信息 -->