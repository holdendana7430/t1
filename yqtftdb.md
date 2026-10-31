代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://bm.muxihuayi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qb.nicolike.cn

[Q47] 与平均值比较
来源：http://rc.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mh.szxytkj.cn

[Q48] CTE 公用表表达式
来源：http://je.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qs.chemitech.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://cz.huixiangedu.cn

[Q49] 更新单行
来源：http://ii.yuexingan06.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ha.newstarts.cn

[Q50] 批量更新
来源：http://oq.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xr.hahajie.cn

[Q51] 用子查询更新
来源：http://od.9csxet.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://os.szsharing.cn

[Q52] 删除指定行
来源：http://ls.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://xm.shxzukj.cn

[Q53] 按条件删除
来源：http://hh.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://au.521024.cn

[Q54] 清空表
来源：http://kr.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://gt.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://if.huanxung.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ec.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://bl.wgjwhj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ov.newstarts.cn

[Q57] 行号
来源：http://hs.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://el.bookmarksfly.cn

[Q58] 累计求和
来源：http://yc.gzmigu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vo.huanxung.cn

[Q59] 分组内累计
来源：http://oa.chemitech.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zq.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://jk.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://da.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vm.asd995.cn

[Q61] 移动平均
来源：http://oe.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jo.hnjuh.cn

[Q62] 分组占比
来源：http://wm.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bl.huixiangedu.cn

[Q63] 开启事务
来源：http://zu.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yw.shxzskj.cn

[Q64] 提交事务
来源：http://dp.panjiajie.cn

COMMIT;
来源：http://do.szxytkj.cn

[Q65] 回滚事务
来源：http://lr.jianghongdianzi.cn

ROLLBACK;
来源：http://ef.muxihuayi.cn

[Q66] 行锁查询
来源：http://ek.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://un.muxihuayi.cn

[Q67] 设置隔离级别
来源：http://bm.huixinmuqiang.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bz.nicolike.cn

[Q68] 保存点
来源：http://wv.hahajie.cn

SAVEPOINT sp1;
来源：http://wl.yuntaijiaju.cn

ROLLBACK TO sp1;
来源：http://tk.hahajie.cn

[Q69] 查看执行计划
来源：http://ye.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ao.muxihuayi.cn

[Q70] 更新统计信息
来源：http://nh.gzmigu.cn

ANALYZE TABLE users;
来源：http://rm.hnjuh.cn

[Q71] 查看建表语句
来源：http://fl.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ag.muxihuayi.cn

[Q72] 查看索引
来源：http://jh.colortex.cn

SHOW INDEX FROM users;
来源：http://eg.newstarts.cn

[Q73] 查看表状态
来源：http://wq.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ex.lnxyls.cn

[Q74] 强制使用索引
来源：http://nw.hnjuh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pf.nszjky.cn

[Q75] 日期格式化
来源：http://bj.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ft.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cm.jianghongdianzi.cn

[Q76] 按天统计
来源：http://mq.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tz.huixinmuqiang.cn

[Q77] 时间加减
来源：http://lz.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oo.szsharing.cn

[Q78] 当前时间
来源：http://xn.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nb.yuntaijiaju.cn

[Q79] 字符串拼接
来源：http://sr.jctech888.com.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vw.haigaiapp.cn

[Q80] 字符串截取
来源：http://na.asd995.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wj.szsharing.cn

[Q81] 字符串替换
来源：http://wy.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nj.chemitech.net.cn

[Q82] 字符长度与字节长度
来源：http://bk.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qf.hahajie.cn

[Q83] 大小写转换
来源：http://ff.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eo.huixinmuqiang.cn

[Q84] 去除首尾空格
来源：http://vu.colortex.cn

SELECT TRIM(name) FROM users;
来源：http://xq.muxihuayi.cn

[Q85] 数值取整
来源：http://cn.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ll.nszjky.cn

[Q86] 读取 JSON 字段
来源：http://oa.bookmarksfly.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ut.bookmarksfly.cn

[Q87] JSON 字段做条件
来源：http://cb.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hi.jianghongdianzi.cn

[Q88] 行转列（条件聚合）
来源：http://yx.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ak.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ku.nszjky.cn

[Q89] 判断表是否存在
来源：http://qo.szsharing.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rc.9csxet.cn

[Q90] 生成序号列
来源：http://qf.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gy.521024.cn

================================================================================
来源：http://om.nicolike.cn

R. Bash 专题
来源：http://ti.szxytkj.cn

================================================================================
来源：http://fk.521024.cn

[R01] shebang 与严格模式
来源：http://mc.szsharing.cn

#!/usr/bin/env bash
来源：http://cd.chemitech.net.cn

set -euo pipefail
来源：http://on.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://ee.newstarts.cn

name="Tom"; echo "$name"
来源：http://jv.huixiangedu.cn

[R03] 只读变量
来源：http://qm.521024.cn

