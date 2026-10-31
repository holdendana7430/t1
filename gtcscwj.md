代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://te.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://sv.wgjwhj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://it.haigaiapp.cn

[Q57] 行号
来源：http://cf.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nj.shtwfgs.cn

[Q58] 累计求和
来源：http://mp.gzmigu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jo.panjiajie.cn

[Q59] 分组内累计
来源：http://wy.huanxung.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://eo.chemitech.net.cn

[Q60] 取上一行 / 下一行
来源：http://lh.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bh.nszjky.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gr.shxzukj.cn

[Q61] 移动平均
来源：http://yo.shtwfgs.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qi.wgjwhj.cn

[Q62] 分组占比
来源：http://zb.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://et.wgjwhj.cn

[Q63] 开启事务
来源：http://kx.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uo.szxytkj.cn

[Q64] 提交事务
来源：http://tf.jctech888.com.cn

COMMIT;
来源：http://wr.chemitech.net.cn

[Q65] 回滚事务
来源：http://kn.nicolike.cn

ROLLBACK;
来源：http://ue.nicolike.cn

[Q66] 行锁查询
来源：http://im.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fn.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://oc.gzmigu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dt.nicolike.cn

[Q68] 保存点
来源：http://mj.bjjhwx.cn

SAVEPOINT sp1;
来源：http://ko.szxytkj.cn

ROLLBACK TO sp1;
来源：http://pi.bjjhwx.cn

[Q69] 查看执行计划
来源：http://aj.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ko.colortex.cn

[Q70] 更新统计信息
来源：http://cp.colortex.cn

ANALYZE TABLE users;
来源：http://tw.nicolike.cn

[Q71] 查看建表语句
来源：http://fl.panjiajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tu.newstarts.cn

[Q72] 查看索引
来源：http://vl.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://qt.lnxyls.cn

[Q73] 查看表状态
来源：http://wu.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://em.lnxyls.cn

[Q74] 强制使用索引
来源：http://hz.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qq.newstarts.cn

[Q75] 日期格式化
来源：http://qp.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vp.shxzukj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gt.hnjuh.cn

[Q76] 按天统计
来源：http://bg.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qu.jianghongdianzi.cn

[Q77] 时间加减
来源：http://gr.huixiangedu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://je.lnxyls.cn

[Q78] 当前时间
来源：http://ip.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ax.hahajie.cn

[Q79] 字符串拼接
来源：http://wr.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ja.shtwfgs.cn

[Q80] 字符串截取
来源：http://st.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://em.bjjhwx.cn

[Q81] 字符串替换
来源：http://bi.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gb.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://wh.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://he.lnxyls.cn

[Q83] 大小写转换
来源：http://to.shtwfgs.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ou.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://rn.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://wd.colortex.cn

[Q85] 数值取整
来源：http://av.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xx.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://ri.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://or.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://xo.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bf.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://pe.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oq.szsharing.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://re.yuntaijiaju.cn

[Q89] 判断表是否存在
来源：http://wm.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ae.jctech888.com.cn

[Q90] 生成序号列
来源：http://hh.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wn.yuntaijiaju.cn

================================================================================
来源：http://to.shxzskj.cn

R. Bash 专题
来源：http://rz.newstarts.cn

================================================================================
来源：http://gt.szsharing.cn

[R01] shebang 与严格模式
来源：http://cv.haigaiapp.cn

#!/usr/bin/env bash
来源：http://tj.bjjhwx.cn

set -euo pipefail
来源：http://in.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://jk.szsharing.cn

name="Tom"; echo "$name"
来源：http://dd.asd995.cn

[R03] 只读变量
来源：http://bb.shxzukj.cn

readonly PI=3.14
来源：http://ql.jctech888.com.cn

[R04] 位置参数
来源：http://re.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ya.nszjky.cn

[R05] 参数默认值
来源：http://xc.shxzskj.cn

name="${1:-default}"
来源：http://gs.panjiajie.cn

[R06] 判断命令是否存在
来源：http://zn.gzmigu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hm.yuexingan06.cn

[R07] if 判断文件
来源：http://uw.jianghongdianzi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://am.jctech888.com.cn

[R08] 数值比较
来源：http://nr.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jq.521024.cn

[R09] 字符串比较
来源：http://ek.bookmarksfly.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rz.huixiangedu.cn

[R10] 正则匹配
来源：http://iz.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jv.lnxyls.cn

[R11] case 多分支
来源：http://qo.yuntaijiaju.cn

case "$1" in
来源：http://pq.nszjky.cn

start) echo "启动" ;;
来源：http://ry.haigaiapp.cn

stop)  echo "停止" ;;
来源：http://xj.9csxet.cn

*)     echo "未知命令" ;;
来源：http://vs.huixinmuqiang.cn

