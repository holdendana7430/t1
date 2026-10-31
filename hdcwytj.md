代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://ae.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://go.haigaiapp.cn

[Q47] 与平均值比较
来源：http://td.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iq.hnjuh.cn

[Q48] CTE 公用表表达式
来源：http://jj.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jo.colortex.cn

SELECT * FROM t WHERE c > 5;
来源：http://nk.huixiangedu.cn

[Q49] 更新单行
来源：http://nr.panjiajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sz.colortex.cn

[Q50] 批量更新
来源：http://ux.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lk.bookmarksfly.cn

[Q51] 用子查询更新
来源：http://qq.huixiangedu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://db.haigaiapp.cn

[Q52] 删除指定行
来源：http://qg.521024.cn

DELETE FROM users WHERE id = 10;
来源：http://gu.gzmigu.cn

[Q53] 按条件删除
来源：http://dk.bookmarksfly.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gs.shxzskj.cn

[Q54] 清空表
来源：http://ho.9csxet.cn

TRUNCATE TABLE logs;
来源：http://cr.wgjwhj.cn

[Q55] 排名（并列占位）
来源：http://wz.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oy.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://kc.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bd.asd995.cn

[Q57] 行号
来源：http://fr.szsharing.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jp.yuntaijiaju.cn

[Q58] 累计求和
来源：http://lg.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ni.hahajie.cn

[Q59] 分组内累计
来源：http://tl.jianghongdianzi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gc.huixiangedu.cn

[Q60] 取上一行 / 下一行
来源：http://nh.bookmarksfly.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qj.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bc.muxihuayi.cn

[Q61] 移动平均
来源：http://wh.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rv.nicolike.cn

[Q62] 分组占比
来源：http://aj.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://od.lnxyls.cn

[Q63] 开启事务
来源：http://ve.lnxyls.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wj.szxytkj.cn

[Q64] 提交事务
来源：http://oh.521024.cn

COMMIT;
来源：http://gb.wgjwhj.cn

[Q65] 回滚事务
来源：http://do.muxihuayi.cn

ROLLBACK;
来源：http://mh.9csxet.cn

[Q66] 行锁查询
来源：http://md.hahajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qj.huanxung.cn

[Q67] 设置隔离级别
来源：http://yh.szsharing.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wu.asd995.cn

[Q68] 保存点
来源：http://pp.huixiangedu.cn

SAVEPOINT sp1;
来源：http://yt.huixiangedu.cn

ROLLBACK TO sp1;
来源：http://np.chemitech.net.cn

[Q69] 查看执行计划
来源：http://le.haigaiapp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pz.asd995.cn

[Q70] 更新统计信息
来源：http://uc.521024.cn

ANALYZE TABLE users;
来源：http://ku.panjiajie.cn

[Q71] 查看建表语句
来源：http://ug.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://en.bookmarksfly.cn

[Q72] 查看索引
来源：http://bs.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://aa.nicolike.cn

[Q73] 查看表状态
来源：http://fx.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lz.chemitech.net.cn

[Q74] 强制使用索引
来源：http://qo.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vs.521024.cn

[Q75] 日期格式化
来源：http://ks.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://um.shxzukj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pj.haigaiapp.cn

[Q76] 按天统计
来源：http://jb.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mw.muxihuayi.cn

[Q77] 时间加减
来源：http://dy.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dx.yuexingan06.cn

[Q78] 当前时间
来源：http://qh.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sm.nszjky.cn

[Q79] 字符串拼接
来源：http://xp.wgjwhj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://um.bjjhwx.cn

[Q80] 字符串截取
来源：http://pc.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ha.shxzukj.cn

[Q81] 字符串替换
来源：http://wa.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tn.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://ke.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dq.521024.cn

[Q83] 大小写转换
来源：http://jf.huanxung.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ox.lnxyls.cn

[Q84] 去除首尾空格
来源：http://wu.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://og.9csxet.cn

[Q85] 数值取整
来源：http://tn.shxzskj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rs.hahajie.cn

[Q86] 读取 JSON 字段
来源：http://bs.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uy.shxzukj.cn

[Q87] JSON 字段做条件
来源：http://sn.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://je.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://kk.szsharing.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oe.lnxyls.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qk.hnjuh.cn

[Q89] 判断表是否存在
来源：http://mi.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fb.colortex.cn

[Q90] 生成序号列
来源：http://om.jctech888.com.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://um.haigaiapp.cn

================================================================================
来源：http://jj.huixiangedu.cn

R. Bash 专题
来源：http://io.jctech888.com.cn

================================================================================
来源：http://rk.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://ma.colortex.cn

