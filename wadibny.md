代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tt.gzmigu.cn

[Q58] 累计求和
来源：http://dk.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mf.colortex.cn

[Q59] 分组内累计
来源：http://if.jctech888.com.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tj.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://sz.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iw.jctech888.com.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ds.asd995.cn

[Q61] 移动平均
来源：http://je.haigaiapp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mn.gzmigu.cn

[Q62] 分组占比
来源：http://lt.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://aa.yuexingan06.cn

[Q63] 开启事务
来源：http://id.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zq.asd995.cn

[Q64] 提交事务
来源：http://av.nicolike.cn

COMMIT;
来源：http://er.bjjhwx.cn

[Q65] 回滚事务
来源：http://vp.hahajie.cn

ROLLBACK;
来源：http://kh.nszjky.cn

[Q66] 行锁查询
来源：http://ny.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hk.nszjky.cn

[Q67] 设置隔离级别
来源：http://cf.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://by.521024.cn

[Q68] 保存点
来源：http://or.huixiangedu.cn

SAVEPOINT sp1;
来源：http://dk.shtwfgs.cn

ROLLBACK TO sp1;
来源：http://ol.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://lg.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vh.hahajie.cn

[Q70] 更新统计信息
来源：http://pd.lnxyls.cn

ANALYZE TABLE users;
来源：http://kc.nszjky.cn

[Q71] 查看建表语句
来源：http://ad.nszjky.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rj.huixinmuqiang.cn

[Q72] 查看索引
来源：http://fw.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://rc.szxytkj.cn

[Q73] 查看表状态
来源：http://ws.hnjuh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://eo.newstarts.cn

[Q74] 强制使用索引
来源：http://oa.shtwfgs.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://op.chemitech.net.cn

[Q75] 日期格式化
来源：http://sz.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ac.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mb.jianghongdianzi.cn

[Q76] 按天统计
来源：http://mf.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yl.haigaiapp.cn

[Q77] 时间加减
来源：http://ah.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://au.nicolike.cn

[Q78] 当前时间
来源：http://ak.panjiajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xm.asd995.cn

[Q79] 字符串拼接
来源：http://er.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wm.nszjky.cn

[Q80] 字符串截取
来源：http://jl.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ba.szxytkj.cn

[Q81] 字符串替换
来源：http://mh.hnjuh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ps.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://kl.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rp.nszjky.cn

[Q83] 大小写转换
来源：http://qi.chemitech.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yt.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://sc.shxzukj.cn

SELECT TRIM(name) FROM users;
来源：http://zh.bjjhwx.cn

[Q85] 数值取整
来源：http://lj.szxytkj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hc.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://ys.gzmigu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vl.bjjhwx.cn

[Q87] JSON 字段做条件
来源：http://cg.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zn.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://bw.newstarts.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lg.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eu.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://hz.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ej.shxzskj.cn

[Q90] 生成序号列
来源：http://sh.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://no.jctech888.com.cn

================================================================================
来源：http://vo.shxzskj.cn

R. Bash 专题
来源：http://tt.panjiajie.cn

================================================================================
来源：http://oj.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://uz.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://np.hahajie.cn

set -euo pipefail
来源：http://xp.asd995.cn

[R02] 变量赋值与使用
来源：http://mi.lnxyls.cn

name="Tom"; echo "$name"
来源：http://je.yuexingan06.cn

[R03] 只读变量
来源：http://ur.huanxung.cn

readonly PI=3.14
来源：http://nb.shtwfgs.cn

[R04] 位置参数
来源：http://hn.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sc.colortex.cn

[R05] 参数默认值
来源：http://rh.chemitech.net.cn

name="${1:-default}"
来源：http://mv.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://ys.newstarts.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uo.huixiangedu.cn

[R07] if 判断文件
来源：http://fh.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mp.bjjhwx.cn

[R08] 数值比较
来源：http://eh.jianghongdianzi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mc.colortex.cn

[R09] 字符串比较
来源：http://np.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yx.gzmigu.cn

[R10] 正则匹配
来源：http://uj.panjiajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nl.hahajie.cn

[R11] case 多分支
来源：http://aa.bookmarksfly.cn

case "$1" in
来源：http://pf.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://aw.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://wf.wgjwhj.cn

*)     echo "未知命令" ;;
来源：http://oj.szxytkj.cn

esac
来源：http://ko.szsharing.cn

[R12] for 遍历文件
来源：http://sb.bjjhwx.cn

for f in *.txt; do echo "$f"; done
来源：http://ne.hahajie.cn

[R13] for 计数循环
来源：http://vm.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://vn.shxzskj.cn

[R14] C 风格 for
来源：http://oh.lnxyls.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ud.chemitech.net.cn

