代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://in.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://so.bookmarksfly.cn

JOIN products p ON p.id = o.product_id;
来源：http://yx.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://vb.wgjwhj.cn

SELECT u.name, o.amount FROM users u
来源：http://pb.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bk.huanxung.cn

[Q43] 标量子查询
来源：http://fh.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ve.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://ko.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pf.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://qf.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hu.bjjhwx.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hc.muxihuayi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xm.chemitech.net.cn

[Q47] 与平均值比较
来源：http://tm.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bs.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://hk.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yr.shxzukj.cn

SELECT * FROM t WHERE c > 5;
来源：http://rp.nszjky.cn

[Q49] 更新单行
来源：http://cy.bookmarksfly.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yk.yuntaijiaju.cn

[Q50] 批量更新
来源：http://zs.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zh.9csxet.cn

[Q51] 用子查询更新
来源：http://ds.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sr.muxihuayi.cn

[Q52] 删除指定行
来源：http://qu.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://rj.panjiajie.cn

[Q53] 按条件删除
来源：http://hm.bookmarksfly.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xb.gzmigu.cn

[Q54] 清空表
来源：http://xi.wgjwhj.cn

TRUNCATE TABLE logs;
来源：http://ui.nicolike.cn

[Q55] 排名（并列占位）
来源：http://rx.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nh.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://tf.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kn.jctech888.com.cn

[Q57] 行号
来源：http://od.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nx.shxzukj.cn

[Q58] 累计求和
来源：http://vb.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gv.shxzskj.cn

[Q59] 分组内累计
来源：http://in.bookmarksfly.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mx.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://uu.9csxet.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jv.jctech888.com.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zq.haigaiapp.cn

[Q61] 移动平均
来源：http://dt.gzmigu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://px.jianghongdianzi.cn

[Q62] 分组占比
来源：http://ux.lnxyls.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ki.huixinmuqiang.cn

[Q63] 开启事务
来源：http://lq.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xj.newstarts.cn

[Q64] 提交事务
来源：http://rj.bjjhwx.cn

COMMIT;
来源：http://pw.newstarts.cn

[Q65] 回滚事务
来源：http://oo.shtwfgs.cn

ROLLBACK;
来源：http://ij.chemitech.net.cn

[Q66] 行锁查询
来源：http://ri.lnxyls.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://df.nszjky.cn

[Q67] 设置隔离级别
来源：http://ex.szsharing.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kd.nicolike.cn

[Q68] 保存点
来源：http://ba.haigaiapp.cn

SAVEPOINT sp1;
来源：http://io.nszjky.cn

ROLLBACK TO sp1;
来源：http://yh.panjiajie.cn

[Q69] 查看执行计划
来源：http://xg.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pf.muxihuayi.cn

[Q70] 更新统计信息
来源：http://jk.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://wk.bjjhwx.cn

[Q71] 查看建表语句
来源：http://os.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hk.yuntaijiaju.cn

[Q72] 查看索引
来源：http://qx.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://vq.shxzskj.cn

[Q73] 查看表状态
来源：http://bs.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pd.muxihuayi.cn

[Q74] 强制使用索引
来源：http://dk.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yg.9csxet.cn

[Q75] 日期格式化
来源：http://iq.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kn.colortex.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ns.szsharing.cn

[Q76] 按天统计
来源：http://js.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aj.bjjhwx.cn

[Q77] 时间加减
来源：http://vp.huixiangedu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://it.colortex.cn

[Q78] 当前时间
来源：http://do.jianghongdianzi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ly.jianghongdianzi.cn

[Q79] 字符串拼接
来源：http://hd.huixiangedu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xu.chemitech.net.cn

[Q80] 字符串截取
来源：http://wz.bjjhwx.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://co.shtwfgs.cn

[Q81] 字符串替换
来源：http://mq.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kn.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://bz.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ez.asd995.cn

[Q83] 大小写转换
来源：http://ae.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kr.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://ie.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://zx.yuexingan06.cn

[Q85] 数值取整
来源：http://er.yuntaijiaju.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zt.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://et.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bo.nicolike.cn

[Q87] JSON 字段做条件
来源：http://mp.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qp.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://bu.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://md.jctech888.com.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uo.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://po.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rj.asd995.cn

[Q90] 生成序号列
来源：http://aq.chemitech.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nu.huanxung.cn

================================================================================
来源：http://xe.lnxyls.cn

R. Bash 专题
来源：http://wq.shxzskj.cn

