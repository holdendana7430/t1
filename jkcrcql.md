代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://or.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tj.9csxet.cn

[Q47] 与平均值比较
来源：http://oe.colortex.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fg.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://qd.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ct.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://iu.panjiajie.cn

[Q49] 更新单行
来源：http://ue.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pf.chemitech.net.cn

[Q50] 批量更新
来源：http://zk.shtwfgs.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ul.newstarts.cn

[Q51] 用子查询更新
来源：http://jp.shxzskj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://od.huanxung.cn

[Q52] 删除指定行
来源：http://rw.521024.cn

DELETE FROM users WHERE id = 10;
来源：http://ml.szxytkj.cn

[Q53] 按条件删除
来源：http://fz.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ux.521024.cn

[Q54] 清空表
来源：http://qf.wgjwhj.cn

TRUNCATE TABLE logs;
来源：http://vj.szxytkj.cn

[Q55] 排名（并列占位）
来源：http://gu.jianghongdianzi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rn.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://po.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oy.9csxet.cn

[Q57] 行号
来源：http://hm.asd995.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cz.yuexingan06.cn

[Q58] 累计求和
来源：http://qj.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ua.nicolike.cn

[Q59] 分组内累计
来源：http://yx.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zi.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://ky.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pa.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rd.huixinmuqiang.cn

[Q61] 移动平均
来源：http://oj.lnxyls.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gi.chemitech.net.cn

[Q62] 分组占比
来源：http://io.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tz.wgjwhj.cn

[Q63] 开启事务
来源：http://hs.panjiajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gd.huixiangedu.cn

[Q64] 提交事务
来源：http://sj.521024.cn

COMMIT;
来源：http://xa.shxzskj.cn

[Q65] 回滚事务
来源：http://hs.haigaiapp.cn

ROLLBACK;
来源：http://wa.asd995.cn

[Q66] 行锁查询
来源：http://oi.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kq.newstarts.cn

[Q67] 设置隔离级别
来源：http://np.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qh.shxzskj.cn

[Q68] 保存点
来源：http://ym.muxihuayi.cn

SAVEPOINT sp1;
来源：http://tc.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://xm.szsharing.cn

[Q69] 查看执行计划
来源：http://on.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yh.shxzukj.cn

[Q70] 更新统计信息
来源：http://cu.muxihuayi.cn

ANALYZE TABLE users;
来源：http://su.wgjwhj.cn

[Q71] 查看建表语句
来源：http://jd.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qd.chemitech.net.cn

[Q72] 查看索引
来源：http://ww.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://ei.9csxet.cn

[Q73] 查看表状态
来源：http://oy.chemitech.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hj.jianghongdianzi.cn

[Q74] 强制使用索引
来源：http://sn.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lx.shtwfgs.cn

[Q75] 日期格式化
来源：http://jn.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rj.szxytkj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lt.huanxung.cn

[Q76] 按天统计
来源：http://wn.yuntaijiaju.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fk.nszjky.cn

[Q77] 时间加减
来源：http://ki.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dn.szxytkj.cn

[Q78] 当前时间
来源：http://xb.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xm.haigaiapp.cn

[Q79] 字符串拼接
来源：http://xq.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xj.szxytkj.cn

[Q80] 字符串截取
来源：http://mm.chemitech.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.bookmarksfly.cn

[Q81] 字符串替换
来源：http://wv.nszjky.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pw.muxihuayi.cn

[Q82] 字符长度与字节长度
来源：http://ln.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lw.bookmarksfly.cn

[Q83] 大小写转换
来源：http://ht.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yq.hnjuh.cn

[Q84] 去除首尾空格
来源：http://qk.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://rr.szxytkj.cn

[Q85] 数值取整
来源：http://wr.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dd.nicolike.cn

[Q86] 读取 JSON 字段
来源：http://bt.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jd.yuexingan06.cn

[Q87] JSON 字段做条件
来源：http://kk.huixiangedu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ad.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://bw.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://td.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rs.521024.cn

[Q89] 判断表是否存在
来源：http://yz.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ta.szsharing.cn

[Q90] 生成序号列
来源：http://yw.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tl.wgjwhj.cn

================================================================================
来源：http://jx.szxytkj.cn

R. Bash 专题
来源：http://go.bookmarksfly.cn

================================================================================
来源：http://cn.newstarts.cn

[R01] shebang 与严格模式
来源：http://ue.szxytkj.cn

#!/usr/bin/env bash
来源：http://ez.nszjky.cn

set -euo pipefail
来源：http://qq.bjjhwx.cn

[R02] 变量赋值与使用
来源：http://as.shxzukj.cn

