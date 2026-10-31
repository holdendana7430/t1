代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jm.gzmigu.cn

) t WHERE rn = 1;
来源：http://pp.newstarts.cn

[Q35] 内连接
来源：http://fr.jctech888.com.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://re.9csxet.cn

[Q36] 左连接
来源：http://mm.huixiangedu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jo.asd995.cn

[Q37] 右连接
来源：http://qq.hahajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tj.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://me.lnxyls.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eg.jianghongdianzi.cn

[Q39] 自连接（查上下级）
来源：http://lo.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hd.huanxung.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://li.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pa.newstarts.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ox.gzmigu.cn

[Q41] 多表连接
来源：http://nc.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ma.9csxet.cn

JOIN users u ON u.id = o.user_id
来源：http://dc.yuexingan06.cn

JOIN products p ON p.id = o.product_id;
来源：http://rf.colortex.cn

[Q42] 连接条件附加过滤
来源：http://su.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://mb.huanxung.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://os.colortex.cn

[Q43] 标量子查询
来源：http://yc.hnjuh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lp.hahajie.cn

[Q44] IN 子查询
来源：http://my.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uh.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://eg.bjjhwx.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kh.hnjuh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yj.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bw.huixiangedu.cn

[Q47] 与平均值比较
来源：http://yy.yuexingan06.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xk.nszjky.cn

[Q48] CTE 公用表表达式
来源：http://qq.jianghongdianzi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pm.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://tu.shxzukj.cn

[Q49] 更新单行
来源：http://jq.bookmarksfly.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ry.9csxet.cn

[Q50] 批量更新
来源：http://zj.huixinmuqiang.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lq.panjiajie.cn

[Q51] 用子查询更新
来源：http://ng.wgjwhj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wc.szsharing.cn

[Q52] 删除指定行
来源：http://tf.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://as.wgjwhj.cn

[Q53] 按条件删除
来源：http://iy.9csxet.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ev.nszjky.cn

[Q54] 清空表
来源：http://vl.gzmigu.cn

TRUNCATE TABLE logs;
来源：http://lf.colortex.cn

[Q55] 排名（并列占位）
来源：http://ti.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dy.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://ly.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fy.muxihuayi.cn

[Q57] 行号
来源：http://rn.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ql.wgjwhj.cn

[Q58] 累计求和
来源：http://qn.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sb.wgjwhj.cn

[Q59] 分组内累计
来源：http://py.huixiangedu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://no.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://ss.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xn.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uw.nszjky.cn

[Q61] 移动平均
来源：http://iy.colortex.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rp.newstarts.cn

[Q62] 分组占比
来源：http://yq.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jp.shxzukj.cn

[Q63] 开启事务
来源：http://yg.yuexingan06.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sm.yuexingan06.cn

[Q64] 提交事务
来源：http://yq.jianghongdianzi.cn

COMMIT;
来源：http://iy.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://yy.newstarts.cn

ROLLBACK;
来源：http://ax.newstarts.cn

[Q66] 行锁查询
来源：http://pe.9csxet.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ok.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://oy.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://je.wgjwhj.cn

[Q68] 保存点
来源：http://kj.wgjwhj.cn

SAVEPOINT sp1;
来源：http://he.huixinmuqiang.cn

ROLLBACK TO sp1;
来源：http://xz.hahajie.cn

[Q69] 查看执行计划
来源：http://tp.szsharing.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pj.shtwfgs.cn

[Q70] 更新统计信息
来源：http://at.hahajie.cn

ANALYZE TABLE users;
来源：http://dv.asd995.cn

[Q71] 查看建表语句
来源：http://lm.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oz.bookmarksfly.cn

[Q72] 查看索引
来源：http://gs.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://hz.chemitech.net.cn

[Q73] 查看表状态
来源：http://wq.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gg.jctech888.com.cn

[Q74] 强制使用索引
来源：http://if.shtwfgs.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kf.gzmigu.cn

[Q75] 日期格式化
来源：http://vh.nicolike.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dq.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://np.gzmigu.cn

[Q76] 按天统计
来源：http://dw.colortex.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pt.szsharing.cn

[Q77] 时间加减
来源：http://ci.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cn.szxytkj.cn

[Q78] 当前时间
来源：http://hw.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nl.wgjwhj.cn

[Q79] 字符串拼接
来源：http://ci.asd995.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xu.nicolike.cn

[Q80] 字符串截取
来源：http://na.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ep.shtwfgs.cn

[Q81] 字符串替换
来源：http://oo.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rw.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://fd.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xq.nicolike.cn

[Q83] 大小写转换
来源：http://qf.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lv.lnxyls.cn

