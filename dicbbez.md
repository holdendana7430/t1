代发 wailian999

[Q36] 左连接
来源：http://uu.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lu.haigaiapp.cn

[Q37] 右连接
来源：http://ml.9csxet.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rl.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kk.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ur.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://ez.jianghongdianzi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wd.muxihuayi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tn.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://on.shxzukj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cf.huixiangedu.cn

[Q41] 多表连接
来源：http://dl.bookmarksfly.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lo.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://pg.szsharing.cn

JOIN products p ON p.id = o.product_id;
来源：http://js.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://ju.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://bi.colortex.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sw.nszjky.cn

[Q43] 标量子查询
来源：http://va.lnxyls.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vj.bjjhwx.cn

[Q44] IN 子查询
来源：http://id.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vt.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://dg.huixinmuqiang.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ny.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jk.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ns.9csxet.cn

[Q47] 与平均值比较
来源：http://ac.nszjky.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rp.521024.cn

[Q48] CTE 公用表表达式
来源：http://fd.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fb.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://ak.jianghongdianzi.cn

[Q49] 更新单行
来源：http://tj.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xe.muxihuayi.cn

[Q50] 批量更新
来源：http://dq.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ht.muxihuayi.cn

[Q51] 用子查询更新
来源：http://hz.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qy.szsharing.cn

[Q52] 删除指定行
来源：http://uo.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://eh.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://bx.hahajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pu.jianghongdianzi.cn

[Q54] 清空表
来源：http://yl.haigaiapp.cn

TRUNCATE TABLE logs;
来源：http://lw.newstarts.cn

[Q55] 排名（并列占位）
来源：http://hx.gzmigu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mt.yuntaijiaju.cn

[Q56] 密集排名（并列不占位）
来源：http://wy.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ta.haigaiapp.cn

[Q57] 行号
来源：http://cc.szsharing.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fw.wgjwhj.cn

[Q58] 累计求和
来源：http://kt.nszjky.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wg.panjiajie.cn

[Q59] 分组内累计
来源：http://vr.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ev.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://pb.bookmarksfly.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://my.yuntaijiaju.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qw.huixiangedu.cn

[Q61] 移动平均
来源：http://ns.szxytkj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ha.szxytkj.cn

[Q62] 分组占比
来源：http://jy.yuntaijiaju.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gx.shxzskj.cn

[Q63] 开启事务
来源：http://rc.shtwfgs.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hy.panjiajie.cn

[Q64] 提交事务
来源：http://lz.colortex.cn

COMMIT;
来源：http://hk.yuexingan06.cn

[Q65] 回滚事务
来源：http://wa.shtwfgs.cn

ROLLBACK;
来源：http://jz.shxzskj.cn

[Q66] 行锁查询
来源：http://qv.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lj.asd995.cn

[Q67] 设置隔离级别
来源：http://ys.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hd.yuexingan06.cn

[Q68] 保存点
来源：http://td.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://vr.asd995.cn

ROLLBACK TO sp1;
来源：http://fh.gzmigu.cn

[Q69] 查看执行计划
来源：http://nb.muxihuayi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jk.newstarts.cn

[Q70] 更新统计信息
来源：http://mj.nicolike.cn

ANALYZE TABLE users;
来源：http://qj.bjjhwx.cn

[Q71] 查看建表语句
来源：http://lw.szxytkj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://my.nszjky.cn

[Q72] 查看索引
来源：http://it.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://fl.shxzskj.cn

[Q73] 查看表状态
来源：http://rk.szxytkj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kj.bjjhwx.cn

[Q74] 强制使用索引
来源：http://ws.huixinmuqiang.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lh.shxzskj.cn

[Q75] 日期格式化
来源：http://ak.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://js.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hw.hnjuh.cn

[Q76] 按天统计
来源：http://bj.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uz.huanxung.cn

[Q77] 时间加减
来源：http://hc.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vg.panjiajie.cn

[Q78] 当前时间
来源：http://tz.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hm.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://jw.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yh.jctech888.com.cn

[Q80] 字符串截取
来源：http://nd.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ov.nicolike.cn

[Q81] 字符串替换
来源：http://po.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ba.szsharing.cn

[Q82] 字符长度与字节长度
来源：http://ib.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mg.wgjwhj.cn

[Q83] 大小写转换
来源：http://hm.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yq.hahajie.cn

[Q84] 去除首尾空格
来源：http://wm.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://xs.bookmarksfly.cn

[Q85] 数值取整
来源：http://ww.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ip.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://qg.nicolike.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dd.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://tn.yuexingan06.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xy.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://qc.huixiangedu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fg.gzmigu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://an.szxytkj.cn

