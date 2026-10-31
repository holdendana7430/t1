代发 wailian999

[Q36] 左连接
来源：http://dt.nicolike.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rk.gzmigu.cn

[Q37] 右连接
来源：http://rv.bjjhwx.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wx.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jp.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qa.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://pb.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yn.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ny.nicolike.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bo.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zs.bjjhwx.cn

[Q41] 多表连接
来源：http://ft.nicolike.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fk.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://ak.haigaiapp.cn

JOIN products p ON p.id = o.product_id;
来源：http://px.jctech888.com.cn

[Q42] 连接条件附加过滤
来源：http://cu.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://me.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jb.jctech888.com.cn

[Q43] 标量子查询
来源：http://tz.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wn.szsharing.cn

[Q44] IN 子查询
来源：http://op.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xg.szxytkj.cn

[Q45] EXISTS 判断存在
来源：http://qy.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sn.chemitech.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ip.panjiajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yh.haigaiapp.cn

[Q47] 与平均值比较
来源：http://tf.szsharing.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gb.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://zy.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://od.bookmarksfly.cn

SELECT * FROM t WHERE c > 5;
来源：http://fi.huixiangedu.cn

[Q49] 更新单行
来源：http://wa.jianghongdianzi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ie.bjjhwx.cn

[Q50] 批量更新
来源：http://nt.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ii.hahajie.cn

[Q51] 用子查询更新
来源：http://tv.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lh.shxzskj.cn

[Q52] 删除指定行
来源：http://vy.huanxung.cn

DELETE FROM users WHERE id = 10;
来源：http://hf.hnjuh.cn

[Q53] 按条件删除
来源：http://cv.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sz.yuexingan06.cn

[Q54] 清空表
来源：http://zk.bjjhwx.cn

TRUNCATE TABLE logs;
来源：http://xo.huanxung.cn

[Q55] 排名（并列占位）
来源：http://cw.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bl.nicolike.cn

[Q56] 密集排名（并列不占位）
来源：http://bb.colortex.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vu.huixinmuqiang.cn

[Q57] 行号
来源：http://ha.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qz.gzmigu.cn

[Q58] 累计求和
来源：http://tw.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hx.hnjuh.cn

[Q59] 分组内累计
来源：http://db.panjiajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vo.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://wn.chemitech.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cg.haigaiapp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sr.yuexingan06.cn

[Q61] 移动平均
来源：http://aa.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tr.nszjky.cn

[Q62] 分组占比
来源：http://kf.9csxet.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tq.panjiajie.cn

[Q63] 开启事务
来源：http://dv.yuexingan06.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sx.chemitech.net.cn

[Q64] 提交事务
来源：http://by.huanxung.cn

COMMIT;
来源：http://pc.shxzskj.cn

[Q65] 回滚事务
来源：http://yn.muxihuayi.cn

ROLLBACK;
来源：http://aa.nicolike.cn

[Q66] 行锁查询
来源：http://vv.szsharing.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kv.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://qw.panjiajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zd.shtwfgs.cn

[Q68] 保存点
来源：http://ie.szsharing.cn

SAVEPOINT sp1;
来源：http://il.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://jb.huixiangedu.cn

[Q69] 查看执行计划
来源：http://yf.wgjwhj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ya.wgjwhj.cn

[Q70] 更新统计信息
来源：http://ob.hahajie.cn

ANALYZE TABLE users;
来源：http://fk.szxytkj.cn

[Q71] 查看建表语句
来源：http://rr.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ys.panjiajie.cn

[Q72] 查看索引
来源：http://xs.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://fp.asd995.cn

[Q73] 查看表状态
来源：http://ub.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zb.huixiangedu.cn

[Q74] 强制使用索引
来源：http://al.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tl.newstarts.cn

[Q75] 日期格式化
来源：http://ii.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://at.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xu.521024.cn

[Q76] 按天统计
来源：http://yp.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fk.colortex.cn

[Q77] 时间加减
来源：http://io.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wv.jctech888.com.cn

[Q78] 当前时间
来源：http://db.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://br.hahajie.cn

[Q79] 字符串拼接
来源：http://ve.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fc.muxihuayi.cn

[Q80] 字符串截取
来源：http://kz.shxzukj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zz.nszjky.cn

[Q81] 字符串替换
来源：http://lq.muxihuayi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vn.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://fa.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vr.bookmarksfly.cn

[Q83] 大小写转换
来源：http://ax.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ue.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://as.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://ey.hnjuh.cn

[Q85] 数值取整
来源：http://we.shtwfgs.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vm.szxytkj.cn

