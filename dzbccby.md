代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nm.huanxung.cn

[Q32] 分组拼接字符串
来源：http://zj.hahajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wl.bjjhwx.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://id.hahajie.cn

[Q33] 多列分组
来源：http://ve.huixiangedu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dw.szxytkj.cn

[Q34] 每组取第一条
来源：http://rh.shxzukj.cn

SELECT * FROM (
来源：http://er.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yj.huixinmuqiang.cn

) t WHERE rn = 1;
来源：http://xu.huixiangedu.cn

[Q35] 内连接
来源：http://ds.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sb.chemitech.net.cn

[Q36] 左连接
来源：http://sq.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bs.wgjwhj.cn

[Q37] 右连接
来源：http://ha.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oo.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bp.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gl.bjjhwx.cn

[Q39] 自连接（查上下级）
来源：http://li.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nh.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fy.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zo.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zi.huixinmuqiang.cn

[Q41] 多表连接
来源：http://fy.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hn.yuexingan06.cn

JOIN users u ON u.id = o.user_id
来源：http://dp.haigaiapp.cn

JOIN products p ON p.id = o.product_id;
来源：http://lj.yuexingan06.cn

[Q42] 连接条件附加过滤
来源：http://ha.newstarts.cn

SELECT u.name, o.amount FROM users u
来源：http://dd.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vd.shtwfgs.cn

[Q43] 标量子查询
来源：http://xn.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nc.newstarts.cn

[Q44] IN 子查询
来源：http://ls.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cx.nicolike.cn

[Q45] EXISTS 判断存在
来源：http://dt.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fj.nszjky.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ws.huixiangedu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fy.jctech888.com.cn

[Q47] 与平均值比较
来源：http://xp.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://do.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://av.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tm.jctech888.com.cn

SELECT * FROM t WHERE c > 5;
来源：http://bx.huixinmuqiang.cn

[Q49] 更新单行
来源：http://eg.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uj.shxzukj.cn

[Q50] 批量更新
来源：http://ng.szsharing.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xv.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://gl.bjjhwx.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hj.jctech888.com.cn

[Q52] 删除指定行
来源：http://cd.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://ku.huixinmuqiang.cn

[Q53] 按条件删除
来源：http://qr.haigaiapp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lt.hnjuh.cn

[Q54] 清空表
来源：http://cz.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://lr.shxzukj.cn

[Q55] 排名（并列占位）
来源：http://re.newstarts.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oz.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://re.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fn.szxytkj.cn

[Q57] 行号
来源：http://dp.huixiangedu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://aq.newstarts.cn

[Q58] 累计求和
来源：http://vn.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rz.shxzskj.cn

[Q59] 分组内累计
来源：http://ct.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hu.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://wv.bjjhwx.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://px.lnxyls.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://om.bjjhwx.cn

[Q61] 移动平均
来源：http://dl.nszjky.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wu.panjiajie.cn

[Q62] 分组占比
来源：http://we.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fg.hahajie.cn

[Q63] 开启事务
来源：http://mg.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ca.muxihuayi.cn

[Q64] 提交事务
来源：http://yl.szsharing.cn

COMMIT;
来源：http://eo.szxytkj.cn

[Q65] 回滚事务
来源：http://ap.nicolike.cn

ROLLBACK;
来源：http://oi.jctech888.com.cn

[Q66] 行锁查询
来源：http://wy.9csxet.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qt.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://va.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hb.9csxet.cn

[Q68] 保存点
来源：http://ze.gzmigu.cn

SAVEPOINT sp1;
来源：http://sq.yuexingan06.cn

ROLLBACK TO sp1;
来源：http://aj.521024.cn

[Q69] 查看执行计划
来源：http://oo.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xo.lnxyls.cn

[Q70] 更新统计信息
来源：http://bx.panjiajie.cn

ANALYZE TABLE users;
来源：http://sb.haigaiapp.cn

[Q71] 查看建表语句
来源：http://cb.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://az.521024.cn

[Q72] 查看索引
来源：http://cl.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://nf.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://xo.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ju.yuntaijiaju.cn

[Q74] 强制使用索引
来源：http://wf.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zp.nszjky.cn

[Q75] 日期格式化
来源：http://ad.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mz.muxihuayi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vg.shxzskj.cn

[Q76] 按天统计
来源：http://eh.panjiajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lr.huixiangedu.cn

[Q77] 时间加减
来源：http://bu.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pg.bookmarksfly.cn

[Q78] 当前时间
来源：http://ee.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qb.haigaiapp.cn

