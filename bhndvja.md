代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fv.huanxung.cn

[Q52] 删除指定行
来源：http://ds.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://ey.huixiangedu.cn

[Q53] 按条件删除
来源：http://za.gzmigu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jw.521024.cn

[Q54] 清空表
来源：http://po.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://fj.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://rl.newstarts.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wx.yuexingan06.cn

[Q56] 密集排名（并列不占位）
来源：http://gv.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dc.9csxet.cn

[Q57] 行号
来源：http://yy.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://te.newstarts.cn

[Q58] 累计求和
来源：http://zl.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ef.jianghongdianzi.cn

[Q59] 分组内累计
来源：http://xd.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lf.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://hg.nicolike.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mr.newstarts.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://km.shxzskj.cn

[Q61] 移动平均
来源：http://pp.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://en.szsharing.cn

[Q62] 分组占比
来源：http://gb.9csxet.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qr.huixiangedu.cn

[Q63] 开启事务
来源：http://dp.haigaiapp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://is.szxytkj.cn

[Q64] 提交事务
来源：http://pj.521024.cn

COMMIT;
来源：http://ru.newstarts.cn

[Q65] 回滚事务
来源：http://qj.nszjky.cn

ROLLBACK;
来源：http://hh.szsharing.cn

[Q66] 行锁查询
来源：http://fw.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cb.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://lw.szxytkj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bj.chemitech.net.cn

[Q68] 保存点
来源：http://ro.panjiajie.cn

SAVEPOINT sp1;
来源：http://yo.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://pk.nicolike.cn

[Q69] 查看执行计划
来源：http://fw.bookmarksfly.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xl.chemitech.net.cn

[Q70] 更新统计信息
来源：http://qu.yuexingan06.cn

ANALYZE TABLE users;
来源：http://ng.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://as.521024.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wp.panjiajie.cn

[Q72] 查看索引
来源：http://na.huanxung.cn

SHOW INDEX FROM users;
来源：http://gy.lnxyls.cn

[Q73] 查看表状态
来源：http://om.asd995.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dr.hahajie.cn

[Q74] 强制使用索引
来源：http://tv.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bp.huixiangedu.cn

[Q75] 日期格式化
来源：http://bo.huixiangedu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ol.nicolike.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vh.nicolike.cn

[Q76] 按天统计
来源：http://af.nszjky.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uu.521024.cn

[Q77] 时间加减
来源：http://rw.huixiangedu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uu.colortex.cn

[Q78] 当前时间
来源：http://cg.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ek.wgjwhj.cn

[Q79] 字符串拼接
来源：http://hx.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://it.lnxyls.cn

[Q80] 字符串截取
来源：http://yt.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wi.bjjhwx.cn

[Q81] 字符串替换
来源：http://ej.yuexingan06.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kl.asd995.cn

[Q82] 字符长度与字节长度
来源：http://yx.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zz.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://ek.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vt.hahajie.cn

[Q84] 去除首尾空格
来源：http://an.haigaiapp.cn

SELECT TRIM(name) FROM users;
来源：http://ze.haigaiapp.cn

[Q85] 数值取整
来源：http://jc.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tc.yuexingan06.cn

[Q86] 读取 JSON 字段
来源：http://tg.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cy.hahajie.cn

[Q87] JSON 字段做条件
来源：http://ij.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mp.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://xv.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://be.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yt.szsharing.cn

[Q89] 判断表是否存在
来源：http://ym.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ml.shtwfgs.cn

[Q90] 生成序号列
来源：http://ul.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ef.521024.cn

================================================================================
来源：http://cg.lnxyls.cn

R. Bash 专题
来源：http://gr.bjjhwx.cn

================================================================================
来源：http://hz.9csxet.cn

[R01] shebang 与严格模式
来源：http://ev.huixiangedu.cn

#!/usr/bin/env bash
来源：http://mq.shxzskj.cn

set -euo pipefail
来源：http://vc.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://ic.521024.cn

name="Tom"; echo "$name"
来源：http://qh.huanxung.cn

[R03] 只读变量
来源：http://oy.shtwfgs.cn

readonly PI=3.14
来源：http://ly.colortex.cn

[R04] 位置参数
来源：http://pc.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kc.lnxyls.cn

[R05] 参数默认值
来源：http://nz.szxytkj.cn

name="${1:-default}"
来源：http://sv.lnxyls.cn

[R06] 判断命令是否存在
来源：http://nd.bjjhwx.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://au.gzmigu.cn

[R07] if 判断文件
来源：http://eq.9csxet.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yy.nszjky.cn

[R08] 数值比较
来源：http://oy.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cy.nicolike.cn

[R09] 字符串比较
来源：http://nx.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tc.szsharing.cn

