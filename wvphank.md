代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jz.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://ve.nszjky.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tv.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ra.wgjwhj.cn

[Q33] 多列分组
来源：http://iv.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gt.panjiajie.cn

[Q34] 每组取第一条
来源：http://ko.yuntaijiaju.cn

SELECT * FROM (
来源：http://mv.521024.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qr.huanxung.cn

) t WHERE rn = 1;
来源：http://oc.colortex.cn

[Q35] 内连接
来源：http://du.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fr.asd995.cn

[Q36] 左连接
来源：http://bk.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://im.nszjky.cn

[Q37] 右连接
来源：http://wj.lnxyls.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sg.gzmigu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ak.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://we.panjiajie.cn

[Q39] 自连接（查上下级）
来源：http://dk.gzmigu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zd.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dt.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://am.newstarts.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pb.lnxyls.cn

[Q41] 多表连接
来源：http://ye.nicolike.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hx.wgjwhj.cn

JOIN users u ON u.id = o.user_id
来源：http://xp.muxihuayi.cn

JOIN products p ON p.id = o.product_id;
来源：http://cz.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://vt.9csxet.cn

SELECT u.name, o.amount FROM users u
来源：http://fu.yuntaijiaju.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://op.szxytkj.cn

[Q43] 标量子查询
来源：http://ji.hnjuh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gi.asd995.cn

[Q44] IN 子查询
来源：http://pd.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://id.asd995.cn

[Q45] EXISTS 判断存在
来源：http://kf.lnxyls.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gq.huanxung.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sp.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wx.shtwfgs.cn

[Q47] 与平均值比较
来源：http://mz.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zh.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://md.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cl.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://cq.yuexingan06.cn

[Q49] 更新单行
来源：http://yr.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wr.huixiangedu.cn

[Q50] 批量更新
来源：http://gh.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tc.jctech888.com.cn

[Q51] 用子查询更新
来源：http://yp.521024.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hu.colortex.cn

[Q52] 删除指定行
来源：http://nf.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://mb.haigaiapp.cn

[Q53] 按条件删除
来源：http://jc.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ts.muxihuayi.cn

[Q54] 清空表
来源：http://uc.nszjky.cn

TRUNCATE TABLE logs;
来源：http://sf.bookmarksfly.cn

[Q55] 排名（并列占位）
来源：http://gr.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ys.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://ou.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dk.muxihuayi.cn

[Q57] 行号
来源：http://nz.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jf.gzmigu.cn

[Q58] 累计求和
来源：http://fv.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://of.9csxet.cn

[Q59] 分组内累计
来源：http://aq.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yx.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://dp.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tp.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nh.huanxung.cn

[Q61] 移动平均
来源：http://ct.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ho.haigaiapp.cn

[Q62] 分组占比
来源：http://ag.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wl.huanxung.cn

[Q63] 开启事务
来源：http://lw.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pd.hnjuh.cn

[Q64] 提交事务
来源：http://oj.szxytkj.cn

COMMIT;
来源：http://qv.hnjuh.cn

[Q65] 回滚事务
来源：http://qv.gzmigu.cn

ROLLBACK;
来源：http://dw.521024.cn

[Q66] 行锁查询
来源：http://pp.9csxet.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xh.newstarts.cn

[Q67] 设置隔离级别
来源：http://sp.yuexingan06.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yp.huixiangedu.cn

[Q68] 保存点
来源：http://gz.bjjhwx.cn

SAVEPOINT sp1;
来源：http://vk.newstarts.cn

ROLLBACK TO sp1;
来源：http://tu.shtwfgs.cn

[Q69] 查看执行计划
来源：http://iu.lnxyls.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lo.jctech888.com.cn

[Q70] 更新统计信息
来源：http://vy.nszjky.cn

ANALYZE TABLE users;
来源：http://ry.nszjky.cn

[Q71] 查看建表语句
来源：http://rs.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sq.asd995.cn

[Q72] 查看索引
来源：http://ay.asd995.cn

SHOW INDEX FROM users;
来源：http://wv.521024.cn

[Q73] 查看表状态
来源：http://hk.bookmarksfly.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ft.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://hb.lnxyls.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://iz.jctech888.com.cn

[Q75] 日期格式化
来源：http://mp.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pw.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bv.huanxung.cn

[Q76] 按天统计
来源：http://jy.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eb.nszjky.cn

[Q77] 时间加减
来源：http://do.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wj.jctech888.com.cn

[Q78] 当前时间
来源：http://co.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uk.9csxet.cn

[Q79] 字符串拼接
来源：http://tt.haigaiapp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vz.haigaiapp.cn

[Q80] 字符串截取
来源：http://kt.shtwfgs.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://br.shxzskj.cn

