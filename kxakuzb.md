代发 wailian999

[Q36] 左连接
来源：http://tv.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://td.szxytkj.cn

[Q37] 右连接
来源：http://iq.bookmarksfly.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wo.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hi.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tp.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://lp.jctech888.com.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kg.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nw.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lg.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fm.wgjwhj.cn

[Q41] 多表连接
来源：http://rd.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ft.huixiangedu.cn

JOIN users u ON u.id = o.user_id
来源：http://dg.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://kl.szxytkj.cn

[Q42] 连接条件附加过滤
来源：http://pi.chemitech.net.cn

SELECT u.name, o.amount FROM users u
来源：http://zs.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tp.jianghongdianzi.cn

[Q43] 标量子查询
来源：http://yn.wgjwhj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ww.chemitech.net.cn

[Q44] IN 子查询
来源：http://sy.szxytkj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wx.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://qx.newstarts.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pt.521024.cn

[Q46] NOT EXISTS 判断不存在
来源：http://iq.9csxet.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jl.haigaiapp.cn

[Q47] 与平均值比较
来源：http://za.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hd.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://ws.521024.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tl.shxzukj.cn

SELECT * FROM t WHERE c > 5;
来源：http://ic.jctech888.com.cn

[Q49] 更新单行
来源：http://pf.shtwfgs.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rr.huixiangedu.cn

[Q50] 批量更新
来源：http://vd.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qp.asd995.cn

[Q51] 用子查询更新
来源：http://ot.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sp.hnjuh.cn

[Q52] 删除指定行
来源：http://xl.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://hn.newstarts.cn

[Q53] 按条件删除
来源：http://oj.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://be.panjiajie.cn

[Q54] 清空表
来源：http://wq.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://px.haigaiapp.cn

[Q55] 排名（并列占位）
来源：http://kx.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cn.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://lb.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://po.9csxet.cn

[Q57] 行号
来源：http://yi.hnjuh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ms.521024.cn

[Q58] 累计求和
来源：http://nb.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wy.panjiajie.cn

[Q59] 分组内累计
来源：http://nr.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uk.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://iw.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yb.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bc.wgjwhj.cn

[Q61] 移动平均
来源：http://xj.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fr.hahajie.cn

[Q62] 分组占比
来源：http://eq.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ei.gzmigu.cn

[Q63] 开启事务
来源：http://jw.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rk.bookmarksfly.cn

[Q64] 提交事务
来源：http://qw.haigaiapp.cn

COMMIT;
来源：http://pn.panjiajie.cn

[Q65] 回滚事务
来源：http://ga.bjjhwx.cn

ROLLBACK;
来源：http://nl.shxzukj.cn

[Q66] 行锁查询
来源：http://of.9csxet.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ue.newstarts.cn

[Q67] 设置隔离级别
来源：http://qy.nszjky.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jf.haigaiapp.cn

[Q68] 保存点
来源：http://lb.haigaiapp.cn

SAVEPOINT sp1;
来源：http://be.szxytkj.cn

ROLLBACK TO sp1;
来源：http://yf.nszjky.cn

[Q69] 查看执行计划
来源：http://ph.wgjwhj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tv.asd995.cn

[Q70] 更新统计信息
来源：http://ed.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://mb.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://su.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ri.newstarts.cn

[Q72] 查看索引
来源：http://zs.521024.cn

SHOW INDEX FROM users;
来源：http://nh.bookmarksfly.cn

[Q73] 查看表状态
来源：http://oj.huixiangedu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://db.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://gn.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bv.jctech888.com.cn

[Q75] 日期格式化
来源：http://zm.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ps.szxytkj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://si.szxytkj.cn

[Q76] 按天统计
来源：http://su.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vk.nicolike.cn

[Q77] 时间加减
来源：http://ep.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mf.jctech888.com.cn

[Q78] 当前时间
来源：http://ml.yuexingan06.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gi.bjjhwx.cn

[Q79] 字符串拼接
来源：http://xm.9csxet.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kr.huixiangedu.cn

[Q80] 字符串截取
来源：http://mm.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://de.panjiajie.cn

[Q81] 字符串替换
来源：http://ce.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qu.521024.cn

[Q82] 字符长度与字节长度
来源：http://ew.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ig.hnjuh.cn

[Q83] 大小写转换
来源：http://qd.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ve.9csxet.cn

[Q84] 去除首尾空格
来源：http://iw.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://mi.hnjuh.cn

[Q85] 数值取整
来源：http://dx.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://li.szxytkj.cn

[Q86] 读取 JSON 字段
来源：http://my.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mn.huanxung.cn