[R10] 正则匹配
来源：http://ou.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vo.bjjhwx.cn

[R11] case 多分支
来源：http://ue.jianghongdianzi.cn

case "$1" in
来源：http://jm.panjiajie.cn

start) echo "启动" ;;
来源：http://xa.yuexingan06.cn

stop)  echo "停止" ;;
来源：http://md.521024.cn

*)     echo "未知命令" ;;
来源：http://gv.shtwfgs.cn

esac
来源：http://jg.jctech888.com.cn

[R12] for 遍历文件
来源：http://nl.szsharing.cn

for f in *.txt; do echo "$f"; done
来源：http://dp.yuexingan06.cn

[R13] for 计数循环
来源：http://lf.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://ig.shxzukj.cn

[R14] C 风格 for
来源：http://yn.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://le.muxihuayi.cn

[R15] while 逐行读文件
来源：http://dn.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xe.gzmigu.cn

[R16] until 等待条件
来源：http://bd.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xk.huixiangedu.cn

[R17] 数组定义与取值
来源：http://hu.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gb.hahajie.cn

[R18] 遍历数组
来源：http://zy.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zh.huixinmuqiang.cn

[R19] 数组长度
来源：http://so.colortex.cn

echo "${#arr[@]}"
来源：http://ul.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://gm.hnjuh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cp.bjjhwx.cn

[R21] 字符串长度
来源：http://ur.shxzukj.cn

echo "${#s}"
来源：http://bn.gzmigu.cn

[R22] 截取子串
来源：http://vm.gzmigu.cn

echo "${s:0:5}"
来源：http://up.gzmigu.cn

[R23] 字符串替换
来源：http://aq.lnxyls.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xh.lnxyls.cn

[R24] 大小写转换
来源：http://nl.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fh.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://ua.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yy.hahajie.cn

[R26] 命令替换
来源：http://rs.colortex.cn

now=$(date +%F); echo "$now"
来源：http://jt.huixiangedu.cn

[R27] 算术展开
来源：http://pa.nszjky.cn

echo $((1 + 2 * 3))
来源：http://wj.wgjwhj.cn

[R28] 浮点运算
来源：http://gj.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://pa.shtwfgs.cn

[R29] 定义函数
来源：http://oj.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gb.521024.cn

[R30] 函数返回状态码
来源：http://ce.shxzskj.cn

f() { return 0; }; f || echo "失败了"
来源：http://ll.shxzukj.cn

[R31] 局部变量
来源：http://bw.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://ct.shxzskj.cn

[R32] 参数个数校验
来源：http://af.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bn.521024.cn

[R33] 捕获错误并提示行号
来源：http://kt.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cl.szxytkj.cn

[R34] 退出时清理
来源：http://nn.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sl.hahajie.cn

[R35] 后台执行并等待
来源：http://du.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vo.hahajie.cn

[R36] 并发执行多个任务
来源：http://pp.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://de.jianghongdianzi.cn

[R37] 把输出赋给变量
来源：http://xm.gzmigu.cn

files=$(ls -1)
来源：http://ev.gzmigu.cn

[R38] 管道串联
来源：http://xj.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://fh.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://sc.nicolike.cn

cmd > out.log 2>&1
来源：http://ue.jctech888.com.cn

[R40] 追加写日志
来源：http://gp.asd995.cn

echo "log" >> out.log
来源：http://se.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://ie.szsharing.cn

cmd >/dev/null 2>&1
来源：http://ea.hnjuh.cn

[R42] 输入重定向
来源：http://ez.521024.cn

wc -l < a.txt
来源：http://zj.521024.cn

[R43] 按名字查找文件
来源：http://ms.shxzskj.cn

find . -name "*.log" -type f
来源：http://aa.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://br.hnjuh.cn

find . -mtime -7 -type f
来源：http://ko.huixinmuqiang.cn

[R45] 批量删除
来源：http://ee.hnjuh.cn

find . -name "*.tmp" -delete
来源：http://fx.hahajie.cn

[R46] 递归替换文件内容
来源：http://ma.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sn.shtwfgs.cn

[R47] sed 单行替换
来源：http://yj.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://np.huanxung.cn

[R48] awk 取指定列
来源：http://ac.hahajie.cn

awk '{print $1, $3}' a.txt
来源：http://rv.muxihuayi.cn

[R49] awk 带条件
来源：http://ig.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yu.hahajie.cn

[R50] awk 求和
来源：http://bl.yuexingan06.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pj.shxzskj.cn

[R51] 排序去重取前几
来源：http://nl.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ku.chemitech.net.cn

[R52] 统计行数
来源：http://bq.chemitech.net.cn

wc -l a.txt
来源：http://bf.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://hl.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sp.haigaiapp.cn

[R54] 比较两个文件
来源：http://zq.yuntaijiaju.cn

