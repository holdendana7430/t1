代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zp.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://ux.jctech888.com.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yk.lnxyls.cn

[Q57] 行号
来源：http://ci.hnjuh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gw.yuntaijiaju.cn

[Q58] 累计求和
来源：http://kf.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qt.szsharing.cn

[Q59] 分组内累计
来源：http://hs.colortex.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ba.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://tt.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://md.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ha.huixiangedu.cn

[Q61] 移动平均
来源：http://jm.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dh.jianghongdianzi.cn

[Q62] 分组占比
来源：http://hb.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rj.bookmarksfly.cn

[Q63] 开启事务
来源：http://wz.yuexingan06.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kh.newstarts.cn

[Q64] 提交事务
来源：http://jj.jctech888.com.cn

COMMIT;
来源：http://xm.chemitech.net.cn

[Q65] 回滚事务
来源：http://om.521024.cn

ROLLBACK;
来源：http://fs.gzmigu.cn

[Q66] 行锁查询
来源：http://ye.gzmigu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vw.nicolike.cn

[Q67] 设置隔离级别
来源：http://ce.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ib.9csxet.cn

[Q68] 保存点
来源：http://oa.haigaiapp.cn

SAVEPOINT sp1;
来源：http://uw.hnjuh.cn

ROLLBACK TO sp1;
来源：http://vf.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://vk.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tv.hahajie.cn

[Q70] 更新统计信息
来源：http://sl.asd995.cn

ANALYZE TABLE users;
来源：http://tt.huanxung.cn

[Q71] 查看建表语句
来源：http://tx.haigaiapp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rc.shxzukj.cn

[Q72] 查看索引
来源：http://wo.huanxung.cn

SHOW INDEX FROM users;
来源：http://bm.huixiangedu.cn

[Q73] 查看表状态
来源：http://pz.newstarts.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ae.huanxung.cn

[Q74] 强制使用索引
来源：http://vz.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rn.nszjky.cn

[Q75] 日期格式化
来源：http://ic.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hl.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xm.huixiangedu.cn

[Q76] 按天统计
来源：http://hm.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mo.lnxyls.cn

[Q77] 时间加减
来源：http://oa.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kt.huixinmuqiang.cn

[Q78] 当前时间
来源：http://ma.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mz.jianghongdianzi.cn

[Q79] 字符串拼接
来源：http://yy.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jj.jctech888.com.cn

[Q80] 字符串截取
来源：http://ad.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qq.shtwfgs.cn

[Q81] 字符串替换
来源：http://ia.nszjky.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tc.panjiajie.cn

[Q82] 字符长度与字节长度
来源：http://xb.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wu.panjiajie.cn

[Q83] 大小写转换
来源：http://gf.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yc.jianghongdianzi.cn

[Q84] 去除首尾空格
来源：http://eq.colortex.cn

SELECT TRIM(name) FROM users;
来源：http://bi.9csxet.cn

[Q85] 数值取整
来源：http://qj.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wo.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://xi.wgjwhj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hu.huixiangedu.cn

[Q87] JSON 字段做条件
来源：http://gz.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kz.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://ka.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ix.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nh.huanxung.cn

[Q89] 判断表是否存在
来源：http://el.asd995.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mj.hahajie.cn

[Q90] 生成序号列
来源：http://uw.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://re.shxzukj.cn

================================================================================
来源：http://mb.huanxung.cn

R. Bash 专题
来源：http://vr.shxzukj.cn

================================================================================
来源：http://xr.nszjky.cn

[R01] shebang 与严格模式
来源：http://wr.shxzskj.cn

#!/usr/bin/env bash
来源：http://oc.hnjuh.cn

set -euo pipefail
来源：http://ko.huanxung.cn

[R02] 变量赋值与使用
来源：http://pm.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://cp.chemitech.net.cn

[R03] 只读变量
来源：http://df.newstarts.cn

readonly PI=3.14
来源：http://jn.hahajie.cn

[R04] 位置参数
来源：http://nz.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lg.yuntaijiaju.cn

[R05] 参数默认值
来源：http://zb.muxihuayi.cn

name="${1:-default}"
来源：http://gk.hahajie.cn

[R06] 判断命令是否存在
来源：http://ih.bjjhwx.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hn.yuexingan06.cn

[R07] if 判断文件
来源：http://hj.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nd.szxytkj.cn

[R08] 数值比较
来源：http://hy.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kw.jctech888.com.cn

[R09] 字符串比较
来源：http://kn.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wq.9csxet.cn

[R10] 正则匹配
来源：http://yo.lnxyls.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aw.huixiangedu.cn

[R11] case 多分支
来源：http://tf.szxytkj.cn

case "$1" in
来源：http://xb.yuexingan06.cn

start) echo "启动" ;;
来源：http://iu.szsharing.cn

