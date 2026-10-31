代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ss.shxzukj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xk.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iw.bjjhwx.cn

[Q41] 多表连接
来源：http://uc.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hu.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://uv.colortex.cn

JOIN products p ON p.id = o.product_id;
来源：http://bx.jctech888.com.cn

[Q42] 连接条件附加过滤
来源：http://mi.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://rp.chemitech.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://iw.huanxung.cn

[Q43] 标量子查询
来源：http://xn.hnjuh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jv.nicolike.cn

[Q44] IN 子查询
来源：http://wy.szxytkj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://em.colortex.cn

[Q45] EXISTS 判断存在
来源：http://dm.521024.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://og.nszjky.cn

[Q46] NOT EXISTS 判断不存在
来源：http://du.panjiajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qu.huixinmuqiang.cn

[Q47] 与平均值比较
来源：http://nh.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ro.colortex.cn

[Q48] CTE 公用表表达式
来源：http://ax.yuexingan06.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wl.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://we.bookmarksfly.cn

[Q49] 更新单行
来源：http://bl.yuntaijiaju.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zy.shxzukj.cn

[Q50] 批量更新
来源：http://db.chemitech.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rz.nszjky.cn

[Q51] 用子查询更新
来源：http://xe.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bx.shtwfgs.cn

[Q52] 删除指定行
来源：http://cn.nszjky.cn

DELETE FROM users WHERE id = 10;
来源：http://ds.nicolike.cn

[Q53] 按条件删除
来源：http://wq.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://em.yuexingan06.cn

[Q54] 清空表
来源：http://yf.gzmigu.cn

TRUNCATE TABLE logs;
来源：http://rm.hnjuh.cn

[Q55] 排名（并列占位）
来源：http://de.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://av.yuntaijiaju.cn

[Q56] 密集排名（并列不占位）
来源：http://ig.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mk.huanxung.cn

[Q57] 行号
来源：http://cw.nszjky.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xm.jctech888.com.cn

[Q58] 累计求和
来源：http://jy.muxihuayi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fp.wgjwhj.cn

[Q59] 分组内累计
来源：http://ja.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ni.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://mr.haigaiapp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lv.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fp.huixiangedu.cn

[Q61] 移动平均
来源：http://zt.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ag.szsharing.cn

[Q62] 分组占比
来源：http://ia.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sy.521024.cn

[Q63] 开启事务
来源：http://ux.hnjuh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sr.yuntaijiaju.cn

[Q64] 提交事务
来源：http://hz.huixiangedu.cn

COMMIT;
来源：http://av.szsharing.cn

[Q65] 回滚事务
来源：http://br.jctech888.com.cn

ROLLBACK;
来源：http://ov.yuntaijiaju.cn

[Q66] 行锁查询
来源：http://ha.szsharing.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jn.asd995.cn

[Q67] 设置隔离级别
来源：http://oj.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://he.hnjuh.cn

[Q68] 保存点
来源：http://mi.jctech888.com.cn

SAVEPOINT sp1;
来源：http://sa.nicolike.cn

ROLLBACK TO sp1;
来源：http://vj.gzmigu.cn

[Q69] 查看执行计划
来源：http://mp.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rr.newstarts.cn

[Q70] 更新统计信息
来源：http://xs.huixiangedu.cn

ANALYZE TABLE users;
来源：http://wz.huixiangedu.cn

[Q71] 查看建表语句
来源：http://dj.gzmigu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rt.huixiangedu.cn

[Q72] 查看索引
来源：http://ly.nszjky.cn

SHOW INDEX FROM users;
来源：http://ub.lnxyls.cn

[Q73] 查看表状态
来源：http://aa.haigaiapp.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mi.hnjuh.cn

[Q74] 强制使用索引
来源：http://bu.bookmarksfly.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xc.wgjwhj.cn

[Q75] 日期格式化
来源：http://rx.nicolike.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lr.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://og.yuexingan06.cn

[Q76] 按天统计
来源：http://xl.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uu.jctech888.com.cn

[Q77] 时间加减
来源：http://od.wgjwhj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rb.shtwfgs.cn

[Q78] 当前时间
来源：http://ov.huixinmuqiang.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sa.jianghongdianzi.cn

[Q79] 字符串拼接
来源：http://ir.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qf.bjjhwx.cn

[Q80] 字符串截取
来源：http://tq.bjjhwx.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aj.szxytkj.cn

[Q81] 字符串替换
来源：http://ao.newstarts.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ec.colortex.cn

[Q82] 字符长度与字节长度
来源：http://xw.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ib.huanxung.cn

[Q83] 大小写转换
来源：http://jw.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pe.asd995.cn

[Q84] 去除首尾空格
来源：http://lv.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://om.hahajie.cn

[Q85] 数值取整
来源：http://kk.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mp.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://dv.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://al.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://lv.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kd.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://do.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uq.panjiajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xm.nszjky.cn