[Q86] 读取 JSON 字段
来源：http://dq.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yl.bjjhwx.cn

[Q87] JSON 字段做条件
来源：http://yd.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://io.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://wd.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://th.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ku.gzmigu.cn

[Q89] 判断表是否存在
来源：http://ht.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oa.huanxung.cn

[Q90] 生成序号列
来源：http://oc.shxzukj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ch.bjjhwx.cn

================================================================================
来源：http://rl.jctech888.com.cn

R. Bash 专题
来源：http://xr.shxzskj.cn

================================================================================
来源：http://tk.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://fm.9csxet.cn

#!/usr/bin/env bash
来源：http://gm.hnjuh.cn

set -euo pipefail
来源：http://ax.szxytkj.cn

[R02] 变量赋值与使用
来源：http://nz.nicolike.cn

name="Tom"; echo "$name"
来源：http://vn.bookmarksfly.cn

[R03] 只读变量
来源：http://dw.huanxung.cn

readonly PI=3.14
来源：http://yv.shtwfgs.cn

[R04] 位置参数
来源：http://nw.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ax.lnxyls.cn

[R05] 参数默认值
来源：http://fi.gzmigu.cn

name="${1:-default}"
来源：http://au.szsharing.cn

[R06] 判断命令是否存在
来源：http://zz.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://av.jctech888.com.cn

[R07] if 判断文件
来源：http://wq.panjiajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bw.huixiangedu.cn

[R08] 数值比较
来源：http://ti.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jy.chemitech.net.cn

[R09] 字符串比较
来源：http://lw.jctech888.com.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ad.9csxet.cn

[R10] 正则匹配
来源：http://yv.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qv.chemitech.net.cn

[R11] case 多分支
来源：http://ot.wgjwhj.cn

case "$1" in
来源：http://bj.muxihuayi.cn

start) echo "启动" ;;
来源：http://di.szsharing.cn

stop)  echo "停止" ;;
来源：http://pf.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://zx.szsharing.cn

esac
来源：http://xk.yuexingan06.cn

[R12] for 遍历文件
来源：http://tc.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://nh.9csxet.cn

[R13] for 计数循环
来源：http://xi.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://ce.panjiajie.cn

[R14] C 风格 for
来源：http://pr.hahajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yh.newstarts.cn

[R15] while 逐行读文件
来源：http://sn.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wz.bjjhwx.cn

[R16] until 等待条件
来源：http://qk.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ho.haigaiapp.cn

[R17] 数组定义与取值
来源：http://pg.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pm.asd995.cn

[R18] 遍历数组
来源：http://cn.szxytkj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nj.bjjhwx.cn

[R19] 数组长度
来源：http://dk.asd995.cn

echo "${#arr[@]}"
来源：http://in.huanxung.cn

[R20] 关联数组（字典）
来源：http://un.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zo.nszjky.cn

[R21] 字符串长度
来源：http://gw.bjjhwx.cn

echo "${#s}"
来源：http://az.jctech888.com.cn

[R22] 截取子串
来源：http://sz.gzmigu.cn

echo "${s:0:5}"
来源：http://cg.nicolike.cn

[R23] 字符串替换
来源：http://oc.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nz.yuexingan06.cn

[R24] 大小写转换
来源：http://nf.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uk.yuntaijiaju.cn

[R25] 去后缀 / 去前缀
来源：http://pw.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xh.nicolike.cn

[R26] 命令替换
来源：http://lu.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://rj.shxzskj.cn

[R27] 算术展开
来源：http://mv.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://zs.bookmarksfly.cn

[R28] 浮点运算
来源：http://rt.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://ws.hnjuh.cn

[R29] 定义函数
来源：http://bb.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lo.haigaiapp.cn

[R30] 函数返回状态码
来源：http://mq.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://zh.shxzskj.cn

[R31] 局部变量
来源：http://lr.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://gg.9csxet.cn

[R32] 参数个数校验
来源：http://lk.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sa.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://kx.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gc.shxzukj.cn

[R34] 退出时清理
来源：http://st.chemitech.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dq.nicolike.cn

[R35] 后台执行并等待
来源：http://kl.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xs.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://ml.shxzskj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cf.gzmigu.cn

[R37] 把输出赋给变量
来源：http://rz.nicolike.cn

files=$(ls -1)
来源：http://ms.jctech888.com.cn

[R38] 管道串联
来源：http://zy.szxytkj.cn

cat a.txt | grep -i error | wc -l
来源：http://ck.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://ab.521024.cn

cmd > out.log 2>&1
来源：http://bl.chemitech.net.cn

[R40] 追加写日志
来源：http://bk.gzmigu.cn