#!/usr/bin/env bash
来源：http://hf.hahajie.cn

set -euo pipefail
来源：http://ux.gzmigu.cn

[R02] 变量赋值与使用
来源：http://ob.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://zd.gzmigu.cn

[R03] 只读变量
来源：http://dh.hnjuh.cn

readonly PI=3.14
来源：http://gi.shxzukj.cn

[R04] 位置参数
来源：http://qy.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kf.asd995.cn

[R05] 参数默认值
来源：http://jp.yuntaijiaju.cn

name="${1:-default}"
来源：http://nn.panjiajie.cn

[R06] 判断命令是否存在
来源：http://vi.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gm.muxihuayi.cn

[R07] if 判断文件
来源：http://rc.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xi.shxzskj.cn

[R08] 数值比较
来源：http://qv.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gv.colortex.cn

[R09] 字符串比较
来源：http://gm.lnxyls.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fw.hahajie.cn

[R10] 正则匹配
来源：http://th.colortex.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fi.shtwfgs.cn

[R11] case 多分支
来源：http://no.chemitech.net.cn

case "$1" in
来源：http://uz.asd995.cn

start) echo "启动" ;;
来源：http://kr.hahajie.cn

stop)  echo "停止" ;;
来源：http://xy.newstarts.cn

*)     echo "未知命令" ;;
来源：http://ew.huixinmuqiang.cn

esac
来源：http://qb.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://tk.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://vv.huixinmuqiang.cn

[R13] for 计数循环
来源：http://zo.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://hf.yuexingan06.cn

[R14] C 风格 for
来源：http://jy.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wj.huanxung.cn

[R15] while 逐行读文件
来源：http://zz.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://st.lnxyls.cn

[R16] until 等待条件
来源：http://sg.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ja.haigaiapp.cn

[R17] 数组定义与取值
来源：http://jm.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://re.hahajie.cn

[R18] 遍历数组
来源：http://vp.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fm.haigaiapp.cn

[R19] 数组长度
来源：http://fw.yuexingan06.cn

echo "${#arr[@]}"
来源：http://yx.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://av.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sl.wgjwhj.cn

[R21] 字符串长度
来源：http://co.jianghongdianzi.cn

echo "${#s}"
来源：http://da.chemitech.net.cn

[R22] 截取子串
来源：http://vn.huixiangedu.cn

echo "${s:0:5}"
来源：http://uu.hnjuh.cn

[R23] 字符串替换
来源：http://le.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nf.shtwfgs.cn

[R24] 大小写转换
来源：http://ci.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mb.521024.cn

[R25] 去后缀 / 去前缀
来源：http://ta.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dy.szsharing.cn

[R26] 命令替换
来源：http://bs.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://od.szxytkj.cn

[R27] 算术展开
来源：http://fo.asd995.cn

echo $((1 + 2 * 3))
来源：http://xu.shxzskj.cn

[R28] 浮点运算
来源：http://rg.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://ew.panjiajie.cn

[R29] 定义函数
来源：http://sw.yuntaijiaju.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oq.colortex.cn

[R30] 函数返回状态码
来源：http://ze.muxihuayi.cn

f() { return 0; }; f || echo "失败了"
来源：http://hs.gzmigu.cn

[R31] 局部变量
来源：http://bk.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://hr.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://xw.yuexingan06.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vr.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://vx.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ul.bjjhwx.cn

[R34] 退出时清理
来源：http://pb.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ky.gzmigu.cn

[R35] 后台执行并等待
来源：http://pm.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oz.huanxung.cn

[R36] 并发执行多个任务
来源：http://cc.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pg.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://ov.jianghongdianzi.cn

files=$(ls -1)
来源：http://kj.haigaiapp.cn

[R38] 管道串联
来源：http://nz.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://nl.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://co.hahajie.cn

cmd > out.log 2>&1
来源：http://gp.newstarts.cn

[R40] 追加写日志
来源：http://mj.newstarts.cn

echo "log" >> out.log
来源：http://jw.huanxung.cn

[R41] 丢弃输出
来源：http://xq.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://az.huanxung.cn

[R42] 输入重定向
来源：http://oz.haigaiapp.cn

wc -l < a.txt
来源：http://ft.szxytkj.cn

[R43] 按名字查找文件
来源：http://ir.huanxung.cn

find . -name "*.log" -type f
来源：http://fs.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://nu.huixinmuqiang.cn

find . -mtime -7 -type f
来源：http://gt.huixinmuqiang.cn

[R45] 批量删除
来源：http://bv.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://ak.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://xd.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://er.jianghongdianzi.cn

