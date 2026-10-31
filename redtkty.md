代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gy.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lj.shtwfgs.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pz.hnjuh.cn

[Q41] 多表连接
来源：http://ok.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ng.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://cr.yuexingan06.cn

JOIN products p ON p.id = o.product_id;
来源：http://km.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://kp.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://cs.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rz.shxzskj.cn

[Q43] 标量子查询
来源：http://km.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qk.shtwfgs.cn

[Q44] IN 子查询
来源：http://gp.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nn.haigaiapp.cn

[Q45] EXISTS 判断存在
来源：http://cm.bjjhwx.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ox.shxzukj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ah.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ey.hnjuh.cn

[Q47] 与平均值比较
来源：http://ml.shxzskj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hj.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://my.panjiajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yc.jianghongdianzi.cn

SELECT * FROM t WHERE c > 5;
来源：http://fx.jianghongdianzi.cn

[Q49] 更新单行
来源：http://yj.bookmarksfly.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ze.szxytkj.cn

[Q50] 批量更新
来源：http://cz.panjiajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://en.colortex.cn

[Q51] 用子查询更新
来源：http://me.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ek.yuntaijiaju.cn

[Q52] 删除指定行
来源：http://fu.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://fx.nicolike.cn

[Q53] 按条件删除
来源：http://hb.huixiangedu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iy.yuntaijiaju.cn

[Q54] 清空表
来源：http://fh.yuexingan06.cn

TRUNCATE TABLE logs;
来源：http://pw.asd995.cn

[Q55] 排名（并列占位）
来源：http://vj.shxzskj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uz.yuexingan06.cn

[Q56] 密集排名（并列不占位）
来源：http://er.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xk.hnjuh.cn

[Q57] 行号
来源：http://oh.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://by.asd995.cn

[Q58] 累计求和
来源：http://ed.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sx.jctech888.com.cn

[Q59] 分组内累计
来源：http://sk.yuntaijiaju.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bz.521024.cn

[Q60] 取上一行 / 下一行
来源：http://jn.gzmigu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vd.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gd.chemitech.net.cn

[Q61] 移动平均
来源：http://rb.hnjuh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xn.9csxet.cn

[Q62] 分组占比
来源：http://ro.hnjuh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rk.yuexingan06.cn

[Q63] 开启事务
来源：http://hd.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gd.huixinmuqiang.cn

[Q64] 提交事务
来源：http://oo.hahajie.cn

COMMIT;
来源：http://ri.hahajie.cn

[Q65] 回滚事务
来源：http://xn.asd995.cn

ROLLBACK;
来源：http://ao.jianghongdianzi.cn

[Q66] 行锁查询
来源：http://qz.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ya.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://cz.yuexingan06.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dv.9csxet.cn

[Q68] 保存点
来源：http://qm.nicolike.cn

SAVEPOINT sp1;
来源：http://ax.colortex.cn

ROLLBACK TO sp1;
来源：http://ab.lnxyls.cn

[Q69] 查看执行计划
来源：http://re.muxihuayi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jm.muxihuayi.cn

[Q70] 更新统计信息
来源：http://ma.colortex.cn

ANALYZE TABLE users;
来源：http://pf.9csxet.cn

[Q71] 查看建表语句
来源：http://ix.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fb.szxytkj.cn

[Q72] 查看索引
来源：http://xn.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://te.huixiangedu.cn

[Q73] 查看表状态
来源：http://sm.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ud.newstarts.cn

[Q74] 强制使用索引
来源：http://ps.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://at.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://fp.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dx.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zc.bookmarksfly.cn

[Q76] 按天统计
来源：http://iu.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gy.gzmigu.cn

[Q77] 时间加减
来源：http://bg.szxytkj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ow.lnxyls.cn

[Q78] 当前时间
来源：http://ss.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vy.panjiajie.cn

[Q79] 字符串拼接
来源：http://ce.521024.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://my.shxzskj.cn

[Q80] 字符串截取
来源：http://xz.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bc.9csxet.cn

[Q81] 字符串替换
来源：http://yc.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yi.bookmarksfly.cn

[Q82] 字符长度与字节长度
来源：http://mh.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bj.9csxet.cn

[Q83] 大小写转换
来源：http://ah.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vv.yuntaijiaju.cn

[Q84] 去除首尾空格
来源：http://zz.521024.cn

SELECT TRIM(name) FROM users;
来源：http://xy.huixiangedu.cn

[Q85] 数值取整
来源：http://lo.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://et.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://fc.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zt.newstarts.cn

[Q87] JSON 字段做条件
来源：http://ju.nicolike.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nt.9csxet.cn

