代发 wailian999

[Q44] IN 子查询
来源：http://jp.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rq.lnxyls.cn

[Q45] EXISTS 判断存在
来源：http://ll.newstarts.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vu.nszjky.cn

[Q46] NOT EXISTS 判断不存在
来源：http://es.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ix.jctech888.com.cn

[Q47] 与平均值比较
来源：http://tt.szxytkj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jq.yuexingan06.cn

[Q48] CTE 公用表表达式
来源：http://lc.panjiajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fr.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://bf.haigaiapp.cn

[Q49] 更新单行
来源：http://sp.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bs.asd995.cn

[Q50] 批量更新
来源：http://ni.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rv.gzmigu.cn

[Q51] 用子查询更新
来源：http://ra.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xw.huixinmuqiang.cn

[Q52] 删除指定行
来源：http://jd.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://uq.shxzskj.cn

[Q53] 按条件删除
来源：http://yz.shtwfgs.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oe.hnjuh.cn

[Q54] 清空表
来源：http://sz.lnxyls.cn

TRUNCATE TABLE logs;
来源：http://js.gzmigu.cn

[Q55] 排名（并列占位）
来源：http://qu.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lu.newstarts.cn

[Q56] 密集排名（并列不占位）
来源：http://vt.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uw.shxzukj.cn

[Q57] 行号
来源：http://ix.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bn.yuexingan06.cn

[Q58] 累计求和
来源：http://do.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sr.huixinmuqiang.cn

[Q59] 分组内累计
来源：http://yh.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xv.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://ez.bookmarksfly.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ho.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ol.huanxung.cn

[Q61] 移动平均
来源：http://sh.gzmigu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vo.szsharing.cn

[Q62] 分组占比
来源：http://gs.yuntaijiaju.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://df.szsharing.cn

[Q63] 开启事务
来源：http://eo.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ew.shtwfgs.cn

[Q64] 提交事务
来源：http://mp.jctech888.com.cn

COMMIT;
来源：http://ki.jctech888.com.cn

[Q65] 回滚事务
来源：http://yd.shxzskj.cn

ROLLBACK;
来源：http://bc.521024.cn

[Q66] 行锁查询
来源：http://yb.9csxet.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rh.huixiangedu.cn

[Q67] 设置隔离级别
来源：http://re.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bk.yuntaijiaju.cn

[Q68] 保存点
来源：http://kl.shxzukj.cn

SAVEPOINT sp1;
来源：http://rk.hnjuh.cn

ROLLBACK TO sp1;
来源：http://rr.521024.cn

[Q69] 查看执行计划
来源：http://tr.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pz.9csxet.cn

[Q70] 更新统计信息
来源：http://io.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://lp.yuexingan06.cn

[Q71] 查看建表语句
来源：http://gx.yuntaijiaju.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yh.huixinmuqiang.cn

[Q72] 查看索引
来源：http://dg.szsharing.cn

SHOW INDEX FROM users;
来源：http://tf.hnjuh.cn

[Q73] 查看表状态
来源：http://tn.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wx.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://nw.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ud.asd995.cn

[Q75] 日期格式化
来源：http://as.muxihuayi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://so.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pn.bjjhwx.cn

[Q76] 按天统计
来源：http://ur.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ki.huanxung.cn

[Q77] 时间加减
来源：http://fc.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fh.shtwfgs.cn

[Q78] 当前时间
来源：http://ev.haigaiapp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iu.newstarts.cn

[Q79] 字符串拼接
来源：http://ls.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://us.yuexingan06.cn

[Q80] 字符串截取
来源：http://cb.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ol.haigaiapp.cn

[Q81] 字符串替换
来源：http://rn.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tq.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://oe.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ww.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://so.asd995.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zg.asd995.cn

[Q84] 去除首尾空格
来源：http://yv.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://br.szsharing.cn

[Q85] 数值取整
来源：http://cm.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tp.yuexingan06.cn

[Q86] 读取 JSON 字段
来源：http://gv.nicolike.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dd.9csxet.cn

[Q87] JSON 字段做条件
来源：http://il.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ib.szsharing.cn

[Q88] 行转列（条件聚合）
来源：http://or.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gn.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ma.bjjhwx.cn

[Q89] 判断表是否存在
来源：http://in.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zk.9csxet.cn

[Q90] 生成序号列
来源：http://kw.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cb.newstarts.cn

================================================================================
来源：http://uo.huixiangedu.cn

R. Bash 专题
来源：http://wp.huanxung.cn

================================================================================
来源：http://fa.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://kf.szxytkj.cn

#!/usr/bin/env bash
来源：http://yj.panjiajie.cn

set -euo pipefail
来源：http://vb.szxytkj.cn

[R02] 变量赋值与使用
来源：http://el.newstarts.cn

name="Tom"; echo "$name"
来源：http://px.muxihuayi.cn