[R15] while 逐行读文件
来源：http://uh.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qz.colortex.cn

[R16] until 等待条件
来源：http://wh.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zw.huixinmuqiang.cn

[R17] 数组定义与取值
来源：http://hz.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jq.haigaiapp.cn

[R18] 遍历数组
来源：http://fe.hahajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cw.jctech888.com.cn

[R19] 数组长度
来源：http://wv.gzmigu.cn

echo "${#arr[@]}"
来源：http://tx.nszjky.cn

[R20] 关联数组（字典）
来源：http://uc.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ov.szsharing.cn

[R21] 字符串长度
来源：http://sv.yuntaijiaju.cn

echo "${#s}"
来源：http://rm.haigaiapp.cn

[R22] 截取子串
来源：http://bt.shtwfgs.cn

echo "${s:0:5}"
来源：http://se.521024.cn

[R23] 字符串替换
来源：http://ay.hahajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pq.nszjky.cn

[R24] 大小写转换
来源：http://wq.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://if.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://lj.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vy.hnjuh.cn

[R26] 命令替换
来源：http://ok.shxzukj.cn

now=$(date +%F); echo "$now"
来源：http://dn.nicolike.cn

[R27] 算术展开
来源：http://xy.newstarts.cn

echo $((1 + 2 * 3))
来源：http://sa.nicolike.cn

[R28] 浮点运算
来源：http://by.nszjky.cn

echo "scale=2; 10/3" | bc
来源：http://nm.szxytkj.cn

[R29] 定义函数
来源：http://to.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lz.asd995.cn

[R30] 函数返回状态码
来源：http://mr.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://eg.chemitech.net.cn

[R31] 局部变量
来源：http://fd.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://kx.nicolike.cn

[R32] 参数个数校验
来源：http://gg.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fu.muxihuayi.cn

[R33] 捕获错误并提示行号
来源：http://fk.panjiajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ly.muxihuayi.cn

[R34] 退出时清理
来源：http://un.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ff.hnjuh.cn

[R35] 后台执行并等待
来源：http://qo.nicolike.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dg.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://zf.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dt.jianghongdianzi.cn

[R37] 把输出赋给变量
来源：http://hf.nicolike.cn

files=$(ls -1)
来源：http://bl.gzmigu.cn

[R38] 管道串联
来源：http://fo.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://js.colortex.cn

[R39] 重定向标准输出与错误
来源：http://rm.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://av.nszjky.cn

[R40] 追加写日志
来源：http://af.szxytkj.cn

echo "log" >> out.log
来源：http://wb.hnjuh.cn

[R41] 丢弃输出
来源：http://yo.shtwfgs.cn

cmd >/dev/null 2>&1
来源：http://jt.shxzukj.cn

[R42] 输入重定向
来源：http://rk.colortex.cn

wc -l < a.txt
来源：http://hv.chemitech.net.cn

[R43] 按名字查找文件
来源：http://md.wgjwhj.cn

find . -name "*.log" -type f
来源：http://lo.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://pg.huixinmuqiang.cn

find . -mtime -7 -type f
来源：http://rn.hahajie.cn

[R45] 批量删除
来源：http://ut.521024.cn

find . -name "*.tmp" -delete
来源：http://cu.shxzskj.cn

[R46] 递归替换文件内容
来源：http://bm.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pe.bookmarksfly.cn

[R47] sed 单行替换
来源：http://po.shxzukj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cl.haigaiapp.cn

[R48] awk 取指定列
来源：http://jv.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://sd.521024.cn

[R49] awk 带条件
来源：http://kk.wgjwhj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ep.gzmigu.cn

[R50] awk 求和
来源：http://hk.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jz.colortex.cn

[R51] 排序去重取前几
来源：http://gr.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sd.yuntaijiaju.cn

[R52] 统计行数
来源：http://fq.nszjky.cn

wc -l a.txt
来源：http://yi.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://ez.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://la.huixiangedu.cn

[R54] 比较两个文件
来源：http://ek.muxihuayi.cn

diff a.txt b.txt
来源：http://vf.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://lq.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://om.panjiajie.cn

[R56] 远程拷贝
来源：http://uo.shxzskj.cn

scp file user@host:/path/
来源：http://ys.haigaiapp.cn

[R57] 远程执行命令
来源：http://ci.bjjhwx.cn

ssh user@host 'uptime'
来源：http://sr.huixinmuqiang.cn

[R58] 下载文件
来源：http://qn.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cf.nszjky.cn

[R59] 发 POST JSON
来源：http://yj.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://aj.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://xl.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cn.colortex.cn

[R61] 磁盘占用
来源：http://wj.lnxyls.cn

