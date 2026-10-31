代发 wailian999

[Q33] 多列分组
来源：http://ih.szxytkj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wv.bjjhwx.cn

[Q34] 每组取第一条
来源：http://za.jianghongdianzi.cn

SELECT * FROM (
来源：http://ar.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://di.huixinmuqiang.cn

) t WHERE rn = 1;
来源：http://vm.szxytkj.cn

[Q35] 内连接
来源：http://iu.bjjhwx.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jc.nicolike.cn

[Q36] 左连接
来源：http://ol.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wb.asd995.cn

[Q37] 右连接
来源：http://zw.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eq.yuntaijiaju.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dr.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xe.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://kz.hahajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://eq.yuntaijiaju.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tq.newstarts.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xp.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jg.wgjwhj.cn

[Q41] 多表连接
来源：http://tz.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yv.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://kf.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://uk.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://hb.hnjuh.cn

SELECT u.name, o.amount FROM users u
来源：http://bm.shxzukj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mm.panjiajie.cn

[Q43] 标量子查询
来源：http://xs.panjiajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yk.shtwfgs.cn

[Q44] IN 子查询
来源：http://qt.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xd.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://fa.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cp.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://in.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pq.chemitech.net.cn

[Q47] 与平均值比较
来源：http://zz.yuntaijiaju.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ko.yuntaijiaju.cn

[Q48] CTE 公用表表达式
来源：http://pn.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qt.jianghongdianzi.cn

SELECT * FROM t WHERE c > 5;
来源：http://fz.nszjky.cn

[Q49] 更新单行
来源：http://og.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ef.shtwfgs.cn

[Q50] 批量更新
来源：http://rm.colortex.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xd.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://bl.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ss.chemitech.net.cn

[Q52] 删除指定行
来源：http://gr.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://il.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://uc.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eq.lnxyls.cn

[Q54] 清空表
来源：http://uc.bookmarksfly.cn

TRUNCATE TABLE logs;
来源：http://ca.colortex.cn

[Q55] 排名（并列占位）
来源：http://wz.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jf.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://ck.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zn.lnxyls.cn

[Q57] 行号
来源：http://lj.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ff.newstarts.cn

[Q58] 累计求和
来源：http://oc.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://el.521024.cn

[Q59] 分组内累计
来源：http://sh.colortex.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cl.haigaiapp.cn

[Q60] 取上一行 / 下一行
来源：http://ci.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yd.haigaiapp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hq.gzmigu.cn

[Q61] 移动平均
来源：http://qc.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yi.szsharing.cn

[Q62] 分组占比
来源：http://yi.colortex.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://an.bjjhwx.cn

[Q63] 开启事务
来源：http://ij.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pe.wgjwhj.cn

[Q64] 提交事务
来源：http://wa.jianghongdianzi.cn

COMMIT;
来源：http://hx.huanxung.cn

[Q65] 回滚事务
来源：http://dq.jctech888.com.cn

ROLLBACK;
来源：http://gj.9csxet.cn

[Q66] 行锁查询
来源：http://yn.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ao.colortex.cn

[Q67] 设置隔离级别
来源：http://lm.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mj.lnxyls.cn

[Q68] 保存点
来源：http://sw.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://nv.521024.cn

ROLLBACK TO sp1;
来源：http://xi.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://va.huixinmuqiang.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lc.hnjuh.cn

[Q70] 更新统计信息
来源：http://md.521024.cn

ANALYZE TABLE users;
来源：http://zu.wgjwhj.cn

[Q71] 查看建表语句
来源：http://ev.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mi.shxzukj.cn

[Q72] 查看索引
来源：http://gn.nszjky.cn

SHOW INDEX FROM users;
来源：http://ey.9csxet.cn

[Q73] 查看表状态
来源：http://pl.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hg.szxytkj.cn

[Q74] 强制使用索引
来源：http://ml.huixiangedu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cw.shtwfgs.cn

[Q75] 日期格式化
来源：http://fb.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ab.asd995.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://il.muxihuayi.cn

[Q76] 按天统计
来源：http://pj.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tx.huanxung.cn

[Q77] 时间加减
来源：http://ev.gzmigu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nv.jctech888.com.cn

[Q78] 当前时间
来源：http://pj.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sv.haigaiapp.cn

[Q79] 字符串拼接
来源：http://gi.521024.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ry.shxzskj.cn

[Q80] 字符串截取
来源：http://xa.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iw.wgjwhj.cn

[Q81] 字符串替换
来源：http://cd.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yy.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://ua.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oc.jctech888.com.cn

[Q83] 大小写转换
来源：http://ev.yuexingan06.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eu.panjiajie.cn