================================================================================
来源：http://dl.shxzskj.cn

[R01] shebang 与严格模式
来源：http://vn.hnjuh.cn

#!/usr/bin/env bash
来源：http://tl.szxytkj.cn

set -euo pipefail
来源：http://mh.panjiajie.cn

[R02] 变量赋值与使用
来源：http://sx.nszjky.cn

name="Tom"; echo "$name"
来源：http://as.asd995.cn

[R03] 只读变量
来源：http://kx.gzmigu.cn

readonly PI=3.14
来源：http://sk.huixiangedu.cn

[R04] 位置参数
来源：http://ta.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gz.lnxyls.cn

[R05] 参数默认值
来源：http://zo.shxzskj.cn

name="${1:-default}"
来源：http://wg.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://qg.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vt.asd995.cn

[R07] if 判断文件
来源：http://ns.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://do.yuntaijiaju.cn

[R08] 数值比较
来源：http://lo.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fl.szsharing.cn

[R09] 字符串比较
来源：http://jx.lnxyls.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bo.szsharing.cn

[R10] 正则匹配
来源：http://wt.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iq.wgjwhj.cn

[R11] case 多分支
来源：http://de.huixiangedu.cn

case "$1" in
来源：http://ca.nicolike.cn

start) echo "启动" ;;
来源：http://eo.yuexingan06.cn

stop)  echo "停止" ;;
来源：http://rm.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://yl.szxytkj.cn

esac
来源：http://ep.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://gl.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://vr.newstarts.cn

[R13] for 计数循环
来源：http://nx.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://zi.szxytkj.cn

[R14] C 风格 for
来源：http://rp.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uo.hnjuh.cn

[R15] while 逐行读文件
来源：http://nk.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oq.nicolike.cn

[R16] until 等待条件
来源：http://ey.yuexingan06.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wb.gzmigu.cn

[R17] 数组定义与取值
来源：http://rl.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wm.szxytkj.cn

[R18] 遍历数组
来源：http://vf.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vh.huixiangedu.cn

[R19] 数组长度
来源：http://mw.jctech888.com.cn

echo "${#arr[@]}"
来源：http://op.szsharing.cn

[R20] 关联数组（字典）
来源：http://ek.nszjky.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ge.hahajie.cn

[R21] 字符串长度
来源：http://ey.hnjuh.cn

echo "${#s}"
来源：http://ky.shtwfgs.cn

[R22] 截取子串
来源：http://iw.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://es.szsharing.cn

[R23] 字符串替换
来源：http://zo.bjjhwx.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cy.bookmarksfly.cn

[R24] 大小写转换
来源：http://lg.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wk.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://gv.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://va.haigaiapp.cn

[R26] 命令替换
来源：http://ap.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://jo.szxytkj.cn

[R27] 算术展开
来源：http://hz.huixinmuqiang.cn

echo $((1 + 2 * 3))
来源：http://cx.jianghongdianzi.cn

[R28] 浮点运算
来源：http://gg.521024.cn

echo "scale=2; 10/3" | bc
来源：http://sa.nszjky.cn

[R29] 定义函数
来源：http://lh.colortex.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vx.huanxung.cn

[R30] 函数返回状态码
来源：http://gq.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://zu.szsharing.cn

[R31] 局部变量
来源：http://zx.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://dv.521024.cn

[R32] 参数个数校验
来源：http://ji.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ct.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://qc.muxihuayi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nx.9csxet.cn

[R34] 退出时清理
来源：http://kb.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ej.huixiangedu.cn

[R35] 后台执行并等待
来源：http://go.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zg.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://qg.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vw.nicolike.cn

[R37] 把输出赋给变量
来源：http://yr.huixiangedu.cn

files=$(ls -1)
来源：http://ja.huanxung.cn

[R38] 管道串联
来源：http://ds.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://zf.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://nc.jctech888.com.cn

cmd > out.log 2>&1
来源：http://eo.colortex.cn

[R40] 追加写日志
来源：http://yn.yuntaijiaju.cn

echo "log" >> out.log
来源：http://nq.newstarts.cn

[R41] 丢弃输出
来源：http://gu.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://wf.nszjky.cn

[R42] 输入重定向
来源：http://ls.shxzskj.cn

wc -l < a.txt
来源：http://mf.huanxung.cn

[R43] 按名字查找文件
来源：http://bm.panjiajie.cn

