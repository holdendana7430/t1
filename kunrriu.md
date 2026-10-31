代发 wailian999

[Q44] IN 子查询
来源：http://jh.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zk.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://bk.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ui.asd995.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vd.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nl.nszjky.cn

[Q47] 与平均值比较
来源：http://en.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xl.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://td.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fw.panjiajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://hf.szsharing.cn

[Q49] 更新单行
来源：http://vf.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://li.chemitech.net.cn

[Q50] 批量更新
来源：http://wm.panjiajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://el.nicolike.cn

[Q51] 用子查询更新
来源：http://tu.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ww.szsharing.cn

[Q52] 删除指定行
来源：http://sz.muxihuayi.cn

DELETE FROM users WHERE id = 10;
来源：http://jw.nicolike.cn

[Q53] 按条件删除
来源：http://ne.nicolike.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ev.shxzskj.cn

[Q54] 清空表
来源：http://lt.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://xd.521024.cn

[Q55] 排名（并列占位）
来源：http://ne.hnjuh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wk.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://ce.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dn.jctech888.com.cn

[Q57] 行号
来源：http://iu.bjjhwx.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pq.panjiajie.cn

[Q58] 累计求和
来源：http://kz.lnxyls.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tb.muxihuayi.cn

[Q59] 分组内累计
来源：http://kg.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gj.jctech888.com.cn

[Q60] 取上一行 / 下一行
来源：http://dc.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vh.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mn.chemitech.net.cn

[Q61] 移动平均
来源：http://tx.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gw.huanxung.cn

[Q62] 分组占比
来源：http://on.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ue.9csxet.cn

[Q63] 开启事务
来源：http://zm.hnjuh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ix.yuexingan06.cn

[Q64] 提交事务
来源：http://kq.bookmarksfly.cn

COMMIT;
来源：http://br.panjiajie.cn

[Q65] 回滚事务
来源：http://eo.nicolike.cn

ROLLBACK;
来源：http://co.nszjky.cn

[Q66] 行锁查询
来源：http://ie.huanxung.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://up.shxzukj.cn

[Q67] 设置隔离级别
来源：http://kb.haigaiapp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ca.shtwfgs.cn

[Q68] 保存点
来源：http://sk.shxzukj.cn

SAVEPOINT sp1;
来源：http://rz.colortex.cn

ROLLBACK TO sp1;
来源：http://az.asd995.cn

[Q69] 查看执行计划
来源：http://kh.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pp.hahajie.cn

[Q70] 更新统计信息
来源：http://hg.szxytkj.cn

ANALYZE TABLE users;
来源：http://df.shxzskj.cn

[Q71] 查看建表语句
来源：http://rz.yuntaijiaju.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fl.colortex.cn

[Q72] 查看索引
来源：http://ym.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://fp.nszjky.cn

[Q73] 查看表状态
来源：http://gs.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fd.shxzskj.cn

[Q74] 强制使用索引
来源：http://ra.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mr.lnxyls.cn

[Q75] 日期格式化
来源：http://kl.chemitech.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hs.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gc.hahajie.cn

[Q76] 按天统计
来源：http://mt.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nu.colortex.cn

[Q77] 时间加减
来源：http://bn.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rz.colortex.cn

[Q78] 当前时间
来源：http://dp.haigaiapp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oj.shtwfgs.cn

[Q79] 字符串拼接
来源：http://mv.colortex.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hc.hahajie.cn

[Q80] 字符串截取
来源：http://bo.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lr.muxihuayi.cn

[Q81] 字符串替换
来源：http://gq.nszjky.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iz.colortex.cn

[Q82] 字符长度与字节长度
来源：http://fl.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gv.wgjwhj.cn

[Q83] 大小写转换
来源：http://bq.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ow.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://sd.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://qv.huixinmuqiang.cn

[Q85] 数值取整
来源：http://lf.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://it.szxytkj.cn

[Q86] 读取 JSON 字段
来源：http://ug.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dy.9csxet.cn

[Q87] JSON 字段做条件
来源：http://sy.huixiangedu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ci.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://ff.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oi.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hp.newstarts.cn

[Q89] 判断表是否存在
来源：http://rx.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cq.9csxet.cn

[Q90] 生成序号列
来源：http://xn.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lo.colortex.cn

================================================================================
来源：http://zt.gzmigu.cn

R. Bash 专题
来源：http://dn.yuntaijiaju.cn

================================================================================
来源：http://xg.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://ap.wgjwhj.cn

#!/usr/bin/env bash
来源：http://sv.szsharing.cn

set -euo pipefail
来源：http://uc.bookmarksfly.cn

[R02] 变量赋值与使用
来源：http://ig.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://ey.asd995.cn

