代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://lb.gzmigu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://de.shxzskj.cn

[Q43] 标量子查询
来源：http://xk.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dk.gzmigu.cn

[Q44] IN 子查询
来源：http://ik.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ph.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://hr.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jo.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zd.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nc.asd995.cn

[Q47] 与平均值比较
来源：http://vs.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bn.szxytkj.cn

[Q48] CTE 公用表表达式
来源：http://gf.newstarts.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://db.gzmigu.cn

SELECT * FROM t WHERE c > 5;
来源：http://va.jianghongdianzi.cn

[Q49] 更新单行
来源：http://js.jianghongdianzi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://aq.bookmarksfly.cn

[Q50] 批量更新
来源：http://jg.colortex.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://te.bjjhwx.cn

[Q51] 用子查询更新
来源：http://zm.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://on.nicolike.cn

[Q52] 删除指定行
来源：http://ha.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://yu.gzmigu.cn

[Q53] 按条件删除
来源：http://qz.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hy.huanxung.cn

[Q54] 清空表
来源：http://vn.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://iw.newstarts.cn

[Q55] 排名（并列占位）
来源：http://dp.nicolike.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://af.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://ro.haigaiapp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sl.9csxet.cn

[Q57] 行号
来源：http://yk.shxzskj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://di.bjjhwx.cn

[Q58] 累计求和
来源：http://gq.9csxet.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sa.yuntaijiaju.cn

[Q59] 分组内累计
来源：http://jb.huanxung.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cy.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://hx.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dq.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vz.chemitech.net.cn

[Q61] 移动平均
来源：http://bg.haigaiapp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://za.521024.cn

[Q62] 分组占比
来源：http://pw.shtwfgs.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ls.chemitech.net.cn

[Q63] 开启事务
来源：http://vw.haigaiapp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zv.lnxyls.cn

[Q64] 提交事务
来源：http://yx.huixiangedu.cn

COMMIT;
来源：http://gy.szxytkj.cn

[Q65] 回滚事务
来源：http://hf.bookmarksfly.cn

ROLLBACK;
来源：http://od.wgjwhj.cn

[Q66] 行锁查询
来源：http://ot.huixinmuqiang.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://on.wgjwhj.cn

[Q67] 设置隔离级别
来源：http://zt.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kt.panjiajie.cn

[Q68] 保存点
来源：http://cb.lnxyls.cn

SAVEPOINT sp1;
来源：http://cm.bookmarksfly.cn

ROLLBACK TO sp1;
来源：http://kn.jctech888.com.cn

[Q69] 查看执行计划
来源：http://ss.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ja.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://ie.huixiangedu.cn

ANALYZE TABLE users;
来源：http://mt.hnjuh.cn

[Q71] 查看建表语句
来源：http://kw.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pp.colortex.cn

[Q72] 查看索引
来源：http://pb.szxytkj.cn

SHOW INDEX FROM users;
来源：http://bs.wgjwhj.cn

[Q73] 查看表状态
来源：http://mn.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://od.szxytkj.cn

[Q74] 强制使用索引
来源：http://xw.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jc.521024.cn

[Q75] 日期格式化
来源：http://zg.nicolike.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kf.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vn.nicolike.cn

[Q76] 按天统计
来源：http://by.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rp.hahajie.cn

[Q77] 时间加减
来源：http://sc.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zg.shxzskj.cn

[Q78] 当前时间
来源：http://mz.9csxet.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://as.muxihuayi.cn

[Q79] 字符串拼接
来源：http://en.9csxet.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jt.haigaiapp.cn

[Q80] 字符串截取
来源：http://ho.panjiajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gv.521024.cn

[Q81] 字符串替换
来源：http://cl.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iw.muxihuayi.cn

[Q82] 字符长度与字节长度
来源：http://oo.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tu.szxytkj.cn

[Q83] 大小写转换
来源：http://je.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pk.hnjuh.cn

[Q84] 去除首尾空格
来源：http://yn.colortex.cn

SELECT TRIM(name) FROM users;
来源：http://qh.panjiajie.cn

[Q85] 数值取整
来源：http://rb.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xb.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://hh.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ix.9csxet.cn

[Q87] JSON 字段做条件
来源：http://zv.nszjky.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wn.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://rq.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ud.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sf.huixinmuqiang.cn

[Q89] 判断表是否存在
来源：http://gv.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rl.bjjhwx.cn

[Q90] 生成序号列
来源：http://ed.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yu.panjiajie.cn

================================================================================
来源：http://ev.wgjwhj.cn

R. Bash 专题
来源：http://tv.shxzukj.cn

================================================================================
来源：http://od.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://hg.521024.cn

#!/usr/bin/env bash
来源：http://to.521024.cn

set -euo pipefail
来源：http://dk.hahajie.cn