stop)  echo "停止" ;;
来源：http://he.muxihuayi.cn

*)     echo "未知命令" ;;
来源：http://nm.szxytkj.cn

esac
来源：http://wj.hahajie.cn

[R12] for 遍历文件
来源：http://hc.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://vn.521024.cn

[R13] for 计数循环
来源：http://vm.asd995.cn

for i in {1..10}; do echo "$i"; done
来源：http://fk.huanxung.cn

[R14] C 风格 for
来源：http://dj.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ew.szxytkj.cn

[R15] while 逐行读文件
来源：http://jp.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zn.colortex.cn

[R16] until 等待条件
来源：http://gc.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fw.colortex.cn

[R17] 数组定义与取值
来源：http://lc.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pw.haigaiapp.cn

[R18] 遍历数组
来源：http://lh.colortex.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uo.yuntaijiaju.cn

[R19] 数组长度
来源：http://ue.szsharing.cn

echo "${#arr[@]}"
来源：http://jz.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://uc.bookmarksfly.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://or.jctech888.com.cn

[R21] 字符串长度
来源：http://ez.huixiangedu.cn

echo "${#s}"
来源：http://po.nszjky.cn

[R22] 截取子串
来源：http://ha.shtwfgs.cn

echo "${s:0:5}"
来源：http://iy.jianghongdianzi.cn

[R23] 字符串替换
来源：http://us.hahajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iz.colortex.cn

[R24] 大小写转换
来源：http://lo.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kw.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://st.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qs.bjjhwx.cn

[R26] 命令替换
来源：http://bo.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://ml.gzmigu.cn

[R27] 算术展开
来源：http://ei.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://ok.colortex.cn

[R28] 浮点运算
来源：http://rk.asd995.cn

echo "scale=2; 10/3" | bc
来源：http://wb.yuntaijiaju.cn

[R29] 定义函数
来源：http://rq.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://za.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://xt.szxytkj.cn

f() { return 0; }; f || echo "失败了"
来源：http://ju.gzmigu.cn

[R31] 局部变量
来源：http://dy.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://dz.szsharing.cn

[R32] 参数个数校验
来源：http://az.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://by.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://gc.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sr.shtwfgs.cn

[R34] 退出时清理
来源：http://ca.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ic.jctech888.com.cn

[R35] 后台执行并等待
来源：http://ng.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sy.hnjuh.cn

[R36] 并发执行多个任务
来源：http://on.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zf.nicolike.cn

[R37] 把输出赋给变量
来源：http://kv.szxytkj.cn

files=$(ls -1)
来源：http://zp.521024.cn

[R38] 管道串联
来源：http://vy.szxytkj.cn

cat a.txt | grep -i error | wc -l
来源：http://vg.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://zm.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://lk.9csxet.cn

[R40] 追加写日志
来源：http://il.gzmigu.cn

echo "log" >> out.log
来源：http://aw.huixiangedu.cn

[R41] 丢弃输出
来源：http://fr.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://ka.yuexingan06.cn

[R42] 输入重定向
来源：http://ij.nszjky.cn

wc -l < a.txt
来源：http://gb.9csxet.cn

[R43] 按名字查找文件
来源：http://zt.muxihuayi.cn

find . -name "*.log" -type f
来源：http://jq.szsharing.cn

[R44] 按修改时间查找
来源：http://qi.huixinmuqiang.cn

find . -mtime -7 -type f
来源：http://ny.bjjhwx.cn

[R45] 批量删除
来源：http://yy.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://gk.newstarts.cn

[R46] 递归替换文件内容
来源：http://tr.muxihuayi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gz.szsharing.cn

[R47] sed 单行替换
来源：http://hs.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fd.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://dj.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://tn.szsharing.cn

[R49] awk 带条件
来源：http://te.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gi.szxytkj.cn

[R50] awk 求和
来源：http://cr.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sp.szxytkj.cn

[R51] 排序去重取前几
来源：http://nt.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lo.shxzskj.cn

[R52] 统计行数
来源：http://up.wgjwhj.cn

wc -l a.txt
来源：http://me.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://ic.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xc.nszjky.cn

[R54] 比较两个文件
来源：http://iq.haigaiapp.cn

diff a.txt b.txt
来源：http://pi.lnxyls.cn

[R55] 压缩与解压
来源：http://sr.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cz.muxihuayi.cn

[R56] 远程拷贝
来源：http://oe.szsharing.cn

scp file user@host:/path/
来源：http://mz.521024.cn

[R57] 远程执行命令
来源：http://zc.hnjuh.cn

ssh user@host 'uptime'
来源：http://bt.yuexingan06.cn

[R58] 下载文件
来源：http://pe.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lz.chemitech.net.cn

