代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rq.muxihuayi.cn

[Q50] 批量更新
来源：http://ue.shtwfgs.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ik.colortex.cn

[Q51] 用子查询更新
来源：http://nv.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dm.jctech888.com.cn

[Q52] 删除指定行
来源：http://lp.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://wk.chemitech.net.cn

[Q53] 按条件删除
来源：http://rk.panjiajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hb.shxzukj.cn

[Q54] 清空表
来源：http://jv.szsharing.cn

TRUNCATE TABLE logs;
来源：http://xv.wgjwhj.cn

[Q55] 排名（并列占位）
来源：http://ul.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eh.shtwfgs.cn

[Q56] 密集排名（并列不占位）
来源：http://ne.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://it.9csxet.cn

[Q57] 行号
来源：http://nf.nszjky.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tu.nicolike.cn

[Q58] 累计求和
来源：http://mr.nicolike.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lf.huixinmuqiang.cn

[Q59] 分组内累计
来源：http://en.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qs.521024.cn

[Q60] 取上一行 / 下一行
来源：http://qr.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gw.yuntaijiaju.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ny.huanxung.cn

[Q61] 移动平均
来源：http://fl.bjjhwx.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rg.huixiangedu.cn

[Q62] 分组占比
来源：http://yg.hnjuh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ai.chemitech.net.cn

[Q63] 开启事务
来源：http://yo.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cz.9csxet.cn

[Q64] 提交事务
来源：http://ni.jianghongdianzi.cn

COMMIT;
来源：http://qy.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://ph.shxzukj.cn

ROLLBACK;
来源：http://ld.wgjwhj.cn

[Q66] 行锁查询
来源：http://ef.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ie.hnjuh.cn

[Q67] 设置隔离级别
来源：http://vk.nszjky.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://om.shxzskj.cn

[Q68] 保存点
来源：http://kn.szsharing.cn

SAVEPOINT sp1;
来源：http://rq.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://fl.newstarts.cn

[Q69] 查看执行计划
来源：http://wu.newstarts.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yv.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://zy.panjiajie.cn

ANALYZE TABLE users;
来源：http://jq.huanxung.cn

[Q71] 查看建表语句
来源：http://vo.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://si.huixiangedu.cn

[Q72] 查看索引
来源：http://go.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://xh.colortex.cn

[Q73] 查看表状态
来源：http://pj.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cm.colortex.cn

[Q74] 强制使用索引
来源：http://xm.jianghongdianzi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cl.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://lx.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://to.haigaiapp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jq.chemitech.net.cn

[Q76] 按天统计
来源：http://br.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fj.newstarts.cn

[Q77] 时间加减
来源：http://wb.shtwfgs.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vr.521024.cn

[Q78] 当前时间
来源：http://xx.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jp.nicolike.cn

[Q79] 字符串拼接
来源：http://qi.wgjwhj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wz.huixiangedu.cn

[Q80] 字符串截取
来源：http://kq.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rm.lnxyls.cn

[Q81] 字符串替换
来源：http://kw.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qz.yuexingan06.cn

[Q82] 字符长度与字节长度
来源：http://td.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cq.shxzukj.cn

[Q83] 大小写转换
来源：http://is.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sx.huanxung.cn

[Q84] 去除首尾空格
来源：http://an.shxzskj.cn

SELECT TRIM(name) FROM users;
来源：http://zf.asd995.cn

[Q85] 数值取整
来源：http://rf.colortex.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fn.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://at.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pr.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://qb.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ny.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://if.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cn.asd995.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ye.yuntaijiaju.cn

[Q89] 判断表是否存在
来源：http://vj.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xs.haigaiapp.cn

[Q90] 生成序号列
来源：http://cy.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pq.hahajie.cn

================================================================================
来源：http://kb.shtwfgs.cn

R. Bash 专题
来源：http://tf.521024.cn

================================================================================
来源：http://km.newstarts.cn

[R01] shebang 与严格模式
来源：http://fm.lnxyls.cn

#!/usr/bin/env bash
来源：http://rk.huanxung.cn

set -euo pipefail
来源：http://kp.gzmigu.cn

[R02] 变量赋值与使用
来源：http://wb.shtwfgs.cn

name="Tom"; echo "$name"
来源：http://gv.jianghongdianzi.cn

[R03] 只读变量
来源：http://rt.panjiajie.cn

readonly PI=3.14
来源：http://yc.bookmarksfly.cn

[R04] 位置参数
来源：http://ne.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vc.lnxyls.cn

[R05] 参数默认值
来源：http://ye.yuntaijiaju.cn

name="${1:-default}"
来源：http://da.521024.cn

[R06] 判断命令是否存在
来源：http://pk.newstarts.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wx.shxzskj.cn

