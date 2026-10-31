代发 wailian999

[Q36] 左连接
来源：http://sk.panjiajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fx.newstarts.cn

[Q37] 右连接
来源：http://uj.yuexingan06.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gh.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tw.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jv.jianghongdianzi.cn

[Q39] 自连接（查上下级）
来源：http://ll.jctech888.com.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ey.nicolike.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jo.521024.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pj.yuexingan06.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tc.9csxet.cn

[Q41] 多表连接
来源：http://wr.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://eh.panjiajie.cn

JOIN users u ON u.id = o.user_id
来源：http://ea.lnxyls.cn

JOIN products p ON p.id = o.product_id;
来源：http://ri.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://zv.asd995.cn

SELECT u.name, o.amount FROM users u
来源：http://ys.panjiajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vm.huixinmuqiang.cn

[Q43] 标量子查询
来源：http://if.szsharing.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://us.shxzskj.cn

[Q44] IN 子查询
来源：http://tp.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bf.szsharing.cn

[Q45] EXISTS 判断存在
来源：http://uo.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pb.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ni.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mo.huixiangedu.cn

[Q47] 与平均值比较
来源：http://mv.szxytkj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ob.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://ng.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://af.bjjhwx.cn

SELECT * FROM t WHERE c > 5;
来源：http://wc.haigaiapp.cn

[Q49] 更新单行
来源：http://sn.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ce.jctech888.com.cn

[Q50] 批量更新
来源：http://yz.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sj.huixiangedu.cn

[Q51] 用子查询更新
来源：http://bh.asd995.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://be.shtwfgs.cn

[Q52] 删除指定行
来源：http://dc.gzmigu.cn

DELETE FROM users WHERE id = 10;
来源：http://qm.huixiangedu.cn

[Q53] 按条件删除
来源：http://za.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ur.lnxyls.cn

[Q54] 清空表
来源：http://ce.gzmigu.cn

TRUNCATE TABLE logs;
来源：http://be.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://il.szxytkj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mq.yuntaijiaju.cn

[Q56] 密集排名（并列不占位）
来源：http://kf.jianghongdianzi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://na.muxihuayi.cn

[Q57] 行号
来源：http://sk.gzmigu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ke.jianghongdianzi.cn

[Q58] 累计求和
来源：http://fk.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tr.9csxet.cn

[Q59] 分组内累计
来源：http://lb.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://we.huixinmuqiang.cn

[Q60] 取上一行 / 下一行
来源：http://ta.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wh.colortex.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dy.huixinmuqiang.cn

[Q61] 移动平均
来源：http://nm.shxzukj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ka.bjjhwx.cn

[Q62] 分组占比
来源：http://ni.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rx.nszjky.cn

[Q63] 开启事务
来源：http://mk.wgjwhj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vy.asd995.cn

[Q64] 提交事务
来源：http://zv.shxzskj.cn

COMMIT;
来源：http://qt.9csxet.cn

[Q65] 回滚事务
来源：http://to.haigaiapp.cn

ROLLBACK;
来源：http://tt.521024.cn

[Q66] 行锁查询
来源：http://jo.gzmigu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fb.muxihuayi.cn

[Q67] 设置隔离级别
来源：http://bm.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mw.gzmigu.cn

[Q68] 保存点
来源：http://xk.shtwfgs.cn

SAVEPOINT sp1;
来源：http://eq.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://al.jctech888.com.cn

[Q69] 查看执行计划
来源：http://lv.muxihuayi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rg.shxzskj.cn

[Q70] 更新统计信息
来源：http://bf.bookmarksfly.cn

ANALYZE TABLE users;
来源：http://ju.muxihuayi.cn

[Q71] 查看建表语句
来源：http://wl.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bq.muxihuayi.cn

[Q72] 查看索引
来源：http://sb.hahajie.cn

SHOW INDEX FROM users;
来源：http://oi.szxytkj.cn

[Q73] 查看表状态
来源：http://fs.szxytkj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ge.yuntaijiaju.cn

[Q74] 强制使用索引
来源：http://gl.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dm.haigaiapp.cn

[Q75] 日期格式化
来源：http://zq.chemitech.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zk.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fl.bookmarksfly.cn

[Q76] 按天统计
来源：http://ll.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fe.nszjky.cn

[Q77] 时间加减
来源：http://ns.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uu.nszjky.cn

[Q78] 当前时间
来源：http://ia.nszjky.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mi.yuntaijiaju.cn

[Q79] 字符串拼接
来源：http://wq.szsharing.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bm.9csxet.cn

[Q80] 字符串截取
来源：http://qv.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zw.shtwfgs.cn

[Q81] 字符串替换
来源：http://al.muxihuayi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rd.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://to.9csxet.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kh.nicolike.cn

