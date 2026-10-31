代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ue.9csxet.cn

) t WHERE rn = 1;
来源：http://nf.jianghongdianzi.cn

[Q35] 内连接
来源：http://wk.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tr.huixiangedu.cn

[Q36] 左连接
来源：http://rz.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mh.hahajie.cn

[Q37] 右连接
来源：http://pg.szsharing.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wq.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cn.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://am.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://qr.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yv.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nd.nicolike.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ft.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://va.huanxung.cn

[Q41] 多表连接
来源：http://hj.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kx.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://kr.panjiajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://hb.lnxyls.cn

[Q42] 连接条件附加过滤
来源：http://hi.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://qy.chemitech.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://el.shxzskj.cn

[Q43] 标量子查询
来源：http://mo.asd995.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ej.asd995.cn

[Q44] IN 子查询
来源：http://bh.szsharing.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tz.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://nq.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ri.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gw.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zc.panjiajie.cn

[Q47] 与平均值比较
来源：http://vp.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xx.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://nq.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rn.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://dy.nicolike.cn

[Q49] 更新单行
来源：http://xd.shxzukj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://md.muxihuayi.cn

[Q50] 批量更新
来源：http://fx.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xs.szsharing.cn

[Q51] 用子查询更新
来源：http://pn.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://do.chemitech.net.cn

[Q52] 删除指定行
来源：http://qg.haigaiapp.cn

DELETE FROM users WHERE id = 10;
来源：http://in.jctech888.com.cn

[Q53] 按条件删除
来源：http://kf.huixiangedu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gm.hnjuh.cn

[Q54] 清空表
来源：http://gr.521024.cn

TRUNCATE TABLE logs;
来源：http://vh.huanxung.cn

[Q55] 排名（并列占位）
来源：http://ap.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ez.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://yl.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xd.szsharing.cn

[Q57] 行号
来源：http://ia.9csxet.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ul.szxytkj.cn

[Q58] 累计求和
来源：http://ui.9csxet.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ja.gzmigu.cn

[Q59] 分组内累计
来源：http://ql.huixiangedu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wh.521024.cn

[Q60] 取上一行 / 下一行
来源：http://ok.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://li.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vj.jctech888.com.cn

[Q61] 移动平均
来源：http://cv.nszjky.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nb.wgjwhj.cn

[Q62] 分组占比
来源：http://rm.lnxyls.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yl.jianghongdianzi.cn

[Q63] 开启事务
来源：http://dk.haigaiapp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jg.bookmarksfly.cn

[Q64] 提交事务
来源：http://se.haigaiapp.cn

COMMIT;
来源：http://nu.newstarts.cn

[Q65] 回滚事务
来源：http://mq.yuexingan06.cn

ROLLBACK;
来源：http://bp.jianghongdianzi.cn

[Q66] 行锁查询
来源：http://jj.jianghongdianzi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iw.muxihuayi.cn

[Q67] 设置隔离级别
来源：http://bo.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ek.panjiajie.cn

[Q68] 保存点
来源：http://gc.gzmigu.cn

SAVEPOINT sp1;
来源：http://rp.shtwfgs.cn

ROLLBACK TO sp1;
来源：http://wj.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://sg.newstarts.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qt.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://gy.huixiangedu.cn

ANALYZE TABLE users;
来源：http://hx.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://dk.huanxung.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jq.nicolike.cn

[Q72] 查看索引
来源：http://cy.shxzukj.cn

SHOW INDEX FROM users;
来源：http://dg.newstarts.cn

[Q73] 查看表状态
来源：http://oo.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fu.jctech888.com.cn

[Q74] 强制使用索引
来源：http://zu.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sb.shxzukj.cn

[Q75] 日期格式化
来源：http://ep.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ab.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ie.hnjuh.cn

[Q76] 按天统计
来源：http://ac.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oj.huixiangedu.cn

[Q77] 时间加减
来源：http://mn.shtwfgs.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ao.bjjhwx.cn

[Q78] 当前时间
来源：http://nv.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pf.yuexingan06.cn

[Q79] 字符串拼接
来源：http://df.lnxyls.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rh.wgjwhj.cn

[Q80] 字符串截取
来源：http://ii.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nr.asd995.cn

[Q81] 字符串替换
来源：http://sz.newstarts.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vf.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://ry.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xw.gzmigu.cn

[Q83] 大小写转换
来源：http://fa.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sp.panjiajie.cn

