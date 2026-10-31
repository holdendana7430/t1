代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://kc.9csxet.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rk.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://to.gzmigu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://no.huanxung.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jp.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ur.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fs.chemitech.net.cn

[Q41] 多表连接
来源：http://ek.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gq.shtwfgs.cn

JOIN users u ON u.id = o.user_id
来源：http://td.newstarts.cn

JOIN products p ON p.id = o.product_id;
来源：http://fh.panjiajie.cn

[Q42] 连接条件附加过滤
来源：http://gd.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://ws.szxytkj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qb.9csxet.cn

[Q43] 标量子查询
来源：http://uq.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ih.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://vf.gzmigu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fo.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://ne.shxzskj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mw.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vq.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rn.bjjhwx.cn

[Q47] 与平均值比较
来源：http://rv.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ma.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://xu.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zs.shxzskj.cn

SELECT * FROM t WHERE c > 5;
来源：http://hv.hnjuh.cn

[Q49] 更新单行
来源：http://rc.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ut.9csxet.cn

[Q50] 批量更新
来源：http://mh.panjiajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ja.jianghongdianzi.cn

[Q51] 用子查询更新
来源：http://ai.chemitech.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wp.shxzskj.cn

[Q52] 删除指定行
来源：http://qp.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://po.yuntaijiaju.cn

[Q53] 按条件删除
来源：http://ha.wgjwhj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sl.colortex.cn

[Q54] 清空表
来源：http://nl.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://ot.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://cc.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sl.haigaiapp.cn

[Q56] 密集排名（并列不占位）
来源：http://ov.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ic.haigaiapp.cn

[Q57] 行号
来源：http://fq.gzmigu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hx.huixinmuqiang.cn

[Q58] 累计求和
来源：http://qr.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uv.nszjky.cn

[Q59] 分组内累计
来源：http://al.huixiangedu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qn.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://oz.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dx.newstarts.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ps.shtwfgs.cn

[Q61] 移动平均
来源：http://bw.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mz.newstarts.cn

[Q62] 分组占比
来源：http://bq.nicolike.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wv.newstarts.cn

[Q63] 开启事务
来源：http://py.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rz.bjjhwx.cn

[Q64] 提交事务
来源：http://wt.yuexingan06.cn

COMMIT;
来源：http://cj.nszjky.cn

[Q65] 回滚事务
来源：http://le.shxzskj.cn

ROLLBACK;
来源：http://sc.huanxung.cn

[Q66] 行锁查询
来源：http://xx.9csxet.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fr.huixiangedu.cn

[Q67] 设置隔离级别
来源：http://xy.haigaiapp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rc.huixinmuqiang.cn

[Q68] 保存点
来源：http://oa.shxzskj.cn

SAVEPOINT sp1;
来源：http://rf.gzmigu.cn

ROLLBACK TO sp1;
来源：http://vg.szxytkj.cn

[Q69] 查看执行计划
来源：http://va.wgjwhj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hg.9csxet.cn

[Q70] 更新统计信息
来源：http://yd.panjiajie.cn

ANALYZE TABLE users;
来源：http://ca.jctech888.com.cn

[Q71] 查看建表语句
来源：http://mu.chemitech.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ia.jianghongdianzi.cn

[Q72] 查看索引
来源：http://po.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://hb.shxzskj.cn

[Q73] 查看表状态
来源：http://pn.jctech888.com.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zk.hnjuh.cn

[Q74] 强制使用索引
来源：http://xx.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nv.9csxet.cn

[Q75] 日期格式化
来源：http://ad.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vs.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uo.szxytkj.cn

[Q76] 按天统计
来源：http://hh.newstarts.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wf.shxzskj.cn

[Q77] 时间加减
来源：http://yn.hahajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jy.lnxyls.cn

[Q78] 当前时间
来源：http://cg.lnxyls.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://io.yuexingan06.cn

[Q79] 字符串拼接
来源：http://zr.nszjky.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mk.asd995.cn

[Q80] 字符串截取
来源：http://jc.shxzukj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iv.bookmarksfly.cn

[Q81] 字符串替换
来源：http://yw.bjjhwx.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ch.yuexingan06.cn

[Q82] 字符长度与字节长度
来源：http://zj.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xr.shtwfgs.cn

[Q83] 大小写转换
来源：http://sf.gzmigu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ze.jianghongdianzi.cn

[Q84] 去除首尾空格
来源：http://on.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://ck.colortex.cn

[Q85] 数值取整
来源：http://ne.nicolike.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://er.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://xb.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pl.nszjky.cn

[Q87] JSON 字段做条件
来源：http://ex.panjiajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qe.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://gf.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://on.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oq.lnxyls.cn