esac
来源：http://kj.bjjhwx.cn

[R12] for 遍历文件
来源：http://gw.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://bd.gzmigu.cn

[R13] for 计数循环
来源：http://mf.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://ra.521024.cn

[R14] C 风格 for
来源：http://ek.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wx.lnxyls.cn

[R15] while 逐行读文件
来源：http://yc.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://na.nszjky.cn

[R16] until 等待条件
来源：http://yn.newstarts.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nc.521024.cn

[R17] 数组定义与取值
来源：http://vj.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://id.panjiajie.cn

[R18] 遍历数组
来源：http://sw.9csxet.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ls.huixinmuqiang.cn

[R19] 数组长度
来源：http://qq.yuexingan06.cn

echo "${#arr[@]}"
来源：http://ly.nszjky.cn

[R20] 关联数组（字典）
来源：http://sy.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zm.huanxung.cn

[R21] 字符串长度
来源：http://nv.nszjky.cn

echo "${#s}"
来源：http://if.521024.cn

[R22] 截取子串
来源：http://xi.nszjky.cn

echo "${s:0:5}"
来源：http://yz.shxzskj.cn

[R23] 字符串替换
来源：http://ab.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ei.shxzskj.cn

[R24] 大小写转换
来源：http://un.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ur.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://jl.shtwfgs.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ea.yuexingan06.cn

[R26] 命令替换
来源：http://fj.asd995.cn

now=$(date +%F); echo "$now"
来源：http://il.huixinmuqiang.cn

[R27] 算术展开
来源：http://bk.huixinmuqiang.cn

echo $((1 + 2 * 3))
来源：http://jo.yuntaijiaju.cn

[R28] 浮点运算
来源：http://rv.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://xh.yuntaijiaju.cn

[R29] 定义函数
来源：http://np.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kl.hnjuh.cn

[R30] 函数返回状态码
来源：http://do.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://tj.9csxet.cn

[R31] 局部变量
来源：http://kb.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://gk.nicolike.cn

[R32] 参数个数校验
来源：http://fl.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bt.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://fu.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ev.chemitech.net.cn

[R34] 退出时清理
来源：http://ub.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ln.hnjuh.cn

[R35] 后台执行并等待
来源：http://wn.hnjuh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gg.panjiajie.cn

[R36] 并发执行多个任务
来源：http://id.nszjky.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rc.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://uw.huanxung.cn

files=$(ls -1)
来源：http://gf.shtwfgs.cn

[R38] 管道串联
来源：http://pd.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://ym.jctech888.com.cn

[R39] 重定向标准输出与错误
来源：http://ln.muxihuayi.cn

cmd > out.log 2>&1
来源：http://dz.shxzskj.cn

[R40] 追加写日志
来源：http://ys.bookmarksfly.cn

echo "log" >> out.log
来源：http://wm.colortex.cn

[R41] 丢弃输出
来源：http://tx.nicolike.cn

cmd >/dev/null 2>&1
来源：http://nu.shxzukj.cn

[R42] 输入重定向
来源：http://mf.huixinmuqiang.cn

wc -l < a.txt
来源：http://ir.521024.cn

[R43] 按名字查找文件
来源：http://gv.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://ku.jctech888.com.cn

[R44] 按修改时间查找
来源：http://cr.shxzukj.cn

find . -mtime -7 -type f
来源：http://hz.szxytkj.cn

[R45] 批量删除
来源：http://of.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://fi.asd995.cn

[R46] 递归替换文件内容
来源：http://kl.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ei.nicolike.cn

[R47] sed 单行替换
来源：http://gb.shxzskj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pa.colortex.cn

[R48] awk 取指定列
来源：http://ob.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://ix.521024.cn

[R49] awk 带条件
来源：http://hj.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sd.yuexingan06.cn

[R50] awk 求和
来源：http://qx.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bq.nszjky.cn

[R51] 排序去重取前几
来源：http://th.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sr.shtwfgs.cn

[R52] 统计行数
来源：http://tt.huixiangedu.cn

wc -l a.txt
来源：http://lv.nszjky.cn

[R53] 查看文件头与实时尾
来源：http://ix.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rs.yuexingan06.cn

[R54] 比较两个文件
来源：http://ni.hahajie.cn

diff a.txt b.txt
来源：http://xw.nszjky.cn

[R55] 压缩与解压
来源：http://uf.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ik.muxihuayi.cn

[R56] 远程拷贝
来源：http://yv.asd995.cn

scp file user@host:/path/
来源：http://dd.shxzskj.cn

[R57] 远程执行命令
来源：http://mb.newstarts.cn

ssh user@host 'uptime'
来源：http://em.hnjuh.cn

[R58] 下载文件
来源：http://xf.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yw.hnjuh.cn

