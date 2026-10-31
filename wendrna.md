代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://kc.huixiangedu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zz.hahajie.cn

[Q47] 与平均值比较
来源：http://ff.shtwfgs.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iv.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://sf.newstarts.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ye.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://mz.nicolike.cn

[Q49] 更新单行
来源：http://cp.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kr.wgjwhj.cn

[Q50] 批量更新
来源：http://uj.yuntaijiaju.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ds.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://ry.yuntaijiaju.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://we.bjjhwx.cn

[Q52] 删除指定行
来源：http://ut.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://dc.huixiangedu.cn

[Q53] 按条件删除
来源：http://nn.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rk.yuexingan06.cn

[Q54] 清空表
来源：http://sg.521024.cn

TRUNCATE TABLE logs;
来源：http://rf.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://zh.nszjky.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zd.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://wy.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zd.huanxung.cn

[Q57] 行号
来源：http://fw.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ni.nicolike.cn

[Q58] 累计求和
来源：http://ni.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ny.shtwfgs.cn

[Q59] 分组内累计
来源：http://hg.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ws.panjiajie.cn

[Q60] 取上一行 / 下一行
来源：http://ok.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rv.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jw.hnjuh.cn

[Q61] 移动平均
来源：http://hq.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oo.gzmigu.cn

[Q62] 分组占比
来源：http://xc.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vw.chemitech.net.cn

[Q63] 开启事务
来源：http://fm.jctech888.com.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mg.szsharing.cn

[Q64] 提交事务
来源：http://qm.colortex.cn

COMMIT;
来源：http://tg.hnjuh.cn

[Q65] 回滚事务
来源：http://oo.huixinmuqiang.cn

ROLLBACK;
来源：http://pm.huixinmuqiang.cn

[Q66] 行锁查询
来源：http://zn.chemitech.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ig.hnjuh.cn

[Q67] 设置隔离级别
来源：http://dk.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fw.huanxung.cn

[Q68] 保存点
来源：http://jx.shtwfgs.cn

SAVEPOINT sp1;
来源：http://jr.colortex.cn

ROLLBACK TO sp1;
来源：http://ty.shxzskj.cn

[Q69] 查看执行计划
来源：http://sa.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lg.lnxyls.cn

[Q70] 更新统计信息
来源：http://yz.huanxung.cn

ANALYZE TABLE users;
来源：http://uw.hnjuh.cn

[Q71] 查看建表语句
来源：http://ti.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ca.hahajie.cn

[Q72] 查看索引
来源：http://xi.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://rg.haigaiapp.cn

[Q73] 查看表状态
来源：http://qx.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yp.newstarts.cn

[Q74] 强制使用索引
来源：http://hv.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ij.lnxyls.cn

[Q75] 日期格式化
来源：http://tq.huanxung.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tr.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bi.szxytkj.cn

[Q76] 按天统计
来源：http://ay.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yx.jianghongdianzi.cn

[Q77] 时间加减
来源：http://im.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vv.shxzukj.cn

[Q78] 当前时间
来源：http://wi.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mw.nicolike.cn

[Q79] 字符串拼接
来源：http://lq.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wq.shtwfgs.cn

[Q80] 字符串截取
来源：http://mg.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kp.yuexingan06.cn

[Q81] 字符串替换
来源：http://rj.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://px.lnxyls.cn

[Q82] 字符长度与字节长度
来源：http://oy.szsharing.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gg.jctech888.com.cn

[Q83] 大小写转换
来源：http://bp.szsharing.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dy.yuexingan06.cn

[Q84] 去除首尾空格
来源：http://ay.shxzukj.cn

SELECT TRIM(name) FROM users;
来源：http://it.yuntaijiaju.cn

[Q85] 数值取整
来源：http://ez.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fd.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://eh.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ac.colortex.cn

[Q87] JSON 字段做条件
来源：http://ub.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ep.521024.cn

[Q88] 行转列（条件聚合）
来源：http://do.huixiangedu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kj.hnjuh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sd.521024.cn

[Q89] 判断表是否存在
来源：http://ox.jianghongdianzi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ow.colortex.cn

[Q90] 生成序号列
来源：http://zs.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cg.nicolike.cn

================================================================================
来源：http://lk.muxihuayi.cn

R. Bash 专题
来源：http://ss.newstarts.cn

================================================================================
来源：http://pg.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://zt.yuexingan06.cn

#!/usr/bin/env bash
来源：http://gy.bookmarksfly.cn

set -euo pipefail
来源：http://xv.nszjky.cn

[R02] 变量赋值与使用
来源：http://sr.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://my.hahajie.cn

[R03] 只读变量
来源：http://ik.nicolike.cn