[Q84] 去除首尾空格
来源：http://lp.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://oe.huixiangedu.cn

[Q85] 数值取整
来源：http://ax.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gs.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://qw.panjiajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tn.colortex.cn

[Q87] JSON 字段做条件
来源：http://td.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ua.hahajie.cn

[Q88] 行转列（条件聚合）
来源：http://bu.huixinmuqiang.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ci.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ky.colortex.cn

[Q89] 判断表是否存在
来源：http://jc.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cl.huixinmuqiang.cn

[Q90] 生成序号列
来源：http://av.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zq.jianghongdianzi.cn

================================================================================
来源：http://fo.huanxung.cn

R. Bash 专题
来源：http://zy.yuntaijiaju.cn

================================================================================
来源：http://ra.nicolike.cn

[R01] shebang 与严格模式
来源：http://dk.muxihuayi.cn

#!/usr/bin/env bash
来源：http://zq.nszjky.cn

set -euo pipefail
来源：http://re.hnjuh.cn

[R02] 变量赋值与使用
来源：http://hl.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://vm.lnxyls.cn

[R03] 只读变量
来源：http://ta.nicolike.cn

readonly PI=3.14
来源：http://cb.521024.cn

[R04] 位置参数
来源：http://vv.bjjhwx.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nk.hahajie.cn

[R05] 参数默认值
来源：http://xp.muxihuayi.cn

name="${1:-default}"
来源：http://uz.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://tf.jctech888.com.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pq.jctech888.com.cn

[R07] if 判断文件
来源：http://wb.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zy.szsharing.cn

[R08] 数值比较
来源：http://mv.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ga.gzmigu.cn

[R09] 字符串比较
来源：http://ni.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wb.haigaiapp.cn

[R10] 正则匹配
来源：http://vo.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rr.szsharing.cn

[R11] case 多分支
来源：http://ak.huixiangedu.cn

case "$1" in
来源：http://dg.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://le.hahajie.cn

stop)  echo "停止" ;;
来源：http://au.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://pe.szxytkj.cn

esac
来源：http://cc.panjiajie.cn

[R12] for 遍历文件
来源：http://mm.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://uh.bjjhwx.cn

[R13] for 计数循环
来源：http://ea.jianghongdianzi.cn

for i in {1..10}; do echo "$i"; done
来源：http://fm.haigaiapp.cn

[R14] C 风格 for
来源：http://np.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://we.gzmigu.cn

[R15] while 逐行读文件
来源：http://ub.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zi.panjiajie.cn

[R16] until 等待条件
来源：http://hy.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://se.yuntaijiaju.cn

[R17] 数组定义与取值
来源：http://yq.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kp.asd995.cn

[R18] 遍历数组
来源：http://bf.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ps.newstarts.cn

[R19] 数组长度
来源：http://lh.shtwfgs.cn

echo "${#arr[@]}"
来源：http://vn.shxzskj.cn

[R20] 关联数组（字典）
来源：http://dd.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zd.bjjhwx.cn

[R21] 字符串长度
来源：http://qf.huixinmuqiang.cn

echo "${#s}"
来源：http://gc.newstarts.cn

[R22] 截取子串
来源：http://zl.shxzukj.cn

echo "${s:0:5}"
来源：http://dh.asd995.cn

[R23] 字符串替换
来源：http://ds.521024.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ho.haigaiapp.cn

[R24] 大小写转换
来源：http://vz.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qd.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://zd.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://th.hnjuh.cn

[R26] 命令替换
来源：http://fy.szxytkj.cn

now=$(date +%F); echo "$now"
来源：http://fp.huixiangedu.cn

[R27] 算术展开
来源：http://fb.9csxet.cn

echo $((1 + 2 * 3))
来源：http://ka.panjiajie.cn

[R28] 浮点运算
来源：http://wm.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://fk.muxihuayi.cn

[R29] 定义函数
来源：http://dj.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ro.asd995.cn

[R30] 函数返回状态码
来源：http://hf.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://sp.521024.cn

[R31] 局部变量
来源：http://qy.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://rz.huanxung.cn

[R32] 参数个数校验
来源：http://ei.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qo.newstarts.cn

[R33] 捕获错误并提示行号
来源：http://aa.gzmigu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://va.huixinmuqiang.cn

[R34] 退出时清理
来源：http://uu.chemitech.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cp.huixiangedu.cn

[R35] 后台执行并等待
来源：http://ey.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://he.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://vn.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tz.521024.cn

[R37] 把输出赋给变量
来源：http://bz.yuntaijiaju.cn