[Q84] 去除首尾空格
来源：http://eu.bookmarksfly.cn

SELECT TRIM(name) FROM users;
来源：http://bf.shxzukj.cn

[Q85] 数值取整
来源：http://pp.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mt.hnjuh.cn

[Q86] 读取 JSON 字段
来源：http://jl.muxihuayi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cn.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://gz.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xa.521024.cn

[Q88] 行转列（条件聚合）
来源：http://wq.huixinmuqiang.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://up.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tj.huanxung.cn

[Q89] 判断表是否存在
来源：http://up.huixinmuqiang.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vq.wgjwhj.cn

[Q90] 生成序号列
来源：http://qu.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qn.szsharing.cn

================================================================================
来源：http://cc.shtwfgs.cn

R. Bash 专题
来源：http://mz.colortex.cn

================================================================================
来源：http://vh.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://ra.hnjuh.cn

#!/usr/bin/env bash
来源：http://ja.yuexingan06.cn

set -euo pipefail
来源：http://vo.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://ef.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://hp.asd995.cn

[R03] 只读变量
来源：http://cf.yuexingan06.cn

readonly PI=3.14
来源：http://rc.panjiajie.cn

[R04] 位置参数
来源：http://aj.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tc.521024.cn

[R05] 参数默认值
来源：http://gq.panjiajie.cn

name="${1:-default}"
来源：http://ch.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://xy.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yt.muxihuayi.cn

[R07] if 判断文件
来源：http://ve.bjjhwx.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://km.shxzskj.cn

[R08] 数值比较
来源：http://ds.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rm.hnjuh.cn

[R09] 字符串比较
来源：http://xn.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ix.panjiajie.cn

[R10] 正则匹配
来源：http://cp.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shtwfgs.cn

[R11] case 多分支
来源：http://xr.haigaiapp.cn

case "$1" in
来源：http://fl.huixiangedu.cn

start) echo "启动" ;;
来源：http://yy.lnxyls.cn

stop)  echo "停止" ;;
来源：http://wu.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://db.colortex.cn

esac
来源：http://zc.wgjwhj.cn

[R12] for 遍历文件
来源：http://rh.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://vc.yuntaijiaju.cn

[R13] for 计数循环
来源：http://af.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://et.hahajie.cn

[R14] C 风格 for
来源：http://ns.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ay.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://gy.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hr.jctech888.com.cn

[R16] until 等待条件
来源：http://fs.shxzskj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rn.jctech888.com.cn

[R17] 数组定义与取值
来源：http://vr.huanxung.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jj.hnjuh.cn

[R18] 遍历数组
来源：http://wy.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aj.szsharing.cn

[R19] 数组长度
来源：http://ye.muxihuayi.cn

echo "${#arr[@]}"
来源：http://bm.nicolike.cn

[R20] 关联数组（字典）
来源：http://tv.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://su.lnxyls.cn

[R21] 字符串长度
来源：http://lf.nicolike.cn

echo "${#s}"
来源：http://jt.newstarts.cn

[R22] 截取子串
来源：http://gj.gzmigu.cn

echo "${s:0:5}"
来源：http://qu.panjiajie.cn

[R23] 字符串替换
来源：http://gg.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rd.bookmarksfly.cn

[R24] 大小写转换
来源：http://sg.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ly.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://vo.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xy.bookmarksfly.cn

[R26] 命令替换
来源：http://xm.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://rw.shxzskj.cn

[R27] 算术展开
来源：http://cd.hahajie.cn

echo $((1 + 2 * 3))
来源：http://fz.szxytkj.cn

[R28] 浮点运算
来源：http://kb.newstarts.cn

echo "scale=2; 10/3" | bc
来源：http://gc.jianghongdianzi.cn

[R29] 定义函数
来源：http://ib.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ui.shxzskj.cn

[R30] 函数返回状态码
来源：http://fi.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://of.shxzukj.cn

[R31] 局部变量
来源：http://hy.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://tz.521024.cn

[R32] 参数个数校验
来源：http://ug.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wl.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://ba.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ne.asd995.cn

[R34] 退出时清理
来源：http://er.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dj.muxihuayi.cn

[R35] 后台执行并等待
来源：http://pa.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zq.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://mu.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cy.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://jo.nszjky.cn

files=$(ls -1)
来源：http://ax.haigaiapp.cn

[R38] 管道串联
来源：http://gz.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://gb.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://tw.nicolike.cn