diff a.txt b.txt
来源：http://mo.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://oh.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://si.newstarts.cn

[R56] 远程拷贝
来源：http://pr.lnxyls.cn

scp file user@host:/path/
来源：http://po.jctech888.com.cn

[R57] 远程执行命令
来源：http://pv.huixiangedu.cn

ssh user@host 'uptime'
来源：http://kf.yuexingan06.cn

[R58] 下载文件
来源：http://ie.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fj.chemitech.net.cn

[R59] 发 POST JSON
来源：http://hi.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ud.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://ik.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gs.shxzskj.cn

[R61] 磁盘占用
来源：http://ah.hahajie.cn

df -h;  du -sh *
来源：http://bu.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://ho.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://cu.yuexingan06.cn

[R63] 内存与进程
来源：http://tm.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://br.9csxet.cn

[R64] 结束进程
来源：http://mf.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://ty.gzmigu.cn

[R65] 查看端口占用
来源：http://vo.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yu.shxzskj.cn

[R66] 定时任务
来源：http://pd.huixiangedu.cn

crontab -e;  crontab -l
来源：http://ij.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://sr.szsharing.cn

openssl rand -hex 16
来源：http://wh.newstarts.cn

[R68] 计算文件校验值
来源：http://zk.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uk.szxytkj.cn

[R69] 生成随机密码
来源：http://at.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://vf.lnxyls.cn

[R70] 时间戳与互转
来源：http://ib.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://xq.lnxyls.cn

[R71] 日期格式化
来源：http://jw.jianghongdianzi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bc.9csxet.cn

[R72] 等待端口就绪
来源：http://nj.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vu.gzmigu.cn

[R73] 分割大日志
来源：http://iy.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://zp.muxihuayi.cn

[R74] 批量重命名
来源：http://qv.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tl.yuexingan06.cn

[R75] 导出环境变量
来源：http://ol.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://hy.bjjhwx.cn

[R76] 使用临时文件
来源：http://um.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rt.nicolike.cn

[R77] 读取用户输入
来源：http://ia.szsharing.cn

read -rp "请输入: " ans
来源：http://ln.huanxung.cn

[R78] 交互式菜单
来源：http://xt.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hy.shtwfgs.cn

[R79] 解析命令行选项
来源：http://kc.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dn.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://iv.nicolike.cn

time ./run.sh
来源：http://eu.gzmigu.cn

================================================================================
来源：http://bo.gzmigu.cn

S. C / C++ 专题
来源：http://db.lnxyls.cn

================================================================================
来源：http://ks.jianghongdianzi.cn

[S01] C：Hello World
来源：http://mc.haigaiapp.cn

#include <stdio.h>
来源：http://gk.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://iz.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://nn.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://ib.huixiangedu.cn

[S03] C：读入整数
来源：http://pp.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://iz.shtwfgs.cn

[S04] C：字符串复制
来源：http://ad.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://un.521024.cn

[S05] C：字符串长度
来源：http://rz.hahajie.cn

strlen(s)
来源：http://vf.lnxyls.cn

[S06] C：字符串比较
来源：http://us.9csxet.cn

strcmp(a, b) == 0
来源：http://lc.huanxung.cn

[S07] C：数组遍历求和
来源：http://vh.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lk.9csxet.cn

[S08] C：动态内存分配与释放
来源：http://yo.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vp.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://en.hnjuh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://al.yuexingan06.cn

[S10] C：指针与解引用
来源：http://bj.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://ei.panjiajie.cn

[S11] C：逐行读文件
来源：http://pm.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://tb.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mp.jianghongdianzi.cn

fclose(f);
来源：http://qa.shxzskj.cn

[S12] C：写文件
来源：http://sv.lnxyls.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cc.gzmigu.cn

[S13] C：宏定义
来源：http://hk.newstarts.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hk.jctech888.com.cn

[S14] C：枚举
来源：http://nb.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://ku.hnjuh.cn

[S15] C：类型转换
来源：http://hv.panjiajie.cn

(double) a / b
来源：http://cy.huanxung.cn

[S16] C：位操作置位
来源：http://hz.521024.cn

x |= (1 << 3);
来源：http://bb.lnxyls.cn

[S17] C：安全拼接字符串
来源：http://jj.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dw.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://uq.haigaiapp.cn

int main(int argc, char **argv)
来源：http://ff.hahajie.cn

[S19] C：快速排序
来源：http://cy.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uk.huanxung.cn

[S20] C：二分查找
来源：http://ei.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://an.nicolike.cn

[S21] C：字符类别判断
来源：http://rc.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ze.gzmigu.cn

[S22] C：字符串转数字
来源：http://ay.yuntaijiaju.cn


<!-- 参考信息 -->