[R59] 发 POST JSON
来源：http://zd.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://do.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://mk.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pw.huixiangedu.cn

[R61] 磁盘占用
来源：http://ic.huanxung.cn

df -h;  du -sh *
来源：http://nj.9csxet.cn

[R62] 找最占空间的文件
来源：http://yy.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://tn.szsharing.cn

[R63] 内存与进程
来源：http://nk.panjiajie.cn

free -h;  ps aux | grep nginx
来源：http://ba.bjjhwx.cn

[R64] 结束进程
来源：http://jl.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://qc.nicolike.cn

[R65] 查看端口占用
来源：http://cs.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qw.huixiangedu.cn

[R66] 定时任务
来源：http://wb.newstarts.cn

crontab -e;  crontab -l
来源：http://ja.521024.cn

[R67] 生成随机十六进制串
来源：http://gx.panjiajie.cn

openssl rand -hex 16
来源：http://ck.9csxet.cn

[R68] 计算文件校验值
来源：http://wf.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yi.nszjky.cn

[R69] 生成随机密码
来源：http://zv.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://ls.newstarts.cn

[R70] 时间戳与互转
来源：http://ra.szsharing.cn

date +%s;  date -d @1700000000
来源：http://uy.shtwfgs.cn

[R71] 日期格式化
来源：http://dr.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://es.haigaiapp.cn

[R72] 等待端口就绪
来源：http://fq.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ak.bookmarksfly.cn

[R73] 分割大日志
来源：http://an.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://iv.521024.cn

[R74] 批量重命名
来源：http://il.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qs.asd995.cn

[R75] 导出环境变量
来源：http://pu.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://ye.huanxung.cn

[R76] 使用临时文件
来源：http://wr.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sd.szsharing.cn

[R77] 读取用户输入
来源：http://rm.shxzukj.cn

read -rp "请输入: " ans
来源：http://tc.9csxet.cn

[R78] 交互式菜单
来源：http://yi.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ui.jctech888.com.cn

[R79] 解析命令行选项
来源：http://lt.9csxet.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ek.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://hf.shxzukj.cn

time ./run.sh
来源：http://ul.9csxet.cn

================================================================================
来源：http://tz.shxzukj.cn

S. C / C++ 专题
来源：http://qf.jianghongdianzi.cn

================================================================================
来源：http://rh.szxytkj.cn

[S01] C：Hello World
来源：http://qi.huixiangedu.cn

#include <stdio.h>
来源：http://qe.521024.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sa.asd995.cn

[S02] C：变量与格式化输出
来源：http://ne.wgjwhj.cn

int a = 10; printf("%d\n", a);
来源：http://ex.panjiajie.cn

[S03] C：读入整数
来源：http://fe.shxzukj.cn

int x; scanf("%d", &x);
来源：http://yi.chemitech.net.cn

[S04] C：字符串复制
来源：http://eb.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nw.szsharing.cn

[S05] C：字符串长度
来源：http://ru.yuexingan06.cn

strlen(s)
来源：http://tc.yuexingan06.cn

[S06] C：字符串比较
来源：http://df.nicolike.cn

strcmp(a, b) == 0
来源：http://oy.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://it.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fd.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://rd.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ew.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://nv.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://do.szsharing.cn

[S10] C：指针与解引用
来源：http://sh.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://pi.yuexingan06.cn

[S11] C：逐行读文件
来源：http://tk.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://hu.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://if.jctech888.com.cn

fclose(f);
来源：http://ei.muxihuayi.cn

[S12] C：写文件
来源：http://hr.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rw.hahajie.cn

[S13] C：宏定义
来源：http://zx.newstarts.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hn.huanxung.cn

[S14] C：枚举
来源：http://tt.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://uf.huanxung.cn

[S15] C：类型转换
来源：http://st.yuntaijiaju.cn

(double) a / b
来源：http://xv.yuexingan06.cn

[S16] C：位操作置位
来源：http://wp.szxytkj.cn

x |= (1 << 3);
来源：http://qj.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://sk.muxihuayi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cu.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://bu.szsharing.cn

int main(int argc, char **argv)
来源：http://tm.asd995.cn

[S19] C：快速排序
来源：http://mm.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ud.szxytkj.cn

[S20] C：二分查找
来源：http://hj.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hd.hahajie.cn

[S21] C：字符类别判断
来源：http://nk.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dp.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://dt.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fl.hnjuh.cn

[S23] C：随机数
来源：http://ft.huixinmuqiang.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wg.521024.cn

[S24] C：获取本地时间
来源：http://nf.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vn.newstarts.cn

[S25] C：内存拷贝
来源：http://es.521024.cn

memcpy(dst, src, n);
来源：http://hk.nicolike.cn

[S26] C：内存清零
来源：http://hj.newstarts.cn


<!-- 参考信息 -->