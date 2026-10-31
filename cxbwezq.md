代发 wailian999

[Q48] CTE 公用表表达式
来源：http://el.panjiajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ct.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://ln.nszjky.cn

[Q49] 更新单行
来源：http://eo.shtwfgs.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kw.asd995.cn

[Q50] 批量更新
来源：http://hq.bookmarksfly.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yc.szxytkj.cn

[Q51] 用子查询更新
来源：http://qb.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zi.yuexingan06.cn

[Q52] 删除指定行
来源：http://qq.wgjwhj.cn

DELETE FROM users WHERE id = 10;
来源：http://gd.521024.cn

[Q53] 按条件删除
来源：http://zt.bookmarksfly.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://js.muxihuayi.cn

[Q54] 清空表
来源：http://rs.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://yw.hahajie.cn

[Q55] 排名（并列占位）
来源：http://vt.lnxyls.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mi.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://zb.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cm.hnjuh.cn

[Q57] 行号
来源：http://cl.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xx.szxytkj.cn

[Q58] 累计求和
来源：http://ez.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tp.muxihuayi.cn

[Q59] 分组内累计
来源：http://re.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uk.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://ts.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gn.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nf.panjiajie.cn

[Q61] 移动平均
来源：http://ms.shtwfgs.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hl.chemitech.net.cn

[Q62] 分组占比
来源：http://pc.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wx.huanxung.cn

[Q63] 开启事务
来源：http://ss.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mr.shxzskj.cn

[Q64] 提交事务
来源：http://qk.bookmarksfly.cn

COMMIT;
来源：http://ud.shxzukj.cn

[Q65] 回滚事务
来源：http://sh.wgjwhj.cn

ROLLBACK;
来源：http://ac.yuntaijiaju.cn

[Q66] 行锁查询
来源：http://tc.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zd.nszjky.cn

[Q67] 设置隔离级别
来源：http://lk.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lm.bookmarksfly.cn

[Q68] 保存点
来源：http://no.gzmigu.cn

SAVEPOINT sp1;
来源：http://tk.yuexingan06.cn

ROLLBACK TO sp1;
来源：http://nh.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://de.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cl.huixiangedu.cn

[Q70] 更新统计信息
来源：http://pd.hnjuh.cn

ANALYZE TABLE users;
来源：http://ej.shxzukj.cn

[Q71] 查看建表语句
来源：http://lg.bjjhwx.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yq.shxzukj.cn

[Q72] 查看索引
来源：http://ta.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://tk.nicolike.cn

[Q73] 查看表状态
来源：http://me.hahajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ji.bjjhwx.cn

[Q74] 强制使用索引
来源：http://gk.lnxyls.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fq.chemitech.net.cn

[Q75] 日期格式化
来源：http://vb.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gn.newstarts.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ub.chemitech.net.cn

[Q76] 按天统计
来源：http://pg.huixinmuqiang.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://np.bookmarksfly.cn

[Q77] 时间加减
来源：http://jw.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vs.bookmarksfly.cn

[Q78] 当前时间
来源：http://bi.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ao.panjiajie.cn

[Q79] 字符串拼接
来源：http://uh.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ve.shxzukj.cn

[Q80] 字符串截取
来源：http://on.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vt.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://wy.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dq.yuexingan06.cn

[Q82] 字符长度与字节长度
来源：http://gf.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://na.shxzskj.cn

[Q83] 大小写转换
来源：http://tv.huanxung.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ow.colortex.cn

[Q84] 去除首尾空格
来源：http://du.shxzskj.cn

SELECT TRIM(name) FROM users;
来源：http://gc.jianghongdianzi.cn

[Q85] 数值取整
来源：http://bt.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jw.colortex.cn

[Q86] 读取 JSON 字段
来源：http://sa.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kr.chemitech.net.cn

[Q87] JSON 字段做条件
来源：http://ha.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uc.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://jp.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lb.panjiajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wq.szsharing.cn

[Q89] 判断表是否存在
来源：http://dj.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ne.colortex.cn

[Q90] 生成序号列
来源：http://mz.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uf.nicolike.cn

================================================================================
来源：http://fi.jianghongdianzi.cn

R. Bash 专题
来源：http://vx.yuexingan06.cn

================================================================================
来源：http://sk.shxzskj.cn

[R01] shebang 与严格模式
来源：http://pf.gzmigu.cn

#!/usr/bin/env bash
来源：http://zv.huanxung.cn

set -euo pipefail
来源：http://pz.shxzskj.cn

[R02] 变量赋值与使用
来源：http://gy.szsharing.cn

name="Tom"; echo "$name"
来源：http://za.huanxung.cn

[R03] 只读变量
来源：http://sn.nszjky.cn

readonly PI=3.14
来源：http://ue.lnxyls.cn