[Q83] 大小写转换
来源：http://gm.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://so.newstarts.cn

[Q84] 去除首尾空格
来源：http://ca.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://fb.521024.cn

[Q85] 数值取整
来源：http://eh.9csxet.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lw.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://mj.bjjhwx.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xa.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://or.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rt.huixinmuqiang.cn

[Q88] 行转列（条件聚合）
来源：http://xm.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zp.wgjwhj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lx.9csxet.cn

[Q89] 判断表是否存在
来源：http://dp.yuntaijiaju.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mq.shxzskj.cn

[Q90] 生成序号列
来源：http://gy.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rh.chemitech.net.cn

================================================================================
来源：http://kd.huanxung.cn

R. Bash 专题
来源：http://yd.nicolike.cn

================================================================================
来源：http://mk.shtwfgs.cn

[R01] shebang 与严格模式
来源：http://oy.muxihuayi.cn

#!/usr/bin/env bash
来源：http://sy.nszjky.cn

set -euo pipefail
来源：http://cq.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://ry.gzmigu.cn

name="Tom"; echo "$name"
来源：http://ku.panjiajie.cn

[R03] 只读变量
来源：http://aa.asd995.cn

readonly PI=3.14
来源：http://qi.wgjwhj.cn

[R04] 位置参数
来源：http://qc.chemitech.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ey.szxytkj.cn

[R05] 参数默认值
来源：http://hm.huixiangedu.cn

name="${1:-default}"
来源：http://hh.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://gk.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gt.huanxung.cn

[R07] if 判断文件
来源：http://yq.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pv.huixinmuqiang.cn

[R08] 数值比较
来源：http://kk.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hy.asd995.cn

[R09] 字符串比较
来源：http://fv.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ck.shxzukj.cn

[R10] 正则匹配
来源：http://wd.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ke.panjiajie.cn

[R11] case 多分支
来源：http://ve.lnxyls.cn

case "$1" in
来源：http://ca.jctech888.com.cn

start) echo "启动" ;;
来源：http://az.lnxyls.cn

stop)  echo "停止" ;;
来源：http://rj.9csxet.cn

*)     echo "未知命令" ;;
来源：http://ck.asd995.cn

esac
来源：http://mn.muxihuayi.cn

[R12] for 遍历文件
来源：http://bd.szsharing.cn

for f in *.txt; do echo "$f"; done
来源：http://id.wgjwhj.cn

[R13] for 计数循环
来源：http://pg.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://lw.szxytkj.cn

[R14] C 风格 for
来源：http://qw.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xh.shxzskj.cn

[R15] while 逐行读文件
来源：http://br.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cc.szsharing.cn

[R16] until 等待条件
来源：http://zy.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mk.bjjhwx.cn

[R17] 数组定义与取值
来源：http://yx.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ha.bookmarksfly.cn

[R18] 遍历数组
来源：http://wq.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ti.szsharing.cn

[R19] 数组长度
来源：http://ru.hnjuh.cn

echo "${#arr[@]}"
来源：http://pc.asd995.cn

[R20] 关联数组（字典）
来源：http://zm.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dy.yuntaijiaju.cn

[R21] 字符串长度
来源：http://do.hnjuh.cn

echo "${#s}"
来源：http://vs.shxzskj.cn

[R22] 截取子串
来源：http://ob.hnjuh.cn

echo "${s:0:5}"
来源：http://lb.shxzskj.cn

[R23] 字符串替换
来源：http://wz.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dl.newstarts.cn

[R24] 大小写转换
来源：http://gv.szxytkj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pm.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://rl.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xp.panjiajie.cn

[R26] 命令替换
来源：http://cg.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://pb.yuexingan06.cn

[R27] 算术展开
来源：http://sz.gzmigu.cn

echo $((1 + 2 * 3))
来源：http://sw.muxihuayi.cn

[R28] 浮点运算
来源：http://vr.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://mq.huanxung.cn

[R29] 定义函数
来源：http://tz.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zi.szsharing.cn

[R30] 函数返回状态码
来源：http://pa.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://ib.wgjwhj.cn

[R31] 局部变量
来源：http://sl.hnjuh.cn

f() { local x=1; echo "$x"; }
来源：http://hj.colortex.cn

[R32] 参数个数校验
来源：http://dn.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ob.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://hy.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iq.panjiajie.cn

[R34] 退出时清理
来源：http://vp.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vx.shxzukj.cn

[R35] 后台执行并等待
来源：http://uj.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ef.shxzskj.cn

[R36] 并发执行多个任务
来源：http://nk.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qu.nicolike.cn

[R37] 把输出赋给变量
来源：http://pk.wgjwhj.cn

files=$(ls -1)
来源：http://il.shxzskj.cn

