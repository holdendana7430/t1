代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vs.huixinmuqiang.cn

) t WHERE rn = 1;
来源：http://kj.bjjhwx.cn

[Q35] 内连接
来源：http://xb.shxzukj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yw.muxihuayi.cn

[Q36] 左连接
来源：http://zz.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yp.bookmarksfly.cn

[Q37] 右连接
来源：http://xf.chemitech.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ri.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://iu.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qu.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://tt.jctech888.com.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rn.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dw.yuexingan06.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ox.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ox.newstarts.cn

[Q41] 多表连接
来源：http://fq.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jm.chemitech.net.cn

JOIN users u ON u.id = o.user_id
来源：http://bh.yuexingan06.cn

JOIN products p ON p.id = o.product_id;
来源：http://mh.muxihuayi.cn

[Q42] 连接条件附加过滤
来源：http://oa.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://ux.yuntaijiaju.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vz.hnjuh.cn

[Q43] 标量子查询
来源：http://gd.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cv.shtwfgs.cn

[Q44] IN 子查询
来源：http://pr.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jh.bookmarksfly.cn

[Q45] EXISTS 判断存在
来源：http://mq.wgjwhj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hu.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nv.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qv.szxytkj.cn

[Q47] 与平均值比较
来源：http://np.haigaiapp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zb.colortex.cn

[Q48] CTE 公用表表达式
来源：http://bx.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hv.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://ni.bjjhwx.cn

[Q49] 更新单行
来源：http://ou.chemitech.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nk.shxzukj.cn

[Q50] 批量更新
来源：http://hd.panjiajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bx.panjiajie.cn

[Q51] 用子查询更新
来源：http://qd.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hs.bookmarksfly.cn

[Q52] 删除指定行
来源：http://tm.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://go.9csxet.cn

[Q53] 按条件删除
来源：http://nw.asd995.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ts.yuntaijiaju.cn

[Q54] 清空表
来源：http://gb.haigaiapp.cn

TRUNCATE TABLE logs;
来源：http://zb.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://nf.jianghongdianzi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yg.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://ov.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xe.muxihuayi.cn

[Q57] 行号
来源：http://kv.bjjhwx.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ed.521024.cn

[Q58] 累计求和
来源：http://xb.shxzukj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zq.shxzukj.cn

[Q59] 分组内累计
来源：http://tu.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cg.gzmigu.cn

[Q60] 取上一行 / 下一行
来源：http://gr.wgjwhj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ol.shtwfgs.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kw.gzmigu.cn

[Q61] 移动平均
来源：http://rb.wgjwhj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nh.521024.cn

[Q62] 分组占比
来源：http://mk.huixiangedu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hp.shxzukj.cn

[Q63] 开启事务
来源：http://gl.haigaiapp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qq.shxzskj.cn

[Q64] 提交事务
来源：http://ui.szxytkj.cn

COMMIT;
来源：http://rj.hahajie.cn

[Q65] 回滚事务
来源：http://ru.jctech888.com.cn

ROLLBACK;
来源：http://nm.haigaiapp.cn

[Q66] 行锁查询
来源：http://yr.lnxyls.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dv.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://ya.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yf.nicolike.cn

[Q68] 保存点
来源：http://ft.lnxyls.cn

SAVEPOINT sp1;
来源：http://fb.colortex.cn

ROLLBACK TO sp1;
来源：http://tr.gzmigu.cn

[Q69] 查看执行计划
来源：http://lk.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kn.gzmigu.cn

[Q70] 更新统计信息
来源：http://ma.lnxyls.cn

ANALYZE TABLE users;
来源：http://vl.muxihuayi.cn

[Q71] 查看建表语句
来源：http://wj.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cs.bjjhwx.cn

[Q72] 查看索引
来源：http://qm.panjiajie.cn

SHOW INDEX FROM users;
来源：http://mj.bjjhwx.cn

[Q73] 查看表状态
来源：http://gh.jctech888.com.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hx.bjjhwx.cn

[Q74] 强制使用索引
来源：http://xr.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ey.shtwfgs.cn

[Q75] 日期格式化
来源：http://xc.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://py.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vh.lnxyls.cn

[Q76] 按天统计
来源：http://wg.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hi.wgjwhj.cn

[Q77] 时间加减
来源：http://hc.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ab.9csxet.cn

[Q78] 当前时间
来源：http://vk.nszjky.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lk.9csxet.cn

[Q79] 字符串拼接
来源：http://kw.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sx.szxytkj.cn

[Q80] 字符串截取
来源：http://lx.nicolike.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lj.jctech888.com.cn

[Q81] 字符串替换
来源：http://hv.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iy.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://ij.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ar.newstarts.cn

[Q83] 大小写转换
来源：http://uj.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gv.9csxet.cn