readonly PI=3.14
来源：http://mp.muxihuayi.cn

[R04] 位置参数
来源：http://qf.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oi.wgjwhj.cn

[R05] 参数默认值
来源：http://ll.9csxet.cn

name="${1:-default}"
来源：http://to.shxzukj.cn

[R06] 判断命令是否存在
来源：http://gs.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vt.bookmarksfly.cn

[R07] if 判断文件
来源：http://gm.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zj.huanxung.cn

[R08] 数值比较
来源：http://gt.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hi.muxihuayi.cn

[R09] 字符串比较
来源：http://sf.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bh.asd995.cn

[R10] 正则匹配
来源：http://wf.shtwfgs.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jz.lnxyls.cn

[R11] case 多分支
来源：http://zp.jianghongdianzi.cn

case "$1" in
来源：http://wm.gzmigu.cn

start) echo "启动" ;;
来源：http://vq.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://ch.9csxet.cn

*)     echo "未知命令" ;;
来源：http://ut.9csxet.cn

esac
来源：http://ai.lnxyls.cn

[R12] for 遍历文件
来源：http://xp.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://ss.hahajie.cn

[R13] for 计数循环
来源：http://qo.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://zm.hnjuh.cn

[R14] C 风格 for
来源：http://cm.lnxyls.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nl.shxzukj.cn

[R15] while 逐行读文件
来源：http://eo.yuexingan06.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dz.haigaiapp.cn

[R16] until 等待条件
来源：http://nv.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ul.gzmigu.cn

[R17] 数组定义与取值
来源：http://ym.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dq.nicolike.cn

[R18] 遍历数组
来源：http://kn.huixiangedu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cg.huixiangedu.cn

[R19] 数组长度
来源：http://bm.szxytkj.cn

echo "${#arr[@]}"
来源：http://kb.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://pz.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://al.szsharing.cn

[R21] 字符串长度
来源：http://rf.muxihuayi.cn

echo "${#s}"
来源：http://ph.lnxyls.cn

[R22] 截取子串
来源：http://zg.chemitech.net.cn

echo "${s:0:5}"
来源：http://mp.bookmarksfly.cn

[R23] 字符串替换
来源：http://pj.lnxyls.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nx.colortex.cn

[R24] 大小写转换
来源：http://ze.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mk.shtwfgs.cn

[R25] 去后缀 / 去前缀
来源：http://vr.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rz.lnxyls.cn

[R26] 命令替换
来源：http://yd.yuexingan06.cn

now=$(date +%F); echo "$now"
来源：http://xv.bookmarksfly.cn

[R27] 算术展开
来源：http://lm.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://yv.asd995.cn

[R28] 浮点运算
来源：http://rw.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://xq.jctech888.com.cn

[R29] 定义函数
来源：http://zp.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jl.newstarts.cn

[R30] 函数返回状态码
来源：http://qn.muxihuayi.cn

f() { return 0; }; f || echo "失败了"
来源：http://xs.521024.cn

[R31] 局部变量
来源：http://ml.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://ad.shtwfgs.cn

[R32] 参数个数校验
来源：http://jb.haigaiapp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sm.521024.cn

[R33] 捕获错误并提示行号
来源：http://ik.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wm.hnjuh.cn

[R34] 退出时清理
来源：http://vy.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://eu.bjjhwx.cn

[R35] 后台执行并等待
来源：http://eb.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://iv.521024.cn

[R36] 并发执行多个任务
来源：http://mv.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jm.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://mm.shtwfgs.cn

files=$(ls -1)
来源：http://iy.chemitech.net.cn

[R38] 管道串联
来源：http://cz.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://yc.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://tg.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://vw.nicolike.cn

[R40] 追加写日志
来源：http://ow.lnxyls.cn

echo "log" >> out.log
来源：http://hs.wgjwhj.cn

[R41] 丢弃输出
来源：http://av.colortex.cn

cmd >/dev/null 2>&1
来源：http://md.jctech888.com.cn

[R42] 输入重定向
来源：http://od.huanxung.cn

wc -l < a.txt
来源：http://jf.szxytkj.cn

[R43] 按名字查找文件
来源：http://gj.muxihuayi.cn

find . -name "*.log" -type f
来源：http://jl.newstarts.cn

[R44] 按修改时间查找
来源：http://pg.hahajie.cn

find . -mtime -7 -type f
来源：http://wf.521024.cn

[R45] 批量删除
来源：http://kl.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://pv.521024.cn

[R46] 递归替换文件内容
来源：http://zg.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qn.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://ds.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oi.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://iz.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://kt.jctech888.com.cn

[R49] awk 带条件
来源：http://rn.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yv.jctech888.com.cn