[Q81] 字符串替换
来源：http://ha.huixiangedu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rh.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://wd.9csxet.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://am.9csxet.cn

[Q83] 大小写转换
来源：http://rq.huixiangedu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://we.bjjhwx.cn

[Q84] 去除首尾空格
来源：http://dk.yuexingan06.cn

SELECT TRIM(name) FROM users;
来源：http://ow.hahajie.cn

[Q85] 数值取整
来源：http://oq.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dx.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://dp.muxihuayi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://od.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://lk.nszjky.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://au.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://xa.hnjuh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hv.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wf.chemitech.net.cn

[Q89] 判断表是否存在
来源：http://fo.asd995.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pr.huixinmuqiang.cn

[Q90] 生成序号列
来源：http://df.huixiangedu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nk.panjiajie.cn

================================================================================
来源：http://of.wgjwhj.cn

R. Bash 专题
来源：http://xi.jianghongdianzi.cn

================================================================================
来源：http://xv.9csxet.cn

[R01] shebang 与严格模式
来源：http://va.shxzskj.cn

#!/usr/bin/env bash
来源：http://cy.shtwfgs.cn

set -euo pipefail
来源：http://eb.asd995.cn

[R02] 变量赋值与使用
来源：http://af.shxzskj.cn

name="Tom"; echo "$name"
来源：http://hy.haigaiapp.cn

[R03] 只读变量
来源：http://vq.haigaiapp.cn

readonly PI=3.14
来源：http://bo.9csxet.cn

[R04] 位置参数
来源：http://xu.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ai.shtwfgs.cn

[R05] 参数默认值
来源：http://at.lnxyls.cn

name="${1:-default}"
来源：http://pz.panjiajie.cn

[R06] 判断命令是否存在
来源：http://gc.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qv.bjjhwx.cn

[R07] if 判断文件
来源：http://vh.nszjky.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jy.hahajie.cn

[R08] 数值比较
来源：http://rv.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://me.asd995.cn

[R09] 字符串比较
来源：http://ev.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bf.asd995.cn

[R10] 正则匹配
来源：http://tw.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qd.shxzskj.cn

[R11] case 多分支
来源：http://um.bjjhwx.cn

case "$1" in
来源：http://uf.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://nf.newstarts.cn

stop)  echo "停止" ;;
来源：http://wu.521024.cn

*)     echo "未知命令" ;;
来源：http://ls.hahajie.cn

esac
来源：http://sz.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://mb.huixinmuqiang.cn

for f in *.txt; do echo "$f"; done
来源：http://xz.shtwfgs.cn

[R13] for 计数循环
来源：http://li.jianghongdianzi.cn

for i in {1..10}; do echo "$i"; done
来源：http://gh.nszjky.cn

[R14] C 风格 for
来源：http://sy.9csxet.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eb.521024.cn

[R15] while 逐行读文件
来源：http://uw.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mz.gzmigu.cn

[R16] until 等待条件
来源：http://yb.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sy.huixinmuqiang.cn

[R17] 数组定义与取值
来源：http://wd.bookmarksfly.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vz.huixinmuqiang.cn

[R18] 遍历数组
来源：http://ng.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fa.wgjwhj.cn

[R19] 数组长度
来源：http://oi.shxzskj.cn

echo "${#arr[@]}"
来源：http://km.shxzukj.cn

[R20] 关联数组（字典）
来源：http://uo.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tr.hnjuh.cn

[R21] 字符串长度
来源：http://ub.huixiangedu.cn

echo "${#s}"
来源：http://gd.colortex.cn

[R22] 截取子串
来源：http://yj.asd995.cn

echo "${s:0:5}"
来源：http://fj.bjjhwx.cn

[R23] 字符串替换
来源：http://zy.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uo.gzmigu.cn

[R24] 大小写转换
来源：http://oq.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sg.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://fl.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qg.yuexingan06.cn

[R26] 命令替换
来源：http://km.521024.cn

now=$(date +%F); echo "$now"
来源：http://ad.shtwfgs.cn

[R27] 算术展开
来源：http://dt.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://hz.huanxung.cn

[R28] 浮点运算
来源：http://so.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://yl.newstarts.cn

[R29] 定义函数
来源：http://wf.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jz.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://ii.newstarts.cn

f() { return 0; }; f || echo "失败了"
来源：http://pe.lnxyls.cn

[R31] 局部变量
来源：http://xu.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://vp.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://ti.chemitech.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ws.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://dt.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wd.szsharing.cn

[R34] 退出时清理
来源：http://kg.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zd.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://hg.jianghongdianzi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hd.521024.cn

[R36] 并发执行多个任务
来源：http://py.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bj.newstarts.cn

[R37] 把输出赋给变量
来源：http://ro.hahajie.cn