[Q84] 去除首尾空格
来源：http://mb.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://eh.shxzskj.cn

[Q85] 数值取整
来源：http://hh.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xd.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://ws.chemitech.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yh.shxzukj.cn

[Q87] JSON 字段做条件
来源：http://xn.nszjky.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hn.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://mw.huixinmuqiang.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vf.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bg.szxytkj.cn

[Q89] 判断表是否存在
来源：http://yk.haigaiapp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://py.shxzskj.cn

[Q90] 生成序号列
来源：http://gj.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://su.huixiangedu.cn

================================================================================
来源：http://tb.colortex.cn

R. Bash 专题
来源：http://en.jctech888.com.cn

================================================================================
来源：http://ly.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://zo.huixinmuqiang.cn

#!/usr/bin/env bash
来源：http://wy.shxzukj.cn

set -euo pipefail
来源：http://iu.muxihuayi.cn

[R02] 变量赋值与使用
来源：http://qu.huanxung.cn

name="Tom"; echo "$name"
来源：http://vw.shtwfgs.cn

[R03] 只读变量
来源：http://tx.nszjky.cn

readonly PI=3.14
来源：http://cz.lnxyls.cn

[R04] 位置参数
来源：http://cf.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sl.shtwfgs.cn

[R05] 参数默认值
来源：http://fe.hnjuh.cn

name="${1:-default}"
来源：http://vf.9csxet.cn

[R06] 判断命令是否存在
来源：http://ox.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ub.jctech888.com.cn

[R07] if 判断文件
来源：http://yj.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dr.9csxet.cn

[R08] 数值比较
来源：http://sb.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ap.yuexingan06.cn

[R09] 字符串比较
来源：http://bg.lnxyls.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ab.asd995.cn

[R10] 正则匹配
来源：http://xk.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ad.szsharing.cn

[R11] case 多分支
来源：http://bw.bookmarksfly.cn

case "$1" in
来源：http://oe.wgjwhj.cn

start) echo "启动" ;;
来源：http://ah.panjiajie.cn

stop)  echo "停止" ;;
来源：http://qv.shtwfgs.cn

*)     echo "未知命令" ;;
来源：http://zv.muxihuayi.cn

esac
来源：http://dw.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://op.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://oh.gzmigu.cn

[R13] for 计数循环
来源：http://wh.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://pz.wgjwhj.cn

[R14] C 风格 for
来源：http://bl.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tj.wgjwhj.cn

[R15] while 逐行读文件
来源：http://jo.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yb.nicolike.cn

[R16] until 等待条件
来源：http://hj.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hd.newstarts.cn

[R17] 数组定义与取值
来源：http://gc.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ri.shxzskj.cn

[R18] 遍历数组
来源：http://qk.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zz.yuntaijiaju.cn

[R19] 数组长度
来源：http://jk.hahajie.cn

echo "${#arr[@]}"
来源：http://er.asd995.cn

[R20] 关联数组（字典）
来源：http://uf.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://py.panjiajie.cn

[R21] 字符串长度
来源：http://qv.bjjhwx.cn

echo "${#s}"
来源：http://os.wgjwhj.cn

[R22] 截取子串
来源：http://fy.asd995.cn

echo "${s:0:5}"
来源：http://kh.jianghongdianzi.cn

[R23] 字符串替换
来源：http://dz.yuexingan06.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mz.huanxung.cn

[R24] 大小写转换
来源：http://bi.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://am.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://td.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ys.gzmigu.cn

[R26] 命令替换
来源：http://tk.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://th.nicolike.cn

[R27] 算术展开
来源：http://ke.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://lp.jianghongdianzi.cn

[R28] 浮点运算
来源：http://lg.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://lq.521024.cn

[R29] 定义函数
来源：http://po.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nd.nszjky.cn

[R30] 函数返回状态码
来源：http://xl.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://tv.huanxung.cn

[R31] 局部变量
来源：http://ep.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://nb.hnjuh.cn

[R32] 参数个数校验
来源：http://gd.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jb.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://es.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://en.nicolike.cn

[R34] 退出时清理
来源：http://uh.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xr.colortex.cn

[R35] 后台执行并等待
来源：http://eg.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tj.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://si.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ad.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://ol.colortex.cn

files=$(ls -1)
来源：http://fc.hnjuh.cn

[R38] 管道串联
来源：http://nq.hnjuh.cn

cat a.txt | grep -i error | wc -l
来源：http://xd.jctech888.com.cn

[R39] 重定向标准输出与错误
来源：http://sq.asd995.cn

cmd > out.log 2>&1
来源：http://za.shtwfgs.cn

[R40] 追加写日志
来源：http://nd.bjjhwx.cn