[Q87] JSON 字段做条件
来源：http://nk.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qe.9csxet.cn

[Q88] 行转列（条件聚合）
来源：http://qv.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://si.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fr.colortex.cn

[Q89] 判断表是否存在
来源：http://nl.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bk.wgjwhj.cn

[Q90] 生成序号列
来源：http://ov.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mj.asd995.cn

================================================================================
来源：http://lo.yuexingan06.cn

R. Bash 专题
来源：http://nf.bookmarksfly.cn

================================================================================
来源：http://fw.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://yr.huixiangedu.cn

#!/usr/bin/env bash
来源：http://bb.jctech888.com.cn

set -euo pipefail
来源：http://ou.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://pg.newstarts.cn

name="Tom"; echo "$name"
来源：http://ec.nicolike.cn

[R03] 只读变量
来源：http://yz.bookmarksfly.cn

readonly PI=3.14
来源：http://fp.wgjwhj.cn

[R04] 位置参数
来源：http://xa.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pk.nszjky.cn

[R05] 参数默认值
来源：http://bi.szxytkj.cn

name="${1:-default}"
来源：http://zf.szxytkj.cn

[R06] 判断命令是否存在
来源：http://dh.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fq.nicolike.cn

[R07] if 判断文件
来源：http://jh.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hd.9csxet.cn

[R08] 数值比较
来源：http://lj.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://te.9csxet.cn

[R09] 字符串比较
来源：http://xr.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sq.yuntaijiaju.cn

[R10] 正则匹配
来源：http://eo.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cz.huixiangedu.cn

[R11] case 多分支
来源：http://ho.gzmigu.cn

case "$1" in
来源：http://uv.shtwfgs.cn

start) echo "启动" ;;
来源：http://mn.huanxung.cn

stop)  echo "停止" ;;
来源：http://ks.asd995.cn

*)     echo "未知命令" ;;
来源：http://cz.colortex.cn

esac
来源：http://le.bjjhwx.cn

[R12] for 遍历文件
来源：http://aq.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://xz.shxzskj.cn

[R13] for 计数循环
来源：http://yt.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://yj.nszjky.cn

[R14] C 风格 for
来源：http://ow.hahajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://df.shxzskj.cn

[R15] while 逐行读文件
来源：http://uz.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qs.shtwfgs.cn

[R16] until 等待条件
来源：http://rx.nszjky.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://py.wgjwhj.cn

[R17] 数组定义与取值
来源：http://ba.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kw.huanxung.cn

[R18] 遍历数组
来源：http://ip.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ng.huanxung.cn

[R19] 数组长度
来源：http://mo.jianghongdianzi.cn

echo "${#arr[@]}"
来源：http://tk.hnjuh.cn

[R20] 关联数组（字典）
来源：http://kj.bookmarksfly.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uy.jctech888.com.cn

[R21] 字符串长度
来源：http://tf.lnxyls.cn

echo "${#s}"
来源：http://qf.panjiajie.cn

[R22] 截取子串
来源：http://cg.wgjwhj.cn

echo "${s:0:5}"
来源：http://xg.521024.cn

[R23] 字符串替换
来源：http://wh.asd995.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sh.szxytkj.cn

[R24] 大小写转换
来源：http://of.szxytkj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hh.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://hr.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lt.muxihuayi.cn

[R26] 命令替换
来源：http://ou.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://hx.jctech888.com.cn

[R27] 算术展开
来源：http://qv.yuntaijiaju.cn

echo $((1 + 2 * 3))
来源：http://vs.nicolike.cn

[R28] 浮点运算
来源：http://az.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://ge.shtwfgs.cn

[R29] 定义函数
来源：http://xi.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rk.szsharing.cn

[R30] 函数返回状态码
来源：http://ji.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://rw.wgjwhj.cn

[R31] 局部变量
来源：http://tt.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://ib.asd995.cn

[R32] 参数个数校验
来源：http://gd.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://is.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://fc.huanxung.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ws.521024.cn

[R34] 退出时清理
来源：http://rs.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lb.newstarts.cn

[R35] 后台执行并等待
来源：http://cp.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kk.huanxung.cn

[R36] 并发执行多个任务
来源：http://xm.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://us.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://gj.muxihuayi.cn

files=$(ls -1)
来源：http://ft.lnxyls.cn

[R38] 管道串联
来源：http://dd.hnjuh.cn

cat a.txt | grep -i error | wc -l
来源：http://vw.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://fj.newstarts.cn

cmd > out.log 2>&1
来源：http://mq.nszjky.cn

[R40] 追加写日志
来源：http://bn.colortex.cn

echo "log" >> out.log
来源：http://qx.haigaiapp.cn