files=$(ls -1)
来源：http://ur.chemitech.net.cn

[R38] 管道串联
来源：http://eb.lnxyls.cn

cat a.txt | grep -i error | wc -l
来源：http://sv.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://ct.bjjhwx.cn

cmd > out.log 2>&1
来源：http://ds.bookmarksfly.cn

[R40] 追加写日志
来源：http://np.lnxyls.cn

echo "log" >> out.log
来源：http://yl.chemitech.net.cn

[R41] 丢弃输出
来源：http://ww.asd995.cn

cmd >/dev/null 2>&1
来源：http://hk.yuexingan06.cn

[R42] 输入重定向
来源：http://lf.wgjwhj.cn

wc -l < a.txt
来源：http://yv.shxzukj.cn

[R43] 按名字查找文件
来源：http://ly.szxytkj.cn

find . -name "*.log" -type f
来源：http://ck.szsharing.cn

[R44] 按修改时间查找
来源：http://ln.521024.cn

find . -mtime -7 -type f
来源：http://wy.wgjwhj.cn

[R45] 批量删除
来源：http://cz.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://op.gzmigu.cn

[R46] 递归替换文件内容
来源：http://jx.muxihuayi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tx.newstarts.cn

[R47] sed 单行替换
来源：http://rx.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vj.muxihuayi.cn

[R48] awk 取指定列
来源：http://qi.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://ph.yuntaijiaju.cn

[R49] awk 带条件
来源：http://dt.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ha.bjjhwx.cn

[R50] awk 求和
来源：http://nn.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://he.shxzskj.cn

[R51] 排序去重取前几
来源：http://xv.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nc.shxzskj.cn

[R52] 统计行数
来源：http://fc.panjiajie.cn

wc -l a.txt
来源：http://rw.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://go.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bg.chemitech.net.cn

[R54] 比较两个文件
来源：http://sv.chemitech.net.cn

diff a.txt b.txt
来源：http://ez.gzmigu.cn

[R55] 压缩与解压
来源：http://hq.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ef.wgjwhj.cn

[R56] 远程拷贝
来源：http://ol.huanxung.cn

scp file user@host:/path/
来源：http://xn.hahajie.cn

[R57] 远程执行命令
来源：http://kr.szsharing.cn

ssh user@host 'uptime'
来源：http://fl.hahajie.cn

[R58] 下载文件
来源：http://qn.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yh.chemitech.net.cn

[R59] 发 POST JSON
来源：http://hd.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bo.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://lf.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sn.haigaiapp.cn

[R61] 磁盘占用
来源：http://qi.chemitech.net.cn

df -h;  du -sh *
来源：http://ri.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://gr.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://wk.huixiangedu.cn

[R63] 内存与进程
来源：http://fr.haigaiapp.cn

free -h;  ps aux | grep nginx
来源：http://hi.huanxung.cn

[R64] 结束进程
来源：http://fz.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://oy.chemitech.net.cn

[R65] 查看端口占用
来源：http://hd.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://al.chemitech.net.cn

[R66] 定时任务
来源：http://ig.huixiangedu.cn

crontab -e;  crontab -l
来源：http://lp.521024.cn

[R67] 生成随机十六进制串
来源：http://dv.nicolike.cn

openssl rand -hex 16
来源：http://zn.9csxet.cn

[R68] 计算文件校验值
来源：http://rd.521024.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nk.panjiajie.cn

[R69] 生成随机密码
来源：http://ih.colortex.cn

head -c 16 /dev/urandom | base64
来源：http://ne.newstarts.cn

[R70] 时间戳与互转
来源：http://pn.hahajie.cn

date +%s;  date -d @1700000000
来源：http://rc.chemitech.net.cn

[R71] 日期格式化
来源：http://mx.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ql.shxzskj.cn

[R72] 等待端口就绪
来源：http://rk.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wp.shxzukj.cn

[R73] 分割大日志
来源：http://by.shxzskj.cn

split -l 1000 big.log part_
来源：http://ip.jctech888.com.cn

[R74] 批量重命名
来源：http://pf.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ow.chemitech.net.cn

[R75] 导出环境变量
来源：http://yb.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://ko.szsharing.cn

[R76] 使用临时文件
来源：http://yr.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://us.colortex.cn

[R77] 读取用户输入
来源：http://xz.nszjky.cn

read -rp "请输入: " ans
来源：http://ph.521024.cn

[R78] 交互式菜单
来源：http://yk.9csxet.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nk.huixiangedu.cn

[R79] 解析命令行选项
来源：http://yx.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mm.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://ip.colortex.cn

time ./run.sh
来源：http://rd.521024.cn

================================================================================
来源：http://dw.newstarts.cn


<!-- 参考信息 -->