name="Tom"; echo "$name"
来源：http://jk.muxihuayi.cn

[R03] 只读变量
来源：http://ep.nicolike.cn

readonly PI=3.14
来源：http://nd.colortex.cn

[R04] 位置参数
来源：http://ap.521024.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://op.bookmarksfly.cn

[R05] 参数默认值
来源：http://by.hahajie.cn

name="${1:-default}"
来源：http://nw.nicolike.cn

[R06] 判断命令是否存在
来源：http://ay.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jo.newstarts.cn

[R07] if 判断文件
来源：http://hs.jctech888.com.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ur.jctech888.com.cn

[R08] 数值比较
来源：http://qk.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://oe.wgjwhj.cn

[R09] 字符串比较
来源：http://zr.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lt.muxihuayi.cn

[R10] 正则匹配
来源：http://th.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zf.muxihuayi.cn

[R11] case 多分支
来源：http://hm.yuntaijiaju.cn

case "$1" in
来源：http://pd.nszjky.cn

start) echo "启动" ;;
来源：http://ml.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://kp.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://qb.521024.cn

esac
来源：http://dd.gzmigu.cn

[R12] for 遍历文件
来源：http://yf.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://xz.wgjwhj.cn

[R13] for 计数循环
来源：http://or.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://fg.newstarts.cn

[R14] C 风格 for
来源：http://kb.huanxung.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uu.shxzskj.cn

[R15] while 逐行读文件
来源：http://vi.huixiangedu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ue.huanxung.cn

[R16] until 等待条件
来源：http://ag.521024.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fv.nszjky.cn

[R17] 数组定义与取值
来源：http://bl.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qo.wgjwhj.cn

[R18] 遍历数组
来源：http://nk.wgjwhj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rh.muxihuayi.cn

[R19] 数组长度
来源：http://lg.nicolike.cn

echo "${#arr[@]}"
来源：http://kj.9csxet.cn

[R20] 关联数组（字典）
来源：http://rb.nszjky.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://js.newstarts.cn

[R21] 字符串长度
来源：http://gt.haigaiapp.cn

echo "${#s}"
来源：http://cl.shxzukj.cn

[R22] 截取子串
来源：http://ze.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://ku.chemitech.net.cn

[R23] 字符串替换
来源：http://im.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vu.nicolike.cn

[R24] 大小写转换
来源：http://qd.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bv.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://su.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ka.panjiajie.cn

[R26] 命令替换
来源：http://hi.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://na.lnxyls.cn

[R27] 算术展开
来源：http://ao.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://ok.huixiangedu.cn

[R28] 浮点运算
来源：http://vv.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://xu.521024.cn

[R29] 定义函数
来源：http://ne.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ll.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://df.nicolike.cn

f() { return 0; }; f || echo "失败了"
来源：http://qz.chemitech.net.cn

[R31] 局部变量
来源：http://ja.huanxung.cn

f() { local x=1; echo "$x"; }
来源：http://sn.wgjwhj.cn

[R32] 参数个数校验
来源：http://tf.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jc.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://pf.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nb.huanxung.cn

[R34] 退出时清理
来源：http://pv.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ey.hnjuh.cn

[R35] 后台执行并等待
来源：http://js.hahajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uo.gzmigu.cn

[R36] 并发执行多个任务
来源：http://cb.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yn.9csxet.cn

[R37] 把输出赋给变量
来源：http://wx.colortex.cn

files=$(ls -1)
来源：http://em.panjiajie.cn

[R38] 管道串联
来源：http://vp.lnxyls.cn

cat a.txt | grep -i error | wc -l
来源：http://bj.shtwfgs.cn

[R39] 重定向标准输出与错误
来源：http://qi.nicolike.cn

cmd > out.log 2>&1
来源：http://bm.jctech888.com.cn

[R40] 追加写日志
来源：http://jo.asd995.cn

echo "log" >> out.log
来源：http://vh.shxzskj.cn

[R41] 丢弃输出
来源：http://uh.colortex.cn

cmd >/dev/null 2>&1
来源：http://aw.bookmarksfly.cn

[R42] 输入重定向
来源：http://bu.shtwfgs.cn

wc -l < a.txt
来源：http://oa.yuexingan06.cn

[R43] 按名字查找文件
来源：http://yw.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://tm.nicolike.cn

[R44] 按修改时间查找
来源：http://bo.colortex.cn

find . -mtime -7 -type f
来源：http://ke.gzmigu.cn

[R45] 批量删除
来源：http://lt.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://hy.nicolike.cn

[R46] 递归替换文件内容
来源：http://qh.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://en.huixiangedu.cn

[R47] sed 单行替换
来源：http://sk.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vq.521024.cn

