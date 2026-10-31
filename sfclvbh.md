代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qt.nicolike.cn

) t WHERE rn = 1;
来源：http://bq.bookmarksfly.cn

[Q35] 内连接
来源：http://xz.bookmarksfly.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sg.szsharing.cn

[Q36] 左连接
来源：http://oa.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tu.panjiajie.cn

[Q37] 右连接
来源：http://th.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hd.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zh.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zs.hnjuh.cn

[Q39] 自连接（查上下级）
来源：http://zw.521024.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zl.shxzukj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://my.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sj.shxzukj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yd.hnjuh.cn

[Q41] 多表连接
来源：http://pr.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vl.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://wa.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://tu.shtwfgs.cn

[Q42] 连接条件附加过滤
来源：http://mg.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://yf.shtwfgs.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sj.newstarts.cn

[Q43] 标量子查询
来源：http://kr.szxytkj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jl.szxytkj.cn

[Q44] IN 子查询
来源：http://du.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lm.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://ky.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qg.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://je.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qu.muxihuayi.cn

[Q47] 与平均值比较
来源：http://df.haigaiapp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://as.521024.cn

[Q48] CTE 公用表表达式
来源：http://ou.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kq.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://on.shxzukj.cn

[Q49] 更新单行
来源：http://sj.yuntaijiaju.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ox.bjjhwx.cn

[Q50] 批量更新
来源：http://xl.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ux.shxzukj.cn

[Q51] 用子查询更新
来源：http://ar.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rg.nicolike.cn

[Q52] 删除指定行
来源：http://js.521024.cn

DELETE FROM users WHERE id = 10;
来源：http://sj.huanxung.cn

[Q53] 按条件删除
来源：http://tm.nicolike.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gp.jctech888.com.cn

[Q54] 清空表
来源：http://uc.521024.cn

TRUNCATE TABLE logs;
来源：http://hv.521024.cn

[Q55] 排名（并列占位）
来源：http://uf.lnxyls.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bd.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://ad.jctech888.com.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://be.huixiangedu.cn

[Q57] 行号
来源：http://ti.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ks.bjjhwx.cn

[Q58] 累计求和
来源：http://pd.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yp.szxytkj.cn

[Q59] 分组内累计
来源：http://qd.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://op.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://eo.gzmigu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ld.newstarts.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lx.colortex.cn

[Q61] 移动平均
来源：http://ap.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wn.szxytkj.cn

[Q62] 分组占比
来源：http://of.hnjuh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ux.shtwfgs.cn

[Q63] 开启事务
来源：http://qp.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cf.shxzukj.cn

[Q64] 提交事务
来源：http://yq.yuntaijiaju.cn

COMMIT;
来源：http://dg.huanxung.cn

[Q65] 回滚事务
来源：http://yu.yuntaijiaju.cn

ROLLBACK;
来源：http://sa.shxzskj.cn

[Q66] 行锁查询
来源：http://ih.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lf.jianghongdianzi.cn

[Q67] 设置隔离级别
来源：http://vj.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ee.yuexingan06.cn

[Q68] 保存点
来源：http://qd.nicolike.cn

SAVEPOINT sp1;
来源：http://wk.panjiajie.cn

ROLLBACK TO sp1;
来源：http://vi.shxzskj.cn

[Q69] 查看执行计划
来源：http://ti.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kk.chemitech.net.cn

[Q70] 更新统计信息
来源：http://tu.shxzukj.cn

ANALYZE TABLE users;
来源：http://yb.lnxyls.cn

[Q71] 查看建表语句
来源：http://zf.chemitech.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wq.newstarts.cn

[Q72] 查看索引
来源：http://fh.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://tc.jianghongdianzi.cn

[Q73] 查看表状态
来源：http://rr.521024.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ey.nszjky.cn

[Q74] 强制使用索引
来源：http://dh.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://og.nszjky.cn

[Q75] 日期格式化
来源：http://ag.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://av.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ai.yuntaijiaju.cn

[Q76] 按天统计
来源：http://ug.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oj.newstarts.cn

[Q77] 时间加减
来源：http://ze.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zd.yuexingan06.cn

[Q78] 当前时间
来源：http://py.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kc.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://ug.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ue.hnjuh.cn

[Q80] 字符串截取
来源：http://jb.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cy.szsharing.cn

[Q81] 字符串替换
来源：http://qp.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://op.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://pr.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mm.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://qi.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rg.colortex.cn

[Q84] 去除首尾空格
来源：http://ei.shxzukj.cn

SELECT TRIM(name) FROM users;
来源：http://eo.nicolike.cn