[R02] 变量赋值与使用
来源：http://fd.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://kq.szsharing.cn

[R03] 只读变量
来源：http://ky.jctech888.com.cn

readonly PI=3.14
来源：http://gi.nszjky.cn

[R04] 位置参数
来源：http://yt.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jo.newstarts.cn

[R05] 参数默认值
来源：http://no.panjiajie.cn

name="${1:-default}"
来源：http://hl.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://ot.shtwfgs.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ta.shxzukj.cn

[R07] if 判断文件
来源：http://gt.newstarts.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zs.asd995.cn

[R08] 数值比较
来源：http://vm.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pr.bjjhwx.cn

[R09] 字符串比较
来源：http://bx.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fi.hahajie.cn

[R10] 正则匹配
来源：http://bg.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wf.shxzukj.cn

[R11] case 多分支
来源：http://wv.huanxung.cn

case "$1" in
来源：http://ld.huixiangedu.cn

start) echo "启动" ;;
来源：http://rh.521024.cn

stop)  echo "停止" ;;
来源：http://jg.newstarts.cn

*)     echo "未知命令" ;;
来源：http://cr.jctech888.com.cn

esac
来源：http://kv.jctech888.com.cn

[R12] for 遍历文件
来源：http://xv.colortex.cn

for f in *.txt; do echo "$f"; done
来源：http://zl.wgjwhj.cn

[R13] for 计数循环
来源：http://nm.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://qv.shxzskj.cn

[R14] C 风格 for
来源：http://xe.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wf.huixiangedu.cn

[R15] while 逐行读文件
来源：http://bi.jctech888.com.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mg.shxzskj.cn

[R16] until 等待条件
来源：http://tm.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://og.chemitech.net.cn

[R17] 数组定义与取值
来源：http://oa.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wk.hnjuh.cn

[R18] 遍历数组
来源：http://ao.newstarts.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ye.shxzskj.cn

[R19] 数组长度
来源：http://he.panjiajie.cn

echo "${#arr[@]}"
来源：http://sb.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://ct.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oy.yuexingan06.cn

[R21] 字符串长度
来源：http://ip.shxzskj.cn

echo "${#s}"
来源：http://gu.nszjky.cn

[R22] 截取子串
来源：http://db.newstarts.cn

echo "${s:0:5}"
来源：http://jn.hahajie.cn

[R23] 字符串替换
来源：http://xd.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hg.colortex.cn

[R24] 大小写转换
来源：http://ih.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zb.panjiajie.cn

[R25] 去后缀 / 去前缀
来源：http://rt.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wa.huanxung.cn

[R26] 命令替换
来源：http://ri.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://kq.szsharing.cn

[R27] 算术展开
来源：http://xp.nszjky.cn

echo $((1 + 2 * 3))
来源：http://cs.bookmarksfly.cn

[R28] 浮点运算
来源：http://vq.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://gv.yuexingan06.cn

[R29] 定义函数
来源：http://hd.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ps.bjjhwx.cn

[R30] 函数返回状态码
来源：http://gy.521024.cn

f() { return 0; }; f || echo "失败了"
来源：http://pd.yuexingan06.cn

[R31] 局部变量
来源：http://lc.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://az.bookmarksfly.cn

[R32] 参数个数校验
来源：http://vn.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fu.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://xb.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cu.chemitech.net.cn

[R34] 退出时清理
来源：http://hh.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hm.asd995.cn

[R35] 后台执行并等待
来源：http://em.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://di.newstarts.cn

[R36] 并发执行多个任务
来源：http://zd.nszjky.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://du.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://vc.muxihuayi.cn

files=$(ls -1)
来源：http://xz.lnxyls.cn

[R38] 管道串联
来源：http://eh.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://dk.521024.cn

[R39] 重定向标准输出与错误
来源：http://nu.lnxyls.cn

cmd > out.log 2>&1
来源：http://rd.muxihuayi.cn

[R40] 追加写日志
来源：http://su.jianghongdianzi.cn

echo "log" >> out.log
来源：http://xj.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://bx.colortex.cn

cmd >/dev/null 2>&1
来源：http://xt.9csxet.cn

[R42] 输入重定向
来源：http://mr.muxihuayi.cn

wc -l < a.txt
来源：http://rr.shxzskj.cn

[R43] 按名字查找文件
来源：http://vo.hahajie.cn

find . -name "*.log" -type f
来源：http://fl.wgjwhj.cn

[R44] 按修改时间查找
来源：http://gc.shxzukj.cn

find . -mtime -7 -type f
来源：http://xm.haigaiapp.cn

[R45] 批量删除
来源：http://yf.szxytkj.cn

find . -name "*.tmp" -delete
来源：http://lr.yuntaijiaju.cn