[Q89] 判断表是否存在
来源：http://lc.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gq.hahajie.cn

[Q90] 生成序号列
来源：http://jt.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nl.lnxyls.cn

================================================================================
来源：http://oz.panjiajie.cn

R. Bash 专题
来源：http://ed.lnxyls.cn

================================================================================
来源：http://nj.nicolike.cn

[R01] shebang 与严格模式
来源：http://yg.bjjhwx.cn

#!/usr/bin/env bash
来源：http://yi.asd995.cn

set -euo pipefail
来源：http://uc.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://zp.bjjhwx.cn

name="Tom"; echo "$name"
来源：http://lo.jctech888.com.cn

[R03] 只读变量
来源：http://hy.hahajie.cn

readonly PI=3.14
来源：http://yc.wgjwhj.cn

[R04] 位置参数
来源：http://ao.hnjuh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hv.wgjwhj.cn

[R05] 参数默认值
来源：http://ws.hnjuh.cn

name="${1:-default}"
来源：http://xk.shxzskj.cn

[R06] 判断命令是否存在
来源：http://dg.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lr.colortex.cn

[R07] if 判断文件
来源：http://ay.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rv.gzmigu.cn

[R08] 数值比较
来源：http://zy.hahajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xc.lnxyls.cn

[R09] 字符串比较
来源：http://aq.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wx.jianghongdianzi.cn

[R10] 正则匹配
来源：http://jo.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gt.haigaiapp.cn

[R11] case 多分支
来源：http://rr.shxzskj.cn

case "$1" in
来源：http://ns.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://nz.yuexingan06.cn

stop)  echo "停止" ;;
来源：http://lz.newstarts.cn

*)     echo "未知命令" ;;
来源：http://co.huixiangedu.cn

esac
来源：http://oy.bookmarksfly.cn

[R12] for 遍历文件
来源：http://ql.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://qi.newstarts.cn

[R13] for 计数循环
来源：http://uz.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://jp.hnjuh.cn

[R14] C 风格 for
来源：http://uo.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sk.colortex.cn

[R15] while 逐行读文件
来源：http://jj.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ss.bjjhwx.cn

[R16] until 等待条件
来源：http://yv.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nf.nszjky.cn

[R17] 数组定义与取值
来源：http://lq.bjjhwx.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bl.hnjuh.cn

[R18] 遍历数组
来源：http://lg.9csxet.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vj.wgjwhj.cn

[R19] 数组长度
来源：http://cm.hnjuh.cn

echo "${#arr[@]}"
来源：http://hb.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://pb.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jo.haigaiapp.cn

[R21] 字符串长度
来源：http://zs.colortex.cn

echo "${#s}"
来源：http://no.jianghongdianzi.cn

[R22] 截取子串
来源：http://ag.gzmigu.cn

echo "${s:0:5}"
来源：http://in.huixinmuqiang.cn

[R23] 字符串替换
来源：http://bq.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sa.bjjhwx.cn

[R24] 大小写转换
来源：http://jf.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cn.huixinmuqiang.cn

[R25] 去后缀 / 去前缀
来源：http://vj.huixiangedu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zt.yuexingan06.cn

[R26] 命令替换
来源：http://os.asd995.cn

now=$(date +%F); echo "$now"
来源：http://ms.szxytkj.cn

[R27] 算术展开
来源：http://bl.nszjky.cn

echo $((1 + 2 * 3))
来源：http://qh.hahajie.cn

[R28] 浮点运算
来源：http://bs.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://ph.521024.cn

[R29] 定义函数
来源：http://lh.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wu.newstarts.cn

[R30] 函数返回状态码
来源：http://vt.wgjwhj.cn

f() { return 0; }; f || echo "失败了"
来源：http://ue.chemitech.net.cn

[R31] 局部变量
来源：http://nr.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://lm.lnxyls.cn

[R32] 参数个数校验
来源：http://tj.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hu.colortex.cn

[R33] 捕获错误并提示行号
来源：http://nj.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://om.hnjuh.cn

[R34] 退出时清理
来源：http://yn.yuntaijiaju.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gh.lnxyls.cn

[R35] 后台执行并等待
来源：http://zc.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://st.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://ds.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lq.asd995.cn

[R37] 把输出赋给变量
来源：http://hm.newstarts.cn

files=$(ls -1)
来源：http://uy.szxytkj.cn

[R38] 管道串联
来源：http://qc.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://rd.shtwfgs.cn

[R39] 重定向标准输出与错误
来源：http://fy.wgjwhj.cn

cmd > out.log 2>&1
来源：http://go.asd995.cn