cmd > out.log 2>&1
来源：http://jz.chemitech.net.cn

[R40] 追加写日志
来源：http://uk.muxihuayi.cn

echo "log" >> out.log
来源：http://fo.hahajie.cn

[R41] 丢弃输出
来源：http://xf.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://mu.haigaiapp.cn

[R42] 输入重定向
来源：http://aa.huanxung.cn

wc -l < a.txt
来源：http://hb.gzmigu.cn

[R43] 按名字查找文件
来源：http://ih.asd995.cn

find . -name "*.log" -type f
来源：http://po.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://hi.jctech888.com.cn

find . -mtime -7 -type f
来源：http://mf.shtwfgs.cn

[R45] 批量删除
来源：http://vx.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://ir.huanxung.cn

[R46] 递归替换文件内容
来源：http://gs.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hh.huixiangedu.cn

[R47] sed 单行替换
来源：http://lb.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vl.chemitech.net.cn

[R48] awk 取指定列
来源：http://we.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://lj.muxihuayi.cn

[R49] awk 带条件
来源：http://bs.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vw.newstarts.cn

[R50] awk 求和
来源：http://pv.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tf.9csxet.cn

[R51] 排序去重取前几
来源：http://sk.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yp.muxihuayi.cn

[R52] 统计行数
来源：http://gs.jianghongdianzi.cn

wc -l a.txt
来源：http://yj.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://ty.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uj.shxzukj.cn

[R54] 比较两个文件
来源：http://br.gzmigu.cn

diff a.txt b.txt
来源：http://rp.huixiangedu.cn

[R55] 压缩与解压
来源：http://wl.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fx.huanxung.cn

[R56] 远程拷贝
来源：http://pe.bjjhwx.cn

scp file user@host:/path/
来源：http://aa.szsharing.cn

[R57] 远程执行命令
来源：http://le.jctech888.com.cn

ssh user@host 'uptime'
来源：http://my.szsharing.cn

[R58] 下载文件
来源：http://gr.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mo.wgjwhj.cn

[R59] 发 POST JSON
来源：http://fm.haigaiapp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dl.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://zn.huanxung.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gu.haigaiapp.cn

[R61] 磁盘占用
来源：http://mb.szsharing.cn

df -h;  du -sh *
来源：http://be.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://sf.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://lh.wgjwhj.cn

[R63] 内存与进程
来源：http://du.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://iu.wgjwhj.cn

[R64] 结束进程
来源：http://qe.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://cp.colortex.cn

[R65] 查看端口占用
来源：http://ug.jctech888.com.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nd.hnjuh.cn

[R66] 定时任务
来源：http://vr.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://gz.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://as.9csxet.cn

openssl rand -hex 16
来源：http://nd.yuexingan06.cn

[R68] 计算文件校验值
来源：http://mh.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vi.huanxung.cn

[R69] 生成随机密码
来源：http://tr.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://ma.szsharing.cn

[R70] 时间戳与互转
来源：http://dm.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://br.huixiangedu.cn

[R71] 日期格式化
来源：http://fv.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ke.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://mv.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oi.chemitech.net.cn

[R73] 分割大日志
来源：http://oq.hnjuh.cn

split -l 1000 big.log part_
来源：http://hl.hnjuh.cn

[R74] 批量重命名
来源：http://of.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ua.newstarts.cn

[R75] 导出环境变量
来源：http://lb.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://ik.nszjky.cn

[R76] 使用临时文件
来源：http://fi.asd995.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://or.asd995.cn

[R77] 读取用户输入
来源：http://ct.shxzskj.cn

read -rp "请输入: " ans
来源：http://th.panjiajie.cn

[R78] 交互式菜单
来源：http://br.panjiajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yu.hahajie.cn

[R79] 解析命令行选项
来源：http://kq.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uw.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://gf.asd995.cn

time ./run.sh
来源：http://ck.bookmarksfly.cn

================================================================================
来源：http://vy.haigaiapp.cn

S. C / C++ 专题
来源：http://of.yuntaijiaju.cn

================================================================================
来源：http://on.huixinmuqiang.cn

[S01] C：Hello World
来源：http://ux.szxytkj.cn

#include <stdio.h>
来源：http://su.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ln.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://ny.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://vk.huanxung.cn

[S03] C：读入整数
来源：http://rw.asd995.cn


<!-- 参考信息 -->