[R50] awk 求和
来源：http://kb.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mg.9csxet.cn

[R51] 排序去重取前几
来源：http://ys.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wn.bjjhwx.cn

[R52] 统计行数
来源：http://qz.huixiangedu.cn

wc -l a.txt
来源：http://ba.colortex.cn

[R53] 查看文件头与实时尾
来源：http://sp.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yx.gzmigu.cn

[R54] 比较两个文件
来源：http://dz.shtwfgs.cn

diff a.txt b.txt
来源：http://kp.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://so.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zi.jctech888.com.cn

[R56] 远程拷贝
来源：http://dm.bjjhwx.cn

scp file user@host:/path/
来源：http://nv.haigaiapp.cn

[R57] 远程执行命令
来源：http://za.colortex.cn

ssh user@host 'uptime'
来源：http://gn.shxzukj.cn

[R58] 下载文件
来源：http://rp.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ir.huixiangedu.cn

[R59] 发 POST JSON
来源：http://he.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sa.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://hn.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yn.wgjwhj.cn

[R61] 磁盘占用
来源：http://kj.bjjhwx.cn

df -h;  du -sh *
来源：http://zi.muxihuayi.cn

[R62] 找最占空间的文件
来源：http://hv.asd995.cn

du -ah . | sort -rh | head -10
来源：http://uu.huanxung.cn

[R63] 内存与进程
来源：http://kl.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://hl.shxzskj.cn

[R64] 结束进程
来源：http://of.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://ex.wgjwhj.cn

[R65] 查看端口占用
来源：http://gn.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ar.shxzukj.cn

[R66] 定时任务
来源：http://cb.szxytkj.cn

crontab -e;  crontab -l
来源：http://xz.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://jr.nicolike.cn

openssl rand -hex 16
来源：http://di.huixiangedu.cn

[R68] 计算文件校验值
来源：http://xy.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ox.bookmarksfly.cn

[R69] 生成随机密码
来源：http://ro.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://zv.asd995.cn

[R70] 时间戳与互转
来源：http://go.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://ya.panjiajie.cn

[R71] 日期格式化
来源：http://xp.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mh.newstarts.cn

[R72] 等待端口就绪
来源：http://wz.chemitech.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cs.shtwfgs.cn

[R73] 分割大日志
来源：http://la.yuexingan06.cn

split -l 1000 big.log part_
来源：http://wt.nicolike.cn

[R74] 批量重命名
来源：http://yk.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://at.hnjuh.cn

[R75] 导出环境变量
来源：http://hm.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://ti.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://mx.shxzukj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wf.shtwfgs.cn

[R77] 读取用户输入
来源：http://ns.muxihuayi.cn

read -rp "请输入: " ans
来源：http://tu.yuexingan06.cn

[R78] 交互式菜单
来源：http://wx.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tu.chemitech.net.cn

[R79] 解析命令行选项
来源：http://tr.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sd.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://pf.nicolike.cn

time ./run.sh
来源：http://ew.asd995.cn

================================================================================
来源：http://cr.szxytkj.cn

S. C / C++ 专题
来源：http://tp.jctech888.com.cn

================================================================================
来源：http://zo.szsharing.cn

[S01] C：Hello World
来源：http://ka.nszjky.cn

#include <stdio.h>
来源：http://fm.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xu.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://ov.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://dj.huixiangedu.cn

[S03] C：读入整数
来源：http://bl.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://hc.huanxung.cn

[S04] C：字符串复制
来源：http://dl.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ga.muxihuayi.cn

[S05] C：字符串长度
来源：http://gu.521024.cn

strlen(s)
来源：http://fa.colortex.cn

[S06] C：字符串比较
来源：http://px.haigaiapp.cn

strcmp(a, b) == 0
来源：http://qq.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://vu.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://is.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://ke.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://my.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://cc.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tj.huixiangedu.cn

[S10] C：指针与解引用
来源：http://dj.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://qv.huanxung.cn

[S11] C：逐行读文件
来源：http://ft.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://gl.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gl.bookmarksfly.cn

fclose(f);
来源：http://tp.huixiangedu.cn

[S12] C：写文件
来源：http://ot.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tz.szsharing.cn

[S13] C：宏定义
来源：http://sy.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zw.shtwfgs.cn

[S14] C：枚举
来源：http://ay.shxzukj.cn

enum Color { RED, GREEN, BLUE };
来源：http://pg.bookmarksfly.cn

[S15] C：类型转换
来源：http://ol.muxihuayi.cn

(double) a / b
来源：http://di.lnxyls.cn

[S16] C：位操作置位
来源：http://xm.nszjky.cn


<!-- 参考信息 -->