echo "log" >> out.log
来源：http://uz.huixiangedu.cn

[R41] 丢弃输出
来源：http://ej.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://xx.huixinmuqiang.cn

[R42] 输入重定向
来源：http://lp.yuexingan06.cn

wc -l < a.txt
来源：http://di.lnxyls.cn

[R43] 按名字查找文件
来源：http://wi.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://kb.yuexingan06.cn

[R44] 按修改时间查找
来源：http://ef.huanxung.cn

find . -mtime -7 -type f
来源：http://rr.huixiangedu.cn

[R45] 批量删除
来源：http://oa.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://kt.szxytkj.cn

[R46] 递归替换文件内容
来源：http://es.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://aq.gzmigu.cn

[R47] sed 单行替换
来源：http://te.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qa.hahajie.cn

[R48] awk 取指定列
来源：http://gp.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://fw.huixiangedu.cn

[R49] awk 带条件
来源：http://so.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lu.newstarts.cn

[R50] awk 求和
来源：http://ju.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rg.huixiangedu.cn

[R51] 排序去重取前几
来源：http://ra.lnxyls.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bv.haigaiapp.cn

[R52] 统计行数
来源：http://hp.huixiangedu.cn

wc -l a.txt
来源：http://kv.panjiajie.cn

[R53] 查看文件头与实时尾
来源：http://ek.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ou.nszjky.cn

[R54] 比较两个文件
来源：http://vl.jctech888.com.cn

diff a.txt b.txt
来源：http://yj.yuexingan06.cn

[R55] 压缩与解压
来源：http://ix.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bd.bjjhwx.cn

[R56] 远程拷贝
来源：http://dl.huixiangedu.cn

scp file user@host:/path/
来源：http://vr.szxytkj.cn

[R57] 远程执行命令
来源：http://vh.asd995.cn

ssh user@host 'uptime'
来源：http://by.chemitech.net.cn

[R58] 下载文件
来源：http://oj.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bl.hnjuh.cn

[R59] 发 POST JSON
来源：http://gw.yuexingan06.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://um.521024.cn

[R60] 只看 HTTP 状态码
来源：http://uc.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dv.nicolike.cn

[R61] 磁盘占用
来源：http://eo.jctech888.com.cn

df -h;  du -sh *
来源：http://be.huixinmuqiang.cn

[R62] 找最占空间的文件
来源：http://va.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://eo.newstarts.cn

[R63] 内存与进程
来源：http://er.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://xo.newstarts.cn

[R64] 结束进程
来源：http://nh.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://px.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://kz.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://za.colortex.cn

[R66] 定时任务
来源：http://zd.gzmigu.cn

crontab -e;  crontab -l
来源：http://np.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://oa.newstarts.cn

openssl rand -hex 16
来源：http://vv.szsharing.cn

[R68] 计算文件校验值
来源：http://pc.hnjuh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://in.panjiajie.cn

[R69] 生成随机密码
来源：http://rr.colortex.cn

head -c 16 /dev/urandom | base64
来源：http://cy.bjjhwx.cn

[R70] 时间戳与互转
来源：http://mw.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://zf.huixinmuqiang.cn

[R71] 日期格式化
来源：http://fc.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xu.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://pu.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tk.muxihuayi.cn

[R73] 分割大日志
来源：http://ft.asd995.cn

split -l 1000 big.log part_
来源：http://qj.bookmarksfly.cn

[R74] 批量重命名
来源：http://ya.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kg.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://bi.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://gr.shxzskj.cn

[R76] 使用临时文件
来源：http://zi.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kp.9csxet.cn

[R77] 读取用户输入
来源：http://py.panjiajie.cn

read -rp "请输入: " ans
来源：http://kf.huanxung.cn

[R78] 交互式菜单
来源：http://ph.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tt.shxzskj.cn

[R79] 解析命令行选项
来源：http://sx.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://se.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://ym.bookmarksfly.cn

time ./run.sh
来源：http://vg.gzmigu.cn

================================================================================
来源：http://ip.bookmarksfly.cn

S. C / C++ 专题
来源：http://sk.521024.cn

================================================================================
来源：http://ok.szxytkj.cn

[S01] C：Hello World
来源：http://mg.jianghongdianzi.cn

#include <stdio.h>
来源：http://tv.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pc.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://xh.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://zx.521024.cn

[S03] C：读入整数
来源：http://ap.newstarts.cn

int x; scanf("%d", &x);
来源：http://zg.nszjky.cn

[S04] C：字符串复制
来源：http://qx.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xj.hahajie.cn

[S05] C：字符串长度
来源：http://yd.szsharing.cn


<!-- 参考信息 -->