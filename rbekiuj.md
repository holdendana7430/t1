代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oa.jctech888.com.cn

[Q54] 清空表
来源：http://oo.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://xq.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://iq.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dt.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://ql.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mn.nszjky.cn

[Q57] 行号
来源：http://oe.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uj.hnjuh.cn

[Q58] 累计求和
来源：http://av.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xs.9csxet.cn

[Q59] 分组内累计
来源：http://lq.521024.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gk.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://hm.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kw.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pm.newstarts.cn

[Q61] 移动平均
来源：http://mg.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ti.yuexingan06.cn

[Q62] 分组占比
来源：http://wn.colortex.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hu.huixiangedu.cn

[Q63] 开启事务
来源：http://sh.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pr.asd995.cn

[Q64] 提交事务
来源：http://zf.bookmarksfly.cn

COMMIT;
来源：http://li.yuexingan06.cn

[Q65] 回滚事务
来源：http://ml.colortex.cn

ROLLBACK;
来源：http://re.bjjhwx.cn

[Q66] 行锁查询
来源：http://iv.asd995.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gh.hahajie.cn

[Q67] 设置隔离级别
来源：http://qp.huixiangedu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xa.wgjwhj.cn

[Q68] 保存点
来源：http://ud.szsharing.cn

SAVEPOINT sp1;
来源：http://ih.huixinmuqiang.cn

ROLLBACK TO sp1;
来源：http://bf.9csxet.cn

[Q69] 查看执行计划
来源：http://vz.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ek.shxzskj.cn

[Q70] 更新统计信息
来源：http://bp.chemitech.net.cn

ANALYZE TABLE users;
来源：http://kd.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://ao.521024.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hf.huanxung.cn

[Q72] 查看索引
来源：http://nq.chemitech.net.cn

SHOW INDEX FROM users;
来源：http://mx.muxihuayi.cn

[Q73] 查看表状态
来源：http://wj.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nb.yuexingan06.cn

[Q74] 强制使用索引
来源：http://pb.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://os.huanxung.cn

[Q75] 日期格式化
来源：http://eq.huixiangedu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sk.szxytkj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ho.yuexingan06.cn

[Q76] 按天统计
来源：http://te.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gx.yuntaijiaju.cn

[Q77] 时间加减
来源：http://is.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wa.nicolike.cn

[Q78] 当前时间
来源：http://vo.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jv.asd995.cn

[Q79] 字符串拼接
来源：http://ns.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pe.muxihuayi.cn

[Q80] 字符串截取
来源：http://qr.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cc.bookmarksfly.cn

[Q81] 字符串替换
来源：http://xt.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hr.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://fy.szsharing.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ar.chemitech.net.cn

[Q83] 大小写转换
来源：http://vb.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vk.jianghongdianzi.cn

[Q84] 去除首尾空格
来源：http://ll.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://vm.jianghongdianzi.cn

[Q85] 数值取整
来源：http://wq.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://df.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://je.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yk.huanxung.cn

[Q87] JSON 字段做条件
来源：http://re.bookmarksfly.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wk.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://wz.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hj.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://es.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://if.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fi.hahajie.cn

[Q90] 生成序号列
来源：http://cn.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ma.newstarts.cn

================================================================================
来源：http://mg.9csxet.cn

R. Bash 专题
来源：http://go.nicolike.cn

================================================================================
来源：http://eg.shxzskj.cn

[R01] shebang 与严格模式
来源：http://zc.nszjky.cn

#!/usr/bin/env bash
来源：http://xx.nicolike.cn

set -euo pipefail
来源：http://hz.gzmigu.cn

[R02] 变量赋值与使用
来源：http://dd.bookmarksfly.cn

name="Tom"; echo "$name"
来源：http://bq.muxihuayi.cn

[R03] 只读变量
来源：http://go.lnxyls.cn

readonly PI=3.14
来源：http://lu.lnxyls.cn

[R04] 位置参数
来源：http://sn.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vw.yuexingan06.cn

[R05] 参数默认值
来源：http://fk.chemitech.net.cn

name="${1:-default}"
来源：http://ps.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://ze.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ng.muxihuayi.cn

[R07] if 判断文件
来源：http://hc.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ei.wgjwhj.cn

[R08] 数值比较
来源：http://ee.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vw.muxihuayi.cn

[R09] 字符串比较
来源：http://hu.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mu.hahajie.cn

[R10] 正则匹配
来源：http://zf.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qh.muxihuayi.cn

[R11] case 多分支
来源：http://bl.9csxet.cn

case "$1" in
来源：http://ga.lnxyls.cn

