代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ws.wgjwhj.cn

[Q32] 分组拼接字符串
来源：http://ui.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gv.huixiangedu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wi.jianghongdianzi.cn

[Q33] 多列分组
来源：http://qa.haigaiapp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ko.wgjwhj.cn

[Q34] 每组取第一条
来源：http://zz.haigaiapp.cn

SELECT * FROM (
来源：http://aa.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hy.shxzskj.cn

) t WHERE rn = 1;
来源：http://rm.chemitech.net.cn

[Q35] 内连接
来源：http://ri.bookmarksfly.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uw.huixiangedu.cn

[Q36] 左连接
来源：http://ns.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vm.shxzukj.cn

[Q37] 右连接
来源：http://at.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lq.hnjuh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://uu.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xe.bjjhwx.cn

[Q39] 自连接（查上下级）
来源：http://nb.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kg.huixinmuqiang.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ye.yuexingan06.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wu.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ny.szxytkj.cn

[Q41] 多表连接
来源：http://mh.colortex.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tw.nicolike.cn

JOIN users u ON u.id = o.user_id
来源：http://mr.muxihuayi.cn

JOIN products p ON p.id = o.product_id;
来源：http://ho.asd995.cn

[Q42] 连接条件附加过滤
来源：http://hm.newstarts.cn

SELECT u.name, o.amount FROM users u
来源：http://vl.huixiangedu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xd.newstarts.cn

[Q43] 标量子查询
来源：http://xw.szxytkj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cb.asd995.cn

[Q44] IN 子查询
来源：http://my.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nt.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://io.panjiajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sh.chemitech.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ia.huixiangedu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nb.huixinmuqiang.cn

[Q47] 与平均值比较
来源：http://su.szxytkj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ue.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://je.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hn.panjiajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://tz.hnjuh.cn

[Q49] 更新单行
来源：http://jz.yuexingan06.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qj.colortex.cn

[Q50] 批量更新
来源：http://sp.huixinmuqiang.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cj.haigaiapp.cn

[Q51] 用子查询更新
来源：http://bw.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gd.jctech888.com.cn

[Q52] 删除指定行
来源：http://ae.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://hz.bjjhwx.cn

[Q53] 按条件删除
来源：http://am.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qd.huanxung.cn

[Q54] 清空表
来源：http://dn.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://db.shtwfgs.cn

[Q55] 排名（并列占位）
来源：http://hk.jianghongdianzi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jv.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://cv.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ai.nicolike.cn

[Q57] 行号
来源：http://of.nszjky.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xx.gzmigu.cn

[Q58] 累计求和
来源：http://pk.haigaiapp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wv.shxzukj.cn

[Q59] 分组内累计
来源：http://rn.colortex.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tv.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://qw.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ji.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ps.hahajie.cn

[Q61] 移动平均
来源：http://eg.bjjhwx.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://no.newstarts.cn

[Q62] 分组占比
来源：http://cx.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zl.colortex.cn

[Q63] 开启事务
来源：http://yb.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vf.szsharing.cn

[Q64] 提交事务
来源：http://jb.huixiangedu.cn

COMMIT;
来源：http://ab.bjjhwx.cn

[Q65] 回滚事务
来源：http://an.bjjhwx.cn

ROLLBACK;
来源：http://vv.lnxyls.cn

[Q66] 行锁查询
来源：http://cy.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tt.shxzskj.cn

[Q67] 设置隔离级别
来源：http://so.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://od.shxzskj.cn

[Q68] 保存点
来源：http://gn.gzmigu.cn

SAVEPOINT sp1;
来源：http://ta.yuexingan06.cn

ROLLBACK TO sp1;
来源：http://ea.huanxung.cn

[Q69] 查看执行计划
来源：http://xr.9csxet.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vu.newstarts.cn

[Q70] 更新统计信息
来源：http://go.shxzukj.cn

ANALYZE TABLE users;
来源：http://pl.huixiangedu.cn

[Q71] 查看建表语句
来源：http://ma.yuexingan06.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lb.newstarts.cn

[Q72] 查看索引
来源：http://zd.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://gj.wgjwhj.cn

[Q73] 查看表状态
来源：http://yz.huixiangedu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hh.huixiangedu.cn

[Q74] 强制使用索引
来源：http://qj.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tj.panjiajie.cn

[Q75] 日期格式化
来源：http://mv.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ex.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xz.gzmigu.cn

[Q76] 按天统计
来源：http://qw.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oz.9csxet.cn

[Q77] 时间加减
来源：http://sp.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kd.jctech888.com.cn

