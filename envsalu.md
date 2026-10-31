代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ep.nszjky.cn

[Q50] 批量更新
来源：http://kk.chemitech.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dx.wgjwhj.cn

[Q51] 用子查询更新
来源：http://sd.wgjwhj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sg.hahajie.cn

[Q52] 删除指定行
来源：http://kd.huixiangedu.cn

DELETE FROM users WHERE id = 10;
来源：http://fa.hahajie.cn

[Q53] 按条件删除
来源：http://cx.huixiangedu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qm.shxzukj.cn

[Q54] 清空表
来源：http://jk.bjjhwx.cn

TRUNCATE TABLE logs;
来源：http://zy.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://ee.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tc.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://vc.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fs.yuntaijiaju.cn

[Q57] 行号
来源：http://kf.nszjky.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eo.9csxet.cn

[Q58] 累计求和
来源：http://ii.yuntaijiaju.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qy.haigaiapp.cn

[Q59] 分组内累计
来源：http://cz.jianghongdianzi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ay.bookmarksfly.cn

[Q60] 取上一行 / 下一行
来源：http://vc.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uh.huixinmuqiang.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xb.wgjwhj.cn

[Q61] 移动平均
来源：http://tv.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fq.yuexingan06.cn

[Q62] 分组占比
来源：http://bj.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kk.yuexingan06.cn

[Q63] 开启事务
来源：http://to.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xk.muxihuayi.cn

[Q64] 提交事务
来源：http://hj.bjjhwx.cn

COMMIT;
来源：http://ju.bjjhwx.cn

[Q65] 回滚事务
来源：http://yt.jianghongdianzi.cn

ROLLBACK;
来源：http://zy.colortex.cn

[Q66] 行锁查询
来源：http://xn.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ua.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://iz.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hk.gzmigu.cn

[Q68] 保存点
来源：http://qw.panjiajie.cn

SAVEPOINT sp1;
来源：http://ss.9csxet.cn

ROLLBACK TO sp1;
来源：http://hq.haigaiapp.cn

[Q69] 查看执行计划
来源：http://vn.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kp.jctech888.com.cn

[Q70] 更新统计信息
来源：http://as.nicolike.cn

ANALYZE TABLE users;
来源：http://tr.newstarts.cn

[Q71] 查看建表语句
来源：http://lj.yuexingan06.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cj.gzmigu.cn

[Q72] 查看索引
来源：http://wa.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://za.panjiajie.cn

[Q73] 查看表状态
来源：http://tw.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gd.asd995.cn

[Q74] 强制使用索引
来源：http://au.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sj.gzmigu.cn

[Q75] 日期格式化
来源：http://yq.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xn.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tn.huixinmuqiang.cn

[Q76] 按天统计
来源：http://ct.newstarts.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://by.wgjwhj.cn

[Q77] 时间加减
来源：http://nk.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://af.bjjhwx.cn

[Q78] 当前时间
来源：http://gz.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pw.nszjky.cn

[Q79] 字符串拼接
来源：http://aq.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ep.jianghongdianzi.cn

[Q80] 字符串截取
来源：http://at.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://py.chemitech.net.cn

[Q81] 字符串替换
来源：http://nh.jctech888.com.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hc.muxihuayi.cn

[Q82] 字符长度与字节长度
来源：http://wz.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nr.9csxet.cn

[Q83] 大小写转换
来源：http://ax.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://aw.jianghongdianzi.cn

[Q84] 去除首尾空格
来源：http://xp.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://pb.jctech888.com.cn

[Q85] 数值取整
来源：http://yv.bookmarksfly.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ug.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://fg.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zb.521024.cn

[Q87] JSON 字段做条件
来源：http://wg.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lt.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://bf.huixiangedu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://at.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://da.muxihuayi.cn

[Q89] 判断表是否存在
来源：http://wx.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.panjiajie.cn

[Q90] 生成序号列
来源：http://py.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qv.521024.cn

================================================================================
来源：http://vi.huixinmuqiang.cn

R. Bash 专题
来源：http://fm.yuexingan06.cn

================================================================================
来源：http://fa.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://oy.hnjuh.cn

#!/usr/bin/env bash
来源：http://wq.bookmarksfly.cn

set -euo pipefail
来源：http://qk.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://di.521024.cn

name="Tom"; echo "$name"
来源：http://qq.jctech888.com.cn

[R03] 只读变量
来源：http://cq.szxytkj.cn

readonly PI=3.14
来源：http://cm.shxzskj.cn

[R04] 位置参数
来源：http://pu.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lk.gzmigu.cn

[R05] 参数默认值
来源：http://ae.szxytkj.cn

name="${1:-default}"
来源：http://af.szxytkj.cn

[R06] 判断命令是否存在
来源：http://rr.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jx.szxytkj.cn

[R07] if 判断文件
来源：http://fc.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xc.jianghongdianzi.cn