[R03] 只读变量
来源：http://pm.shtwfgs.cn

readonly PI=3.14
来源：http://ge.shtwfgs.cn

[R04] 位置参数
来源：http://lw.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wm.bjjhwx.cn

[R05] 参数默认值
来源：http://wr.szxytkj.cn

name="${1:-default}"
来源：http://bi.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://tt.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gy.haigaiapp.cn

[R07] if 判断文件
来源：http://ba.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xd.huixinmuqiang.cn

[R08] 数值比较
来源：http://eh.gzmigu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bt.wgjwhj.cn

[R09] 字符串比较
来源：http://mg.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wj.panjiajie.cn

[R10] 正则匹配
来源：http://tw.yuexingan06.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mv.bjjhwx.cn

[R11] case 多分支
来源：http://fd.bjjhwx.cn

case "$1" in
来源：http://ei.huixiangedu.cn

start) echo "启动" ;;
来源：http://yn.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://wn.newstarts.cn

*)     echo "未知命令" ;;
来源：http://fu.huixiangedu.cn

esac
来源：http://ka.yuexingan06.cn

[R12] for 遍历文件
来源：http://kc.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://es.yuntaijiaju.cn

[R13] for 计数循环
来源：http://ng.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://qu.colortex.cn

[R14] C 风格 for
来源：http://sk.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hk.jianghongdianzi.cn

[R15] while 逐行读文件
来源：http://hx.shtwfgs.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hs.muxihuayi.cn

[R16] until 等待条件
来源：http://kf.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gp.szsharing.cn

[R17] 数组定义与取值
来源：http://sg.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ou.9csxet.cn

[R18] 遍历数组
来源：http://im.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kd.muxihuayi.cn

[R19] 数组长度
来源：http://fs.hnjuh.cn

echo "${#arr[@]}"
来源：http://aa.huanxung.cn

[R20] 关联数组（字典）
来源：http://rb.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://es.shxzskj.cn

[R21] 字符串长度
来源：http://fr.yuntaijiaju.cn

echo "${#s}"
来源：http://wn.szsharing.cn

[R22] 截取子串
来源：http://gm.newstarts.cn

echo "${s:0:5}"
来源：http://mr.jctech888.com.cn

[R23] 字符串替换
来源：http://zz.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gl.chemitech.net.cn

[R24] 大小写转换
来源：http://oc.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hf.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://ya.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lh.gzmigu.cn

[R26] 命令替换
来源：http://wq.szxytkj.cn

now=$(date +%F); echo "$now"
来源：http://dm.muxihuayi.cn

[R27] 算术展开
来源：http://mn.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://ou.chemitech.net.cn

[R28] 浮点运算
来源：http://nf.asd995.cn

echo "scale=2; 10/3" | bc
来源：http://pf.huanxung.cn

[R29] 定义函数
来源：http://un.bjjhwx.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tu.shxzukj.cn

[R30] 函数返回状态码
来源：http://rh.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://ax.shxzskj.cn

[R31] 局部变量
来源：http://nf.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://ev.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://nj.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zh.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://gq.gzmigu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ca.yuntaijiaju.cn

[R34] 退出时清理
来源：http://uw.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sf.wgjwhj.cn

[R35] 后台执行并等待
来源：http://od.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dh.521024.cn

[R36] 并发执行多个任务
来源：http://fd.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ge.nicolike.cn

[R37] 把输出赋给变量
来源：http://hy.newstarts.cn

files=$(ls -1)
来源：http://oy.szxytkj.cn

[R38] 管道串联
来源：http://pa.szxytkj.cn

cat a.txt | grep -i error | wc -l
来源：http://rw.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://um.szsharing.cn

cmd > out.log 2>&1
来源：http://yi.gzmigu.cn

[R40] 追加写日志
来源：http://jg.hnjuh.cn

echo "log" >> out.log
来源：http://fi.hahajie.cn

[R41] 丢弃输出
来源：http://xc.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://fd.hnjuh.cn

[R42] 输入重定向
来源：http://xq.nszjky.cn

wc -l < a.txt
来源：http://lf.yuntaijiaju.cn

[R43] 按名字查找文件
来源：http://uu.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://uh.jctech888.com.cn

[R44] 按修改时间查找
来源：http://ok.huixinmuqiang.cn

find . -mtime -7 -type f
来源：http://vy.jianghongdianzi.cn

[R45] 批量删除
来源：http://oz.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://vz.hahajie.cn

[R46] 递归替换文件内容
来源：http://zg.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dm.huixiangedu.cn

[R47] sed 单行替换
来源：http://gl.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://je.shtwfgs.cn

[R48] awk 取指定列
来源：http://wv.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://ym.521024.cn

[R49] awk 带条件
来源：http://yj.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ba.haigaiapp.cn

[R50] awk 求和
来源：http://mo.bookmarksfly.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dz.wgjwhj.cn