files=$(ls -1)
来源：http://dn.shtwfgs.cn

[R38] 管道串联
来源：http://xm.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://lk.yuexingan06.cn

[R39] 重定向标准输出与错误
来源：http://eg.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://st.huixinmuqiang.cn

[R40] 追加写日志
来源：http://bu.nicolike.cn

echo "log" >> out.log
来源：http://ha.asd995.cn

[R41] 丢弃输出
来源：http://ag.newstarts.cn

cmd >/dev/null 2>&1
来源：http://pj.hahajie.cn

[R42] 输入重定向
来源：http://gg.gzmigu.cn

wc -l < a.txt
来源：http://zs.chemitech.net.cn

[R43] 按名字查找文件
来源：http://df.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://fg.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://uy.huixinmuqiang.cn

find . -mtime -7 -type f
来源：http://sc.nicolike.cn

[R45] 批量删除
来源：http://sb.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://ao.shxzukj.cn

[R46] 递归替换文件内容
来源：http://kh.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dd.wgjwhj.cn

[R47] sed 单行替换
来源：http://ls.shxzukj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dr.shtwfgs.cn

[R48] awk 取指定列
来源：http://lp.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://jh.szsharing.cn

[R49] awk 带条件
来源：http://ic.huixinmuqiang.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qz.yuntaijiaju.cn

[R50] awk 求和
来源：http://bi.bookmarksfly.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dl.chemitech.net.cn

[R51] 排序去重取前几
来源：http://rd.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hv.haigaiapp.cn

[R52] 统计行数
来源：http://pv.lnxyls.cn

wc -l a.txt
来源：http://lq.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://aj.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nw.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://nz.asd995.cn

diff a.txt b.txt
来源：http://rk.shtwfgs.cn

[R55] 压缩与解压
来源：http://zr.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tr.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://wg.huanxung.cn

scp file user@host:/path/
来源：http://eu.wgjwhj.cn

[R57] 远程执行命令
来源：http://xf.wgjwhj.cn

ssh user@host 'uptime'
来源：http://ud.jianghongdianzi.cn

[R58] 下载文件
来源：http://vt.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fz.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://sw.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ig.jctech888.com.cn

[R60] 只看 HTTP 状态码
来源：http://pq.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xw.shtwfgs.cn

[R61] 磁盘占用
来源：http://gn.muxihuayi.cn

df -h;  du -sh *
来源：http://nb.shxzskj.cn

[R62] 找最占空间的文件
来源：http://wp.colortex.cn

du -ah . | sort -rh | head -10
来源：http://iv.newstarts.cn

[R63] 内存与进程
来源：http://ce.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://ni.shtwfgs.cn

[R64] 结束进程
来源：http://ry.nicolike.cn

kill -9 $(pgrep -f app.py)
来源：http://pe.9csxet.cn

[R65] 查看端口占用
来源：http://jx.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lq.shxzukj.cn

[R66] 定时任务
来源：http://pz.newstarts.cn

crontab -e;  crontab -l
来源：http://ch.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://qy.huanxung.cn

openssl rand -hex 16
来源：http://rp.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://nc.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yy.hnjuh.cn

[R69] 生成随机密码
来源：http://ah.jctech888.com.cn

head -c 16 /dev/urandom | base64
来源：http://wm.huixiangedu.cn

[R70] 时间戳与互转
来源：http://gx.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://lu.huanxung.cn

[R71] 日期格式化
来源：http://id.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qy.nicolike.cn

[R72] 等待端口就绪
来源：http://mm.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nn.huixiangedu.cn

[R73] 分割大日志
来源：http://ta.shtwfgs.cn

split -l 1000 big.log part_
来源：http://il.shxzukj.cn

[R74] 批量重命名
来源：http://oz.jctech888.com.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sn.jctech888.com.cn

[R75] 导出环境变量
来源：http://sx.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://sh.shtwfgs.cn

[R76] 使用临时文件
来源：http://tq.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uk.nicolike.cn

[R77] 读取用户输入
来源：http://cr.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://lt.yuexingan06.cn

[R78] 交互式菜单
来源：http://rl.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ai.lnxyls.cn

[R79] 解析命令行选项
来源：http://lc.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ar.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://bi.nszjky.cn

time ./run.sh
来源：http://zc.hahajie.cn

================================================================================
来源：http://pl.asd995.cn

S. C / C++ 专题
来源：http://pj.szsharing.cn

================================================================================
来源：http://dm.yuntaijiaju.cn

[S01] C：Hello World
来源：http://br.huixiangedu.cn

#include <stdio.h>
来源：http://cu.hahajie.cn


<!-- 参考信息 -->