echo "log" >> out.log
来源：http://md.colortex.cn

[R41] 丢弃输出
来源：http://cw.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://yn.asd995.cn

[R42] 输入重定向
来源：http://jh.lnxyls.cn

wc -l < a.txt
来源：http://lx.huixiangedu.cn

[R43] 按名字查找文件
来源：http://xl.haigaiapp.cn

find . -name "*.log" -type f
来源：http://lr.521024.cn

[R44] 按修改时间查找
来源：http://aa.9csxet.cn

find . -mtime -7 -type f
来源：http://pu.bookmarksfly.cn

[R45] 批量删除
来源：http://tp.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://ce.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://gg.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dr.nszjky.cn

[R47] sed 单行替换
来源：http://aw.shxzukj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qe.nicolike.cn

[R48] awk 取指定列
来源：http://do.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://wi.9csxet.cn

[R49] awk 带条件
来源：http://qk.asd995.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ry.hahajie.cn

[R50] awk 求和
来源：http://qf.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qq.huanxung.cn

[R51] 排序去重取前几
来源：http://iw.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://va.panjiajie.cn

[R52] 统计行数
来源：http://eu.chemitech.net.cn

wc -l a.txt
来源：http://uq.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://mx.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pc.bjjhwx.cn

[R54] 比较两个文件
来源：http://lf.yuntaijiaju.cn

diff a.txt b.txt
来源：http://fe.jianghongdianzi.cn

[R55] 压缩与解压
来源：http://io.jctech888.com.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fy.szsharing.cn

[R56] 远程拷贝
来源：http://tm.muxihuayi.cn

scp file user@host:/path/
来源：http://gm.chemitech.net.cn

[R57] 远程执行命令
来源：http://ip.szxytkj.cn

ssh user@host 'uptime'
来源：http://dp.colortex.cn

[R58] 下载文件
来源：http://qz.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zt.yuexingan06.cn

[R59] 发 POST JSON
来源：http://tw.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ph.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://ft.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bx.wgjwhj.cn

[R61] 磁盘占用
来源：http://kt.hahajie.cn

df -h;  du -sh *
来源：http://kf.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://kg.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://wy.colortex.cn

[R63] 内存与进程
来源：http://dt.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://pg.bookmarksfly.cn

[R64] 结束进程
来源：http://my.nicolike.cn

kill -9 $(pgrep -f app.py)
来源：http://jt.gzmigu.cn

[R65] 查看端口占用
来源：http://nz.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bu.nszjky.cn

[R66] 定时任务
来源：http://cx.jctech888.com.cn

crontab -e;  crontab -l
来源：http://fw.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://bq.bjjhwx.cn

openssl rand -hex 16
来源：http://xw.hahajie.cn

[R68] 计算文件校验值
来源：http://sz.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vr.bjjhwx.cn

[R69] 生成随机密码
来源：http://lk.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://ob.bjjhwx.cn

[R70] 时间戳与互转
来源：http://at.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://to.bjjhwx.cn

[R71] 日期格式化
来源：http://mt.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zj.huixinmuqiang.cn

[R72] 等待端口就绪
来源：http://gb.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wj.521024.cn

[R73] 分割大日志
来源：http://tm.nszjky.cn

split -l 1000 big.log part_
来源：http://ok.huanxung.cn

[R74] 批量重命名
来源：http://ch.jctech888.com.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kr.jianghongdianzi.cn

[R75] 导出环境变量
来源：http://ww.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://ex.hahajie.cn

[R76] 使用临时文件
来源：http://pn.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rz.colortex.cn

[R77] 读取用户输入
来源：http://nl.nszjky.cn

read -rp "请输入: " ans
来源：http://kh.szsharing.cn

[R78] 交互式菜单
来源：http://xa.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hd.nszjky.cn

[R79] 解析命令行选项
来源：http://mg.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pk.9csxet.cn

[R80] 查看脚本执行耗时
来源：http://gm.muxihuayi.cn

time ./run.sh
来源：http://mo.nicolike.cn

================================================================================
来源：http://si.muxihuayi.cn

S. C / C++ 专题
来源：http://ey.shtwfgs.cn

================================================================================
来源：http://md.newstarts.cn

[S01] C：Hello World
来源：http://xd.szsharing.cn

#include <stdio.h>
来源：http://qq.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qz.huanxung.cn

[S02] C：变量与格式化输出
来源：http://px.wgjwhj.cn

int a = 10; printf("%d\n", a);
来源：http://kv.huixinmuqiang.cn

[S03] C：读入整数
来源：http://oo.bookmarksfly.cn


<!-- 参考信息 -->