[R51] 排序去重取前几
来源：http://aw.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://em.shtwfgs.cn

[R52] 统计行数
来源：http://xs.asd995.cn

wc -l a.txt
来源：http://gi.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://uk.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fu.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://rl.bookmarksfly.cn

diff a.txt b.txt
来源：http://mr.huixiangedu.cn

[R55] 压缩与解压
来源：http://ra.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ua.panjiajie.cn

[R56] 远程拷贝
来源：http://it.hnjuh.cn

scp file user@host:/path/
来源：http://ij.wgjwhj.cn

[R57] 远程执行命令
来源：http://xr.szsharing.cn

ssh user@host 'uptime'
来源：http://mr.hahajie.cn

[R58] 下载文件
来源：http://tr.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kr.521024.cn

[R59] 发 POST JSON
来源：http://mf.jianghongdianzi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kl.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://nn.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ed.nicolike.cn

[R61] 磁盘占用
来源：http://ce.muxihuayi.cn

df -h;  du -sh *
来源：http://uq.muxihuayi.cn

[R62] 找最占空间的文件
来源：http://jg.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://cq.521024.cn

[R63] 内存与进程
来源：http://tp.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://ej.szxytkj.cn

[R64] 结束进程
来源：http://jc.haigaiapp.cn

kill -9 $(pgrep -f app.py)
来源：http://mw.nszjky.cn

[R65] 查看端口占用
来源：http://bh.shtwfgs.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xi.szxytkj.cn

[R66] 定时任务
来源：http://do.hahajie.cn

crontab -e;  crontab -l
来源：http://ch.nicolike.cn

[R67] 生成随机十六进制串
来源：http://tv.nicolike.cn

openssl rand -hex 16
来源：http://ku.jctech888.com.cn

[R68] 计算文件校验值
来源：http://hk.lnxyls.cn

sha256sum a.txt;  md5sum a.txt
来源：http://aw.szsharing.cn

[R69] 生成随机密码
来源：http://kq.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://rj.huixiangedu.cn

[R70] 时间戳与互转
来源：http://rs.9csxet.cn

date +%s;  date -d @1700000000
来源：http://ey.szxytkj.cn

[R71] 日期格式化
来源：http://ux.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xk.wgjwhj.cn

[R72] 等待端口就绪
来源：http://br.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nu.shtwfgs.cn

[R73] 分割大日志
来源：http://iy.hnjuh.cn

split -l 1000 big.log part_
来源：http://jj.newstarts.cn

[R74] 批量重命名
来源：http://sh.jctech888.com.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qd.huixinmuqiang.cn

[R75] 导出环境变量
来源：http://pl.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://xz.chemitech.net.cn

[R76] 使用临时文件
来源：http://vf.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://am.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://bs.chemitech.net.cn

read -rp "请输入: " ans
来源：http://wo.bjjhwx.cn

[R78] 交互式菜单
来源：http://nm.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://eu.gzmigu.cn

[R79] 解析命令行选项
来源：http://up.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tb.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://rk.lnxyls.cn

time ./run.sh
来源：http://at.haigaiapp.cn

================================================================================
来源：http://ga.muxihuayi.cn

S. C / C++ 专题
来源：http://yg.wgjwhj.cn

================================================================================
来源：http://kv.szsharing.cn

[S01] C：Hello World
来源：http://mn.shxzukj.cn

#include <stdio.h>
来源：http://jo.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rv.huanxung.cn

[S02] C：变量与格式化输出
来源：http://cu.shxzukj.cn

int a = 10; printf("%d\n", a);
来源：http://mp.huanxung.cn

[S03] C：读入整数
来源：http://ly.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://ud.asd995.cn

[S04] C：字符串复制
来源：http://cp.panjiajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qu.gzmigu.cn

[S05] C：字符串长度
来源：http://md.huixiangedu.cn

strlen(s)
来源：http://ya.nicolike.cn

[S06] C：字符串比较
来源：http://hv.nicolike.cn

strcmp(a, b) == 0
来源：http://ow.huixiangedu.cn

[S07] C：数组遍历求和
来源：http://tk.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ik.colortex.cn

[S08] C：动态内存分配与释放
来源：http://ls.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ip.521024.cn

[S09] C：结构体定义与初始化
来源：http://yi.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://br.newstarts.cn

[S10] C：指针与解引用
来源：http://dm.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://wh.yuexingan06.cn

[S11] C：逐行读文件
来源：http://io.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://xw.nicolike.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bm.huixinmuqiang.cn

fclose(f);
来源：http://ct.huixinmuqiang.cn

[S12] C：写文件
来源：http://pr.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nq.muxihuayi.cn

[S13] C：宏定义
来源：http://nn.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mq.yuntaijiaju.cn

[S14] C：枚举
来源：http://wb.nicolike.cn


<!-- 参考信息 -->