[Q78] 当前时间
来源：http://iw.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qc.muxihuayi.cn

[Q79] 字符串拼接
来源：http://sm.huanxung.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nc.chemitech.net.cn

[Q80] 字符串截取
来源：http://ei.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://am.shxzukj.cn

[Q81] 字符串替换
来源：http://fo.newstarts.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ha.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://na.szsharing.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pk.jctech888.com.cn

[Q83] 大小写转换
来源：http://lw.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ae.bjjhwx.cn

[Q84] 去除首尾空格
来源：http://ly.521024.cn

SELECT TRIM(name) FROM users;
来源：http://wk.shxzukj.cn

[Q85] 数值取整
来源：http://bn.colortex.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iq.hnjuh.cn

[Q86] 读取 JSON 字段
来源：http://sv.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vr.hahajie.cn

[Q87] JSON 字段做条件
来源：http://pv.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lx.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://pt.huixiangedu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pq.asd995.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tl.nicolike.cn

[Q89] 判断表是否存在
来源：http://cw.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rd.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://iz.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gk.shxzskj.cn

================================================================================
来源：http://us.szxytkj.cn

R. Bash 专题
来源：http://wj.shxzskj.cn

================================================================================
来源：http://hh.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://jt.nicolike.cn

#!/usr/bin/env bash
来源：http://tm.bookmarksfly.cn

set -euo pipefail
来源：http://rv.szxytkj.cn

[R02] 变量赋值与使用
来源：http://vq.szsharing.cn

name="Tom"; echo "$name"
来源：http://wl.chemitech.net.cn

[R03] 只读变量
来源：http://ms.9csxet.cn

readonly PI=3.14
来源：http://yn.muxihuayi.cn

[R04] 位置参数
来源：http://np.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kh.szxytkj.cn

[R05] 参数默认值
来源：http://ea.521024.cn

name="${1:-default}"
来源：http://tf.newstarts.cn

[R06] 判断命令是否存在
来源：http://iu.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ic.szsharing.cn

[R07] if 判断文件
来源：http://eg.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bp.nszjky.cn

[R08] 数值比较
来源：http://hq.gzmigu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wu.huixiangedu.cn

[R09] 字符串比较
来源：http://cv.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rn.shtwfgs.cn

[R10] 正则匹配
来源：http://cd.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uw.shxzskj.cn

[R11] case 多分支
来源：http://nw.nicolike.cn

case "$1" in
来源：http://sj.9csxet.cn

start) echo "启动" ;;
来源：http://ro.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://xc.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://av.shxzskj.cn

esac
来源：http://um.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://nl.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://bc.asd995.cn

[R13] for 计数循环
来源：http://qn.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://yu.hahajie.cn

[R14] C 风格 for
来源：http://rj.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rh.521024.cn

[R15] while 逐行读文件
来源：http://iy.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ny.shxzukj.cn

[R16] until 等待条件
来源：http://pl.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://db.jctech888.com.cn

[R17] 数组定义与取值
来源：http://tn.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cr.jianghongdianzi.cn

[R18] 遍历数组
来源：http://fr.hnjuh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ie.bookmarksfly.cn

[R19] 数组长度
来源：http://wb.9csxet.cn

echo "${#arr[@]}"
来源：http://xd.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://cb.nszjky.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yv.muxihuayi.cn

[R21] 字符串长度
来源：http://gh.haigaiapp.cn

echo "${#s}"
来源：http://wq.hnjuh.cn

[R22] 截取子串
来源：http://jw.asd995.cn

echo "${s:0:5}"
来源：http://en.yuexingan06.cn

[R23] 字符串替换
来源：http://uj.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vq.hnjuh.cn

[R24] 大小写转换
来源：http://nc.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hg.9csxet.cn

[R25] 去后缀 / 去前缀
来源：http://wh.szsharing.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hu.gzmigu.cn

[R26] 命令替换
来源：http://is.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://qo.newstarts.cn

[R27] 算术展开
来源：http://ly.huixinmuqiang.cn

echo $((1 + 2 * 3))
来源：http://mt.panjiajie.cn

[R28] 浮点运算
来源：http://nm.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://zm.nicolike.cn

[R29] 定义函数
来源：http://wf.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rx.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://tx.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://nt.nszjky.cn

[R31] 局部变量
来源：http://cd.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://fn.colortex.cn

[R32] 参数个数校验
来源：http://wq.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mo.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://bg.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vf.wgjwhj.cn

[R34] 退出时清理
来源：http://eq.yuntaijiaju.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dv.bookmarksfly.cn

