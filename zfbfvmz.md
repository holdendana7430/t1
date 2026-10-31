代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bq.jctech888.com.cn

[Q50] 批量更新
来源：http://ij.bookmarksfly.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ys.9csxet.cn

[Q51] 用子查询更新
来源：http://py.9csxet.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xy.bjjhwx.cn

[Q52] 删除指定行
来源：http://xt.shtwfgs.cn

DELETE FROM users WHERE id = 10;
来源：http://ba.chemitech.net.cn

[Q53] 按条件删除
来源：http://pt.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tv.gzmigu.cn

[Q54] 清空表
来源：http://ht.9csxet.cn

TRUNCATE TABLE logs;
来源：http://kk.9csxet.cn

[Q55] 排名（并列占位）
来源：http://ss.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bm.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://kg.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vr.521024.cn

[Q57] 行号
来源：http://kv.asd995.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mv.muxihuayi.cn

[Q58] 累计求和
来源：http://iv.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jx.bookmarksfly.cn

[Q59] 分组内累计
来源：http://hl.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wk.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://gy.chemitech.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zg.newstarts.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kq.521024.cn

[Q61] 移动平均
来源：http://qj.nszjky.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zs.bookmarksfly.cn

[Q62] 分组占比
来源：http://kx.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://by.nicolike.cn

[Q63] 开启事务
来源：http://br.9csxet.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://of.haigaiapp.cn

[Q64] 提交事务
来源：http://jf.shtwfgs.cn

COMMIT;
来源：http://xe.lnxyls.cn

[Q65] 回滚事务
来源：http://sk.szxytkj.cn

ROLLBACK;
来源：http://xz.nszjky.cn

[Q66] 行锁查询
来源：http://yw.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ls.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://bb.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uq.szxytkj.cn

[Q68] 保存点
来源：http://xc.shxzukj.cn

SAVEPOINT sp1;
来源：http://gr.bjjhwx.cn

ROLLBACK TO sp1;
来源：http://fo.9csxet.cn

[Q69] 查看执行计划
来源：http://tx.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xc.chemitech.net.cn

[Q70] 更新统计信息
来源：http://jo.shtwfgs.cn

ANALYZE TABLE users;
来源：http://xh.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://ye.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oc.shxzskj.cn

[Q72] 查看索引
来源：http://hp.nicolike.cn

SHOW INDEX FROM users;
来源：http://ju.colortex.cn

[Q73] 查看表状态
来源：http://av.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kk.panjiajie.cn

[Q74] 强制使用索引
来源：http://dw.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vn.yuexingan06.cn

[Q75] 日期格式化
来源：http://wl.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://og.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xe.jctech888.com.cn

[Q76] 按天统计
来源：http://py.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ln.asd995.cn

[Q77] 时间加减
来源：http://uu.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mh.shxzukj.cn

[Q78] 当前时间
来源：http://qz.9csxet.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uk.haigaiapp.cn

[Q79] 字符串拼接
来源：http://db.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bf.lnxyls.cn

[Q80] 字符串截取
来源：http://py.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iz.9csxet.cn

[Q81] 字符串替换
来源：http://pg.hnjuh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uc.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://uq.yuexingan06.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mo.hahajie.cn

[Q83] 大小写转换
来源：http://cz.asd995.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yy.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://xo.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://yo.nszjky.cn

[Q85] 数值取整
来源：http://pv.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://om.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://wz.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hj.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://bt.hnjuh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ca.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://ns.huanxung.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mg.lnxyls.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://da.bookmarksfly.cn

[Q89] 判断表是否存在
来源：http://qc.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vw.9csxet.cn

[Q90] 生成序号列
来源：http://hp.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ik.newstarts.cn

================================================================================
来源：http://pv.jianghongdianzi.cn

R. Bash 专题
来源：http://wb.huixiangedu.cn

================================================================================
来源：http://qc.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://hc.bjjhwx.cn

#!/usr/bin/env bash
来源：http://hs.colortex.cn

set -euo pipefail
来源：http://qv.9csxet.cn

[R02] 变量赋值与使用
来源：http://ac.hnjuh.cn

name="Tom"; echo "$name"
来源：http://by.gzmigu.cn

[R03] 只读变量
来源：http://kc.shxzskj.cn

readonly PI=3.14
来源：http://zm.newstarts.cn

[R04] 位置参数
来源：http://ru.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cu.shxzukj.cn

[R05] 参数默认值
来源：http://ly.yuntaijiaju.cn

name="${1:-default}"
来源：http://fj.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://rw.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zd.nszjky.cn

[R07] if 判断文件
来源：http://vt.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bx.yuexingan06.cn