[R07] if 判断文件
来源：http://gd.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://or.huixiangedu.cn

[R08] 数值比较
来源：http://jv.huanxung.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sw.haigaiapp.cn

[R09] 字符串比较
来源：http://kj.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://om.panjiajie.cn

[R10] 正则匹配
来源：http://ml.521024.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://es.shxzukj.cn

[R11] case 多分支
来源：http://mm.nicolike.cn

case "$1" in
来源：http://aa.shtwfgs.cn

start) echo "启动" ;;
来源：http://ad.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://ti.newstarts.cn

*)     echo "未知命令" ;;
来源：http://zz.jianghongdianzi.cn

esac
来源：http://ic.chemitech.net.cn

[R12] for 遍历文件
来源：http://sw.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://kq.muxihuayi.cn

[R13] for 计数循环
来源：http://qk.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://mu.521024.cn

[R14] C 风格 for
来源：http://ch.haigaiapp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gv.colortex.cn

[R15] while 逐行读文件
来源：http://ec.huanxung.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nn.asd995.cn

[R16] until 等待条件
来源：http://ur.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kb.nszjky.cn

[R17] 数组定义与取值
来源：http://pp.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cu.chemitech.net.cn

[R18] 遍历数组
来源：http://sq.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ej.gzmigu.cn

[R19] 数组长度
来源：http://al.chemitech.net.cn

echo "${#arr[@]}"
来源：http://nh.bookmarksfly.cn

[R20] 关联数组（字典）
来源：http://li.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iz.chemitech.net.cn

[R21] 字符串长度
来源：http://cu.nicolike.cn

echo "${#s}"
来源：http://rj.colortex.cn

[R22] 截取子串
来源：http://jo.szxytkj.cn

echo "${s:0:5}"
来源：http://rv.szsharing.cn

[R23] 字符串替换
来源：http://yw.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xu.chemitech.net.cn

[R24] 大小写转换
来源：http://nf.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://te.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://oa.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tb.colortex.cn

[R26] 命令替换
来源：http://oy.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://gz.newstarts.cn

[R27] 算术展开
来源：http://fa.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://dg.huixiangedu.cn

[R28] 浮点运算
来源：http://hx.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://hl.hnjuh.cn

[R29] 定义函数
来源：http://ew.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hh.yuexingan06.cn

[R30] 函数返回状态码
来源：http://tw.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://nj.bookmarksfly.cn

[R31] 局部变量
来源：http://xo.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://yv.newstarts.cn

[R32] 参数个数校验
来源：http://lh.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nc.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://nk.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fa.shxzukj.cn

[R34] 退出时清理
来源：http://ut.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dp.9csxet.cn

[R35] 后台执行并等待
来源：http://js.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bl.huixinmuqiang.cn

[R36] 并发执行多个任务
来源：http://dj.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ff.muxihuayi.cn

[R37] 把输出赋给变量
来源：http://cp.chemitech.net.cn

files=$(ls -1)
来源：http://vq.yuexingan06.cn

[R38] 管道串联
来源：http://qe.nicolike.cn

cat a.txt | grep -i error | wc -l
来源：http://ma.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://zq.shtwfgs.cn

cmd > out.log 2>&1
来源：http://bl.jianghongdianzi.cn

[R40] 追加写日志
来源：http://fg.jianghongdianzi.cn

echo "log" >> out.log
来源：http://os.9csxet.cn

[R41] 丢弃输出
来源：http://lc.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://xn.yuntaijiaju.cn

[R42] 输入重定向
来源：http://lr.bookmarksfly.cn

wc -l < a.txt
来源：http://ym.bjjhwx.cn

[R43] 按名字查找文件
来源：http://rm.9csxet.cn

find . -name "*.log" -type f
来源：http://bd.lnxyls.cn

[R44] 按修改时间查找
来源：http://ud.gzmigu.cn

find . -mtime -7 -type f
来源：http://xn.huanxung.cn

[R45] 批量删除
来源：http://gc.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://xz.shxzskj.cn

[R46] 递归替换文件内容
来源：http://zk.shxzukj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zh.nszjky.cn

[R47] sed 单行替换
来源：http://rd.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mp.wgjwhj.cn

[R48] awk 取指定列
来源：http://az.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://bu.nicolike.cn

[R49] awk 带条件
来源：http://nq.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hm.shxzukj.cn

[R50] awk 求和
来源：http://nc.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pe.521024.cn

[R51] 排序去重取前几
来源：http://wt.yuexingan06.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rd.panjiajie.cn

[R52] 统计行数
来源：http://zm.chemitech.net.cn

wc -l a.txt
来源：http://pz.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://sy.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wv.jctech888.com.cn

