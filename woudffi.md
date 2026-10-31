代发 wailian999

[Q33] 多列分组
来源：http://rk.wgjwhj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qz.colortex.cn

[Q34] 每组取第一条
来源：http://cv.huixinmuqiang.cn

SELECT * FROM (
来源：http://ng.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ws.huixiangedu.cn

) t WHERE rn = 1;
来源：http://xu.shxzukj.cn

[Q35] 内连接
来源：http://pl.521024.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qx.huanxung.cn

[Q36] 左连接
来源：http://dp.jctech888.com.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ji.asd995.cn

[Q37] 右连接
来源：http://rm.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ed.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qz.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wu.jctech888.com.cn

[Q39] 自连接（查上下级）
来源：http://ac.jctech888.com.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kn.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pw.huixinmuqiang.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yn.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://un.gzmigu.cn

[Q41] 多表连接
来源：http://mw.jianghongdianzi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ih.haigaiapp.cn

JOIN users u ON u.id = o.user_id
来源：http://gp.jctech888.com.cn

JOIN products p ON p.id = o.product_id;
来源：http://jb.521024.cn

[Q42] 连接条件附加过滤
来源：http://jg.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://dd.muxihuayi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ci.shxzskj.cn

[Q43] 标量子查询
来源：http://qz.szsharing.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gh.newstarts.cn

[Q44] IN 子查询
来源：http://yi.huanxung.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yw.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://bs.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yt.asd995.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ff.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sz.shxzskj.cn

[Q47] 与平均值比较
来源：http://cw.szsharing.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ra.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://va.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gd.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://mm.asd995.cn

[Q49] 更新单行
来源：http://zy.panjiajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qm.jctech888.com.cn

[Q50] 批量更新
来源：http://wp.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://md.huanxung.cn

[Q51] 用子查询更新
来源：http://th.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lf.9csxet.cn

[Q52] 删除指定行
来源：http://qq.shtwfgs.cn

DELETE FROM users WHERE id = 10;
来源：http://my.huixinmuqiang.cn

[Q53] 按条件删除
来源：http://qb.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wt.huanxung.cn

[Q54] 清空表
来源：http://ph.bjjhwx.cn

TRUNCATE TABLE logs;
来源：http://yc.nicolike.cn

[Q55] 排名（并列占位）
来源：http://qc.lnxyls.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dk.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://jb.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://db.chemitech.net.cn

[Q57] 行号
来源：http://vk.jianghongdianzi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wl.jianghongdianzi.cn

[Q58] 累计求和
来源：http://tk.nszjky.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nt.nszjky.cn

[Q59] 分组内累计
来源：http://ji.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ml.gzmigu.cn

[Q60] 取上一行 / 下一行
来源：http://qc.shxzukj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vm.yuntaijiaju.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ec.gzmigu.cn

[Q61] 移动平均
来源：http://pt.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://li.huanxung.cn

[Q62] 分组占比
来源：http://nm.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pe.bjjhwx.cn

[Q63] 开启事务
来源：http://hj.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qu.yuntaijiaju.cn

[Q64] 提交事务
来源：http://qn.shxzukj.cn

COMMIT;
来源：http://mo.szsharing.cn

[Q65] 回滚事务
来源：http://zd.huanxung.cn

ROLLBACK;
来源：http://ok.huixiangedu.cn

[Q66] 行锁查询
来源：http://dm.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yx.shxzukj.cn

[Q67] 设置隔离级别
来源：http://iy.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fp.jctech888.com.cn

[Q68] 保存点
来源：http://vy.szxytkj.cn

SAVEPOINT sp1;
来源：http://iz.shtwfgs.cn

ROLLBACK TO sp1;
来源：http://pg.asd995.cn

[Q69] 查看执行计划
来源：http://wm.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wz.jianghongdianzi.cn

[Q70] 更新统计信息
来源：http://rx.jctech888.com.cn

ANALYZE TABLE users;
来源：http://od.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://qy.jianghongdianzi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uy.huanxung.cn

[Q72] 查看索引
来源：http://ux.huanxung.cn

SHOW INDEX FROM users;
来源：http://le.chemitech.net.cn

[Q73] 查看表状态
来源：http://zo.haigaiapp.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gz.nicolike.cn

[Q74] 强制使用索引
来源：http://pb.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lf.yuexingan06.cn

[Q75] 日期格式化
来源：http://td.jctech888.com.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://md.huanxung.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lh.szxytkj.cn

[Q76] 按天统计
来源：http://ii.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ve.jianghongdianzi.cn

[Q77] 时间加减
来源：http://bo.9csxet.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sh.521024.cn

[Q78] 当前时间
来源：http://tz.gzmigu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mg.shxzukj.cn

[Q79] 字符串拼接
来源：http://rn.huanxung.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tz.newstarts.cn