[R59] 发 POST JSON
来源：http://gg.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kj.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://hq.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ot.chemitech.net.cn

[R61] 磁盘占用
来源：http://ut.hahajie.cn

df -h;  du -sh *
来源：http://hn.muxihuayi.cn

[R62] 找最占空间的文件
来源：http://by.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://bs.hnjuh.cn

[R63] 内存与进程
来源：http://ze.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://oy.yuntaijiaju.cn

[R64] 结束进程
来源：http://xm.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://qz.colortex.cn

[R65] 查看端口占用
来源：http://ha.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qo.huixiangedu.cn

[R66] 定时任务
来源：http://da.9csxet.cn

crontab -e;  crontab -l
来源：http://lg.asd995.cn

[R67] 生成随机十六进制串
来源：http://ks.colortex.cn

openssl rand -hex 16
来源：http://kk.colortex.cn

[R68] 计算文件校验值
来源：http://up.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wx.hnjuh.cn

[R69] 生成随机密码
来源：http://sf.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://hf.asd995.cn

[R70] 时间戳与互转
来源：http://ze.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://no.shxzskj.cn

[R71] 日期格式化
来源：http://cb.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://my.jctech888.com.cn

[R72] 等待端口就绪
来源：http://be.jianghongdianzi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tq.jctech888.com.cn

[R73] 分割大日志
来源：http://ne.colortex.cn

split -l 1000 big.log part_
来源：http://hq.jctech888.com.cn

[R74] 批量重命名
来源：http://su.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iz.colortex.cn

[R75] 导出环境变量
来源：http://vp.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://ho.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://gx.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vj.nszjky.cn

[R77] 读取用户输入
来源：http://ev.huixiangedu.cn

read -rp "请输入: " ans
来源：http://ev.shxzskj.cn

[R78] 交互式菜单
来源：http://be.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fy.jctech888.com.cn

[R79] 解析命令行选项
来源：http://xf.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vc.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://qv.521024.cn

time ./run.sh
来源：http://by.lnxyls.cn

================================================================================
来源：http://gj.wgjwhj.cn

S. C / C++ 专题
来源：http://qz.hahajie.cn

================================================================================
来源：http://xl.newstarts.cn

[S01] C：Hello World
来源：http://yb.nszjky.cn

#include <stdio.h>
来源：http://vy.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gn.colortex.cn

[S02] C：变量与格式化输出
来源：http://kq.chemitech.net.cn

int a = 10; printf("%d\n", a);
来源：http://yt.shxzukj.cn

[S03] C：读入整数
来源：http://ds.szxytkj.cn

int x; scanf("%d", &x);
来源：http://bl.newstarts.cn

[S04] C：字符串复制
来源：http://lx.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ca.szxytkj.cn

[S05] C：字符串长度
来源：http://tn.shtwfgs.cn

strlen(s)
来源：http://qn.haigaiapp.cn

[S06] C：字符串比较
来源：http://ii.bjjhwx.cn

strcmp(a, b) == 0
来源：http://qw.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://uw.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rl.colortex.cn

[S08] C：动态内存分配与释放
来源：http://ml.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sk.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://oo.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pg.521024.cn

[S10] C：指针与解引用
来源：http://ne.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://ze.colortex.cn

[S11] C：逐行读文件
来源：http://zn.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://na.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://oo.gzmigu.cn

fclose(f);
来源：http://fj.jctech888.com.cn

[S12] C：写文件
来源：http://ye.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kr.gzmigu.cn

[S13] C：宏定义
来源：http://rh.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cv.szsharing.cn

[S14] C：枚举
来源：http://mx.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://gv.shxzskj.cn

[S15] C：类型转换
来源：http://zy.nszjky.cn

(double) a / b
来源：http://xg.bookmarksfly.cn

[S16] C：位操作置位
来源：http://fc.newstarts.cn

x |= (1 << 3);
来源：http://ki.521024.cn

[S17] C：安全拼接字符串
来源：http://qt.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rd.newstarts.cn

[S18] C：命令行参数
来源：http://dy.newstarts.cn

int main(int argc, char **argv)
来源：http://ax.lnxyls.cn

[S19] C：快速排序
来源：http://pu.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ls.shxzukj.cn

[S20] C：二分查找
来源：http://ad.9csxet.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uw.muxihuayi.cn

[S21] C：字符类别判断
来源：http://tm.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pv.szxytkj.cn

[S22] C：字符串转数字
来源：http://rb.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ns.chemitech.net.cn

[S23] C：随机数
来源：http://tj.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ci.nicolike.cn

[S24] C：获取本地时间
来源：http://dp.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nh.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://vs.bjjhwx.cn

memcpy(dst, src, n);
来源：http://tg.hnjuh.cn

[S26] C：内存清零
来源：http://dr.jctech888.com.cn


<!-- 参考信息 -->