find . -name "*.log" -type f
来源：http://yq.lnxyls.cn

[R44] 按修改时间查找
来源：http://wb.haigaiapp.cn

find . -mtime -7 -type f
来源：http://qe.hahajie.cn

[R45] 批量删除
来源：http://vq.nicolike.cn

find . -name "*.tmp" -delete
来源：http://ym.shxzskj.cn

[R46] 递归替换文件内容
来源：http://tp.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fb.9csxet.cn

[R47] sed 单行替换
来源：http://ea.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ep.haigaiapp.cn

[R48] awk 取指定列
来源：http://je.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://em.szsharing.cn

[R49] awk 带条件
来源：http://pd.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ut.521024.cn

[R50] awk 求和
来源：http://ng.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bt.hnjuh.cn

[R51] 排序去重取前几
来源：http://bs.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xj.haigaiapp.cn

[R52] 统计行数
来源：http://zv.huanxung.cn

wc -l a.txt
来源：http://ql.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://tr.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fu.521024.cn

[R54] 比较两个文件
来源：http://rd.jctech888.com.cn

diff a.txt b.txt
来源：http://bz.jianghongdianzi.cn

[R55] 压缩与解压
来源：http://rz.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jj.yuexingan06.cn

[R56] 远程拷贝
来源：http://hb.hahajie.cn

scp file user@host:/path/
来源：http://ob.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://cj.gzmigu.cn

ssh user@host 'uptime'
来源：http://lm.jctech888.com.cn

[R58] 下载文件
来源：http://wz.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jl.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://mv.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hg.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://vq.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ga.bjjhwx.cn

[R61] 磁盘占用
来源：http://ym.nicolike.cn

df -h;  du -sh *
来源：http://uq.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://rx.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://am.yuntaijiaju.cn

[R63] 内存与进程
来源：http://xk.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://sy.shxzskj.cn

[R64] 结束进程
来源：http://zi.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://wf.szxytkj.cn

[R65] 查看端口占用
来源：http://cv.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hr.hnjuh.cn

[R66] 定时任务
来源：http://ug.bookmarksfly.cn

crontab -e;  crontab -l
来源：http://jn.newstarts.cn

[R67] 生成随机十六进制串
来源：http://ni.gzmigu.cn

openssl rand -hex 16
来源：http://be.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://ai.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uy.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://tb.huixinmuqiang.cn

head -c 16 /dev/urandom | base64
来源：http://nb.colortex.cn

[R70] 时间戳与互转
来源：http://mh.colortex.cn

date +%s;  date -d @1700000000
来源：http://af.colortex.cn

[R71] 日期格式化
来源：http://yf.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qy.lnxyls.cn

[R72] 等待端口就绪
来源：http://ko.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sg.panjiajie.cn

[R73] 分割大日志
来源：http://gg.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://me.huanxung.cn

[R74] 批量重命名
来源：http://yl.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mt.szsharing.cn

[R75] 导出环境变量
来源：http://pc.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://ue.nszjky.cn

[R76] 使用临时文件
来源：http://ry.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oc.newstarts.cn

[R77] 读取用户输入
来源：http://nd.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://us.panjiajie.cn

[R78] 交互式菜单
来源：http://rg.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zg.colortex.cn

[R79] 解析命令行选项
来源：http://sk.9csxet.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://av.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://jd.yuntaijiaju.cn

time ./run.sh
来源：http://mp.colortex.cn

================================================================================
来源：http://cz.yuntaijiaju.cn

S. C / C++ 专题
来源：http://xx.shtwfgs.cn

================================================================================
来源：http://hl.lnxyls.cn

[S01] C：Hello World
来源：http://sa.panjiajie.cn

#include <stdio.h>
来源：http://dx.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kk.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://fy.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://uj.newstarts.cn

[S03] C：读入整数
来源：http://hn.newstarts.cn

int x; scanf("%d", &x);
来源：http://zd.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://wl.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://go.lnxyls.cn

[S05] C：字符串长度
来源：http://dg.newstarts.cn

strlen(s)
来源：http://nu.colortex.cn

[S06] C：字符串比较
来源：http://uy.szsharing.cn

strcmp(a, b) == 0
来源：http://db.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://bb.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ri.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://qp.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rj.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://qe.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tu.szsharing.cn

[S10] C：指针与解引用
来源：http://hr.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://lk.521024.cn

[S11] C：逐行读文件
来源：http://bw.hahajie.cn


<!-- 参考信息 -->