[R48] awk 取指定列
来源：http://rp.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://wj.wgjwhj.cn

[R49] awk 带条件
来源：http://ys.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qy.panjiajie.cn

[R50] awk 求和
来源：http://hv.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sx.jctech888.com.cn

[R51] 排序去重取前几
来源：http://tr.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://le.9csxet.cn

[R52] 统计行数
来源：http://qi.yuexingan06.cn

wc -l a.txt
来源：http://wo.yuntaijiaju.cn

[R53] 查看文件头与实时尾
来源：http://wq.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xs.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://ky.shxzskj.cn

diff a.txt b.txt
来源：http://xx.jctech888.com.cn

[R55] 压缩与解压
来源：http://gv.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://li.shxzukj.cn

[R56] 远程拷贝
来源：http://tg.hnjuh.cn

scp file user@host:/path/
来源：http://og.huanxung.cn

[R57] 远程执行命令
来源：http://fb.bookmarksfly.cn

ssh user@host 'uptime'
来源：http://hb.521024.cn

[R58] 下载文件
来源：http://dq.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sg.lnxyls.cn

[R59] 发 POST JSON
来源：http://qx.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://or.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://qk.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zc.wgjwhj.cn

[R61] 磁盘占用
来源：http://ul.muxihuayi.cn

df -h;  du -sh *
来源：http://bf.nicolike.cn

[R62] 找最占空间的文件
来源：http://aq.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://je.muxihuayi.cn

[R63] 内存与进程
来源：http://az.521024.cn

free -h;  ps aux | grep nginx
来源：http://cp.jctech888.com.cn

[R64] 结束进程
来源：http://gy.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://vi.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://dx.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kg.panjiajie.cn

[R66] 定时任务
来源：http://el.gzmigu.cn

crontab -e;  crontab -l
来源：http://vd.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://hb.hahajie.cn

openssl rand -hex 16
来源：http://ok.shtwfgs.cn

[R68] 计算文件校验值
来源：http://dd.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zq.szsharing.cn

[R69] 生成随机密码
来源：http://qe.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://hs.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://of.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://tu.yuntaijiaju.cn

[R71] 日期格式化
来源：http://ye.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gw.shxzukj.cn

[R72] 等待端口就绪
来源：http://lp.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bw.shxzukj.cn

[R73] 分割大日志
来源：http://ry.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://ey.bookmarksfly.cn

[R74] 批量重命名
来源：http://sn.shxzskj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dz.newstarts.cn

[R75] 导出环境变量
来源：http://bf.szsharing.cn

export PATH="$HOME/bin:$PATH"
来源：http://pm.nszjky.cn

[R76] 使用临时文件
来源：http://vv.szxytkj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mj.jctech888.com.cn

[R77] 读取用户输入
来源：http://px.wgjwhj.cn

read -rp "请输入: " ans
来源：http://qy.shxzskj.cn

[R78] 交互式菜单
来源：http://cj.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zq.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://rh.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uu.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://bd.nszjky.cn

time ./run.sh
来源：http://qu.yuexingan06.cn

================================================================================
来源：http://yz.huanxung.cn

S. C / C++ 专题
来源：http://gc.shxzskj.cn

================================================================================
来源：http://hx.hahajie.cn

[S01] C：Hello World
来源：http://vt.jctech888.com.cn

#include <stdio.h>
来源：http://pv.jianghongdianzi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vn.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://uz.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://rg.newstarts.cn

[S03] C：读入整数
来源：http://tv.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://go.shtwfgs.cn

[S04] C：字符串复制
来源：http://if.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://id.bookmarksfly.cn

[S05] C：字符串长度
来源：http://fw.jianghongdianzi.cn

strlen(s)
来源：http://ch.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://rg.hahajie.cn

strcmp(a, b) == 0
来源：http://qt.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://bi.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ae.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://hp.huixinmuqiang.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oo.colortex.cn

[S09] C：结构体定义与初始化
来源：http://sk.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jy.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://vm.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://ih.huanxung.cn

[S11] C：逐行读文件
来源：http://dg.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://aa.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://un.asd995.cn

fclose(f);
来源：http://fd.wgjwhj.cn

[S12] C：写文件
来源：http://tr.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vd.nicolike.cn

[S13] C：宏定义
来源：http://fu.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ak.lnxyls.cn

[S14] C：枚举
来源：http://kx.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://ea.lnxyls.cn

[S15] C：类型转换
来源：http://jr.bjjhwx.cn

(double) a / b
来源：http://ey.wgjwhj.cn

[S16] C：位操作置位
来源：http://ra.panjiajie.cn


<!-- 参考信息 -->