start) echo "启动" ;;
来源：http://bb.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://gm.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://xl.jctech888.com.cn

esac
来源：http://us.newstarts.cn

[R12] for 遍历文件
来源：http://xc.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://rd.lnxyls.cn

[R13] for 计数循环
来源：http://rr.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://fu.szsharing.cn

[R14] C 风格 for
来源：http://im.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wn.hahajie.cn

[R15] while 逐行读文件
来源：http://ci.bjjhwx.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bc.hnjuh.cn

[R16] until 等待条件
来源：http://cs.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yr.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://ht.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bd.jianghongdianzi.cn

[R18] 遍历数组
来源：http://qr.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ct.yuexingan06.cn

[R19] 数组长度
来源：http://av.huixiangedu.cn

echo "${#arr[@]}"
来源：http://dc.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://at.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zr.bookmarksfly.cn

[R21] 字符串长度
来源：http://le.521024.cn

echo "${#s}"
来源：http://ue.huixinmuqiang.cn

[R22] 截取子串
来源：http://rg.muxihuayi.cn

echo "${s:0:5}"
来源：http://ew.jianghongdianzi.cn

[R23] 字符串替换
来源：http://lf.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pr.huixiangedu.cn

[R24] 大小写转换
来源：http://ai.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://iv.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://mr.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dg.hahajie.cn

[R26] 命令替换
来源：http://tz.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://na.shtwfgs.cn

[R27] 算术展开
来源：http://vy.nicolike.cn

echo $((1 + 2 * 3))
来源：http://ii.muxihuayi.cn

[R28] 浮点运算
来源：http://ou.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://vf.huixinmuqiang.cn

[R29] 定义函数
来源：http://iw.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zu.shxzskj.cn

[R30] 函数返回状态码
来源：http://ro.lnxyls.cn

f() { return 0; }; f || echo "失败了"
来源：http://ui.hnjuh.cn

[R31] 局部变量
来源：http://zg.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://ji.nszjky.cn

[R32] 参数个数校验
来源：http://dj.yuexingan06.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zd.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://jj.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lo.szsharing.cn

[R34] 退出时清理
来源：http://sv.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gt.9csxet.cn

[R35] 后台执行并等待
来源：http://ek.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nd.panjiajie.cn

[R36] 并发执行多个任务
来源：http://km.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lh.panjiajie.cn

[R37] 把输出赋给变量
来源：http://ti.asd995.cn

files=$(ls -1)
来源：http://nk.bookmarksfly.cn

[R38] 管道串联
来源：http://mk.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://mq.shtwfgs.cn

[R39] 重定向标准输出与错误
来源：http://on.jctech888.com.cn

cmd > out.log 2>&1
来源：http://an.jctech888.com.cn

[R40] 追加写日志
来源：http://vo.bjjhwx.cn

echo "log" >> out.log
来源：http://gq.szxytkj.cn

[R41] 丢弃输出
来源：http://yw.521024.cn

cmd >/dev/null 2>&1
来源：http://jw.panjiajie.cn

[R42] 输入重定向
来源：http://uv.jianghongdianzi.cn

wc -l < a.txt
来源：http://cv.nszjky.cn

[R43] 按名字查找文件
来源：http://sg.panjiajie.cn

find . -name "*.log" -type f
来源：http://ho.bjjhwx.cn

[R44] 按修改时间查找
来源：http://rx.nicolike.cn

find . -mtime -7 -type f
来源：http://cv.nszjky.cn

[R45] 批量删除
来源：http://ms.nszjky.cn

find . -name "*.tmp" -delete
来源：http://yz.nicolike.cn

[R46] 递归替换文件内容
来源：http://zd.shtwfgs.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lr.newstarts.cn

[R47] sed 单行替换
来源：http://wr.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tx.nszjky.cn

[R48] awk 取指定列
来源：http://bx.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://db.jianghongdianzi.cn

[R49] awk 带条件
来源：http://ln.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://es.shxzskj.cn

[R50] awk 求和
来源：http://ua.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fu.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://wk.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ci.huanxung.cn

[R52] 统计行数
来源：http://od.nicolike.cn

wc -l a.txt
来源：http://jw.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://qi.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qd.yuexingan06.cn

[R54] 比较两个文件
来源：http://no.haigaiapp.cn

diff a.txt b.txt
来源：http://be.shxzskj.cn

[R55] 压缩与解压
来源：http://sk.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://th.bookmarksfly.cn

[R56] 远程拷贝
来源：http://ph.bookmarksfly.cn

scp file user@host:/path/
来源：http://jx.shtwfgs.cn