[Q85] 数值取整
来源：http://ru.colortex.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ol.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://wo.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bg.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://gk.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gc.huanxung.cn

[Q88] 行转列（条件聚合）
来源：http://rc.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xl.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cr.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://rt.haigaiapp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gz.bjjhwx.cn

[Q90] 生成序号列
来源：http://uj.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hb.haigaiapp.cn

================================================================================
来源：http://sb.chemitech.net.cn

R. Bash 专题
来源：http://yj.asd995.cn

================================================================================
来源：http://mt.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://rj.huixinmuqiang.cn

#!/usr/bin/env bash
来源：http://pd.muxihuayi.cn

set -euo pipefail
来源：http://cq.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://fc.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://mb.nszjky.cn

[R03] 只读变量
来源：http://xb.huixinmuqiang.cn

readonly PI=3.14
来源：http://oh.521024.cn

[R04] 位置参数
来源：http://mp.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://we.hnjuh.cn

[R05] 参数默认值
来源：http://xa.huixiangedu.cn

name="${1:-default}"
来源：http://ib.huixinmuqiang.cn

[R06] 判断命令是否存在
来源：http://oa.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cw.jctech888.com.cn

[R07] if 判断文件
来源：http://vm.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ub.newstarts.cn

[R08] 数值比较
来源：http://lb.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vk.jianghongdianzi.cn

[R09] 字符串比较
来源：http://sk.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qv.wgjwhj.cn

[R10] 正则匹配
来源：http://po.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://la.newstarts.cn

[R11] case 多分支
来源：http://fd.nicolike.cn

case "$1" in
来源：http://nj.wgjwhj.cn

start) echo "启动" ;;
来源：http://qe.asd995.cn

stop)  echo "停止" ;;
来源：http://qu.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://yj.hnjuh.cn

esac
来源：http://pd.521024.cn

[R12] for 遍历文件
来源：http://me.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://ci.nszjky.cn

[R13] for 计数循环
来源：http://op.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://hv.gzmigu.cn

[R14] C 风格 for
来源：http://sn.hahajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rm.shxzskj.cn

[R15] while 逐行读文件
来源：http://uy.hahajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ti.jianghongdianzi.cn

[R16] until 等待条件
来源：http://tx.yuexingan06.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gx.huanxung.cn

[R17] 数组定义与取值
来源：http://sj.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sz.hahajie.cn

[R18] 遍历数组
来源：http://xe.newstarts.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cv.asd995.cn

[R19] 数组长度
来源：http://sh.shxzukj.cn

echo "${#arr[@]}"
来源：http://bg.nszjky.cn

[R20] 关联数组（字典）
来源：http://ak.hahajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oe.hnjuh.cn

[R21] 字符串长度
来源：http://wi.bjjhwx.cn

echo "${#s}"
来源：http://vr.szxytkj.cn

[R22] 截取子串
来源：http://jy.muxihuayi.cn

echo "${s:0:5}"
来源：http://kp.jctech888.com.cn

[R23] 字符串替换
来源：http://tx.newstarts.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://av.bjjhwx.cn

[R24] 大小写转换
来源：http://pk.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://di.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://kj.szsharing.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://od.colortex.cn

[R26] 命令替换
来源：http://xj.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://db.huanxung.cn

[R27] 算术展开
来源：http://rl.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://ob.bookmarksfly.cn

[R28] 浮点运算
来源：http://bt.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://cv.szxytkj.cn

[R29] 定义函数
来源：http://qt.szsharing.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gv.wgjwhj.cn

[R30] 函数返回状态码
来源：http://wv.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://qm.bjjhwx.cn

[R31] 局部变量
来源：http://ge.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://bq.9csxet.cn

[R32] 参数个数校验
来源：http://rc.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gq.colortex.cn

[R33] 捕获错误并提示行号
来源：http://vh.muxihuayi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lr.shxzskj.cn

[R34] 退出时清理
来源：http://ie.yuexingan06.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ml.huixiangedu.cn

[R35] 后台执行并等待
来源：http://mn.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gy.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://ls.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qv.shxzskj.cn

[R37] 把输出赋给变量
来源：http://dn.yuntaijiaju.cn

files=$(ls -1)
来源：http://jk.lnxyls.cn

[R38] 管道串联
来源：http://bc.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://ge.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://uk.huixiangedu.cn

cmd > out.log 2>&1
来源：http://ks.yuntaijiaju.cn

[R40] 追加写日志
来源：http://qx.huixinmuqiang.cn