[Q79] 字符串拼接
来源：http://ku.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cg.hnjuh.cn

[Q80] 字符串截取
来源：http://to.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ma.colortex.cn

[Q81] 字符串替换
来源：http://lw.jctech888.com.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cx.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://jf.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zg.521024.cn

[Q83] 大小写转换
来源：http://kh.yuexingan06.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://df.shxzskj.cn

[Q84] 去除首尾空格
来源：http://av.jctech888.com.cn

SELECT TRIM(name) FROM users;
来源：http://za.bookmarksfly.cn

[Q85] 数值取整
来源：http://ru.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gr.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://jk.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ev.colortex.cn

[Q87] JSON 字段做条件
来源：http://el.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fo.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://ve.huixiangedu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sv.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gn.521024.cn

[Q89] 判断表是否存在
来源：http://pn.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zs.lnxyls.cn

[Q90] 生成序号列
来源：http://qk.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ka.haigaiapp.cn

================================================================================
来源：http://ps.yuntaijiaju.cn

R. Bash 专题
来源：http://aj.huixiangedu.cn

================================================================================
来源：http://de.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://at.lnxyls.cn

#!/usr/bin/env bash
来源：http://lc.szsharing.cn

set -euo pipefail
来源：http://ou.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://vm.nicolike.cn

name="Tom"; echo "$name"
来源：http://rs.huixinmuqiang.cn

[R03] 只读变量
来源：http://cv.9csxet.cn

readonly PI=3.14
来源：http://de.shxzskj.cn

[R04] 位置参数
来源：http://tg.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://be.hnjuh.cn

[R05] 参数默认值
来源：http://dq.chemitech.net.cn

name="${1:-default}"
来源：http://ue.shxzskj.cn

[R06] 判断命令是否存在
来源：http://sr.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nu.gzmigu.cn

[R07] if 判断文件
来源：http://ii.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ic.wgjwhj.cn

[R08] 数值比较
来源：http://az.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bz.newstarts.cn

[R09] 字符串比较
来源：http://qc.bookmarksfly.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://du.bjjhwx.cn

[R10] 正则匹配
来源：http://wn.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://am.nicolike.cn

[R11] case 多分支
来源：http://iw.shxzukj.cn

case "$1" in
来源：http://hw.asd995.cn

start) echo "启动" ;;
来源：http://ev.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://ke.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://hz.muxihuayi.cn

esac
来源：http://bg.huixiangedu.cn

[R12] for 遍历文件
来源：http://mh.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://gc.haigaiapp.cn

[R13] for 计数循环
来源：http://jv.szsharing.cn

for i in {1..10}; do echo "$i"; done
来源：http://uq.wgjwhj.cn

[R14] C 风格 for
来源：http://jc.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nh.huixiangedu.cn

[R15] while 逐行读文件
来源：http://ba.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pv.hnjuh.cn

[R16] until 等待条件
来源：http://ww.huixiangedu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sp.huanxung.cn

[R17] 数组定义与取值
来源：http://sp.huanxung.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cy.jianghongdianzi.cn

[R18] 遍历数组
来源：http://ni.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mn.shxzskj.cn

[R19] 数组长度
来源：http://pp.9csxet.cn

echo "${#arr[@]}"
来源：http://qn.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://kx.huixinmuqiang.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cb.wgjwhj.cn

[R21] 字符串长度
来源：http://na.colortex.cn

echo "${#s}"
来源：http://jk.wgjwhj.cn

[R22] 截取子串
来源：http://od.9csxet.cn

echo "${s:0:5}"
来源：http://cw.bjjhwx.cn

[R23] 字符串替换
来源：http://uh.asd995.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qc.9csxet.cn

[R24] 大小写转换
来源：http://iy.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://iw.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://ml.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://om.yuntaijiaju.cn

[R26] 命令替换
来源：http://nl.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://my.lnxyls.cn

[R27] 算术展开
来源：http://ft.szsharing.cn

echo $((1 + 2 * 3))
来源：http://vb.nicolike.cn

[R28] 浮点运算
来源：http://tu.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://ky.hnjuh.cn

[R29] 定义函数
来源：http://ie.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zu.9csxet.cn

[R30] 函数返回状态码
来源：http://cf.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://vp.szsharing.cn

[R31] 局部变量
来源：http://mb.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://ts.shxzukj.cn

[R32] 参数个数校验
来源：http://vj.shtwfgs.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fo.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://ra.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gu.hahajie.cn

[R34] 退出时清理
来源：http://vv.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zi.colortex.cn

[R35] 后台执行并等待
来源：http://gj.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://le.hnjuh.cn