[R08] 数值比较
来源：http://na.panjiajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rc.yuntaijiaju.cn

[R09] 字符串比较
来源：http://gb.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fw.bookmarksfly.cn

[R10] 正则匹配
来源：http://gn.shxzukj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ty.lnxyls.cn

[R11] case 多分支
来源：http://rz.bookmarksfly.cn

case "$1" in
来源：http://ka.huixiangedu.cn

start) echo "启动" ;;
来源：http://lx.bookmarksfly.cn

stop)  echo "停止" ;;
来源：http://cw.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://fw.szsharing.cn

esac
来源：http://am.bookmarksfly.cn

[R12] for 遍历文件
来源：http://ct.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://gf.gzmigu.cn

[R13] for 计数循环
来源：http://lj.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://pc.lnxyls.cn

[R14] C 风格 for
来源：http://bx.huixiangedu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sb.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://fk.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rs.shtwfgs.cn

[R16] until 等待条件
来源：http://ii.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ev.yuexingan06.cn

[R17] 数组定义与取值
来源：http://zy.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uo.hahajie.cn

[R18] 遍历数组
来源：http://wy.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zf.bookmarksfly.cn

[R19] 数组长度
来源：http://nx.colortex.cn

echo "${#arr[@]}"
来源：http://br.hahajie.cn

[R20] 关联数组（字典）
来源：http://qw.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tu.shxzskj.cn

[R21] 字符串长度
来源：http://mi.chemitech.net.cn

echo "${#s}"
来源：http://wm.hahajie.cn

[R22] 截取子串
来源：http://vz.wgjwhj.cn

echo "${s:0:5}"
来源：http://cy.bjjhwx.cn

[R23] 字符串替换
来源：http://co.bjjhwx.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pd.bookmarksfly.cn

[R24] 大小写转换
来源：http://wo.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fv.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://mw.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ht.huanxung.cn

[R26] 命令替换
来源：http://go.nicolike.cn

now=$(date +%F); echo "$now"
来源：http://us.yuexingan06.cn

[R27] 算术展开
来源：http://wq.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://no.hnjuh.cn

[R28] 浮点运算
来源：http://nq.9csxet.cn

echo "scale=2; 10/3" | bc
来源：http://qz.colortex.cn

[R29] 定义函数
来源：http://so.newstarts.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qf.gzmigu.cn

[R30] 函数返回状态码
来源：http://lg.muxihuayi.cn

f() { return 0; }; f || echo "失败了"
来源：http://xc.shxzskj.cn

[R31] 局部变量
来源：http://cd.haigaiapp.cn

f() { local x=1; echo "$x"; }
来源：http://bb.colortex.cn

[R32] 参数个数校验
来源：http://xe.chemitech.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kx.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://of.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ws.huixinmuqiang.cn

[R34] 退出时清理
来源：http://jh.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dw.shtwfgs.cn

[R35] 后台执行并等待
来源：http://va.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gc.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://zo.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hb.jianghongdianzi.cn

[R37] 把输出赋给变量
来源：http://hb.huixinmuqiang.cn

files=$(ls -1)
来源：http://yw.jianghongdianzi.cn

[R38] 管道串联
来源：http://fs.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://fz.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://ub.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://xn.yuexingan06.cn

[R40] 追加写日志
来源：http://je.jianghongdianzi.cn

echo "log" >> out.log
来源：http://jh.shxzskj.cn

[R41] 丢弃输出
来源：http://yx.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://fk.lnxyls.cn

[R42] 输入重定向
来源：http://jb.hnjuh.cn

wc -l < a.txt
来源：http://sk.shtwfgs.cn

[R43] 按名字查找文件
来源：http://va.muxihuayi.cn

find . -name "*.log" -type f
来源：http://np.huixiangedu.cn

[R44] 按修改时间查找
来源：http://pf.yuexingan06.cn

find . -mtime -7 -type f
来源：http://po.gzmigu.cn

[R45] 批量删除
来源：http://mt.521024.cn

find . -name "*.tmp" -delete
来源：http://gw.szsharing.cn

[R46] 递归替换文件内容
来源：http://mq.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kh.panjiajie.cn

[R47] sed 单行替换
来源：http://iy.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jb.szsharing.cn

[R48] awk 取指定列
来源：http://fc.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://ia.nszjky.cn

[R49] awk 带条件
来源：http://ws.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sd.colortex.cn

[R50] awk 求和
来源：http://xb.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://du.lnxyls.cn

[R51] 排序去重取前几
来源：http://un.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mz.huixinmuqiang.cn

[R52] 统计行数
来源：http://di.huixiangedu.cn

wc -l a.txt
来源：http://lt.yuntaijiaju.cn

[R53] 查看文件头与实时尾
来源：http://ty.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fx.huixiangedu.cn

[R54] 比较两个文件
来源：http://pw.huanxung.cn