[Q89] 判断表是否存在
来源：http://xc.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xr.szsharing.cn

[Q90] 生成序号列
来源：http://gu.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xc.521024.cn

================================================================================
来源：http://cq.chemitech.net.cn

R. Bash 专题
来源：http://ki.newstarts.cn

================================================================================
来源：http://ry.huanxung.cn

[R01] shebang 与严格模式
来源：http://ld.hahajie.cn

#!/usr/bin/env bash
来源：http://yo.colortex.cn

set -euo pipefail
来源：http://nx.hahajie.cn

[R02] 变量赋值与使用
来源：http://mw.bjjhwx.cn

name="Tom"; echo "$name"
来源：http://dx.newstarts.cn

[R03] 只读变量
来源：http://ez.newstarts.cn

readonly PI=3.14
来源：http://bx.nicolike.cn

[R04] 位置参数
来源：http://bi.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ei.gzmigu.cn

[R05] 参数默认值
来源：http://vi.gzmigu.cn

name="${1:-default}"
来源：http://fo.jctech888.com.cn

[R06] 判断命令是否存在
来源：http://fu.shtwfgs.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ng.hahajie.cn

[R07] if 判断文件
来源：http://ga.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vk.9csxet.cn

[R08] 数值比较
来源：http://kb.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ta.huixinmuqiang.cn

[R09] 字符串比较
来源：http://ea.huanxung.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fp.colortex.cn

[R10] 正则匹配
来源：http://jv.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ni.nicolike.cn

[R11] case 多分支
来源：http://vv.szxytkj.cn

case "$1" in
来源：http://in.szsharing.cn

start) echo "启动" ;;
来源：http://eg.shxzskj.cn

stop)  echo "停止" ;;
来源：http://xf.huanxung.cn

*)     echo "未知命令" ;;
来源：http://kd.muxihuayi.cn

esac
来源：http://lu.9csxet.cn

[R12] for 遍历文件
来源：http://xc.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://yy.asd995.cn

[R13] for 计数循环
来源：http://ly.shxzskj.cn

for i in {1..10}; do echo "$i"; done
来源：http://mi.521024.cn

[R14] C 风格 for
来源：http://rq.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ce.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://vt.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pu.asd995.cn

[R16] until 等待条件
来源：http://lb.newstarts.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iy.chemitech.net.cn

[R17] 数组定义与取值
来源：http://jd.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jp.newstarts.cn

[R18] 遍历数组
来源：http://ll.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qv.shxzukj.cn

[R19] 数组长度
来源：http://js.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://hw.nszjky.cn

[R20] 关联数组（字典）
来源：http://sb.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fq.yuexingan06.cn

[R21] 字符串长度
来源：http://ob.yuexingan06.cn

echo "${#s}"
来源：http://if.huixinmuqiang.cn

[R22] 截取子串
来源：http://kh.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://ji.hahajie.cn

[R23] 字符串替换
来源：http://yi.szxytkj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lg.asd995.cn

[R24] 大小写转换
来源：http://ty.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cp.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://gb.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sv.huanxung.cn

[R26] 命令替换
来源：http://sd.colortex.cn

now=$(date +%F); echo "$now"
来源：http://nc.bjjhwx.cn

[R27] 算术展开
来源：http://qt.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://ry.hnjuh.cn

[R28] 浮点运算
来源：http://ru.muxihuayi.cn

echo "scale=2; 10/3" | bc
来源：http://lf.521024.cn

[R29] 定义函数
来源：http://vh.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zl.colortex.cn

[R30] 函数返回状态码
来源：http://yt.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://dq.huixiangedu.cn

[R31] 局部变量
来源：http://ud.hahajie.cn

f() { local x=1; echo "$x"; }
来源：http://xw.bookmarksfly.cn

[R32] 参数个数校验
来源：http://fj.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jh.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://mw.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uz.szsharing.cn

[R34] 退出时清理
来源：http://pm.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://km.shtwfgs.cn

[R35] 后台执行并等待
来源：http://nm.gzmigu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yz.hnjuh.cn

[R36] 并发执行多个任务
来源：http://le.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ui.hahajie.cn

[R37] 把输出赋给变量
来源：http://wt.asd995.cn

files=$(ls -1)
来源：http://qs.shxzskj.cn

[R38] 管道串联
来源：http://zb.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://kr.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://be.nicolike.cn

cmd > out.log 2>&1
来源：http://lq.muxihuayi.cn

[R40] 追加写日志
来源：http://sh.huixinmuqiang.cn

echo "log" >> out.log
来源：http://ny.521024.cn

[R41] 丢弃输出
来源：http://xz.shxzskj.cn

cmd >/dev/null 2>&1
来源：http://ye.shxzukj.cn

[R42] 输入重定向
来源：http://wy.hnjuh.cn

wc -l < a.txt
来源：http://gs.yuntaijiaju.cn