[R03] 只读变量
来源：http://my.colortex.cn

readonly PI=3.14
来源：http://gv.shtwfgs.cn

[R04] 位置参数
来源：http://cb.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ju.gzmigu.cn

[R05] 参数默认值
来源：http://vg.panjiajie.cn

name="${1:-default}"
来源：http://en.colortex.cn

[R06] 判断命令是否存在
来源：http://en.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xd.szxytkj.cn

[R07] if 判断文件
来源：http://wa.nszjky.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yo.bookmarksfly.cn

[R08] 数值比较
来源：http://nq.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mv.colortex.cn

[R09] 字符串比较
来源：http://hi.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://et.jianghongdianzi.cn

[R10] 正则匹配
来源：http://pa.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bp.colortex.cn

[R11] case 多分支
来源：http://xh.huanxung.cn

case "$1" in
来源：http://vo.panjiajie.cn

start) echo "启动" ;;
来源：http://rm.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://vt.hnjuh.cn

*)     echo "未知命令" ;;
来源：http://or.yuntaijiaju.cn

esac
来源：http://vr.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://nv.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://aw.haigaiapp.cn

[R13] for 计数循环
来源：http://ax.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://gb.asd995.cn

[R14] C 风格 for
来源：http://bp.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vr.chemitech.net.cn

[R15] while 逐行读文件
来源：http://sp.shtwfgs.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dg.hahajie.cn

[R16] until 等待条件
来源：http://mj.haigaiapp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hm.lnxyls.cn

[R17] 数组定义与取值
来源：http://jy.jianghongdianzi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fr.jianghongdianzi.cn

[R18] 遍历数组
来源：http://rh.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sy.nszjky.cn

[R19] 数组长度
来源：http://oo.nszjky.cn

echo "${#arr[@]}"
来源：http://nl.bookmarksfly.cn

[R20] 关联数组（字典）
来源：http://rb.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ic.huixiangedu.cn

[R21] 字符串长度
来源：http://ng.shxzskj.cn

echo "${#s}"
来源：http://je.jctech888.com.cn

[R22] 截取子串
来源：http://pn.shxzskj.cn

echo "${s:0:5}"
来源：http://bb.newstarts.cn

[R23] 字符串替换
来源：http://qu.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dx.huixiangedu.cn

[R24] 大小写转换
来源：http://kl.521024.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yi.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://ye.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rc.gzmigu.cn

[R26] 命令替换
来源：http://ks.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://bh.szsharing.cn

[R27] 算术展开
来源：http://hc.szsharing.cn

echo $((1 + 2 * 3))
来源：http://ju.nicolike.cn

[R28] 浮点运算
来源：http://lc.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://zh.newstarts.cn

[R29] 定义函数
来源：http://mc.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ft.gzmigu.cn

[R30] 函数返回状态码
来源：http://uy.shxzskj.cn

f() { return 0; }; f || echo "失败了"
来源：http://xg.jianghongdianzi.cn

[R31] 局部变量
来源：http://ll.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://fp.haigaiapp.cn

[R32] 参数个数校验
来源：http://cb.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ql.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://wb.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mq.jctech888.com.cn

[R34] 退出时清理
来源：http://sj.9csxet.cn

trap 'rm -f "$tmp"' EXIT
来源：http://df.szsharing.cn

[R35] 后台执行并等待
来源：http://xn.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://je.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://ir.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ji.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://ni.szxytkj.cn

files=$(ls -1)
来源：http://wg.szxytkj.cn

[R38] 管道串联
来源：http://uo.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://rx.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://dh.muxihuayi.cn

cmd > out.log 2>&1
来源：http://qr.hahajie.cn

[R40] 追加写日志
来源：http://uc.gzmigu.cn

echo "log" >> out.log
来源：http://ok.colortex.cn

[R41] 丢弃输出
来源：http://re.shtwfgs.cn

cmd >/dev/null 2>&1
来源：http://wi.nicolike.cn

[R42] 输入重定向
来源：http://wf.9csxet.cn

wc -l < a.txt
来源：http://jt.lnxyls.cn

[R43] 按名字查找文件
来源：http://qn.huixiangedu.cn

find . -name "*.log" -type f
来源：http://vx.hahajie.cn

[R44] 按修改时间查找
来源：http://vi.shxzskj.cn

find . -mtime -7 -type f
来源：http://nj.hnjuh.cn

[R45] 批量删除
来源：http://dw.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://iw.huanxung.cn

[R46] 递归替换文件内容
来源：http://il.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fr.shtwfgs.cn

[R47] sed 单行替换
来源：http://wv.shxzukj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nl.nicolike.cn

[R48] awk 取指定列
来源：http://kz.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://as.jctech888.com.cn