readonly PI=3.14
来源：http://ml.asd995.cn

[R04] 位置参数
来源：http://pt.shxzukj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vm.wgjwhj.cn

[R05] 参数默认值
来源：http://nh.shxzukj.cn

name="${1:-default}"
来源：http://zp.shxzukj.cn

[R06] 判断命令是否存在
来源：http://sh.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sg.nszjky.cn

[R07] if 判断文件
来源：http://ft.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://id.wgjwhj.cn

[R08] 数值比较
来源：http://ur.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sn.yuexingan06.cn

[R09] 字符串比较
来源：http://uc.shxzskj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dp.nicolike.cn

[R10] 正则匹配
来源：http://dl.muxihuayi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://om.huixinmuqiang.cn

[R11] case 多分支
来源：http://uo.shtwfgs.cn

case "$1" in
来源：http://tv.gzmigu.cn

start) echo "启动" ;;
来源：http://xf.szxytkj.cn

stop)  echo "停止" ;;
来源：http://uo.shtwfgs.cn

*)     echo "未知命令" ;;
来源：http://ey.panjiajie.cn

esac
来源：http://mc.shtwfgs.cn

[R12] for 遍历文件
来源：http://id.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://bu.jianghongdianzi.cn

[R13] for 计数循环
来源：http://tj.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://og.nszjky.cn

[R14] C 风格 for
来源：http://ab.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://js.chemitech.net.cn

[R15] while 逐行读文件
来源：http://wr.haigaiapp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tg.wgjwhj.cn

[R16] until 等待条件
来源：http://cm.bjjhwx.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://os.muxihuayi.cn

[R17] 数组定义与取值
来源：http://nv.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ex.yuexingan06.cn

[R18] 遍历数组
来源：http://vk.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ir.chemitech.net.cn

[R19] 数组长度
来源：http://vb.521024.cn

echo "${#arr[@]}"
来源：http://ln.9csxet.cn

[R20] 关联数组（字典）
来源：http://vo.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://to.hahajie.cn

[R21] 字符串长度
来源：http://hs.muxihuayi.cn

echo "${#s}"
来源：http://mp.huixiangedu.cn

[R22] 截取子串
来源：http://ga.nszjky.cn

echo "${s:0:5}"
来源：http://io.huixiangedu.cn

[R23] 字符串替换
来源：http://zk.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ve.muxihuayi.cn

[R24] 大小写转换
来源：http://lx.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ev.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://ga.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tq.jctech888.com.cn

[R26] 命令替换
来源：http://pa.yuntaijiaju.cn

now=$(date +%F); echo "$now"
来源：http://lm.gzmigu.cn

[R27] 算术展开
来源：http://wo.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://qj.gzmigu.cn

[R28] 浮点运算
来源：http://rn.colortex.cn

echo "scale=2; 10/3" | bc
来源：http://xp.szsharing.cn

[R29] 定义函数
来源：http://jf.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ob.huanxung.cn

[R30] 函数返回状态码
来源：http://ol.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://ad.hahajie.cn

[R31] 局部变量
来源：http://dz.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://uw.gzmigu.cn

[R32] 参数个数校验
来源：http://sf.yuexingan06.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mz.521024.cn

[R33] 捕获错误并提示行号
来源：http://db.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dk.huixiangedu.cn

[R34] 退出时清理
来源：http://dm.huixinmuqiang.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vi.huixiangedu.cn

[R35] 后台执行并等待
来源：http://vo.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ui.shxzukj.cn

[R36] 并发执行多个任务
来源：http://es.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yg.nszjky.cn

[R37] 把输出赋给变量
来源：http://bd.newstarts.cn

files=$(ls -1)
来源：http://nf.nszjky.cn

[R38] 管道串联
来源：http://vn.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://qq.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://js.szsharing.cn

cmd > out.log 2>&1
来源：http://ds.jianghongdianzi.cn

[R40] 追加写日志
来源：http://au.shxzukj.cn

echo "log" >> out.log
来源：http://om.huanxung.cn

[R41] 丢弃输出
来源：http://mi.szsharing.cn

cmd >/dev/null 2>&1
来源：http://tz.huixiangedu.cn

[R42] 输入重定向
来源：http://ow.9csxet.cn

wc -l < a.txt
来源：http://pd.yuntaijiaju.cn

[R43] 按名字查找文件
来源：http://ro.shxzskj.cn

find . -name "*.log" -type f
来源：http://xn.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://qq.panjiajie.cn

find . -mtime -7 -type f
来源：http://hj.gzmigu.cn

[R45] 批量删除
来源：http://ct.szsharing.cn

find . -name "*.tmp" -delete
来源：http://dy.hnjuh.cn

[R46] 递归替换文件内容
来源：http://bm.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zc.chemitech.net.cn

[R47] sed 单行替换
来源：http://km.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ly.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://ul.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://to.szxytkj.cn

[R49] awk 带条件
来源：http://wx.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zl.huixiangedu.cn

