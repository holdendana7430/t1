代发 wailian999

[Q36] 左连接
来源：http://ar.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://oy.shxzukj.cn

[Q37] 右连接
来源：http://gc.9csxet.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ub.yuntaijiaju.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pj.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://md.asd995.cn

[Q39] 自连接（查上下级）
来源：http://jg.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gq.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ie.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ai.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mn.bookmarksfly.cn

[Q41] 多表连接
来源：http://oh.shxzskj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://iq.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://oq.nicolike.cn

JOIN products p ON p.id = o.product_id;
来源：http://nv.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://ps.chemitech.net.cn

SELECT u.name, o.amount FROM users u
来源：http://yk.bookmarksfly.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ml.huanxung.cn

[Q43] 标量子查询
来源：http://ti.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xw.jianghongdianzi.cn

[Q44] IN 子查询
来源：http://ls.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://va.szsharing.cn

[Q45] EXISTS 判断存在
来源：http://hm.nicolike.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://io.asd995.cn

[Q46] NOT EXISTS 判断不存在
来源：http://we.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://na.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://dh.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fm.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://xm.shtwfgs.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://le.huanxung.cn

SELECT * FROM t WHERE c > 5;
来源：http://tp.nszjky.cn

[Q49] 更新单行
来源：http://nq.jianghongdianzi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nk.shxzskj.cn

[Q50] 批量更新
来源：http://tu.muxihuayi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hv.asd995.cn

[Q51] 用子查询更新
来源：http://mn.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://il.bookmarksfly.cn

[Q52] 删除指定行
来源：http://eb.nicolike.cn

DELETE FROM users WHERE id = 10;
来源：http://vb.nicolike.cn

[Q53] 按条件删除
来源：http://ck.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ex.bjjhwx.cn

[Q54] 清空表
来源：http://po.szsharing.cn

TRUNCATE TABLE logs;
来源：http://ks.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://ex.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yj.shtwfgs.cn

[Q56] 密集排名（并列不占位）
来源：http://ot.bjjhwx.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hs.huixinmuqiang.cn

[Q57] 行号
来源：http://sp.jianghongdianzi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xm.huixiangedu.cn

[Q58] 累计求和
来源：http://fp.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ko.shtwfgs.cn

[Q59] 分组内累计
来源：http://kb.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gv.gzmigu.cn

[Q60] 取上一行 / 下一行
来源：http://ad.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ro.haigaiapp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kb.wgjwhj.cn

[Q61] 移动平均
来源：http://vo.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ob.hnjuh.cn

[Q62] 分组占比
来源：http://lq.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xe.gzmigu.cn

[Q63] 开启事务
来源：http://oi.nicolike.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://im.newstarts.cn

[Q64] 提交事务
来源：http://hi.nicolike.cn

COMMIT;
来源：http://dg.colortex.cn

[Q65] 回滚事务
来源：http://uq.nicolike.cn

ROLLBACK;
来源：http://od.panjiajie.cn

[Q66] 行锁查询
来源：http://wn.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wj.jctech888.com.cn

[Q67] 设置隔离级别
来源：http://zy.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ui.hahajie.cn

[Q68] 保存点
来源：http://jk.chemitech.net.cn

SAVEPOINT sp1;
来源：http://li.shxzskj.cn

ROLLBACK TO sp1;
来源：http://mf.jctech888.com.cn

[Q69] 查看执行计划
来源：http://xa.bookmarksfly.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uy.asd995.cn

[Q70] 更新统计信息
来源：http://aa.nszjky.cn

ANALYZE TABLE users;
来源：http://il.shxzukj.cn

[Q71] 查看建表语句
来源：http://ze.nicolike.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ge.szsharing.cn

[Q72] 查看索引
来源：http://oq.shxzukj.cn

SHOW INDEX FROM users;
来源：http://bb.wgjwhj.cn

[Q73] 查看表状态
来源：http://ef.chemitech.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://og.nszjky.cn

[Q74] 强制使用索引
来源：http://bz.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ds.nszjky.cn

[Q75] 日期格式化
来源：http://nc.huanxung.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kt.newstarts.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cl.huixinmuqiang.cn

[Q76] 按天统计
来源：http://dv.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zr.colortex.cn

[Q77] 时间加减
来源：http://tp.hahajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ia.huixiangedu.cn

[Q78] 当前时间
来源：http://tx.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jy.muxihuayi.cn

[Q79] 字符串拼接
来源：http://xc.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xv.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://kp.chemitech.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ma.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://jf.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gr.panjiajie.cn

[Q82] 字符长度与字节长度
来源：http://bk.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uq.szsharing.cn

[Q83] 大小写转换
来源：http://zo.gzmigu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cs.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://gt.lnxyls.cn

SELECT TRIM(name) FROM users;
来源：http://ky.hnjuh.cn