[R08] 数值比较
来源：http://lr.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lf.haigaiapp.cn

[R09] 字符串比较
来源：http://qp.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qi.jctech888.com.cn

[R10] 正则匹配
来源：http://ee.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rh.shxzskj.cn

[R11] case 多分支
来源：http://or.bjjhwx.cn

case "$1" in
来源：http://tq.asd995.cn

start) echo "启动" ;;
来源：http://ik.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://ar.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://tp.asd995.cn

esac
来源：http://pb.9csxet.cn

[R12] for 遍历文件
来源：http://do.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://xq.szxytkj.cn

[R13] for 计数循环
来源：http://fg.szsharing.cn

for i in {1..10}; do echo "$i"; done
来源：http://vb.shxzukj.cn

[R14] C 风格 for
来源：http://th.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xu.shxzukj.cn

[R15] while 逐行读文件
来源：http://bu.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ls.colortex.cn

[R16] until 等待条件
来源：http://pm.nszjky.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fr.huixinmuqiang.cn

[R17] 数组定义与取值
来源：http://ja.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bq.szsharing.cn

[R18] 遍历数组
来源：http://kj.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lm.lnxyls.cn

[R19] 数组长度
来源：http://gx.lnxyls.cn

echo "${#arr[@]}"
来源：http://tx.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://hc.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hj.muxihuayi.cn

[R21] 字符串长度
来源：http://nt.bookmarksfly.cn

echo "${#s}"
来源：http://lq.gzmigu.cn

[R22] 截取子串
来源：http://ek.lnxyls.cn

echo "${s:0:5}"
来源：http://vt.asd995.cn

[R23] 字符串替换
来源：http://rg.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rj.haigaiapp.cn

[R24] 大小写转换
来源：http://id.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xe.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://vq.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yi.521024.cn

[R26] 命令替换
来源：http://xn.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://hi.nszjky.cn

[R27] 算术展开
来源：http://wh.asd995.cn

echo $((1 + 2 * 3))
来源：http://hf.gzmigu.cn

[R28] 浮点运算
来源：http://jx.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://zd.shxzukj.cn

[R29] 定义函数
来源：http://za.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uf.huanxung.cn

[R30] 函数返回状态码
来源：http://di.nszjky.cn

f() { return 0; }; f || echo "失败了"
来源：http://st.bjjhwx.cn

[R31] 局部变量
来源：http://hk.gzmigu.cn

f() { local x=1; echo "$x"; }
来源：http://hr.yuexingan06.cn

[R32] 参数个数校验
来源：http://wj.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tw.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://mt.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tu.haigaiapp.cn

[R34] 退出时清理
来源：http://ef.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sw.szxytkj.cn

[R35] 后台执行并等待
来源：http://ge.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ip.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://zn.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dp.panjiajie.cn

[R37] 把输出赋给变量
来源：http://bt.colortex.cn

files=$(ls -1)
来源：http://mi.lnxyls.cn

[R38] 管道串联
来源：http://xx.hnjuh.cn

cat a.txt | grep -i error | wc -l
来源：http://et.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://ip.szxytkj.cn

cmd > out.log 2>&1
来源：http://qn.asd995.cn

[R40] 追加写日志
来源：http://rw.hahajie.cn

echo "log" >> out.log
来源：http://vb.bookmarksfly.cn

[R41] 丢弃输出
来源：http://zx.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://po.hahajie.cn

[R42] 输入重定向
来源：http://uy.wgjwhj.cn

wc -l < a.txt
来源：http://qd.colortex.cn

[R43] 按名字查找文件
来源：http://pc.newstarts.cn

find . -name "*.log" -type f
来源：http://dg.bjjhwx.cn

[R44] 按修改时间查找
来源：http://ye.gzmigu.cn

find . -mtime -7 -type f
来源：http://cy.muxihuayi.cn

[R45] 批量删除
来源：http://gw.521024.cn

find . -name "*.tmp" -delete
来源：http://zt.newstarts.cn

[R46] 递归替换文件内容
来源：http://sf.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ho.asd995.cn

[R47] sed 单行替换
来源：http://fa.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ux.panjiajie.cn

[R48] awk 取指定列
来源：http://dn.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://du.gzmigu.cn

[R49] awk 带条件
来源：http://zg.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ve.hnjuh.cn

[R50] awk 求和
来源：http://kg.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cz.huixiangedu.cn

[R51] 排序去重取前几
来源：http://zc.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zu.szxytkj.cn

[R52] 统计行数
来源：http://vt.szsharing.cn

wc -l a.txt
来源：http://xj.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://wf.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hl.lnxyls.cn

[R54] 比较两个文件
来源：http://ok.szsharing.cn