[R46] 递归替换文件内容
来源：http://aa.hnjuh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mn.chemitech.net.cn

[R47] sed 单行替换
来源：http://lm.shxzukj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nb.9csxet.cn

[R48] awk 取指定列
来源：http://zq.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://ny.9csxet.cn

[R49] awk 带条件
来源：http://nz.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vy.521024.cn

[R50] awk 求和
来源：http://jd.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yk.colortex.cn

[R51] 排序去重取前几
来源：http://uf.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ms.panjiajie.cn

[R52] 统计行数
来源：http://dp.nicolike.cn

wc -l a.txt
来源：http://xu.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://ct.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ah.lnxyls.cn

[R54] 比较两个文件
来源：http://cx.shtwfgs.cn

diff a.txt b.txt
来源：http://ns.asd995.cn

[R55] 压缩与解压
来源：http://ke.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zh.9csxet.cn

[R56] 远程拷贝
来源：http://pt.bjjhwx.cn

scp file user@host:/path/
来源：http://yz.shxzskj.cn

[R57] 远程执行命令
来源：http://kh.szxytkj.cn

ssh user@host 'uptime'
来源：http://kg.huanxung.cn

[R58] 下载文件
来源：http://xb.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tf.hahajie.cn

[R59] 发 POST JSON
来源：http://jy.jianghongdianzi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xl.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://ca.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lb.shxzukj.cn

[R61] 磁盘占用
来源：http://ao.nicolike.cn

df -h;  du -sh *
来源：http://zt.asd995.cn

[R62] 找最占空间的文件
来源：http://gc.bookmarksfly.cn

du -ah . | sort -rh | head -10
来源：http://ng.wgjwhj.cn

[R63] 内存与进程
来源：http://tt.newstarts.cn

free -h;  ps aux | grep nginx
来源：http://uj.huixiangedu.cn

[R64] 结束进程
来源：http://ub.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://nw.chemitech.net.cn

[R65] 查看端口占用
来源：http://sj.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qu.gzmigu.cn

[R66] 定时任务
来源：http://or.shtwfgs.cn

crontab -e;  crontab -l
来源：http://ua.asd995.cn

[R67] 生成随机十六进制串
来源：http://xw.huixiangedu.cn

openssl rand -hex 16
来源：http://jo.521024.cn

[R68] 计算文件校验值
来源：http://xv.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://df.colortex.cn

[R69] 生成随机密码
来源：http://vf.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://af.gzmigu.cn

[R70] 时间戳与互转
来源：http://dk.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://iv.shxzukj.cn

[R71] 日期格式化
来源：http://sp.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://od.nicolike.cn

[R72] 等待端口就绪
来源：http://gz.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uf.asd995.cn

[R73] 分割大日志
来源：http://qs.shxzskj.cn

split -l 1000 big.log part_
来源：http://yn.szxytkj.cn

[R74] 批量重命名
来源：http://yo.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xz.asd995.cn

[R75] 导出环境变量
来源：http://wf.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://hg.shxzukj.cn

[R76] 使用临时文件
来源：http://ty.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hi.wgjwhj.cn

[R77] 读取用户输入
来源：http://zh.shtwfgs.cn

read -rp "请输入: " ans
来源：http://jk.wgjwhj.cn

[R78] 交互式菜单
来源：http://wp.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ji.colortex.cn

[R79] 解析命令行选项
来源：http://ec.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ik.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://pg.szxytkj.cn

time ./run.sh
来源：http://na.hnjuh.cn

================================================================================
来源：http://xh.chemitech.net.cn

S. C / C++ 专题
来源：http://iw.chemitech.net.cn

================================================================================
来源：http://cu.521024.cn

[S01] C：Hello World
来源：http://sq.haigaiapp.cn

#include <stdio.h>
来源：http://qq.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vk.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://cy.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://bw.haigaiapp.cn

[S03] C：读入整数
来源：http://bl.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://yz.jctech888.com.cn

[S04] C：字符串复制
来源：http://mz.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pg.panjiajie.cn

[S05] C：字符串长度
来源：http://tm.lnxyls.cn

strlen(s)
来源：http://ml.hahajie.cn

[S06] C：字符串比较
来源：http://jp.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://ys.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://dq.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mq.huixinmuqiang.cn

[S08] C：动态内存分配与释放
来源：http://ho.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qd.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://hd.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ir.521024.cn

[S10] C：指针与解引用
来源：http://re.521024.cn

int *p = &a;  *p = 5;
来源：http://ei.szsharing.cn

[S11] C：逐行读文件
来源：http://kx.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://bn.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ea.asd995.cn

fclose(f);
来源：http://vv.szxytkj.cn

[S12] C：写文件
来源：http://ho.bookmarksfly.cn


<!-- 参考信息 -->