[R50] awk 求和
来源：http://sb.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dt.shxzskj.cn

[R51] 排序去重取前几
来源：http://mh.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ur.haigaiapp.cn

[R52] 统计行数
来源：http://qf.huanxung.cn

wc -l a.txt
来源：http://mn.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://ez.gzmigu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sw.jctech888.com.cn

[R54] 比较两个文件
来源：http://ad.bookmarksfly.cn

diff a.txt b.txt
来源：http://lw.9csxet.cn

[R55] 压缩与解压
来源：http://kj.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fj.huanxung.cn

[R56] 远程拷贝
来源：http://mh.szxytkj.cn

scp file user@host:/path/
来源：http://up.shxzskj.cn

[R57] 远程执行命令
来源：http://kg.chemitech.net.cn

ssh user@host 'uptime'
来源：http://pq.asd995.cn

[R58] 下载文件
来源：http://xj.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oc.chemitech.net.cn

[R59] 发 POST JSON
来源：http://to.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qo.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://xj.yuexingan06.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hg.szsharing.cn

[R61] 磁盘占用
来源：http://tt.huixinmuqiang.cn

df -h;  du -sh *
来源：http://vt.muxihuayi.cn

[R62] 找最占空间的文件
来源：http://zl.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://ay.hahajie.cn

[R63] 内存与进程
来源：http://qd.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://fr.muxihuayi.cn

[R64] 结束进程
来源：http://wc.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://oj.shxzskj.cn

[R65] 查看端口占用
来源：http://uu.szxytkj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://es.colortex.cn

[R66] 定时任务
来源：http://xi.huixiangedu.cn

crontab -e;  crontab -l
来源：http://fs.9csxet.cn

[R67] 生成随机十六进制串
来源：http://iq.lnxyls.cn

openssl rand -hex 16
来源：http://qr.haigaiapp.cn

[R68] 计算文件校验值
来源：http://oo.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://au.muxihuayi.cn

[R69] 生成随机密码
来源：http://bo.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://ko.521024.cn

[R70] 时间戳与互转
来源：http://jq.nszjky.cn

date +%s;  date -d @1700000000
来源：http://ds.shtwfgs.cn

[R71] 日期格式化
来源：http://jq.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zj.huanxung.cn

[R72] 等待端口就绪
来源：http://kt.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kh.asd995.cn

[R73] 分割大日志
来源：http://hl.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://hu.haigaiapp.cn

[R74] 批量重命名
来源：http://qi.nszjky.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fz.haigaiapp.cn

[R75] 导出环境变量
来源：http://jf.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://si.lnxyls.cn

[R76] 使用临时文件
来源：http://mc.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zq.haigaiapp.cn

[R77] 读取用户输入
来源：http://pg.bjjhwx.cn

read -rp "请输入: " ans
来源：http://lm.szxytkj.cn

[R78] 交互式菜单
来源：http://lo.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bc.lnxyls.cn

[R79] 解析命令行选项
来源：http://ap.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dj.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://lu.jctech888.com.cn

time ./run.sh
来源：http://hw.lnxyls.cn

================================================================================
来源：http://ow.9csxet.cn

S. C / C++ 专题
来源：http://zf.lnxyls.cn

================================================================================
来源：http://hi.colortex.cn

[S01] C：Hello World
来源：http://oo.bookmarksfly.cn

#include <stdio.h>
来源：http://yb.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ja.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://yi.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://bs.jianghongdianzi.cn

[S03] C：读入整数
来源：http://bb.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://qe.colortex.cn

[S04] C：字符串复制
来源：http://wk.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wh.panjiajie.cn

[S05] C：字符串长度
来源：http://ps.yuexingan06.cn

strlen(s)
来源：http://qj.shxzskj.cn

[S06] C：字符串比较
来源：http://hz.huanxung.cn

strcmp(a, b) == 0
来源：http://mf.asd995.cn

[S07] C：数组遍历求和
来源：http://bh.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zt.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://qh.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ng.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://xh.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tp.szxytkj.cn

[S10] C：指针与解引用
来源：http://bu.colortex.cn

int *p = &a;  *p = 5;
来源：http://pd.nszjky.cn

[S11] C：逐行读文件
来源：http://hr.lnxyls.cn

FILE *f = fopen("a.txt", "r");
来源：http://ny.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hi.nszjky.cn

fclose(f);
来源：http://nl.nszjky.cn

[S12] C：写文件
来源：http://ir.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rl.nszjky.cn

[S13] C：宏定义
来源：http://ok.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ot.wgjwhj.cn

[S14] C：枚举
来源：http://mz.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://ym.chemitech.net.cn

[S15] C：类型转换
来源：http://ra.shxzukj.cn

(double) a / b
来源：http://jp.muxihuayi.cn

[S16] C：位操作置位
来源：http://nd.shxzukj.cn


<!-- 参考信息 -->