diff a.txt b.txt
来源：http://hw.shtwfgs.cn

[R55] 压缩与解压
来源：http://sx.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://um.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://bn.gzmigu.cn

scp file user@host:/path/
来源：http://zc.shxzukj.cn

[R57] 远程执行命令
来源：http://ml.muxihuayi.cn

ssh user@host 'uptime'
来源：http://xk.jianghongdianzi.cn

[R58] 下载文件
来源：http://al.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uh.muxihuayi.cn

[R59] 发 POST JSON
来源：http://ly.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rv.521024.cn

[R60] 只看 HTTP 状态码
来源：http://im.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lo.shxzskj.cn

[R61] 磁盘占用
来源：http://fc.yuntaijiaju.cn

df -h;  du -sh *
来源：http://dt.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://qh.chemitech.net.cn

du -ah . | sort -rh | head -10
来源：http://kz.yuntaijiaju.cn

[R63] 内存与进程
来源：http://hx.yuntaijiaju.cn

free -h;  ps aux | grep nginx
来源：http://mc.yuntaijiaju.cn

[R64] 结束进程
来源：http://ai.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://vr.nszjky.cn

[R65] 查看端口占用
来源：http://fv.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://py.shxzskj.cn

[R66] 定时任务
来源：http://qa.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://kt.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://sk.hahajie.cn

openssl rand -hex 16
来源：http://rp.shxzukj.cn

[R68] 计算文件校验值
来源：http://rg.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pw.haigaiapp.cn

[R69] 生成随机密码
来源：http://ju.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://lf.bjjhwx.cn

[R70] 时间戳与互转
来源：http://bk.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://ov.shxzskj.cn

[R71] 日期格式化
来源：http://rc.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yg.szsharing.cn

[R72] 等待端口就绪
来源：http://ph.yuexingan06.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xf.nicolike.cn

[R73] 分割大日志
来源：http://gh.521024.cn

split -l 1000 big.log part_
来源：http://gw.muxihuayi.cn

[R74] 批量重命名
来源：http://yo.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rz.jctech888.com.cn

[R75] 导出环境变量
来源：http://uk.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://sb.gzmigu.cn

[R76] 使用临时文件
来源：http://ed.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wy.colortex.cn

[R77] 读取用户输入
来源：http://ly.bjjhwx.cn

read -rp "请输入: " ans
来源：http://dt.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://hk.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zc.gzmigu.cn

[R79] 解析命令行选项
来源：http://fj.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fm.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://iy.szsharing.cn

time ./run.sh
来源：http://tt.colortex.cn

================================================================================
来源：http://jp.newstarts.cn

S. C / C++ 专题
来源：http://hd.yuexingan06.cn

================================================================================
来源：http://rg.jctech888.com.cn

[S01] C：Hello World
来源：http://tz.521024.cn

#include <stdio.h>
来源：http://tl.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://to.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://xs.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://md.shxzskj.cn

[S03] C：读入整数
来源：http://ry.colortex.cn

int x; scanf("%d", &x);
来源：http://dc.jctech888.com.cn

[S04] C：字符串复制
来源：http://rt.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xs.shxzskj.cn

[S05] C：字符串长度
来源：http://di.jctech888.com.cn

strlen(s)
来源：http://lw.bjjhwx.cn

[S06] C：字符串比较
来源：http://hp.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://mc.huanxung.cn

[S07] C：数组遍历求和
来源：http://sa.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uc.colortex.cn

[S08] C：动态内存分配与释放
来源：http://fm.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xc.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://dh.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bg.shxzskj.cn

[S10] C：指针与解引用
来源：http://ay.asd995.cn

int *p = &a;  *p = 5;
来源：http://xx.gzmigu.cn

[S11] C：逐行读文件
来源：http://iv.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://fa.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fg.huixinmuqiang.cn

fclose(f);
来源：http://wb.shxzukj.cn

[S12] C：写文件
来源：http://hm.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bg.lnxyls.cn

[S13] C：宏定义
来源：http://jt.nicolike.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uw.panjiajie.cn

[S14] C：枚举
来源：http://gp.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://iv.muxihuayi.cn

[S15] C：类型转换
来源：http://hd.haigaiapp.cn

(double) a / b
来源：http://um.wgjwhj.cn

[S16] C：位操作置位
来源：http://mm.nszjky.cn

x |= (1 << 3);
来源：http://jf.nicolike.cn

[S17] C：安全拼接字符串
来源：http://om.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wx.shtwfgs.cn

[S18] C：命令行参数
来源：http://jv.muxihuayi.cn

int main(int argc, char **argv)
来源：http://qq.huixinmuqiang.cn

[S19] C：快速排序
来源：http://rf.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bo.muxihuayi.cn

[S20] C：二分查找
来源：http://cp.haigaiapp.cn


<!-- 参考信息 -->