[R36] 并发执行多个任务
来源：http://tl.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ck.jianghongdianzi.cn

[R37] 把输出赋给变量
来源：http://xd.gzmigu.cn

files=$(ls -1)
来源：http://xu.yuexingan06.cn

[R38] 管道串联
来源：http://td.nszjky.cn

cat a.txt | grep -i error | wc -l
来源：http://hl.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://rn.haigaiapp.cn

cmd > out.log 2>&1
来源：http://qa.521024.cn

[R40] 追加写日志
来源：http://jh.haigaiapp.cn

echo "log" >> out.log
来源：http://rm.wgjwhj.cn

[R41] 丢弃输出
来源：http://us.yuntaijiaju.cn

cmd >/dev/null 2>&1
来源：http://se.bookmarksfly.cn

[R42] 输入重定向
来源：http://za.huixinmuqiang.cn

wc -l < a.txt
来源：http://gi.gzmigu.cn

[R43] 按名字查找文件
来源：http://qw.szxytkj.cn

find . -name "*.log" -type f
来源：http://vm.huanxung.cn

[R44] 按修改时间查找
来源：http://fg.jctech888.com.cn

find . -mtime -7 -type f
来源：http://fu.bookmarksfly.cn

[R45] 批量删除
来源：http://zi.hahajie.cn

find . -name "*.tmp" -delete
来源：http://bb.newstarts.cn

[R46] 递归替换文件内容
来源：http://gc.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qt.521024.cn

[R47] sed 单行替换
来源：http://wm.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nk.panjiajie.cn

[R48] awk 取指定列
来源：http://hu.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://ud.shxzskj.cn

[R49] awk 带条件
来源：http://ho.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bb.newstarts.cn

[R50] awk 求和
来源：http://cx.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wb.lnxyls.cn

[R51] 排序去重取前几
来源：http://zg.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ek.lnxyls.cn

[R52] 统计行数
来源：http://ru.shtwfgs.cn

wc -l a.txt
来源：http://xv.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://eo.colortex.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://js.9csxet.cn

[R54] 比较两个文件
来源：http://an.shtwfgs.cn

diff a.txt b.txt
来源：http://oh.nszjky.cn

[R55] 压缩与解压
来源：http://ja.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cw.szxytkj.cn

[R56] 远程拷贝
来源：http://rm.9csxet.cn

scp file user@host:/path/
来源：http://oq.hnjuh.cn

[R57] 远程执行命令
来源：http://lc.lnxyls.cn

ssh user@host 'uptime'
来源：http://fx.huanxung.cn

[R58] 下载文件
来源：http://fc.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ex.bjjhwx.cn

[R59] 发 POST JSON
来源：http://ka.shxzskj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bw.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://zh.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lu.newstarts.cn

[R61] 磁盘占用
来源：http://wr.hahajie.cn

df -h;  du -sh *
来源：http://ju.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://ra.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://zz.hahajie.cn

[R63] 内存与进程
来源：http://ie.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://si.asd995.cn

[R64] 结束进程
来源：http://lx.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://xu.yuexingan06.cn

[R65] 查看端口占用
来源：http://ql.colortex.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pg.haigaiapp.cn

[R66] 定时任务
来源：http://pg.9csxet.cn

crontab -e;  crontab -l
来源：http://gw.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://ur.gzmigu.cn

openssl rand -hex 16
来源：http://xs.9csxet.cn

[R68] 计算文件校验值
来源：http://ls.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tw.gzmigu.cn

[R69] 生成随机密码
来源：http://hk.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://qk.haigaiapp.cn

[R70] 时间戳与互转
来源：http://kd.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://st.9csxet.cn

[R71] 日期格式化
来源：http://jf.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zk.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://gp.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ps.szsharing.cn

[R73] 分割大日志
来源：http://tv.haigaiapp.cn

split -l 1000 big.log part_
来源：http://xa.colortex.cn

[R74] 批量重命名
来源：http://if.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vf.panjiajie.cn

[R75] 导出环境变量
来源：http://qn.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://xv.colortex.cn

[R76] 使用临时文件
来源：http://um.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ou.yuexingan06.cn

[R77] 读取用户输入
来源：http://te.colortex.cn

read -rp "请输入: " ans
来源：http://zu.gzmigu.cn

[R78] 交互式菜单
来源：http://eh.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qp.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://fi.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tf.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://bu.muxihuayi.cn

time ./run.sh
来源：http://nl.jctech888.com.cn

================================================================================
来源：http://pn.nszjky.cn


<!-- 参考信息 -->