[Q89] 判断表是否存在
来源：http://qc.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xy.yuexingan06.cn

[Q90] 生成序号列
来源：http://ei.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pn.gzmigu.cn

================================================================================
来源：http://dg.9csxet.cn

R. Bash 专题
来源：http://dr.panjiajie.cn

================================================================================
来源：http://os.nszjky.cn

[R01] shebang 与严格模式
来源：http://wj.jctech888.com.cn

#!/usr/bin/env bash
来源：http://sh.newstarts.cn

set -euo pipefail
来源：http://nw.asd995.cn

[R02] 变量赋值与使用
来源：http://oa.hnjuh.cn

name="Tom"; echo "$name"
来源：http://og.szsharing.cn

[R03] 只读变量
来源：http://jb.shxzskj.cn

readonly PI=3.14
来源：http://dm.huanxung.cn

[R04] 位置参数
来源：http://il.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fp.muxihuayi.cn

[R05] 参数默认值
来源：http://nx.521024.cn

name="${1:-default}"
来源：http://sg.asd995.cn

[R06] 判断命令是否存在
来源：http://zr.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ni.haigaiapp.cn

[R07] if 判断文件
来源：http://nm.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dv.9csxet.cn

[R08] 数值比较
来源：http://vs.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tx.gzmigu.cn

[R09] 字符串比较
来源：http://pe.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mp.panjiajie.cn

[R10] 正则匹配
来源：http://mw.newstarts.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wk.chemitech.net.cn

[R11] case 多分支
来源：http://kb.huixiangedu.cn

case "$1" in
来源：http://tx.yuexingan06.cn

start) echo "启动" ;;
来源：http://nu.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://kf.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://xh.wgjwhj.cn

esac
来源：http://vt.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://en.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://tv.huixiangedu.cn

[R13] for 计数循环
来源：http://qk.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://rc.huixiangedu.cn

[R14] C 风格 for
来源：http://of.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ow.nicolike.cn

[R15] while 逐行读文件
来源：http://qk.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://iv.haigaiapp.cn

[R16] until 等待条件
来源：http://pv.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jj.haigaiapp.cn

[R17] 数组定义与取值
来源：http://ev.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qw.huixiangedu.cn

[R18] 遍历数组
来源：http://by.bookmarksfly.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://as.hnjuh.cn

[R19] 数组长度
来源：http://yo.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://bc.shxzukj.cn

[R20] 关联数组（字典）
来源：http://jl.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://px.shxzskj.cn

[R21] 字符串长度
来源：http://ta.chemitech.net.cn

echo "${#s}"
来源：http://ge.szsharing.cn

[R22] 截取子串
来源：http://zg.nicolike.cn

echo "${s:0:5}"
来源：http://bm.muxihuayi.cn

[R23] 字符串替换
来源：http://vy.shtwfgs.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lh.colortex.cn

[R24] 大小写转换
来源：http://bz.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dg.521024.cn

[R25] 去后缀 / 去前缀
来源：http://fg.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cf.chemitech.net.cn

[R26] 命令替换
来源：http://km.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://be.szsharing.cn

[R27] 算术展开
来源：http://ym.gzmigu.cn

echo $((1 + 2 * 3))
来源：http://bw.hahajie.cn

[R28] 浮点运算
来源：http://fa.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://gu.huixiangedu.cn

[R29] 定义函数
来源：http://pf.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gq.shtwfgs.cn

[R30] 函数返回状态码
来源：http://vo.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://va.jianghongdianzi.cn

[R31] 局部变量
来源：http://nk.hahajie.cn

f() { local x=1; echo "$x"; }
来源：http://cr.shxzskj.cn

[R32] 参数个数校验
来源：http://uh.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vg.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://cx.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eo.521024.cn

[R34] 退出时清理
来源：http://qh.shtwfgs.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vb.hnjuh.cn

[R35] 后台执行并等待
来源：http://xw.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://aw.huixinmuqiang.cn

[R36] 并发执行多个任务
来源：http://cs.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oh.nicolike.cn

[R37] 把输出赋给变量
来源：http://xy.colortex.cn

files=$(ls -1)
来源：http://yx.hnjuh.cn

[R38] 管道串联
来源：http://ck.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://mn.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://bj.hahajie.cn

cmd > out.log 2>&1
来源：http://im.bjjhwx.cn

[R40] 追加写日志
来源：http://tf.newstarts.cn

echo "log" >> out.log
来源：http://xy.gzmigu.cn

[R41] 丢弃输出
来源：http://pv.hahajie.cn

cmd >/dev/null 2>&1
来源：http://bl.colortex.cn

[R42] 输入重定向
来源：http://he.nicolike.cn

wc -l < a.txt
来源：http://er.asd995.cn