echo "log" >> out.log
来源：http://sc.lnxyls.cn

[R41] 丢弃输出
来源：http://rd.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://uu.asd995.cn

[R42] 输入重定向
来源：http://ag.yuntaijiaju.cn

wc -l < a.txt
来源：http://gr.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://cm.huanxung.cn

find . -name "*.log" -type f
来源：http://gz.haigaiapp.cn

[R44] 按修改时间查找
来源：http://lb.muxihuayi.cn

find . -mtime -7 -type f
来源：http://kv.muxihuayi.cn

[R45] 批量删除
来源：http://zc.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://xx.521024.cn

[R46] 递归替换文件内容
来源：http://jj.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zf.shxzskj.cn

[R47] sed 单行替换
来源：http://cy.bookmarksfly.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ml.muxihuayi.cn

[R48] awk 取指定列
来源：http://ve.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://vl.bjjhwx.cn

[R49] awk 带条件
来源：http://kt.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://im.huanxung.cn

[R50] awk 求和
来源：http://km.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jh.bjjhwx.cn

[R51] 排序去重取前几
来源：http://ck.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kj.muxihuayi.cn

[R52] 统计行数
来源：http://nw.szsharing.cn

wc -l a.txt
来源：http://cm.asd995.cn

[R53] 查看文件头与实时尾
来源：http://ol.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zk.huanxung.cn

[R54] 比较两个文件
来源：http://bz.huanxung.cn

diff a.txt b.txt
来源：http://jq.chemitech.net.cn

[R55] 压缩与解压
来源：http://jo.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xp.chemitech.net.cn

[R56] 远程拷贝
来源：http://xp.huanxung.cn

scp file user@host:/path/
来源：http://go.shxzskj.cn

[R57] 远程执行命令
来源：http://qi.szxytkj.cn

ssh user@host 'uptime'
来源：http://ef.szxytkj.cn

[R58] 下载文件
来源：http://ay.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hl.521024.cn

[R59] 发 POST JSON
来源：http://px.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bw.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://hr.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vj.asd995.cn

[R61] 磁盘占用
来源：http://ug.shtwfgs.cn

df -h;  du -sh *
来源：http://et.panjiajie.cn

[R62] 找最占空间的文件
来源：http://kq.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://sj.chemitech.net.cn

[R63] 内存与进程
来源：http://sr.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://xi.gzmigu.cn

[R64] 结束进程
来源：http://ln.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://fe.jctech888.com.cn

[R65] 查看端口占用
来源：http://ew.jctech888.com.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qc.huixiangedu.cn

[R66] 定时任务
来源：http://va.9csxet.cn

crontab -e;  crontab -l
来源：http://cv.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://vr.szxytkj.cn

openssl rand -hex 16
来源：http://ly.hnjuh.cn

[R68] 计算文件校验值
来源：http://eg.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sh.colortex.cn

[R69] 生成随机密码
来源：http://eg.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://pu.nszjky.cn

[R70] 时间戳与互转
来源：http://gn.521024.cn

date +%s;  date -d @1700000000
来源：http://cj.huixinmuqiang.cn

[R71] 日期格式化
来源：http://ov.newstarts.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://go.szsharing.cn

[R72] 等待端口就绪
来源：http://wl.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jv.newstarts.cn

[R73] 分割大日志
来源：http://kr.newstarts.cn

split -l 1000 big.log part_
来源：http://kj.huanxung.cn

[R74] 批量重命名
来源：http://to.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ue.newstarts.cn

[R75] 导出环境变量
来源：http://uq.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://dd.haigaiapp.cn

[R76] 使用临时文件
来源：http://pg.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fs.chemitech.net.cn

[R77] 读取用户输入
来源：http://hj.9csxet.cn

read -rp "请输入: " ans
来源：http://gq.yuexingan06.cn

[R78] 交互式菜单
来源：http://oi.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wx.huixiangedu.cn

[R79] 解析命令行选项
来源：http://as.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fy.asd995.cn

[R80] 查看脚本执行耗时
来源：http://st.hahajie.cn

time ./run.sh
来源：http://ok.hnjuh.cn

================================================================================
来源：http://bb.hahajie.cn

S. C / C++ 专题
来源：http://kk.huanxung.cn

================================================================================
来源：http://kl.hahajie.cn

[S01] C：Hello World
来源：http://pu.shtwfgs.cn

#include <stdio.h>
来源：http://hh.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sb.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://qi.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://lc.lnxyls.cn

[S03] C：读入整数
来源：http://qm.bjjhwx.cn


<!-- 参考信息 -->