[Q88] 行转列（条件聚合）
来源：http://io.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rb.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dq.nicolike.cn

[Q89] 判断表是否存在
来源：http://xy.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jg.huanxung.cn

[Q90] 生成序号列
来源：http://vk.shxzukj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://at.521024.cn

================================================================================
来源：http://qb.huanxung.cn

R. Bash 专题
来源：http://ny.szsharing.cn

================================================================================
来源：http://ga.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://ch.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://no.haigaiapp.cn

set -euo pipefail
来源：http://cz.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://bt.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://sh.bjjhwx.cn

[R03] 只读变量
来源：http://ce.yuexingan06.cn

readonly PI=3.14
来源：http://sg.szsharing.cn

[R04] 位置参数
来源：http://le.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gq.521024.cn

[R05] 参数默认值
来源：http://gh.szxytkj.cn

name="${1:-default}"
来源：http://sz.gzmigu.cn

[R06] 判断命令是否存在
来源：http://ki.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://re.nszjky.cn

[R07] if 判断文件
来源：http://ah.shtwfgs.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oc.szsharing.cn

[R08] 数值比较
来源：http://yc.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nc.bookmarksfly.cn

[R09] 字符串比较
来源：http://oz.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pp.bookmarksfly.cn

[R10] 正则匹配
来源：http://ph.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pi.szsharing.cn

[R11] case 多分支
来源：http://sg.panjiajie.cn

case "$1" in
来源：http://ir.bjjhwx.cn

start) echo "启动" ;;
来源：http://wd.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://gk.szxytkj.cn

*)     echo "未知命令" ;;
来源：http://dr.panjiajie.cn

esac
来源：http://gv.huixiangedu.cn

[R12] for 遍历文件
来源：http://fv.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://rb.huixiangedu.cn

[R13] for 计数循环
来源：http://pk.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://jq.muxihuayi.cn

[R14] C 风格 for
来源：http://au.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fy.jianghongdianzi.cn

[R15] while 逐行读文件
来源：http://lh.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hr.gzmigu.cn

[R16] until 等待条件
来源：http://zq.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://br.shxzskj.cn

[R17] 数组定义与取值
来源：http://qm.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kl.lnxyls.cn

[R18] 遍历数组
来源：http://xp.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sr.colortex.cn

[R19] 数组长度
来源：http://wl.shtwfgs.cn

echo "${#arr[@]}"
来源：http://iq.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://fe.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pr.shtwfgs.cn

[R21] 字符串长度
来源：http://my.haigaiapp.cn

echo "${#s}"
来源：http://fx.newstarts.cn

[R22] 截取子串
来源：http://nu.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://eu.shxzskj.cn

[R23] 字符串替换
来源：http://yx.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pf.bookmarksfly.cn

[R24] 大小写转换
来源：http://ks.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rm.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://xd.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zc.huixiangedu.cn

[R26] 命令替换
来源：http://zs.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://ff.colortex.cn

[R27] 算术展开
来源：http://ua.asd995.cn

echo $((1 + 2 * 3))
来源：http://yf.muxihuayi.cn

[R28] 浮点运算
来源：http://uw.huixiangedu.cn

echo "scale=2; 10/3" | bc
来源：http://vq.colortex.cn

[R29] 定义函数
来源：http://zh.newstarts.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ue.panjiajie.cn

[R30] 函数返回状态码
来源：http://tu.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://bw.haigaiapp.cn

[R31] 局部变量
来源：http://yy.521024.cn

f() { local x=1; echo "$x"; }
来源：http://sf.nicolike.cn

[R32] 参数个数校验
来源：http://nt.szxytkj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://at.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://mf.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gd.huanxung.cn

[R34] 退出时清理
来源：http://ur.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pc.colortex.cn

[R35] 后台执行并等待
来源：http://ky.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zf.nszjky.cn

[R36] 并发执行多个任务
来源：http://un.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://th.hahajie.cn

[R37] 把输出赋给变量
来源：http://au.bookmarksfly.cn

files=$(ls -1)
来源：http://hw.bookmarksfly.cn

[R38] 管道串联
来源：http://da.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://yh.jctech888.com.cn

[R39] 重定向标准输出与错误
来源：http://og.panjiajie.cn

cmd > out.log 2>&1
来源：http://dq.huanxung.cn

[R40] 追加写日志
来源：http://fx.hnjuh.cn

echo "log" >> out.log
来源：http://qo.panjiajie.cn

[R41] 丢弃输出
来源：http://vg.nicolike.cn

cmd >/dev/null 2>&1
来源：http://lr.bookmarksfly.cn

[R42] 输入重定向
来源：http://bt.huanxung.cn

wc -l < a.txt
来源：http://ja.muxihuayi.cn

