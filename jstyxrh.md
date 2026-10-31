代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://rv.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jf.9csxet.cn

[Q43] 标量子查询
来源：http://iz.shtwfgs.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dz.colortex.cn

[Q44] IN 子查询
来源：http://pg.newstarts.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oj.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://er.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vv.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sp.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zp.gzmigu.cn

[Q47] 与平均值比较
来源：http://wn.nicolike.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pq.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://zc.jctech888.com.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gn.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://wy.muxihuayi.cn

[Q49] 更新单行
来源：http://vm.szxytkj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qu.nszjky.cn

[Q50] 批量更新
来源：http://hz.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aa.shxzskj.cn

[Q51] 用子查询更新
来源：http://xl.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nc.bookmarksfly.cn

[Q52] 删除指定行
来源：http://em.panjiajie.cn

DELETE FROM users WHERE id = 10;
来源：http://oc.yuexingan06.cn

[Q53] 按条件删除
来源：http://qv.hahajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bg.huixinmuqiang.cn

[Q54] 清空表
来源：http://qi.newstarts.cn

TRUNCATE TABLE logs;
来源：http://ba.asd995.cn

[Q55] 排名（并列占位）
来源：http://xh.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nx.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://wr.wgjwhj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tk.szsharing.cn

[Q57] 行号
来源：http://ok.jctech888.com.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nx.521024.cn

[Q58] 累计求和
来源：http://vz.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ws.chemitech.net.cn

[Q59] 分组内累计
来源：http://xh.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ue.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://vw.shxzukj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dn.haigaiapp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sv.bookmarksfly.cn

[Q61] 移动平均
来源：http://hf.shxzukj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tj.colortex.cn

[Q62] 分组占比
来源：http://bb.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gw.jianghongdianzi.cn

[Q63] 开启事务
来源：http://uw.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lc.jianghongdianzi.cn

[Q64] 提交事务
来源：http://vj.jianghongdianzi.cn

COMMIT;
来源：http://us.haigaiapp.cn

[Q65] 回滚事务
来源：http://wq.asd995.cn

ROLLBACK;
来源：http://zy.521024.cn

[Q66] 行锁查询
来源：http://ez.gzmigu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qi.asd995.cn

[Q67] 设置隔离级别
来源：http://rs.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hl.wgjwhj.cn

[Q68] 保存点
来源：http://lz.szxytkj.cn

SAVEPOINT sp1;
来源：http://ob.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://rp.muxihuayi.cn

[Q69] 查看执行计划
来源：http://lw.panjiajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yl.huixiangedu.cn

[Q70] 更新统计信息
来源：http://ed.chemitech.net.cn

ANALYZE TABLE users;
来源：http://xu.huixiangedu.cn

[Q71] 查看建表语句
来源：http://dy.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xu.szxytkj.cn

[Q72] 查看索引
来源：http://gz.colortex.cn

SHOW INDEX FROM users;
来源：http://od.yuexingan06.cn

[Q73] 查看表状态
来源：http://lj.shxzskj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fo.shxzskj.cn

[Q74] 强制使用索引
来源：http://dj.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oz.chemitech.net.cn

[Q75] 日期格式化
来源：http://kf.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kt.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ll.521024.cn

[Q76] 按天统计
来源：http://ds.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oq.haigaiapp.cn

[Q77] 时间加减
来源：http://dm.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ej.521024.cn

[Q78] 当前时间
来源：http://rg.szxytkj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hd.hnjuh.cn

[Q79] 字符串拼接
来源：http://lw.huanxung.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hy.haigaiapp.cn

[Q80] 字符串截取
来源：http://em.jianghongdianzi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rw.gzmigu.cn

[Q81] 字符串替换
来源：http://yg.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yn.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://ef.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fk.huanxung.cn

[Q83] 大小写转换
来源：http://rm.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dc.shxzukj.cn

[Q84] 去除首尾空格
来源：http://gd.jctech888.com.cn

SELECT TRIM(name) FROM users;
来源：http://fl.muxihuayi.cn

[Q85] 数值取整
来源：http://vy.nicolike.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ir.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://dx.bjjhwx.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nj.bjjhwx.cn

[Q87] JSON 字段做条件
来源：http://sh.shtwfgs.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://js.chemitech.net.cn

[Q88] 行转列（条件聚合）
来源：http://qb.szsharing.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vb.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cn.hahajie.cn

[Q89] 判断表是否存在
来源：http://jo.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oo.asd995.cn

[Q90] 生成序号列
来源：http://sq.chemitech.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://my.nicolike.cn

================================================================================
来源：http://eg.bjjhwx.cn

R. Bash 专题
来源：http://ph.hahajie.cn