[Q85] 数值取整
来源：http://sr.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vg.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://il.nicolike.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jz.yuexingan06.cn

[Q87] JSON 字段做条件
来源：http://wv.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nr.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://zt.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://at.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jp.hnjuh.cn

[Q89] 判断表是否存在
来源：http://pc.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hx.asd995.cn

[Q90] 生成序号列
来源：http://xu.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bt.yuntaijiaju.cn

================================================================================
来源：http://ej.bjjhwx.cn

R. Bash 专题
来源：http://nd.huixiangedu.cn

================================================================================
来源：http://qa.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://nu.huanxung.cn

#!/usr/bin/env bash
来源：http://mr.nicolike.cn

set -euo pipefail
来源：http://pk.shxzukj.cn

[R02] 变量赋值与使用
来源：http://av.nszjky.cn

name="Tom"; echo "$name"
来源：http://uo.yuexingan06.cn

[R03] 只读变量
来源：http://te.szsharing.cn

readonly PI=3.14
来源：http://jo.gzmigu.cn

[R04] 位置参数
来源：http://pd.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mt.jctech888.com.cn

[R05] 参数默认值
来源：http://pd.szxytkj.cn

name="${1:-default}"
来源：http://gr.wgjwhj.cn

[R06] 判断命令是否存在
来源：http://lr.asd995.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lq.muxihuayi.cn

[R07] if 判断文件
来源：http://yn.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://py.nicolike.cn

[R08] 数值比较
来源：http://qn.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ax.yuexingan06.cn

[R09] 字符串比较
来源：http://ri.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hs.panjiajie.cn

[R10] 正则匹配
来源：http://qp.lnxyls.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zc.bjjhwx.cn

[R11] case 多分支
来源：http://tt.asd995.cn

case "$1" in
来源：http://ne.haigaiapp.cn

start) echo "启动" ;;
来源：http://wt.haigaiapp.cn

stop)  echo "停止" ;;
来源：http://do.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://em.521024.cn

esac
来源：http://fd.szxytkj.cn

[R12] for 遍历文件
来源：http://ya.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://qc.colortex.cn

[R13] for 计数循环
来源：http://su.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://kc.jctech888.com.cn

[R14] C 风格 for
来源：http://bz.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://az.asd995.cn

[R15] while 逐行读文件
来源：http://ua.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vh.chemitech.net.cn

[R16] until 等待条件
来源：http://eu.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ys.chemitech.net.cn

[R17] 数组定义与取值
来源：http://rc.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bp.yuexingan06.cn

[R18] 遍历数组
来源：http://dj.szsharing.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yw.szsharing.cn

[R19] 数组长度
来源：http://cw.nicolike.cn

echo "${#arr[@]}"
来源：http://ah.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://qb.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ol.nszjky.cn

[R21] 字符串长度
来源：http://uj.huanxung.cn

echo "${#s}"
来源：http://fx.szxytkj.cn

[R22] 截取子串
来源：http://se.hnjuh.cn

echo "${s:0:5}"
来源：http://vw.chemitech.net.cn

[R23] 字符串替换
来源：http://xt.bjjhwx.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pq.szxytkj.cn

[R24] 大小写转换
来源：http://si.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lv.panjiajie.cn

[R25] 去后缀 / 去前缀
来源：http://wu.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://by.shxzskj.cn

[R26] 命令替换
来源：http://gu.chemitech.net.cn

now=$(date +%F); echo "$now"
来源：http://ij.chemitech.net.cn

[R27] 算术展开
来源：http://wl.9csxet.cn

echo $((1 + 2 * 3))
来源：http://ma.muxihuayi.cn

[R28] 浮点运算
来源：http://qh.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://ri.huixiangedu.cn

[R29] 定义函数
来源：http://nw.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wq.lnxyls.cn

[R30] 函数返回状态码
来源：http://gj.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://ji.nicolike.cn

[R31] 局部变量
来源：http://ak.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://ec.bjjhwx.cn

[R32] 参数个数校验
来源：http://pp.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pv.yuntaijiaju.cn

[R33] 捕获错误并提示行号
来源：http://pp.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nu.nszjky.cn

[R34] 退出时清理
来源：http://mp.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nf.panjiajie.cn

[R35] 后台执行并等待
来源：http://mk.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nu.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://ib.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vn.nszjky.cn

[R37] 把输出赋给变量
来源：http://pu.hnjuh.cn

files=$(ls -1)
来源：http://xy.szxytkj.cn

[R38] 管道串联
来源：http://rp.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://qr.panjiajie.cn

[R39] 重定向标准输出与错误
来源：http://mj.shxzukj.cn

cmd > out.log 2>&1
来源：http://vr.huanxung.cn

[R40] 追加写日志
来源：http://pf.wgjwhj.cn

echo "log" >> out.log
来源：http://qx.jctech888.com.cn