[R57] 远程执行命令
来源：http://gb.newstarts.cn

ssh user@host 'uptime'
来源：http://oc.9csxet.cn

[R58] 下载文件
来源：http://mw.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hl.asd995.cn

[R59] 发 POST JSON
来源：http://pr.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cn.521024.cn

[R60] 只看 HTTP 状态码
来源：http://gv.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uu.bookmarksfly.cn

[R61] 磁盘占用
来源：http://fk.asd995.cn

df -h;  du -sh *
来源：http://vr.lnxyls.cn

[R62] 找最占空间的文件
来源：http://cn.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://gn.hahajie.cn

[R63] 内存与进程
来源：http://qo.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://pb.hahajie.cn

[R64] 结束进程
来源：http://vp.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://bi.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://ow.huixinmuqiang.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://su.szsharing.cn

[R66] 定时任务
来源：http://np.chemitech.net.cn

crontab -e;  crontab -l
来源：http://lv.haigaiapp.cn

[R67] 生成随机十六进制串
来源：http://ac.9csxet.cn

openssl rand -hex 16
来源：http://od.9csxet.cn

[R68] 计算文件校验值
来源：http://kw.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ay.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://cb.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://ld.9csxet.cn

[R70] 时间戳与互转
来源：http://al.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://xs.newstarts.cn

[R71] 日期格式化
来源：http://vu.jianghongdianzi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qh.szxytkj.cn

[R72] 等待端口就绪
来源：http://rc.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kw.bjjhwx.cn

[R73] 分割大日志
来源：http://fv.9csxet.cn

split -l 1000 big.log part_
来源：http://wg.nszjky.cn

[R74] 批量重命名
来源：http://nc.newstarts.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ps.muxihuayi.cn

[R75] 导出环境变量
来源：http://xq.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://co.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://rm.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ip.colortex.cn

[R77] 读取用户输入
来源：http://ff.colortex.cn

read -rp "请输入: " ans
来源：http://ib.panjiajie.cn

[R78] 交互式菜单
来源：http://mt.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wo.wgjwhj.cn

[R79] 解析命令行选项
来源：http://lh.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rx.asd995.cn

[R80] 查看脚本执行耗时
来源：http://xq.nszjky.cn

time ./run.sh
来源：http://yv.shxzukj.cn

================================================================================
来源：http://uh.szxytkj.cn

S. C / C++ 专题
来源：http://zs.huanxung.cn

================================================================================
来源：http://re.nszjky.cn

[S01] C：Hello World
来源：http://uh.wgjwhj.cn

#include <stdio.h>
来源：http://bu.521024.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ar.shtwfgs.cn

[S02] C：变量与格式化输出
来源：http://ee.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://ej.muxihuayi.cn

[S03] C：读入整数
来源：http://or.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://th.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://lg.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pl.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://ss.yuntaijiaju.cn

strlen(s)
来源：http://td.newstarts.cn

[S06] C：字符串比较
来源：http://za.muxihuayi.cn

strcmp(a, b) == 0
来源：http://cg.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://zp.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jj.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://ts.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fb.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://cn.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cy.shxzskj.cn

[S10] C：指针与解引用
来源：http://cq.shxzukj.cn

int *p = &a;  *p = 5;
来源：http://tv.nicolike.cn

[S11] C：逐行读文件
来源：http://bv.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://ht.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://my.hahajie.cn

fclose(f);
来源：http://jz.haigaiapp.cn

[S12] C：写文件
来源：http://ik.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yt.huanxung.cn

[S13] C：宏定义
来源：http://ol.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ot.huixinmuqiang.cn

[S14] C：枚举
来源：http://et.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://uo.nicolike.cn

[S15] C：类型转换
来源：http://iu.shxzukj.cn

(double) a / b
来源：http://bf.muxihuayi.cn

[S16] C：位操作置位
来源：http://ra.521024.cn

x |= (1 << 3);
来源：http://gc.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://hr.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wh.huixiangedu.cn

[S18] C：命令行参数
来源：http://dm.asd995.cn

int main(int argc, char **argv)
来源：http://yh.lnxyls.cn

[S19] C：快速排序
来源：http://qv.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gf.yuexingan06.cn

[S20] C：二分查找
来源：http://ta.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ta.nicolike.cn

[S21] C：字符类别判断
来源：http://ht.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://so.shxzskj.cn

[S22] C：字符串转数字
来源：http://uf.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ct.newstarts.cn

[S23] C：随机数
来源：http://yb.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sk.jctech888.com.cn

[S24] C：获取本地时间
来源：http://lx.muxihuayi.cn


<!-- 参考信息 -->