================================================================================
来源：http://ej.szxytkj.cn

[R01] shebang 与严格模式
来源：http://ne.huixiangedu.cn

#!/usr/bin/env bash
来源：http://qm.colortex.cn

set -euo pipefail
来源：http://qa.hnjuh.cn

[R02] 变量赋值与使用
来源：http://el.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://rt.wgjwhj.cn

[R03] 只读变量
来源：http://hk.haigaiapp.cn

readonly PI=3.14
来源：http://oj.jianghongdianzi.cn

[R04] 位置参数
来源：http://zr.521024.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bx.huanxung.cn

[R05] 参数默认值
来源：http://vz.panjiajie.cn

name="${1:-default}"
来源：http://tr.newstarts.cn

[R06] 判断命令是否存在
来源：http://uk.bjjhwx.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://to.shxzskj.cn

[R07] if 判断文件
来源：http://nc.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ov.lnxyls.cn

[R08] 数值比较
来源：http://mt.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mw.colortex.cn

[R09] 字符串比较
来源：http://kn.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nz.szxytkj.cn

[R10] 正则匹配
来源：http://mi.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vk.hahajie.cn

[R11] case 多分支
来源：http://tu.shxzskj.cn

case "$1" in
来源：http://ax.hnjuh.cn

start) echo "启动" ;;
来源：http://ex.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://ww.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://en.jianghongdianzi.cn

esac
来源：http://gb.muxihuayi.cn

[R12] for 遍历文件
来源：http://jr.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://dn.huixinmuqiang.cn

[R13] for 计数循环
来源：http://at.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://tq.nszjky.cn

[R14] C 风格 for
来源：http://it.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kn.szxytkj.cn

[R15] while 逐行读文件
来源：http://xv.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jg.hnjuh.cn

[R16] until 等待条件
来源：http://zz.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bc.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://hk.muxihuayi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bd.huixiangedu.cn

[R18] 遍历数组
来源：http://xu.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eu.wgjwhj.cn

[R19] 数组长度
来源：http://jm.lnxyls.cn

echo "${#arr[@]}"
来源：http://yv.panjiajie.cn

[R20] 关联数组（字典）
来源：http://ka.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ri.yuntaijiaju.cn

[R21] 字符串长度
来源：http://ao.chemitech.net.cn

echo "${#s}"
来源：http://gb.muxihuayi.cn

[R22] 截取子串
来源：http://xa.hahajie.cn

echo "${s:0:5}"
来源：http://dg.nszjky.cn

[R23] 字符串替换
来源：http://ta.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sb.hnjuh.cn

[R24] 大小写转换
来源：http://hv.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zc.9csxet.cn

[R25] 去后缀 / 去前缀
来源：http://ez.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bg.yuntaijiaju.cn

[R26] 命令替换
来源：http://do.colortex.cn

now=$(date +%F); echo "$now"
来源：http://vd.colortex.cn

[R27] 算术展开
来源：http://kp.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://kf.szsharing.cn

[R28] 浮点运算
来源：http://vy.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://kd.panjiajie.cn

[R29] 定义函数
来源：http://ga.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ie.jctech888.com.cn

[R30] 函数返回状态码
来源：http://po.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://tx.shtwfgs.cn

[R31] 局部变量
来源：http://xx.bjjhwx.cn

f() { local x=1; echo "$x"; }
来源：http://ye.bjjhwx.cn

[R32] 参数个数校验
来源：http://fi.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vo.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://wg.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tv.bjjhwx.cn

[R34] 退出时清理
来源：http://ky.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://go.huixiangedu.cn

[R35] 后台执行并等待
来源：http://ph.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rx.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://je.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xg.nicolike.cn

[R37] 把输出赋给变量
来源：http://rh.newstarts.cn

files=$(ls -1)
来源：http://qi.chemitech.net.cn

[R38] 管道串联
来源：http://dr.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://ov.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://tt.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://hq.colortex.cn

[R40] 追加写日志
来源：http://wj.hahajie.cn

echo "log" >> out.log
来源：http://et.shtwfgs.cn

[R41] 丢弃输出
来源：http://yu.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://xe.bjjhwx.cn

[R42] 输入重定向
来源：http://ez.shtwfgs.cn

wc -l < a.txt
来源：http://tb.asd995.cn

[R43] 按名字查找文件
来源：http://ru.haigaiapp.cn

find . -name "*.log" -type f
来源：http://rs.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://tg.muxihuayi.cn

find . -mtime -7 -type f
来源：http://js.haigaiapp.cn

[R45] 批量删除
来源：http://dx.jianghongdianzi.cn

find . -name "*.tmp" -delete
来源：http://cx.hahajie.cn

[R46] 递归替换文件内容
来源：http://ff.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oa.colortex.cn