[Q80] 字符串截取
来源：http://pb.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hj.nszjky.cn

[Q81] 字符串替换
来源：http://dk.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oe.lnxyls.cn

[Q82] 字符长度与字节长度
来源：http://hu.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ex.wgjwhj.cn

[Q83] 大小写转换
来源：http://xm.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nn.yuntaijiaju.cn

[Q84] 去除首尾空格
来源：http://eo.newstarts.cn

SELECT TRIM(name) FROM users;
来源：http://fz.bjjhwx.cn

[Q85] 数值取整
来源：http://xq.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mw.newstarts.cn

[Q86] 读取 JSON 字段
来源：http://xj.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wj.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://vm.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yu.521024.cn

[Q88] 行转列（条件聚合）
来源：http://un.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jd.newstarts.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rj.bjjhwx.cn

[Q89] 判断表是否存在
来源：http://jx.521024.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vo.nicolike.cn

[Q90] 生成序号列
来源：http://rp.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dg.panjiajie.cn

================================================================================
来源：http://eg.asd995.cn

R. Bash 专题
来源：http://fn.chemitech.net.cn

================================================================================
来源：http://yp.hahajie.cn

[R01] shebang 与严格模式
来源：http://fg.hnjuh.cn

#!/usr/bin/env bash
来源：http://we.yuntaijiaju.cn

set -euo pipefail
来源：http://hg.colortex.cn

[R02] 变量赋值与使用
来源：http://dz.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://lv.asd995.cn

[R03] 只读变量
来源：http://qz.huixiangedu.cn

readonly PI=3.14
来源：http://cu.nszjky.cn

[R04] 位置参数
来源：http://vk.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pz.panjiajie.cn

[R05] 参数默认值
来源：http://yq.hnjuh.cn

name="${1:-default}"
来源：http://wb.shxzukj.cn

[R06] 判断命令是否存在
来源：http://qw.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ys.jctech888.com.cn

[R07] if 判断文件
来源：http://qk.chemitech.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ly.bookmarksfly.cn

[R08] 数值比较
来源：http://dz.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bw.newstarts.cn

[R09] 字符串比较
来源：http://oq.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zr.huixiangedu.cn

[R10] 正则匹配
来源：http://kz.yuntaijiaju.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nj.hnjuh.cn

[R11] case 多分支
来源：http://io.wgjwhj.cn

case "$1" in
来源：http://ns.shxzukj.cn

start) echo "启动" ;;
来源：http://lp.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://hl.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://ws.lnxyls.cn

esac
来源：http://cg.muxihuayi.cn

[R12] for 遍历文件
来源：http://mp.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://ar.521024.cn

[R13] for 计数循环
来源：http://ep.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://fn.bookmarksfly.cn

[R14] C 风格 for
来源：http://li.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wf.nszjky.cn

[R15] while 逐行读文件
来源：http://tc.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rr.colortex.cn

[R16] until 等待条件
来源：http://ar.bjjhwx.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ax.bjjhwx.cn

[R17] 数组定义与取值
来源：http://ka.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nv.shxzskj.cn

[R18] 遍历数组
来源：http://oh.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qv.hahajie.cn

[R19] 数组长度
来源：http://ph.colortex.cn

echo "${#arr[@]}"
来源：http://jq.panjiajie.cn

[R20] 关联数组（字典）
来源：http://gy.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gh.asd995.cn

[R21] 字符串长度
来源：http://wa.hnjuh.cn

echo "${#s}"
来源：http://it.panjiajie.cn

[R22] 截取子串
来源：http://bm.szxytkj.cn

echo "${s:0:5}"
来源：http://un.muxihuayi.cn

[R23] 字符串替换
来源：http://fl.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sp.huixiangedu.cn

[R24] 大小写转换
来源：http://wh.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hk.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://fc.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ot.gzmigu.cn

[R26] 命令替换
来源：http://jw.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://ej.jianghongdianzi.cn

[R27] 算术展开
来源：http://dl.yuntaijiaju.cn

echo $((1 + 2 * 3))
来源：http://nx.wgjwhj.cn

[R28] 浮点运算
来源：http://bg.newstarts.cn

echo "scale=2; 10/3" | bc
来源：http://gf.yuexingan06.cn

[R29] 定义函数
来源：http://up.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://um.shtwfgs.cn

[R30] 函数返回状态码
来源：http://cg.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://tl.yuexingan06.cn

[R31] 局部变量
来源：http://ws.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://zv.bookmarksfly.cn

[R32] 参数个数校验
来源：http://ea.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rw.jctech888.com.cn

[R33] 捕获错误并提示行号
来源：http://yg.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bq.szsharing.cn

[R34] 退出时清理
来源：http://vb.yuexingan06.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yw.nicolike.cn