[R41] 丢弃输出
来源：http://ov.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://dx.jianghongdianzi.cn

[R42] 输入重定向
来源：http://dr.newstarts.cn

wc -l < a.txt
来源：http://zq.muxihuayi.cn

[R43] 按名字查找文件
来源：http://ml.colortex.cn

find . -name "*.log" -type f
来源：http://as.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://zm.szsharing.cn

find . -mtime -7 -type f
来源：http://si.bookmarksfly.cn

[R45] 批量删除
来源：http://lt.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://sm.gzmigu.cn

[R46] 递归替换文件内容
来源：http://ai.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cp.gzmigu.cn

[R47] sed 单行替换
来源：http://mx.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ks.szxytkj.cn

[R48] awk 取指定列
来源：http://if.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://cx.shxzskj.cn

[R49] awk 带条件
来源：http://sd.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sp.jianghongdianzi.cn

[R50] awk 求和
来源：http://ea.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bm.huanxung.cn

[R51] 排序去重取前几
来源：http://si.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qb.chemitech.net.cn

[R52] 统计行数
来源：http://du.yuntaijiaju.cn

wc -l a.txt
来源：http://id.colortex.cn

[R53] 查看文件头与实时尾
来源：http://yy.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gk.lnxyls.cn

[R54] 比较两个文件
来源：http://dh.huanxung.cn

diff a.txt b.txt
来源：http://fg.chemitech.net.cn

[R55] 压缩与解压
来源：http://zx.shxzukj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nq.colortex.cn

[R56] 远程拷贝
来源：http://wk.nszjky.cn

scp file user@host:/path/
来源：http://aj.lnxyls.cn

[R57] 远程执行命令
来源：http://cw.nszjky.cn

ssh user@host 'uptime'
来源：http://js.hahajie.cn

[R58] 下载文件
来源：http://dg.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cu.bjjhwx.cn

[R59] 发 POST JSON
来源：http://vf.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hr.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://fz.yuexingan06.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://is.huanxung.cn

[R61] 磁盘占用
来源：http://wj.bjjhwx.cn

df -h;  du -sh *
来源：http://dz.gzmigu.cn

[R62] 找最占空间的文件
来源：http://up.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://yo.chemitech.net.cn

[R63] 内存与进程
来源：http://yt.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://cz.nszjky.cn

[R64] 结束进程
来源：http://gc.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://eo.bjjhwx.cn

[R65] 查看端口占用
来源：http://zw.colortex.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mh.colortex.cn

[R66] 定时任务
来源：http://tn.newstarts.cn

crontab -e;  crontab -l
来源：http://gz.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://oh.szsharing.cn

openssl rand -hex 16
来源：http://mb.szxytkj.cn

[R68] 计算文件校验值
来源：http://fk.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zh.jctech888.com.cn

[R69] 生成随机密码
来源：http://vj.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://mn.9csxet.cn

[R70] 时间戳与互转
来源：http://rm.huanxung.cn

date +%s;  date -d @1700000000
来源：http://kv.huixiangedu.cn

[R71] 日期格式化
来源：http://pi.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xx.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://eq.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://md.bjjhwx.cn

[R73] 分割大日志
来源：http://wy.muxihuayi.cn

split -l 1000 big.log part_
来源：http://gu.nicolike.cn

[R74] 批量重命名
来源：http://ty.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uj.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://vx.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://nu.panjiajie.cn

[R76] 使用临时文件
来源：http://xe.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oa.yuexingan06.cn

[R77] 读取用户输入
来源：http://or.yuntaijiaju.cn

read -rp "请输入: " ans
来源：http://ex.hnjuh.cn

[R78] 交互式菜单
来源：http://jc.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vh.shtwfgs.cn

[R79] 解析命令行选项
来源：http://fo.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qm.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://lm.521024.cn

time ./run.sh
来源：http://sm.huixinmuqiang.cn

================================================================================
来源：http://oq.hnjuh.cn

S. C / C++ 专题
来源：http://xj.521024.cn

================================================================================
来源：http://pb.chemitech.net.cn

[S01] C：Hello World
来源：http://so.colortex.cn

#include <stdio.h>
来源：http://wv.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ta.gzmigu.cn

[S02] C：变量与格式化输出
来源：http://xu.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://yr.haigaiapp.cn

[S03] C：读入整数
来源：http://lx.colortex.cn

int x; scanf("%d", &x);
来源：http://vb.muxihuayi.cn

[S04] C：字符串复制
来源：http://ut.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pp.szxytkj.cn

[S05] C：字符串长度
来源：http://bo.huixinmuqiang.cn


<!-- 参考信息 -->