[R47] sed 单行替换
来源：http://vt.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vn.shxzskj.cn

[R48] awk 取指定列
来源：http://fa.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://xj.haigaiapp.cn

[R49] awk 带条件
来源：http://ly.chemitech.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tg.asd995.cn

[R50] awk 求和
来源：http://rl.jctech888.com.cn

awk '{s += $2} END {print s}' a.txt
来源：http://le.chemitech.net.cn

[R51] 排序去重取前几
来源：http://lz.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ez.colortex.cn

[R52] 统计行数
来源：http://fz.jianghongdianzi.cn

wc -l a.txt
来源：http://bb.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://ri.shxzskj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wd.huanxung.cn

[R54] 比较两个文件
来源：http://cz.nicolike.cn

diff a.txt b.txt
来源：http://mx.shtwfgs.cn

[R55] 压缩与解压
来源：http://vn.hahajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ob.wgjwhj.cn

[R56] 远程拷贝
来源：http://ye.hnjuh.cn

scp file user@host:/path/
来源：http://vp.bookmarksfly.cn

[R57] 远程执行命令
来源：http://dq.szxytkj.cn

ssh user@host 'uptime'
来源：http://vp.huixiangedu.cn

[R58] 下载文件
来源：http://jl.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gz.haigaiapp.cn

[R59] 发 POST JSON
来源：http://pk.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ka.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://tt.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nu.newstarts.cn

[R61] 磁盘占用
来源：http://zf.shtwfgs.cn

df -h;  du -sh *
来源：http://gh.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://ur.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://sr.shxzukj.cn

[R63] 内存与进程
来源：http://ml.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://yv.hnjuh.cn

[R64] 结束进程
来源：http://jd.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://ka.chemitech.net.cn

[R65] 查看端口占用
来源：http://ns.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sq.gzmigu.cn

[R66] 定时任务
来源：http://gk.szxytkj.cn

crontab -e;  crontab -l
来源：http://ct.jctech888.com.cn

[R67] 生成随机十六进制串
来源：http://ic.haigaiapp.cn

openssl rand -hex 16
来源：http://qr.colortex.cn

[R68] 计算文件校验值
来源：http://nl.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ka.szsharing.cn

[R69] 生成随机密码
来源：http://jl.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://ku.bjjhwx.cn

[R70] 时间戳与互转
来源：http://tp.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://hm.huanxung.cn

[R71] 日期格式化
来源：http://md.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://as.huixiangedu.cn

[R72] 等待端口就绪
来源：http://ua.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ro.nicolike.cn

[R73] 分割大日志
来源：http://bk.hnjuh.cn

split -l 1000 big.log part_
来源：http://fp.haigaiapp.cn

[R74] 批量重命名
来源：http://ar.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ik.521024.cn

[R75] 导出环境变量
来源：http://rz.bjjhwx.cn

export PATH="$HOME/bin:$PATH"
来源：http://lc.9csxet.cn

[R76] 使用临时文件
来源：http://qe.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fy.colortex.cn

[R77] 读取用户输入
来源：http://ki.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://dx.szxytkj.cn

[R78] 交互式菜单
来源：http://vt.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lv.shtwfgs.cn

[R79] 解析命令行选项
来源：http://io.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jf.shxzukj.cn

[R80] 查看脚本执行耗时
来源：http://gg.shxzukj.cn

time ./run.sh
来源：http://ww.szsharing.cn

================================================================================
来源：http://lw.9csxet.cn

S. C / C++ 专题
来源：http://fu.newstarts.cn

================================================================================
来源：http://tc.bookmarksfly.cn

[S01] C：Hello World
来源：http://ry.9csxet.cn

#include <stdio.h>
来源：http://lg.huixiangedu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hd.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://dy.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://oz.muxihuayi.cn

[S03] C：读入整数
来源：http://uh.gzmigu.cn

int x; scanf("%d", &x);
来源：http://us.bookmarksfly.cn

[S04] C：字符串复制
来源：http://gy.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://va.521024.cn

[S05] C：字符串长度
来源：http://ks.haigaiapp.cn

strlen(s)
来源：http://lk.szxytkj.cn

[S06] C：字符串比较
来源：http://ka.shtwfgs.cn

strcmp(a, b) == 0
来源：http://kk.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://wg.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wl.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://fq.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mp.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://qr.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sg.hnjuh.cn

[S10] C：指针与解引用
来源：http://vg.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://go.521024.cn

[S11] C：逐行读文件
来源：http://up.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://zb.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ez.huanxung.cn

fclose(f);
来源：http://xh.hahajie.cn

[S12] C：写文件
来源：http://ql.lnxyls.cn


<!-- 参考信息 -->