[R04] 位置参数
来源：http://ni.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ze.newstarts.cn

[R05] 参数默认值
来源：http://kw.newstarts.cn

name="${1:-default}"
来源：http://xn.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://xk.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ku.shxzskj.cn

[R07] if 判断文件
来源：http://vt.panjiajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ci.jctech888.com.cn

[R08] 数值比较
来源：http://eo.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ar.chemitech.net.cn

[R09] 字符串比较
来源：http://gb.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gx.huanxung.cn

[R10] 正则匹配
来源：http://rg.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zg.nszjky.cn

[R11] case 多分支
来源：http://fh.huanxung.cn

case "$1" in
来源：http://ps.huanxung.cn

start) echo "启动" ;;
来源：http://lh.shtwfgs.cn

stop)  echo "停止" ;;
来源：http://vt.szxytkj.cn

*)     echo "未知命令" ;;
来源：http://mg.szxytkj.cn

esac
来源：http://uv.shxzskj.cn

[R12] for 遍历文件
来源：http://dr.shxzskj.cn

for f in *.txt; do echo "$f"; done
来源：http://bu.huanxung.cn

[R13] for 计数循环
来源：http://gr.colortex.cn

for i in {1..10}; do echo "$i"; done
来源：http://kj.yuexingan06.cn

[R14] C 风格 for
来源：http://kc.jianghongdianzi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mw.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://fh.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lk.wgjwhj.cn

[R16] until 等待条件
来源：http://hx.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zu.huixiangedu.cn

[R17] 数组定义与取值
来源：http://pw.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://il.yuntaijiaju.cn

[R18] 遍历数组
来源：http://ak.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://em.huixiangedu.cn

[R19] 数组长度
来源：http://vf.gzmigu.cn

echo "${#arr[@]}"
来源：http://ou.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://oa.muxihuayi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dx.lnxyls.cn

[R21] 字符串长度
来源：http://la.colortex.cn

echo "${#s}"
来源：http://hz.gzmigu.cn

[R22] 截取子串
来源：http://cp.yuexingan06.cn

echo "${s:0:5}"
来源：http://vc.jianghongdianzi.cn

[R23] 字符串替换
来源：http://ks.yuexingan06.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aw.nicolike.cn

[R24] 大小写转换
来源：http://dz.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://az.521024.cn

[R25] 去后缀 / 去前缀
来源：http://nn.huanxung.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ki.bjjhwx.cn

[R26] 命令替换
来源：http://oe.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://zc.hnjuh.cn

[R27] 算术展开
来源：http://le.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://qi.chemitech.net.cn

[R28] 浮点运算
来源：http://pd.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://gx.huixinmuqiang.cn

[R29] 定义函数
来源：http://sy.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wz.nszjky.cn

[R30] 函数返回状态码
来源：http://nb.nszjky.cn

f() { return 0; }; f || echo "失败了"
来源：http://au.shtwfgs.cn

[R31] 局部变量
来源：http://po.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://lj.yuexingan06.cn

[R32] 参数个数校验
来源：http://mb.colortex.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cz.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://bn.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ni.lnxyls.cn

[R34] 退出时清理
来源：http://ks.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cp.panjiajie.cn

[R35] 后台执行并等待
来源：http://to.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gf.lnxyls.cn

[R36] 并发执行多个任务
来源：http://wj.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nx.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://wu.shtwfgs.cn

files=$(ls -1)
来源：http://vg.jianghongdianzi.cn

[R38] 管道串联
来源：http://dt.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://lr.haigaiapp.cn

[R39] 重定向标准输出与错误
来源：http://jx.shxzukj.cn

cmd > out.log 2>&1
来源：http://fc.chemitech.net.cn

[R40] 追加写日志
来源：http://wl.hnjuh.cn

echo "log" >> out.log
来源：http://iu.wgjwhj.cn

[R41] 丢弃输出
来源：http://mu.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://hv.huixiangedu.cn

[R42] 输入重定向
来源：http://dn.szxytkj.cn

wc -l < a.txt
来源：http://si.asd995.cn

[R43] 按名字查找文件
来源：http://lr.haigaiapp.cn

find . -name "*.log" -type f
来源：http://iq.wgjwhj.cn

[R44] 按修改时间查找
来源：http://ka.shxzukj.cn

find . -mtime -7 -type f
来源：http://ob.jctech888.com.cn

[R45] 批量删除
来源：http://mu.szxytkj.cn

find . -name "*.tmp" -delete
来源：http://lc.gzmigu.cn

[R46] 递归替换文件内容
来源：http://zk.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vu.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://on.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oe.haigaiapp.cn

[R48] awk 取指定列
来源：http://hf.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://wr.chemitech.net.cn

[R49] awk 带条件
来源：http://fm.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tx.huixinmuqiang.cn