diff a.txt b.txt
来源：http://dd.shxzskj.cn

[R55] 压缩与解压
来源：http://mp.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uq.bjjhwx.cn

[R56] 远程拷贝
来源：http://wa.yuexingan06.cn

scp file user@host:/path/
来源：http://uh.hnjuh.cn

[R57] 远程执行命令
来源：http://ho.haigaiapp.cn

ssh user@host 'uptime'
来源：http://qj.bjjhwx.cn

[R58] 下载文件
来源：http://nu.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cm.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://hj.panjiajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wg.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://rw.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gr.asd995.cn

[R61] 磁盘占用
来源：http://um.hahajie.cn

df -h;  du -sh *
来源：http://qx.muxihuayi.cn

[R62] 找最占空间的文件
来源：http://nb.colortex.cn

du -ah . | sort -rh | head -10
来源：http://nv.nszjky.cn

[R63] 内存与进程
来源：http://mn.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://dr.chemitech.net.cn

[R64] 结束进程
来源：http://sj.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://hz.nicolike.cn

[R65] 查看端口占用
来源：http://io.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ve.panjiajie.cn

[R66] 定时任务
来源：http://qz.nicolike.cn

crontab -e;  crontab -l
来源：http://ei.colortex.cn

[R67] 生成随机十六进制串
来源：http://dr.gzmigu.cn

openssl rand -hex 16
来源：http://cx.shtwfgs.cn

[R68] 计算文件校验值
来源：http://gj.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yd.hnjuh.cn

[R69] 生成随机密码
来源：http://ni.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://uf.shtwfgs.cn

[R70] 时间戳与互转
来源：http://ig.nicolike.cn

date +%s;  date -d @1700000000
来源：http://zt.huixiangedu.cn

[R71] 日期格式化
来源：http://qg.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jy.yuexingan06.cn

[R72] 等待端口就绪
来源：http://ra.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wu.nicolike.cn

[R73] 分割大日志
来源：http://tv.nicolike.cn

split -l 1000 big.log part_
来源：http://qq.haigaiapp.cn

[R74] 批量重命名
来源：http://qq.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://as.shxzskj.cn

[R75] 导出环境变量
来源：http://qp.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://gt.nszjky.cn

[R76] 使用临时文件
来源：http://ae.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qj.chemitech.net.cn

[R77] 读取用户输入
来源：http://px.bjjhwx.cn

read -rp "请输入: " ans
来源：http://zv.szsharing.cn

[R78] 交互式菜单
来源：http://me.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://em.521024.cn

[R79] 解析命令行选项
来源：http://ws.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iw.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://as.bjjhwx.cn

time ./run.sh
来源：http://dh.yuntaijiaju.cn

================================================================================
来源：http://jt.shtwfgs.cn

S. C / C++ 专题
来源：http://ww.muxihuayi.cn

================================================================================
来源：http://of.yuntaijiaju.cn

[S01] C：Hello World
来源：http://bf.shxzukj.cn

#include <stdio.h>
来源：http://wz.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kv.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://kl.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://ke.9csxet.cn

[S03] C：读入整数
来源：http://as.shxzskj.cn

int x; scanf("%d", &x);
来源：http://lu.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://qz.huixiangedu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ue.jctech888.com.cn

[S05] C：字符串长度
来源：http://el.521024.cn

strlen(s)
来源：http://rg.newstarts.cn

[S06] C：字符串比较
来源：http://in.hnjuh.cn

strcmp(a, b) == 0
来源：http://ox.newstarts.cn

[S07] C：数组遍历求和
来源：http://aw.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://be.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://um.jctech888.com.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cf.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://lz.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gw.shxzskj.cn

[S10] C：指针与解引用
来源：http://co.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://ol.haigaiapp.cn

[S11] C：逐行读文件
来源：http://hm.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://pa.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rd.lnxyls.cn

fclose(f);
来源：http://vo.haigaiapp.cn

[S12] C：写文件
来源：http://lv.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://my.wgjwhj.cn

[S13] C：宏定义
来源：http://kl.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tu.yuexingan06.cn

[S14] C：枚举
来源：http://he.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://sv.bjjhwx.cn

[S15] C：类型转换
来源：http://hp.huanxung.cn

(double) a / b
来源：http://iw.hnjuh.cn

[S16] C：位操作置位
来源：http://or.huanxung.cn

x |= (1 << 3);
来源：http://ir.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://sj.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ot.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://ey.chemitech.net.cn

int main(int argc, char **argv)
来源：http://ij.szxytkj.cn

[S19] C：快速排序
来源：http://do.521024.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yz.newstarts.cn

[S20] C：二分查找
来源：http://pj.szxytkj.cn


<!-- 参考信息 -->