[R49] awk 带条件
来源：http://yi.chemitech.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dg.nicolike.cn

[R50] awk 求和
来源：http://it.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mr.bjjhwx.cn

[R51] 排序去重取前几
来源：http://tt.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nv.bjjhwx.cn

[R52] 统计行数
来源：http://cu.9csxet.cn

wc -l a.txt
来源：http://gn.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://go.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sk.hahajie.cn

[R54] 比较两个文件
来源：http://dm.hnjuh.cn

diff a.txt b.txt
来源：http://xl.521024.cn

[R55] 压缩与解压
来源：http://vp.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pu.shxzskj.cn

[R56] 远程拷贝
来源：http://lf.hahajie.cn

scp file user@host:/path/
来源：http://yq.gzmigu.cn

[R57] 远程执行命令
来源：http://tx.wgjwhj.cn

ssh user@host 'uptime'
来源：http://io.haigaiapp.cn

[R58] 下载文件
来源：http://px.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rj.yuexingan06.cn

[R59] 发 POST JSON
来源：http://vn.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yp.yuexingan06.cn

[R60] 只看 HTTP 状态码
来源：http://hp.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yb.yuexingan06.cn

[R61] 磁盘占用
来源：http://mw.huixiangedu.cn

df -h;  du -sh *
来源：http://zx.szsharing.cn

[R62] 找最占空间的文件
来源：http://kk.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://qa.huanxung.cn

[R63] 内存与进程
来源：http://te.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://wa.haigaiapp.cn

[R64] 结束进程
来源：http://ue.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://an.hnjuh.cn

[R65] 查看端口占用
来源：http://kf.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cm.hahajie.cn

[R66] 定时任务
来源：http://qu.yuexingan06.cn

crontab -e;  crontab -l
来源：http://yu.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://bs.nszjky.cn

openssl rand -hex 16
来源：http://xy.shxzskj.cn

[R68] 计算文件校验值
来源：http://bd.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dn.colortex.cn

[R69] 生成随机密码
来源：http://ty.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://bm.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://xr.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://cw.muxihuayi.cn

[R71] 日期格式化
来源：http://wx.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ce.haigaiapp.cn

[R72] 等待端口就绪
来源：http://ea.yuexingan06.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zf.huanxung.cn

[R73] 分割大日志
来源：http://mk.521024.cn

split -l 1000 big.log part_
来源：http://rp.szxytkj.cn

[R74] 批量重命名
来源：http://yh.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qh.lnxyls.cn

[R75] 导出环境变量
来源：http://hb.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://nv.szxytkj.cn

[R76] 使用临时文件
来源：http://bx.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qk.gzmigu.cn

[R77] 读取用户输入
来源：http://fy.haigaiapp.cn

read -rp "请输入: " ans
来源：http://qc.haigaiapp.cn

[R78] 交互式菜单
来源：http://tc.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pt.lnxyls.cn

[R79] 解析命令行选项
来源：http://jf.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zu.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://ta.gzmigu.cn

time ./run.sh
来源：http://rx.nszjky.cn

================================================================================
来源：http://qt.jianghongdianzi.cn

S. C / C++ 专题
来源：http://av.szxytkj.cn

================================================================================
来源：http://hb.huanxung.cn

[S01] C：Hello World
来源：http://nf.chemitech.net.cn

#include <stdio.h>
来源：http://wa.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xb.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://ip.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://gs.asd995.cn

[S03] C：读入整数
来源：http://kq.hnjuh.cn

int x; scanf("%d", &x);
来源：http://ko.nicolike.cn

[S04] C：字符串复制
来源：http://ze.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uz.gzmigu.cn

[S05] C：字符串长度
来源：http://ke.nicolike.cn

strlen(s)
来源：http://ch.muxihuayi.cn

[S06] C：字符串比较
来源：http://ou.muxihuayi.cn

strcmp(a, b) == 0
来源：http://qr.szsharing.cn

[S07] C：数组遍历求和
来源：http://kr.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zs.colortex.cn

[S08] C：动态内存分配与释放
来源：http://zp.jctech888.com.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ag.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://dg.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ng.wgjwhj.cn

[S10] C：指针与解引用
来源：http://xj.nicolike.cn

int *p = &a;  *p = 5;
来源：http://eg.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://ia.lnxyls.cn

FILE *f = fopen("a.txt", "r");
来源：http://fs.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ms.nszjky.cn

fclose(f);
来源：http://pq.asd995.cn

[S12] C：写文件
来源：http://kt.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yx.nicolike.cn

[S13] C：宏定义
来源：http://tn.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://iu.szxytkj.cn

[S14] C：枚举
来源：http://un.hnjuh.cn


<!-- 参考信息 -->