[R43] 按名字查找文件
来源：http://rw.jctech888.com.cn

find . -name "*.log" -type f
来源：http://df.nicolike.cn

[R44] 按修改时间查找
来源：http://wo.hnjuh.cn

find . -mtime -7 -type f
来源：http://pq.hahajie.cn

[R45] 批量删除
来源：http://oy.nszjky.cn

find . -name "*.tmp" -delete
来源：http://ay.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://co.chemitech.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yy.hnjuh.cn

[R47] sed 单行替换
来源：http://en.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wz.huanxung.cn

[R48] awk 取指定列
来源：http://vi.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://lc.nicolike.cn

[R49] awk 带条件
来源：http://vh.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://so.newstarts.cn

[R50] awk 求和
来源：http://fr.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jq.haigaiapp.cn

[R51] 排序去重取前几
来源：http://lx.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vj.szxytkj.cn

[R52] 统计行数
来源：http://xb.lnxyls.cn

wc -l a.txt
来源：http://hl.panjiajie.cn

[R53] 查看文件头与实时尾
来源：http://dw.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wu.shxzukj.cn

[R54] 比较两个文件
来源：http://dm.jctech888.com.cn

diff a.txt b.txt
来源：http://da.hahajie.cn

[R55] 压缩与解压
来源：http://ud.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hc.hnjuh.cn

[R56] 远程拷贝
来源：http://bc.huixiangedu.cn

scp file user@host:/path/
来源：http://gr.hnjuh.cn

[R57] 远程执行命令
来源：http://xh.hahajie.cn

ssh user@host 'uptime'
来源：http://uc.asd995.cn

[R58] 下载文件
来源：http://za.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mg.gzmigu.cn

[R59] 发 POST JSON
来源：http://co.shxzskj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ca.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://qu.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ud.szsharing.cn

[R61] 磁盘占用
来源：http://sd.hnjuh.cn

df -h;  du -sh *
来源：http://al.gzmigu.cn

[R62] 找最占空间的文件
来源：http://xz.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://rm.wgjwhj.cn

[R63] 内存与进程
来源：http://lv.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://hf.9csxet.cn

[R64] 结束进程
来源：http://zh.nicolike.cn

kill -9 $(pgrep -f app.py)
来源：http://tx.huixiangedu.cn

[R65] 查看端口占用
来源：http://cu.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gl.wgjwhj.cn

[R66] 定时任务
来源：http://ku.szxytkj.cn

crontab -e;  crontab -l
来源：http://zo.9csxet.cn

[R67] 生成随机十六进制串
来源：http://uh.nicolike.cn

openssl rand -hex 16
来源：http://ll.hahajie.cn

[R68] 计算文件校验值
来源：http://kg.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pj.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://sz.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://fp.gzmigu.cn

[R70] 时间戳与互转
来源：http://mj.huixinmuqiang.cn

date +%s;  date -d @1700000000
来源：http://pq.wgjwhj.cn

[R71] 日期格式化
来源：http://vg.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xh.asd995.cn

[R72] 等待端口就绪
来源：http://xu.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vz.wgjwhj.cn

[R73] 分割大日志
来源：http://gw.yuexingan06.cn

split -l 1000 big.log part_
来源：http://qz.9csxet.cn

[R74] 批量重命名
来源：http://vz.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hx.9csxet.cn

[R75] 导出环境变量
来源：http://fp.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://pf.szsharing.cn

[R76] 使用临时文件
来源：http://ft.hahajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lf.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://gm.chemitech.net.cn

read -rp "请输入: " ans
来源：http://rq.colortex.cn

[R78] 交互式菜单
来源：http://dj.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ur.newstarts.cn

[R79] 解析命令行选项
来源：http://hw.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fu.asd995.cn

[R80] 查看脚本执行耗时
来源：http://jn.shxzukj.cn

time ./run.sh
来源：http://mx.yuexingan06.cn

================================================================================
来源：http://fk.nszjky.cn

S. C / C++ 专题
来源：http://yx.huixinmuqiang.cn

================================================================================
来源：http://pq.jianghongdianzi.cn

[S01] C：Hello World
来源：http://vm.yuexingan06.cn

#include <stdio.h>
来源：http://ml.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mi.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://wd.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://gw.yuntaijiaju.cn

[S03] C：读入整数
来源：http://gi.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://ae.colortex.cn

[S04] C：字符串复制
来源：http://da.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://eu.huanxung.cn

[S05] C：字符串长度
来源：http://us.newstarts.cn

strlen(s)
来源：http://hh.nicolike.cn

[S06] C：字符串比较
来源：http://rv.lnxyls.cn

strcmp(a, b) == 0
来源：http://hv.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://in.bookmarksfly.cn


<!-- 参考信息 -->