[R38] 管道串联
来源：http://mv.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://zi.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://xl.shtwfgs.cn

cmd > out.log 2>&1
来源：http://nb.newstarts.cn

[R40] 追加写日志
来源：http://fh.shxzskj.cn

echo "log" >> out.log
来源：http://bg.colortex.cn

[R41] 丢弃输出
来源：http://ol.hahajie.cn

cmd >/dev/null 2>&1
来源：http://vo.chemitech.net.cn

[R42] 输入重定向
来源：http://fg.wgjwhj.cn

wc -l < a.txt
来源：http://pm.9csxet.cn

[R43] 按名字查找文件
来源：http://oh.huixiangedu.cn

find . -name "*.log" -type f
来源：http://cu.panjiajie.cn

[R44] 按修改时间查找
来源：http://wm.asd995.cn

find . -mtime -7 -type f
来源：http://ow.huanxung.cn

[R45] 批量删除
来源：http://rs.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://aa.521024.cn

[R46] 递归替换文件内容
来源：http://de.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://td.9csxet.cn

[R47] sed 单行替换
来源：http://bu.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nq.wgjwhj.cn

[R48] awk 取指定列
来源：http://kx.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://gs.haigaiapp.cn

[R49] awk 带条件
来源：http://wx.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qe.szxytkj.cn

[R50] awk 求和
来源：http://md.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pp.chemitech.net.cn

[R51] 排序去重取前几
来源：http://iz.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bc.huixiangedu.cn

[R52] 统计行数
来源：http://xp.szsharing.cn

wc -l a.txt
来源：http://zm.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://fq.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hr.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://jm.shxzukj.cn

diff a.txt b.txt
来源：http://un.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://kk.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jp.szsharing.cn

[R56] 远程拷贝
来源：http://aj.szsharing.cn

scp file user@host:/path/
来源：http://xk.521024.cn

[R57] 远程执行命令
来源：http://ce.hahajie.cn

ssh user@host 'uptime'
来源：http://ne.shxzskj.cn

[R58] 下载文件
来源：http://rb.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uu.hahajie.cn

[R59] 发 POST JSON
来源：http://ap.yuexingan06.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iw.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://dx.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cq.lnxyls.cn

[R61] 磁盘占用
来源：http://gy.hnjuh.cn

df -h;  du -sh *
来源：http://tm.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://ft.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://ha.asd995.cn

[R63] 内存与进程
来源：http://hm.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://em.huanxung.cn

[R64] 结束进程
来源：http://te.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://sk.lnxyls.cn

[R65] 查看端口占用
来源：http://nv.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dq.haigaiapp.cn

[R66] 定时任务
来源：http://kc.huanxung.cn

crontab -e;  crontab -l
来源：http://fd.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://jm.chemitech.net.cn

openssl rand -hex 16
来源：http://dk.shtwfgs.cn

[R68] 计算文件校验值
来源：http://mp.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fu.szxytkj.cn

[R69] 生成随机密码
来源：http://qv.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://uy.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://qx.colortex.cn

date +%s;  date -d @1700000000
来源：http://pa.huixinmuqiang.cn

[R71] 日期格式化
来源：http://qz.nszjky.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ad.asd995.cn

[R72] 等待端口就绪
来源：http://gd.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ow.bookmarksfly.cn

[R73] 分割大日志
来源：http://nc.huanxung.cn

split -l 1000 big.log part_
来源：http://bd.521024.cn

[R74] 批量重命名
来源：http://uw.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yz.haigaiapp.cn

[R75] 导出环境变量
来源：http://po.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://gp.newstarts.cn

[R76] 使用临时文件
来源：http://gz.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xk.hnjuh.cn

[R77] 读取用户输入
来源：http://de.shxzukj.cn

read -rp "请输入: " ans
来源：http://ge.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://eq.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ul.chemitech.net.cn

[R79] 解析命令行选项
来源：http://ru.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://am.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://pt.yuntaijiaju.cn

time ./run.sh
来源：http://bb.yuntaijiaju.cn

================================================================================
来源：http://gp.nicolike.cn

S. C / C++ 专题
来源：http://pm.jctech888.com.cn

================================================================================
来源：http://hs.shtwfgs.cn

[S01] C：Hello World
来源：http://jy.shtwfgs.cn

#include <stdio.h>
来源：http://ny.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sk.shtwfgs.cn

[S02] C：变量与格式化输出
来源：http://vw.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://es.colortex.cn

[S03] C：读入整数
来源：http://wo.9csxet.cn

int x; scanf("%d", &x);
来源：http://ss.chemitech.net.cn

[S04] C：字符串复制
来源：http://pc.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ou.9csxet.cn

[S05] C：字符串长度
来源：http://gl.jianghongdianzi.cn


<!-- 参考信息 -->