[Q84] 去除首尾空格
来源：http://rb.newstarts.cn

SELECT TRIM(name) FROM users;
来源：http://hi.9csxet.cn

[Q85] 数值取整
来源：http://el.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ig.colortex.cn

[Q86] 读取 JSON 字段
来源：http://yj.wgjwhj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ze.nszjky.cn

[Q87] JSON 字段做条件
来源：http://ad.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dr.chemitech.net.cn

[Q88] 行转列（条件聚合）
来源：http://tf.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://so.nszjky.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eg.nszjky.cn

[Q89] 判断表是否存在
来源：http://qg.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oy.colortex.cn

[Q90] 生成序号列
来源：http://no.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pf.yuntaijiaju.cn

================================================================================
来源：http://ch.szsharing.cn

R. Bash 专题
来源：http://gt.panjiajie.cn

================================================================================
来源：http://za.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://gv.nicolike.cn

#!/usr/bin/env bash
来源：http://sa.chemitech.net.cn

set -euo pipefail
来源：http://yl.newstarts.cn

[R02] 变量赋值与使用
来源：http://pv.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://kx.muxihuayi.cn

[R03] 只读变量
来源：http://ua.shxzskj.cn

readonly PI=3.14
来源：http://zn.yuexingan06.cn

[R04] 位置参数
来源：http://jj.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wk.bjjhwx.cn

[R05] 参数默认值
来源：http://bs.lnxyls.cn

name="${1:-default}"
来源：http://ev.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://qv.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uf.szsharing.cn

[R07] if 判断文件
来源：http://ez.bjjhwx.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pj.haigaiapp.cn

[R08] 数值比较
来源：http://qa.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dq.hahajie.cn

[R09] 字符串比较
来源：http://fm.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ea.521024.cn

[R10] 正则匹配
来源：http://ru.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dy.nszjky.cn

[R11] case 多分支
来源：http://vb.9csxet.cn

case "$1" in
来源：http://tn.colortex.cn

start) echo "启动" ;;
来源：http://or.huanxung.cn

stop)  echo "停止" ;;
来源：http://ld.gzmigu.cn

*)     echo "未知命令" ;;
来源：http://lj.nicolike.cn

esac
来源：http://ls.haigaiapp.cn

[R12] for 遍历文件
来源：http://gg.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://jf.521024.cn

[R13] for 计数循环
来源：http://bl.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://sm.chemitech.net.cn

[R14] C 风格 for
来源：http://li.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gj.9csxet.cn

[R15] while 逐行读文件
来源：http://sk.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://em.hnjuh.cn

[R16] until 等待条件
来源：http://gu.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mn.huixinmuqiang.cn

[R17] 数组定义与取值
来源：http://nt.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://iq.wgjwhj.cn

[R18] 遍历数组
来源：http://jy.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hj.newstarts.cn

[R19] 数组长度
来源：http://qq.yuexingan06.cn

echo "${#arr[@]}"
来源：http://jv.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://ip.nszjky.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fk.9csxet.cn

[R21] 字符串长度
来源：http://oh.huixinmuqiang.cn

echo "${#s}"
来源：http://ty.newstarts.cn

[R22] 截取子串
来源：http://aq.nicolike.cn

echo "${s:0:5}"
来源：http://bo.huanxung.cn

[R23] 字符串替换
来源：http://qk.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tz.521024.cn

[R24] 大小写转换
来源：http://qv.hnjuh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wq.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://hb.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lu.panjiajie.cn

[R26] 命令替换
来源：http://cg.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://rd.yuntaijiaju.cn

[R27] 算术展开
来源：http://nt.gzmigu.cn

echo $((1 + 2 * 3))
来源：http://ec.shxzskj.cn

[R28] 浮点运算
来源：http://rg.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://sd.nicolike.cn

[R29] 定义函数
来源：http://ch.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://my.nicolike.cn

[R30] 函数返回状态码
来源：http://od.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://wd.jianghongdianzi.cn

[R31] 局部变量
来源：http://jh.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://kw.9csxet.cn

[R32] 参数个数校验
来源：http://zk.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qa.jctech888.com.cn

[R33] 捕获错误并提示行号
来源：http://fd.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ye.nicolike.cn

[R34] 退出时清理
来源：http://nc.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yc.yuexingan06.cn

[R35] 后台执行并等待
来源：http://br.nicolike.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://in.nicolike.cn

[R36] 并发执行多个任务
来源：http://xr.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pg.nicolike.cn

[R37] 把输出赋给变量
来源：http://vr.chemitech.net.cn

files=$(ls -1)
来源：http://gw.shxzukj.cn

[R38] 管道串联
来源：http://yb.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://ql.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://ox.shxzukj.cn

cmd > out.log 2>&1
来源：http://iy.bjjhwx.cn