[R54] 比较两个文件
来源：http://iw.huixiangedu.cn

diff a.txt b.txt
来源：http://gg.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://hm.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://af.nszjky.cn

[R56] 远程拷贝
来源：http://eb.9csxet.cn

scp file user@host:/path/
来源：http://yq.haigaiapp.cn

[R57] 远程执行命令
来源：http://tm.jctech888.com.cn

ssh user@host 'uptime'
来源：http://ad.szsharing.cn

[R58] 下载文件
来源：http://as.colortex.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aa.jctech888.com.cn

[R59] 发 POST JSON
来源：http://ea.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ie.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://mj.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vq.lnxyls.cn

[R61] 磁盘占用
来源：http://za.bjjhwx.cn

df -h;  du -sh *
来源：http://ic.newstarts.cn

[R62] 找最占空间的文件
来源：http://jo.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://xh.jianghongdianzi.cn

[R63] 内存与进程
来源：http://tn.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://ko.chemitech.net.cn

[R64] 结束进程
来源：http://os.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://jh.shxzskj.cn

[R65] 查看端口占用
来源：http://tw.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://va.jianghongdianzi.cn

[R66] 定时任务
来源：http://sm.shxzukj.cn

crontab -e;  crontab -l
来源：http://kx.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://ow.nicolike.cn

openssl rand -hex 16
来源：http://ah.hnjuh.cn

[R68] 计算文件校验值
来源：http://fv.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qc.colortex.cn

[R69] 生成随机密码
来源：http://jw.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://ha.gzmigu.cn

[R70] 时间戳与互转
来源：http://ou.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://na.nszjky.cn

[R71] 日期格式化
来源：http://rz.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gc.shxzukj.cn

[R72] 等待端口就绪
来源：http://az.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dz.9csxet.cn

[R73] 分割大日志
来源：http://sq.hahajie.cn

split -l 1000 big.log part_
来源：http://mz.huixinmuqiang.cn

[R74] 批量重命名
来源：http://wk.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vd.muxihuayi.cn

[R75] 导出环境变量
来源：http://hd.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://gj.nicolike.cn

[R76] 使用临时文件
来源：http://fe.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ht.szxytkj.cn

[R77] 读取用户输入
来源：http://he.szxytkj.cn

read -rp "请输入: " ans
来源：http://on.nicolike.cn

[R78] 交互式菜单
来源：http://ju.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://el.nicolike.cn

[R79] 解析命令行选项
来源：http://gx.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qg.wgjwhj.cn

[R80] 查看脚本执行耗时
来源：http://ly.jianghongdianzi.cn

time ./run.sh
来源：http://qg.gzmigu.cn

================================================================================
来源：http://oc.bookmarksfly.cn

S. C / C++ 专题
来源：http://dz.nicolike.cn

================================================================================
来源：http://yh.huixinmuqiang.cn

[S01] C：Hello World
来源：http://hy.nicolike.cn

#include <stdio.h>
来源：http://zh.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ao.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://yd.chemitech.net.cn

int a = 10; printf("%d\n", a);
来源：http://lm.hahajie.cn

[S03] C：读入整数
来源：http://gf.asd995.cn

int x; scanf("%d", &x);
来源：http://ko.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://ju.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zr.wgjwhj.cn

[S05] C：字符串长度
来源：http://dj.hahajie.cn

strlen(s)
来源：http://ob.nicolike.cn

[S06] C：字符串比较
来源：http://rr.gzmigu.cn

strcmp(a, b) == 0
来源：http://cn.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://ct.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pu.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://cy.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xw.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://bz.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bt.bjjhwx.cn

[S10] C：指针与解引用
来源：http://nz.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://qn.colortex.cn

[S11] C：逐行读文件
来源：http://fp.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://pa.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yz.huixinmuqiang.cn

fclose(f);
来源：http://sk.huixinmuqiang.cn

[S12] C：写文件
来源：http://vd.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tq.wgjwhj.cn

[S13] C：宏定义
来源：http://ag.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://me.nszjky.cn

[S14] C：枚举
来源：http://iq.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://xk.wgjwhj.cn

[S15] C：类型转换
来源：http://su.colortex.cn

(double) a / b
来源：http://sf.nicolike.cn

[S16] C：位操作置位
来源：http://lr.haigaiapp.cn

x |= (1 << 3);
来源：http://lh.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://qd.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://df.gzmigu.cn

[S18] C：命令行参数
来源：http://zc.hahajie.cn

int main(int argc, char **argv)
来源：http://mf.bookmarksfly.cn

[S19] C：快速排序
来源：http://xc.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oj.panjiajie.cn

[S20] C：二分查找
来源：http://al.huixiangedu.cn


<!-- 参考信息 -->