[R35] 后台执行并等待
来源：http://uo.yuexingan06.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lo.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://uf.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fd.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://jv.panjiajie.cn

files=$(ls -1)
来源：http://we.newstarts.cn

[R38] 管道串联
来源：http://kp.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://ck.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://lk.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://le.newstarts.cn

[R40] 追加写日志
来源：http://zt.jianghongdianzi.cn

echo "log" >> out.log
来源：http://kk.panjiajie.cn

[R41] 丢弃输出
来源：http://oh.wgjwhj.cn

cmd >/dev/null 2>&1
来源：http://rk.bookmarksfly.cn

[R42] 输入重定向
来源：http://xr.newstarts.cn

wc -l < a.txt
来源：http://gz.chemitech.net.cn

[R43] 按名字查找文件
来源：http://zq.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://ah.panjiajie.cn

[R44] 按修改时间查找
来源：http://gp.9csxet.cn

find . -mtime -7 -type f
来源：http://tb.shtwfgs.cn

[R45] 批量删除
来源：http://yz.jianghongdianzi.cn

find . -name "*.tmp" -delete
来源：http://ad.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://er.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zv.muxihuayi.cn

[R47] sed 单行替换
来源：http://sw.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rn.bjjhwx.cn

[R48] awk 取指定列
来源：http://il.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://fh.jianghongdianzi.cn

[R49] awk 带条件
来源：http://nc.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pe.shxzskj.cn

[R50] awk 求和
来源：http://kh.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kz.haigaiapp.cn

[R51] 排序去重取前几
来源：http://uh.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ro.haigaiapp.cn

[R52] 统计行数
来源：http://es.jianghongdianzi.cn

wc -l a.txt
来源：http://ik.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://xq.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nz.szxytkj.cn

[R54] 比较两个文件
来源：http://oe.panjiajie.cn

diff a.txt b.txt
来源：http://vl.lnxyls.cn

[R55] 压缩与解压
来源：http://ab.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ts.hahajie.cn

[R56] 远程拷贝
来源：http://cn.asd995.cn

scp file user@host:/path/
来源：http://oq.wgjwhj.cn

[R57] 远程执行命令
来源：http://ut.asd995.cn

ssh user@host 'uptime'
来源：http://jk.shxzskj.cn

[R58] 下载文件
来源：http://zm.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mi.bjjhwx.cn

[R59] 发 POST JSON
来源：http://sc.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ie.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://om.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lj.muxihuayi.cn

[R61] 磁盘占用
来源：http://pm.jctech888.com.cn

df -h;  du -sh *
来源：http://kv.colortex.cn

[R62] 找最占空间的文件
来源：http://fr.asd995.cn

du -ah . | sort -rh | head -10
来源：http://wd.jctech888.com.cn

[R63] 内存与进程
来源：http://er.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://jb.shxzskj.cn

[R64] 结束进程
来源：http://xw.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://sz.jctech888.com.cn

[R65] 查看端口占用
来源：http://uz.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xm.wgjwhj.cn

[R66] 定时任务
来源：http://pv.lnxyls.cn

crontab -e;  crontab -l
来源：http://nu.szsharing.cn

[R67] 生成随机十六进制串
来源：http://ir.shxzukj.cn

openssl rand -hex 16
来源：http://ij.yuntaijiaju.cn

[R68] 计算文件校验值
来源：http://ex.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gg.szxytkj.cn

[R69] 生成随机密码
来源：http://jp.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://eg.huanxung.cn

[R70] 时间戳与互转
来源：http://di.hahajie.cn

date +%s;  date -d @1700000000
来源：http://ra.newstarts.cn

[R71] 日期格式化
来源：http://js.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pb.newstarts.cn

[R72] 等待端口就绪
来源：http://sg.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vf.szsharing.cn

[R73] 分割大日志
来源：http://ch.shxzskj.cn

split -l 1000 big.log part_
来源：http://pn.521024.cn

[R74] 批量重命名
来源：http://va.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kt.shxzukj.cn

[R75] 导出环境变量
来源：http://qh.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://px.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://me.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lg.panjiajie.cn

[R77] 读取用户输入
来源：http://fv.bjjhwx.cn

read -rp "请输入: " ans
来源：http://er.hahajie.cn

[R78] 交互式菜单
来源：http://pa.9csxet.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oy.newstarts.cn

[R79] 解析命令行选项
来源：http://qt.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://db.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://je.jctech888.com.cn

time ./run.sh
来源：http://dq.lnxyls.cn

================================================================================
来源：http://px.521024.cn


<!-- 参考信息 -->