[R40] 追加写日志
来源：http://an.jctech888.com.cn

echo "log" >> out.log
来源：http://ry.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://on.huanxung.cn

cmd >/dev/null 2>&1
来源：http://bh.hnjuh.cn

[R42] 输入重定向
来源：http://zy.chemitech.net.cn

wc -l < a.txt
来源：http://bz.gzmigu.cn

[R43] 按名字查找文件
来源：http://un.chemitech.net.cn

find . -name "*.log" -type f
来源：http://ox.chemitech.net.cn

[R44] 按修改时间查找
来源：http://yy.huixiangedu.cn

find . -mtime -7 -type f
来源：http://rg.haigaiapp.cn

[R45] 批量删除
来源：http://eh.hahajie.cn

find . -name "*.tmp" -delete
来源：http://pt.lnxyls.cn

[R46] 递归替换文件内容
来源：http://fh.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yu.wgjwhj.cn

[R47] sed 单行替换
来源：http://ej.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lc.jctech888.com.cn

[R48] awk 取指定列
来源：http://ov.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://qr.jctech888.com.cn

[R49] awk 带条件
来源：http://qf.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bg.hahajie.cn

[R50] awk 求和
来源：http://bp.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yf.nicolike.cn

[R51] 排序去重取前几
来源：http://ne.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gh.bjjhwx.cn

[R52] 统计行数
来源：http://tu.bookmarksfly.cn

wc -l a.txt
来源：http://mx.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://ll.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lx.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://lk.colortex.cn

diff a.txt b.txt
来源：http://rn.yuexingan06.cn

[R55] 压缩与解压
来源：http://ws.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yt.nszjky.cn

[R56] 远程拷贝
来源：http://oc.szxytkj.cn

scp file user@host:/path/
来源：http://lr.asd995.cn

[R57] 远程执行命令
来源：http://nk.bookmarksfly.cn

ssh user@host 'uptime'
来源：http://lw.hnjuh.cn

[R58] 下载文件
来源：http://ld.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bl.hahajie.cn

[R59] 发 POST JSON
来源：http://dn.521024.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ut.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://yl.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ry.panjiajie.cn

[R61] 磁盘占用
来源：http://pq.chemitech.net.cn

df -h;  du -sh *
来源：http://se.521024.cn

[R62] 找最占空间的文件
来源：http://pd.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://uj.haigaiapp.cn

[R63] 内存与进程
来源：http://ub.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://gb.bookmarksfly.cn

[R64] 结束进程
来源：http://go.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://rn.gzmigu.cn

[R65] 查看端口占用
来源：http://ap.jctech888.com.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kf.yuexingan06.cn

[R66] 定时任务
来源：http://hj.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://ul.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://ip.521024.cn

openssl rand -hex 16
来源：http://xb.gzmigu.cn

[R68] 计算文件校验值
来源：http://nk.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cp.haigaiapp.cn

[R69] 生成随机密码
来源：http://sz.huixinmuqiang.cn

head -c 16 /dev/urandom | base64
来源：http://rq.gzmigu.cn

[R70] 时间戳与互转
来源：http://qj.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://nt.521024.cn

[R71] 日期格式化
来源：http://wn.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uk.newstarts.cn

[R72] 等待端口就绪
来源：http://zm.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://li.shxzukj.cn

[R73] 分割大日志
来源：http://wu.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://xu.hahajie.cn

[R74] 批量重命名
来源：http://pg.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bl.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://fg.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://zu.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://ij.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tz.haigaiapp.cn

[R77] 读取用户输入
来源：http://uu.yuntaijiaju.cn

read -rp "请输入: " ans
来源：http://kk.haigaiapp.cn

[R78] 交互式菜单
来源：http://go.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lc.gzmigu.cn

[R79] 解析命令行选项
来源：http://sw.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dt.colortex.cn

[R80] 查看脚本执行耗时
来源：http://ps.newstarts.cn

time ./run.sh
来源：http://pu.jctech888.com.cn

================================================================================
来源：http://dr.huixinmuqiang.cn

S. C / C++ 专题
来源：http://vx.haigaiapp.cn

================================================================================
来源：http://es.nszjky.cn

[S01] C：Hello World
来源：http://cm.asd995.cn

#include <stdio.h>
来源：http://oe.panjiajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vz.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://it.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://ia.shxzskj.cn

[S03] C：读入整数
来源：http://yi.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://il.bookmarksfly.cn

[S04] C：字符串复制
来源：http://yg.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xk.szxytkj.cn

[S05] C：字符串长度
来源：http://iu.shxzskj.cn


<!-- 参考信息 -->