[R40] 追加写日志
来源：http://tv.huixinmuqiang.cn

echo "log" >> out.log
来源：http://iy.bookmarksfly.cn

[R41] 丢弃输出
来源：http://qm.yuntaijiaju.cn

cmd >/dev/null 2>&1
来源：http://km.huixiangedu.cn

[R42] 输入重定向
来源：http://kt.lnxyls.cn

wc -l < a.txt
来源：http://kp.szsharing.cn

[R43] 按名字查找文件
来源：http://go.hnjuh.cn

find . -name "*.log" -type f
来源：http://no.haigaiapp.cn

[R44] 按修改时间查找
来源：http://xc.huanxung.cn

find . -mtime -7 -type f
来源：http://hb.yuexingan06.cn

[R45] 批量删除
来源：http://ic.9csxet.cn

find . -name "*.tmp" -delete
来源：http://yz.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://ml.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dw.jianghongdianzi.cn

[R47] sed 单行替换
来源：http://xa.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vd.shxzukj.cn

[R48] awk 取指定列
来源：http://tp.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://nu.521024.cn

[R49] awk 带条件
来源：http://wj.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qo.huanxung.cn

[R50] awk 求和
来源：http://zo.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ww.521024.cn

[R51] 排序去重取前几
来源：http://ag.nszjky.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hx.huixiangedu.cn

[R52] 统计行数
来源：http://bd.jctech888.com.cn

wc -l a.txt
来源：http://di.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://ja.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vs.bookmarksfly.cn

[R54] 比较两个文件
来源：http://jn.yuntaijiaju.cn

diff a.txt b.txt
来源：http://dz.jctech888.com.cn

[R55] 压缩与解压
来源：http://tq.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://to.hnjuh.cn

[R56] 远程拷贝
来源：http://wf.shxzukj.cn

scp file user@host:/path/
来源：http://xy.bookmarksfly.cn

[R57] 远程执行命令
来源：http://lc.szxytkj.cn

ssh user@host 'uptime'
来源：http://if.huanxung.cn

[R58] 下载文件
来源：http://zi.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://be.hnjuh.cn

[R59] 发 POST JSON
来源：http://hn.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sf.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://ky.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gs.bookmarksfly.cn

[R61] 磁盘占用
来源：http://rm.asd995.cn

df -h;  du -sh *
来源：http://ey.newstarts.cn

[R62] 找最占空间的文件
来源：http://lq.jctech888.com.cn

du -ah . | sort -rh | head -10
来源：http://tq.nicolike.cn

[R63] 内存与进程
来源：http://qj.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://pt.shxzukj.cn

[R64] 结束进程
来源：http://oq.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://ut.huixiangedu.cn

[R65] 查看端口占用
来源：http://wo.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jl.chemitech.net.cn

[R66] 定时任务
来源：http://gh.muxihuayi.cn

crontab -e;  crontab -l
来源：http://fu.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://co.haigaiapp.cn

openssl rand -hex 16
来源：http://ll.wgjwhj.cn

[R68] 计算文件校验值
来源：http://qy.521024.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xo.hnjuh.cn

[R69] 生成随机密码
来源：http://cd.huanxung.cn

head -c 16 /dev/urandom | base64
来源：http://hy.huanxung.cn

[R70] 时间戳与互转
来源：http://qt.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://fe.huixiangedu.cn

[R71] 日期格式化
来源：http://hs.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kx.shxzukj.cn

[R72] 等待端口就绪
来源：http://iz.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://li.nicolike.cn

[R73] 分割大日志
来源：http://lw.shxzukj.cn

split -l 1000 big.log part_
来源：http://cn.nszjky.cn

[R74] 批量重命名
来源：http://uc.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ne.9csxet.cn

[R75] 导出环境变量
来源：http://pi.szsharing.cn

export PATH="$HOME/bin:$PATH"
来源：http://fi.shtwfgs.cn

[R76] 使用临时文件
来源：http://sb.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yp.jctech888.com.cn

[R77] 读取用户输入
来源：http://df.shtwfgs.cn

read -rp "请输入: " ans
来源：http://rl.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://wf.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ww.hahajie.cn

[R79] 解析命令行选项
来源：http://kz.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ua.521024.cn

[R80] 查看脚本执行耗时
来源：http://gl.chemitech.net.cn

time ./run.sh
来源：http://xw.yuexingan06.cn

================================================================================
来源：http://aj.colortex.cn

S. C / C++ 专题
来源：http://jh.newstarts.cn

================================================================================
来源：http://nz.hnjuh.cn

[S01] C：Hello World
来源：http://dl.chemitech.net.cn

#include <stdio.h>
来源：http://by.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ac.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://un.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://jt.shxzukj.cn

[S03] C：读入整数
来源：http://rr.bookmarksfly.cn


<!-- 参考信息 -->