[R41] 丢弃输出
来源：http://bg.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://gz.wgjwhj.cn

[R42] 输入重定向
来源：http://yl.yuexingan06.cn

wc -l < a.txt
来源：http://kd.newstarts.cn

[R43] 按名字查找文件
来源：http://sg.jctech888.com.cn

find . -name "*.log" -type f
来源：http://ae.shxzskj.cn

[R44] 按修改时间查找
来源：http://za.panjiajie.cn

find . -mtime -7 -type f
来源：http://oi.yuexingan06.cn

[R45] 批量删除
来源：http://of.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://ah.newstarts.cn

[R46] 递归替换文件内容
来源：http://fu.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uv.shxzskj.cn

[R47] sed 单行替换
来源：http://zi.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ei.huixiangedu.cn

[R48] awk 取指定列
来源：http://pl.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://as.hnjuh.cn

[R49] awk 带条件
来源：http://pa.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yr.shxzukj.cn

[R50] awk 求和
来源：http://co.bookmarksfly.cn

awk '{s += $2} END {print s}' a.txt
来源：http://oj.nicolike.cn

[R51] 排序去重取前几
来源：http://gq.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bw.shxzskj.cn

[R52] 统计行数
来源：http://yj.jianghongdianzi.cn

wc -l a.txt
来源：http://wc.panjiajie.cn

[R53] 查看文件头与实时尾
来源：http://st.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oc.chemitech.net.cn

[R54] 比较两个文件
来源：http://pu.jctech888.com.cn

diff a.txt b.txt
来源：http://wp.shtwfgs.cn

[R55] 压缩与解压
来源：http://ji.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zh.shtwfgs.cn

[R56] 远程拷贝
来源：http://wd.nicolike.cn

scp file user@host:/path/
来源：http://wl.nicolike.cn

[R57] 远程执行命令
来源：http://ng.bookmarksfly.cn

ssh user@host 'uptime'
来源：http://jd.9csxet.cn

[R58] 下载文件
来源：http://gc.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://db.panjiajie.cn

[R59] 发 POST JSON
来源：http://xo.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mc.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://lw.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qn.gzmigu.cn

[R61] 磁盘占用
来源：http://he.szxytkj.cn

df -h;  du -sh *
来源：http://hg.szxytkj.cn

[R62] 找最占空间的文件
来源：http://rj.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://tm.colortex.cn

[R63] 内存与进程
来源：http://hb.yuntaijiaju.cn

free -h;  ps aux | grep nginx
来源：http://ha.shxzukj.cn

[R64] 结束进程
来源：http://ya.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://xm.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://dz.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yz.jctech888.com.cn

[R66] 定时任务
来源：http://hx.newstarts.cn

crontab -e;  crontab -l
来源：http://ip.haigaiapp.cn

[R67] 生成随机十六进制串
来源：http://mi.jctech888.com.cn

openssl rand -hex 16
来源：http://ex.jctech888.com.cn

[R68] 计算文件校验值
来源：http://wg.lnxyls.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jb.muxihuayi.cn

[R69] 生成随机密码
来源：http://xk.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://au.hahajie.cn

[R70] 时间戳与互转
来源：http://xy.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://ri.hahajie.cn

[R71] 日期格式化
来源：http://lk.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kd.yuexingan06.cn

[R72] 等待端口就绪
来源：http://dj.huixinmuqiang.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vb.colortex.cn

[R73] 分割大日志
来源：http://mf.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://ny.yuexingan06.cn

[R74] 批量重命名
来源：http://vf.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nv.hahajie.cn

[R75] 导出环境变量
来源：http://gp.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://hd.haigaiapp.cn

[R76] 使用临时文件
来源：http://nr.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ty.asd995.cn

[R77] 读取用户输入
来源：http://ge.colortex.cn

read -rp "请输入: " ans
来源：http://tr.yuexingan06.cn

[R78] 交互式菜单
来源：http://vh.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jr.shxzskj.cn

[R79] 解析命令行选项
来源：http://ts.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://of.asd995.cn

[R80] 查看脚本执行耗时
来源：http://zu.wgjwhj.cn

time ./run.sh
来源：http://pq.shtwfgs.cn

================================================================================
来源：http://wd.huanxung.cn

S. C / C++ 专题
来源：http://qj.szxytkj.cn

================================================================================
来源：http://nb.szxytkj.cn

[S01] C：Hello World
来源：http://ty.huixiangedu.cn

#include <stdio.h>
来源：http://on.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gw.shtwfgs.cn

[S02] C：变量与格式化输出
来源：http://dt.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://gl.yuntaijiaju.cn

[S03] C：读入整数
来源：http://hf.shxzukj.cn

int x; scanf("%d", &x);
来源：http://qj.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://hp.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://an.haigaiapp.cn

[S05] C：字符串长度
来源：http://el.newstarts.cn


<!-- 参考信息 -->