df -h;  du -sh *
来源：http://uc.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://ai.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://ym.521024.cn

[R63] 内存与进程
来源：http://pk.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://qi.chemitech.net.cn

[R64] 结束进程
来源：http://pq.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://vv.521024.cn

[R65] 查看端口占用
来源：http://zf.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qd.jctech888.com.cn

[R66] 定时任务
来源：http://uz.szsharing.cn

crontab -e;  crontab -l
来源：http://yp.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://za.wgjwhj.cn

openssl rand -hex 16
来源：http://yp.huixiangedu.cn

[R68] 计算文件校验值
来源：http://qg.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ap.521024.cn

[R69] 生成随机密码
来源：http://uv.521024.cn

head -c 16 /dev/urandom | base64
来源：http://hp.shxzukj.cn

[R70] 时间戳与互转
来源：http://xs.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://pk.bjjhwx.cn

[R71] 日期格式化
来源：http://pd.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cc.newstarts.cn

[R72] 等待端口就绪
来源：http://wt.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xe.gzmigu.cn

[R73] 分割大日志
来源：http://wo.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://rf.colortex.cn

[R74] 批量重命名
来源：http://mf.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ir.shxzskj.cn

[R75] 导出环境变量
来源：http://mr.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://lo.colortex.cn

[R76] 使用临时文件
来源：http://pm.shxzskj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://av.muxihuayi.cn

[R77] 读取用户输入
来源：http://la.asd995.cn

read -rp "请输入: " ans
来源：http://ba.hnjuh.cn

[R78] 交互式菜单
来源：http://wo.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bc.muxihuayi.cn

[R79] 解析命令行选项
来源：http://ee.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://th.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://gq.newstarts.cn

time ./run.sh
来源：http://iv.hahajie.cn

================================================================================
来源：http://sr.nszjky.cn

S. C / C++ 专题
来源：http://gi.colortex.cn

================================================================================
来源：http://ko.panjiajie.cn

[S01] C：Hello World
来源：http://mh.yuntaijiaju.cn

#include <stdio.h>
来源：http://nq.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qq.colortex.cn

[S02] C：变量与格式化输出
来源：http://xw.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://wi.bookmarksfly.cn

[S03] C：读入整数
来源：http://xm.huanxung.cn

int x; scanf("%d", &x);
来源：http://vk.nicolike.cn

[S04] C：字符串复制
来源：http://gg.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://am.lnxyls.cn

[S05] C：字符串长度
来源：http://px.gzmigu.cn

strlen(s)
来源：http://fl.newstarts.cn

[S06] C：字符串比较
来源：http://ma.colortex.cn

strcmp(a, b) == 0
来源：http://we.hahajie.cn

[S07] C：数组遍历求和
来源：http://fu.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dd.9csxet.cn

[S08] C：动态内存分配与释放
来源：http://nc.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vc.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://qj.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xa.521024.cn

[S10] C：指针与解引用
来源：http://vr.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://od.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://iy.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://sw.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rc.asd995.cn

fclose(f);
来源：http://sf.colortex.cn

[S12] C：写文件
来源：http://nr.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ay.asd995.cn

[S13] C：宏定义
来源：http://qv.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ks.chemitech.net.cn

[S14] C：枚举
来源：http://rb.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://vb.huixinmuqiang.cn

[S15] C：类型转换
来源：http://mf.huixinmuqiang.cn

(double) a / b
来源：http://xm.hnjuh.cn

[S16] C：位操作置位
来源：http://yd.huanxung.cn

x |= (1 << 3);
来源：http://vj.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://ge.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vh.muxihuayi.cn

[S18] C：命令行参数
来源：http://rs.shxzukj.cn

int main(int argc, char **argv)
来源：http://ux.huixiangedu.cn

[S19] C：快速排序
来源：http://dv.gzmigu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://do.jianghongdianzi.cn

[S20] C：二分查找
来源：http://ij.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cs.lnxyls.cn

[S21] C：字符类别判断
来源：http://oc.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xd.szxytkj.cn

[S22] C：字符串转数字
来源：http://yj.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mi.bjjhwx.cn

[S23] C：随机数
来源：http://vr.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yr.chemitech.net.cn

[S24] C：获取本地时间
来源：http://je.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hg.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://oa.gzmigu.cn

memcpy(dst, src, n);
来源：http://yl.yuntaijiaju.cn

[S26] C：内存清零
来源：http://xv.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://mo.haigaiapp.cn

[S27] C：定义常量
来源：http://ub.shxzskj.cn

const double PI = 3.14159;
来源：http://jm.9csxet.cn

[S28] C：静态变量
来源：http://qk.haigaiapp.cn


<!-- 参考信息 -->