[R43] 按名字查找文件
来源：http://et.shxzskj.cn

find . -name "*.log" -type f
来源：http://dn.chemitech.net.cn

[R44] 按修改时间查找
来源：http://hr.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://io.haigaiapp.cn

[R45] 批量删除
来源：http://ox.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://ey.newstarts.cn

[R46] 递归替换文件内容
来源：http://yi.yuntaijiaju.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dz.nszjky.cn

[R47] sed 单行替换
来源：http://tg.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://on.szsharing.cn

[R48] awk 取指定列
来源：http://ym.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://dz.shxzskj.cn

[R49] awk 带条件
来源：http://hv.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zf.panjiajie.cn

[R50] awk 求和
来源：http://gn.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qh.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://ao.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ra.nicolike.cn

[R52] 统计行数
来源：http://ry.huixiangedu.cn

wc -l a.txt
来源：http://ov.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://er.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://th.hnjuh.cn

[R54] 比较两个文件
来源：http://rm.nszjky.cn

diff a.txt b.txt
来源：http://kg.jctech888.com.cn

[R55] 压缩与解压
来源：http://ik.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sl.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://ge.huixinmuqiang.cn

scp file user@host:/path/
来源：http://cc.nszjky.cn

[R57] 远程执行命令
来源：http://oj.521024.cn

ssh user@host 'uptime'
来源：http://uv.panjiajie.cn

[R58] 下载文件
来源：http://vx.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gr.szsharing.cn

[R59] 发 POST JSON
来源：http://qz.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hh.huixiangedu.cn

[R60] 只看 HTTP 状态码
来源：http://sd.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rh.bjjhwx.cn

[R61] 磁盘占用
来源：http://io.asd995.cn

df -h;  du -sh *
来源：http://wi.hnjuh.cn

[R62] 找最占空间的文件
来源：http://re.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://bj.shtwfgs.cn

[R63] 内存与进程
来源：http://uc.9csxet.cn

free -h;  ps aux | grep nginx
来源：http://tr.lnxyls.cn

[R64] 结束进程
来源：http://fd.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://ss.huixiangedu.cn

[R65] 查看端口占用
来源：http://xy.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zq.szsharing.cn

[R66] 定时任务
来源：http://ad.shtwfgs.cn

crontab -e;  crontab -l
来源：http://wl.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://ch.lnxyls.cn

openssl rand -hex 16
来源：http://ag.9csxet.cn

[R68] 计算文件校验值
来源：http://gz.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bd.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://qa.colortex.cn

head -c 16 /dev/urandom | base64
来源：http://ud.gzmigu.cn

[R70] 时间戳与互转
来源：http://ey.asd995.cn

date +%s;  date -d @1700000000
来源：http://js.nicolike.cn

[R71] 日期格式化
来源：http://nu.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xn.521024.cn

[R72] 等待端口就绪
来源：http://mq.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ph.9csxet.cn

[R73] 分割大日志
来源：http://sr.wgjwhj.cn

split -l 1000 big.log part_
来源：http://og.bjjhwx.cn

[R74] 批量重命名
来源：http://dp.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rn.wgjwhj.cn

[R75] 导出环境变量
来源：http://pi.szsharing.cn

export PATH="$HOME/bin:$PATH"
来源：http://if.gzmigu.cn

[R76] 使用临时文件
来源：http://rs.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eb.bookmarksfly.cn

[R77] 读取用户输入
来源：http://zj.bjjhwx.cn

read -rp "请输入: " ans
来源：http://dj.bjjhwx.cn

[R78] 交互式菜单
来源：http://et.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lb.colortex.cn

[R79] 解析命令行选项
来源：http://hs.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yo.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://fn.panjiajie.cn

time ./run.sh
来源：http://lp.yuexingan06.cn

================================================================================
来源：http://ng.huixinmuqiang.cn

S. C / C++ 专题
来源：http://gg.lnxyls.cn

================================================================================
来源：http://kw.wgjwhj.cn

[S01] C：Hello World
来源：http://ct.asd995.cn

#include <stdio.h>
来源：http://px.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yw.nszjky.cn

[S02] C：变量与格式化输出
来源：http://oa.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://pp.521024.cn

[S03] C：读入整数
来源：http://cx.hnjuh.cn

int x; scanf("%d", &x);
来源：http://dc.wgjwhj.cn

[S04] C：字符串复制
来源：http://aw.huixinmuqiang.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zi.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://jk.wgjwhj.cn

strlen(s)
来源：http://xa.shtwfgs.cn

[S06] C：字符串比较
来源：http://of.newstarts.cn

strcmp(a, b) == 0
来源：http://bu.521024.cn

[S07] C：数组遍历求和
来源：http://pc.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qw.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://hg.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nc.huixinmuqiang.cn

[S09] C：结构体定义与初始化
来源：http://yy.shtwfgs.cn


<!-- 参考信息 -->