[R50] awk 求和
来源：http://tn.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gu.muxihuayi.cn

[R51] 排序去重取前几
来源：http://oz.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://px.huixinmuqiang.cn

[R52] 统计行数
来源：http://bs.521024.cn

wc -l a.txt
来源：http://dc.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://qc.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pw.szsharing.cn

[R54] 比较两个文件
来源：http://qe.hahajie.cn

diff a.txt b.txt
来源：http://vv.521024.cn

[R55] 压缩与解压
来源：http://pl.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qb.shtwfgs.cn

[R56] 远程拷贝
来源：http://cy.nicolike.cn

scp file user@host:/path/
来源：http://vs.521024.cn

[R57] 远程执行命令
来源：http://fm.szsharing.cn

ssh user@host 'uptime'
来源：http://qy.huixinmuqiang.cn

[R58] 下载文件
来源：http://dj.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://si.newstarts.cn

[R59] 发 POST JSON
来源：http://fc.panjiajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gg.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://yv.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pe.lnxyls.cn

[R61] 磁盘占用
来源：http://yk.szsharing.cn

df -h;  du -sh *
来源：http://bt.panjiajie.cn

[R62] 找最占空间的文件
来源：http://nh.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://yd.shxzukj.cn

[R63] 内存与进程
来源：http://qs.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://cv.nszjky.cn

[R64] 结束进程
来源：http://tt.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://xj.chemitech.net.cn

[R65] 查看端口占用
来源：http://mf.muxihuayi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hn.haigaiapp.cn

[R66] 定时任务
来源：http://wh.szxytkj.cn

crontab -e;  crontab -l
来源：http://td.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://py.shtwfgs.cn

openssl rand -hex 16
来源：http://hl.yuexingan06.cn

[R68] 计算文件校验值
来源：http://yb.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qd.521024.cn

[R69] 生成随机密码
来源：http://ml.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://hr.wgjwhj.cn

[R70] 时间戳与互转
来源：http://ns.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://hu.huanxung.cn

[R71] 日期格式化
来源：http://vb.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rv.haigaiapp.cn

[R72] 等待端口就绪
来源：http://hw.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hg.chemitech.net.cn

[R73] 分割大日志
来源：http://rm.chemitech.net.cn

split -l 1000 big.log part_
来源：http://pf.lnxyls.cn

[R74] 批量重命名
来源：http://lx.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yw.lnxyls.cn

[R75] 导出环境变量
来源：http://ds.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://ur.nicolike.cn

[R76] 使用临时文件
来源：http://qj.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hm.shtwfgs.cn

[R77] 读取用户输入
来源：http://wi.nicolike.cn

read -rp "请输入: " ans
来源：http://zr.hahajie.cn

[R78] 交互式菜单
来源：http://vm.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jm.jctech888.com.cn

[R79] 解析命令行选项
来源：http://mn.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sk.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://sw.shxzukj.cn

time ./run.sh
来源：http://xk.asd995.cn

================================================================================
来源：http://ek.huixinmuqiang.cn

S. C / C++ 专题
来源：http://bc.shxzukj.cn

================================================================================
来源：http://tg.hahajie.cn

[S01] C：Hello World
来源：http://bn.szsharing.cn

#include <stdio.h>
来源：http://pz.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cq.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://eh.521024.cn

int a = 10; printf("%d\n", a);
来源：http://wu.asd995.cn

[S03] C：读入整数
来源：http://vn.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://me.nszjky.cn

[S04] C：字符串复制
来源：http://bh.panjiajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jd.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://dd.nicolike.cn

strlen(s)
来源：http://mf.shtwfgs.cn

[S06] C：字符串比较
来源：http://dr.yuexingan06.cn

strcmp(a, b) == 0
来源：http://ou.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://nz.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wl.huixinmuqiang.cn

[S08] C：动态内存分配与释放
来源：http://gx.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ag.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://dc.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oc.asd995.cn

[S10] C：指针与解引用
来源：http://tc.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://ad.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://sf.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://uy.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://be.nicolike.cn

fclose(f);
来源：http://sq.panjiajie.cn

[S12] C：写文件
来源：http://or.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iz.jianghongdianzi.cn

[S13] C：宏定义
来源：http://sm.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fg.nicolike.cn

[S14] C：枚举
来源：http://cg.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://xt.szsharing.cn

[S15] C：类型转换
来源：http://tl.szsharing.cn

(double) a / b
来源：http://xx.9csxet.cn

[S16] C：位操作置位
来源：http://dl.jctech888.com.cn

x |= (1 << 3);
来源：http://yr.hahajie.cn

[S17] C：安全拼接字符串
来源：http://js.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ui.nszjky.cn

[S18] C：命令行参数
来源：http://gn.haigaiapp.cn


<!-- 参考信息 -->