[R47] sed 单行替换
来源：http://no.shxzukj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wk.shtwfgs.cn

[R48] awk 取指定列
来源：http://kx.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://as.nszjky.cn

[R49] awk 带条件
来源：http://uq.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ti.haigaiapp.cn

[R50] awk 求和
来源：http://cq.shxzskj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fr.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://wp.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bn.hnjuh.cn

[R52] 统计行数
来源：http://va.colortex.cn

wc -l a.txt
来源：http://bg.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://rv.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nx.huanxung.cn

[R54] 比较两个文件
来源：http://jf.chemitech.net.cn

diff a.txt b.txt
来源：http://zd.521024.cn

[R55] 压缩与解压
来源：http://gm.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ag.shxzukj.cn

[R56] 远程拷贝
来源：http://wn.hahajie.cn

scp file user@host:/path/
来源：http://ch.jctech888.com.cn

[R57] 远程执行命令
来源：http://ab.asd995.cn

ssh user@host 'uptime'
来源：http://wg.wgjwhj.cn

[R58] 下载文件
来源：http://ye.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yg.szxytkj.cn

[R59] 发 POST JSON
来源：http://am.shxzskj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vh.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://cm.hnjuh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://so.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://ne.asd995.cn

df -h;  du -sh *
来源：http://dw.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://os.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://gl.hahajie.cn

[R63] 内存与进程
来源：http://ji.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://zy.jctech888.com.cn

[R64] 结束进程
来源：http://qd.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://sy.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://eo.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jv.gzmigu.cn

[R66] 定时任务
来源：http://cg.colortex.cn

crontab -e;  crontab -l
来源：http://eo.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://gj.chemitech.net.cn

openssl rand -hex 16
来源：http://ox.muxihuayi.cn

[R68] 计算文件校验值
来源：http://xn.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://az.nszjky.cn

[R69] 生成随机密码
来源：http://mn.huixinmuqiang.cn

head -c 16 /dev/urandom | base64
来源：http://ee.panjiajie.cn

[R70] 时间戳与互转
来源：http://mj.newstarts.cn

date +%s;  date -d @1700000000
来源：http://ms.shxzukj.cn

[R71] 日期格式化
来源：http://ls.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://py.nszjky.cn

[R72] 等待端口就绪
来源：http://vd.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sp.shtwfgs.cn

[R73] 分割大日志
来源：http://uv.hnjuh.cn

split -l 1000 big.log part_
来源：http://mo.asd995.cn

[R74] 批量重命名
来源：http://jz.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hx.hnjuh.cn

[R75] 导出环境变量
来源：http://cp.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://ss.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://uz.shxzskj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fk.huanxung.cn

[R77] 读取用户输入
来源：http://fh.nicolike.cn

read -rp "请输入: " ans
来源：http://hv.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://va.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://na.szxytkj.cn

[R79] 解析命令行选项
来源：http://pf.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ve.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://zu.colortex.cn

time ./run.sh
来源：http://vk.bjjhwx.cn

================================================================================
来源：http://qy.haigaiapp.cn

S. C / C++ 专题
来源：http://ff.shtwfgs.cn

================================================================================
来源：http://sc.nicolike.cn

[S01] C：Hello World
来源：http://xx.hahajie.cn

#include <stdio.h>
来源：http://wp.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zj.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://gi.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://gu.huanxung.cn

[S03] C：读入整数
来源：http://tk.nszjky.cn

int x; scanf("%d", &x);
来源：http://so.shxzskj.cn

[S04] C：字符串复制
来源：http://wu.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wz.panjiajie.cn

[S05] C：字符串长度
来源：http://hw.huanxung.cn

strlen(s)
来源：http://xk.szxytkj.cn

[S06] C：字符串比较
来源：http://ws.bjjhwx.cn

strcmp(a, b) == 0
来源：http://da.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://ur.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ul.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://gn.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bl.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://oq.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qn.shxzukj.cn

[S10] C：指针与解引用
来源：http://es.521024.cn

int *p = &a;  *p = 5;
来源：http://eu.asd995.cn

[S11] C：逐行读文件
来源：http://be.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://xq.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tq.521024.cn

fclose(f);
来源：http://kx.jctech888.com.cn

[S12] C：写文件
来源：http://rl.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zj.9csxet.cn

[S13] C：宏定义
来源：http://mn.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rv.wgjwhj.cn

[S14] C：枚举
来源：http://tr.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://yt.lnxyls.cn

[S15] C：类型转换
来源：http://nu.asd995.cn

(double) a / b
来源：http://yf.9csxet.cn

[S16] C：位操作置位
来源：http://od.asd995.cn


<!-- 参考信息 -->