[R35] 后台执行并等待
来源：http://sz.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rh.nszjky.cn

[R36] 并发执行多个任务
来源：http://cw.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yj.huanxung.cn

[R37] 把输出赋给变量
来源：http://rz.hnjuh.cn

files=$(ls -1)
来源：http://be.9csxet.cn

[R38] 管道串联
来源：http://wu.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://lu.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://dk.yuexingan06.cn

cmd > out.log 2>&1
来源：http://tz.szsharing.cn

[R40] 追加写日志
来源：http://vo.newstarts.cn

echo "log" >> out.log
来源：http://st.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://ek.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://hp.nszjky.cn

[R42] 输入重定向
来源：http://mm.haigaiapp.cn

wc -l < a.txt
来源：http://yp.shtwfgs.cn

[R43] 按名字查找文件
来源：http://me.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://xb.chemitech.net.cn

[R44] 按修改时间查找
来源：http://cl.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://dj.521024.cn

[R45] 批量删除
来源：http://vk.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://oy.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://sg.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zm.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://ey.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xa.lnxyls.cn

[R48] awk 取指定列
来源：http://py.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://mc.wgjwhj.cn

[R49] awk 带条件
来源：http://sh.wgjwhj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://my.huixinmuqiang.cn

[R50] awk 求和
来源：http://vy.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://db.muxihuayi.cn

[R51] 排序去重取前几
来源：http://nc.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://iw.colortex.cn

[R52] 统计行数
来源：http://mh.chemitech.net.cn

wc -l a.txt
来源：http://wp.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://cr.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dt.panjiajie.cn

[R54] 比较两个文件
来源：http://vm.bookmarksfly.cn

diff a.txt b.txt
来源：http://nb.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://ea.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ci.colortex.cn

[R56] 远程拷贝
来源：http://hi.yuexingan06.cn

scp file user@host:/path/
来源：http://vt.szxytkj.cn

[R57] 远程执行命令
来源：http://ge.nszjky.cn

ssh user@host 'uptime'
来源：http://bm.nszjky.cn

[R58] 下载文件
来源：http://bb.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vt.9csxet.cn

[R59] 发 POST JSON
来源：http://cx.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xb.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://zs.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kr.haigaiapp.cn

[R61] 磁盘占用
来源：http://ia.wgjwhj.cn

df -h;  du -sh *
来源：http://wi.colortex.cn

[R62] 找最占空间的文件
来源：http://cf.521024.cn

du -ah . | sort -rh | head -10
来源：http://el.newstarts.cn

[R63] 内存与进程
来源：http://gm.521024.cn

free -h;  ps aux | grep nginx
来源：http://vr.bjjhwx.cn

[R64] 结束进程
来源：http://xx.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://bs.nicolike.cn

[R65] 查看端口占用
来源：http://eo.szxytkj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ml.yuexingan06.cn

[R66] 定时任务
来源：http://st.shxzskj.cn

crontab -e;  crontab -l
来源：http://vn.9csxet.cn

[R67] 生成随机十六进制串
来源：http://db.panjiajie.cn

openssl rand -hex 16
来源：http://yj.nicolike.cn

[R68] 计算文件校验值
来源：http://gi.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kf.newstarts.cn

[R69] 生成随机密码
来源：http://pg.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://yz.hnjuh.cn

[R70] 时间戳与互转
来源：http://ji.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://vi.colortex.cn

[R71] 日期格式化
来源：http://dq.jianghongdianzi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yt.shxzukj.cn

[R72] 等待端口就绪
来源：http://mo.yuexingan06.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ji.haigaiapp.cn

[R73] 分割大日志
来源：http://cf.nicolike.cn

split -l 1000 big.log part_
来源：http://jr.shxzskj.cn

[R74] 批量重命名
来源：http://rr.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vi.shxzukj.cn

[R75] 导出环境变量
来源：http://tr.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://tc.nicolike.cn

[R76] 使用临时文件
来源：http://xq.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oh.lnxyls.cn

[R77] 读取用户输入
来源：http://io.jctech888.com.cn

read -rp "请输入: " ans
来源：http://ni.nicolike.cn

[R78] 交互式菜单
来源：http://ui.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ie.newstarts.cn

[R79] 解析命令行选项
来源：http://va.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qx.asd995.cn

[R80] 查看脚本执行耗时
来源：http://kg.521024.cn

time ./run.sh
来源：http://xy.9csxet.cn

================================================================================
来源：http://rd.gzmigu.cn

S. C / C++ 专题
来源：http://fa.colortex.cn

================================================================================
来源：http://jp.9csxet.cn

[S01] C：Hello World
来源：http://kz.asd995.cn

#include <stdio.h>
来源：http://rq.shxzukj.cn


<!-- 参考信息 -->