[R43] 按名字查找文件
来源：http://sf.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://nn.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://dc.colortex.cn

find . -mtime -7 -type f
来源：http://mf.wgjwhj.cn

[R45] 批量删除
来源：http://ym.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://uc.shxzukj.cn

[R46] 递归替换文件内容
来源：http://ar.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://om.chemitech.net.cn

[R47] sed 单行替换
来源：http://nv.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ua.huixiangedu.cn

[R48] awk 取指定列
来源：http://sf.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://za.szsharing.cn

[R49] awk 带条件
来源：http://da.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zv.chemitech.net.cn

[R50] awk 求和
来源：http://tc.jctech888.com.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gz.jctech888.com.cn

[R51] 排序去重取前几
来源：http://gx.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ib.chemitech.net.cn

[R52] 统计行数
来源：http://cp.jctech888.com.cn

wc -l a.txt
来源：http://yg.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://od.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://of.nszjky.cn

[R54] 比较两个文件
来源：http://vx.yuexingan06.cn

diff a.txt b.txt
来源：http://of.yuexingan06.cn

[R55] 压缩与解压
来源：http://bx.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gi.wgjwhj.cn

[R56] 远程拷贝
来源：http://we.hnjuh.cn

scp file user@host:/path/
来源：http://or.panjiajie.cn

[R57] 远程执行命令
来源：http://fd.nszjky.cn

ssh user@host 'uptime'
来源：http://tx.yuexingan06.cn

[R58] 下载文件
来源：http://ag.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uz.gzmigu.cn

[R59] 发 POST JSON
来源：http://ln.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mh.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://tk.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ix.newstarts.cn

[R61] 磁盘占用
来源：http://yf.muxihuayi.cn

df -h;  du -sh *
来源：http://kv.nicolike.cn

[R62] 找最占空间的文件
来源：http://jx.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://ug.jctech888.com.cn

[R63] 内存与进程
来源：http://pj.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://xd.colortex.cn

[R64] 结束进程
来源：http://ns.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://hn.haigaiapp.cn

[R65] 查看端口占用
来源：http://ge.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://in.huanxung.cn

[R66] 定时任务
来源：http://lj.9csxet.cn

crontab -e;  crontab -l
来源：http://um.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://gm.szxytkj.cn

openssl rand -hex 16
来源：http://gp.asd995.cn

[R68] 计算文件校验值
来源：http://ue.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qp.lnxyls.cn

[R69] 生成随机密码
来源：http://hh.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://au.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://es.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://cz.huixiangedu.cn

[R71] 日期格式化
来源：http://ql.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wf.chemitech.net.cn

[R72] 等待端口就绪
来源：http://yk.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qn.gzmigu.cn

[R73] 分割大日志
来源：http://zo.shtwfgs.cn

split -l 1000 big.log part_
来源：http://mw.huixiangedu.cn

[R74] 批量重命名
来源：http://cn.jianghongdianzi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ze.newstarts.cn

[R75] 导出环境变量
来源：http://vl.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://zh.panjiajie.cn

[R76] 使用临时文件
来源：http://yt.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kf.bookmarksfly.cn

[R77] 读取用户输入
来源：http://dg.bjjhwx.cn

read -rp "请输入: " ans
来源：http://yb.lnxyls.cn

[R78] 交互式菜单
来源：http://uq.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mv.colortex.cn

[R79] 解析命令行选项
来源：http://ar.521024.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://su.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://gn.nszjky.cn

time ./run.sh
来源：http://po.nicolike.cn

================================================================================
来源：http://zt.hnjuh.cn

S. C / C++ 专题
来源：http://dx.bjjhwx.cn

================================================================================
来源：http://gl.newstarts.cn

[S01] C：Hello World
来源：http://xd.panjiajie.cn

#include <stdio.h>
来源：http://sr.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://so.9csxet.cn

[S02] C：变量与格式化输出
来源：http://zl.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://pv.huixiangedu.cn

[S03] C：读入整数
来源：http://wn.szsharing.cn

int x; scanf("%d", &x);
来源：http://li.wgjwhj.cn

[S04] C：字符串复制
来源：http://wx.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sj.bjjhwx.cn

[S05] C：字符串长度
来源：http://em.shxzukj.cn

strlen(s)
来源：http://zf.muxihuayi.cn

[S06] C：字符串比较
来源：http://yd.521024.cn

strcmp(a, b) == 0
来源：http://fm.bookmarksfly.cn

[S07] C：数组遍历求和
来源：http://qw.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bv.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://ks.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://np.521024.cn

[S09] C：结构体定义与初始化
来源：http://ed.nszjky.cn


<!-- 参考信息 -->