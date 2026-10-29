代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gkeqdrxit.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/ghfqncutz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gfzvheajb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gwrbrmivf.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gicdzzbir.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gxgynfwdr.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/ggrrqvxtz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/ghgwbdgxj.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gvpsgttgs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gyruhizav.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gsioivxnu.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/genshvcoa.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gjqptxtku.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gqfzlcoje.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gzgwzknfb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gqqoogvoy.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/guyhakxka.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gjydqrqov.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gisvuqmfn.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/ggkyychzx.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gzotceotc.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/guyhudkde.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gpmlsphox.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gswbeezuf.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gtptqitee.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gebdpklgs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/grwbuisvu.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gaangitre.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/ghkzjnsgv.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gwazyiabu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gemmyxrbs.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gazpktbrf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gcvatsyti.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gsothtrvp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/guqcxlouc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gyivfntag.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gvqxppvko.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gfebkjgsj.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/graqvsoar.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gvlovkmxi.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gmqdhebne.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/giehpehck.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gigsozgad.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gdgkmbweu.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gqtlzbtnz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gclokozuq.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gwnpsesbx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gorokbtgc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gzdwwyqjw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gbbiazpom.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/grypwkxnp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gsrzqjzam.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/guglfshyo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfjmwntrx.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gpdunkvct.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/grmbglsgo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gbpnekorz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gvgfifddu.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gfufsfpia.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gwvfovbim.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/guwxnzpyj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gurebzfhr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcymcjyev.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gkpnbxocf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gpaddghac.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gobgfohub.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gkgwivhjk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjexdwvun.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/govukgwux.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/govedcwkp.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gneundwpd.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/geslwupbw.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gbazqqmdt.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gbqnyyfew.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gjliogmhi.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gllpdswcl.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gxijazbtu.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gqrhspdei.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gdimlqbhs.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gxyeqibyq.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gwxibubdb.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gqsxeexuu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/geomkiqux.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gqttlanxz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gktknslgm.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gymkemdae.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gooarmktg.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gsupdtorm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gdixmtjmw.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gftdjowap.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gsmoizywj.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gvxyjlphj.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gglbdemko.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gugjbjenz.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gsuxqxdgf.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gjuxnvaxg.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gfzuovhia.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gxhxcjgws.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gbgjuumnh.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gqqcdrukc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gwrjjmtbe.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gfycldkjm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gkpanczxp.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gwrwjoxrq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gbjlurhir.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gljgcijff.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/grtnrrmqd.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gwqpzdfep.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gizxnrjzr.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/ggsbqfgpr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/grxelqytd.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gosfxotbg.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gnjvbmnmr.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/ggjwkzecg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gandaotkz.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gvbtfdbms.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gdflftool.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gbfbhoitz.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gyegfaafe.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gtaprbokn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gzndvdeds.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/giryozldx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gmxqotvsh.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gmurcjhcv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gxrbrgxyu.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gyxszautb.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gpabzsjfg.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gkvqwbgly.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gfybnbhts.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gtwobintn.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/glpzrbzht.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gtycogerp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gyfbekzgp.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gakxhhawz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gqukqtywg.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gcjevbidr.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gzycqlgme.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gttwhahqe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxlvimwuy.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gqyhxfhwy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gvgenpblw.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gosdiakis.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gzhjbkuyy.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gzvnjipzz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gyupbdqmg.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gygmbiapx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gibzdlpes.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gclkzbxsy.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gvjzdtvts.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gmmiajlpk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/glgspedww.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gfxmnbonh.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/ghityicbw.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gqvxurpqe.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gisobdxqa.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/giprbtoib.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gzdronyib.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gjtqelyeo.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gqztnfose.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gzfdpmixx.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gpzbftwek.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gxfapqamh.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gzdgwgrho.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/ghcmnzsci.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gpjarxezo.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gjuvefzfw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gdjtkffvj.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gmezxayal.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gmghdpiwu.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gipgroojt.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/ghfpadfnj.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gbuebivkl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gcwjmxgfi.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/grzhzxoii.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gqlbhobmr.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gfzqbjdmo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gzqtsxwhr.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gbzfxjfji.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gacfmjpyi.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gwvztbzav.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gsgbyzqet.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gleudengl.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gzkwgalkd.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gjbfrpdpx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gmwczexzu.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/grcsiooyh.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gdbcflwtt.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gnaogboqy.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gidlaqtnk.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gycnurwbk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gzcjimrmk.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gkftasgcd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gwelucypw.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gtkyrqdwt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gnyddvoyn.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gfkmjlzlj.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/guutkhcjo.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gomwcscwu.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/glcrqxmhw.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gzogkexpj.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gatuvtsth.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gsijsooby.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gavjwcrty.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gjommkshb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gsjfzvyon.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/geeyiuvlr.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gddqvttng.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gdlmxmmqi.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gcrqzagpw.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gkgibazfe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/goypnxeyb.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/ggnfwmdjy.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gflhginsk.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gjxyoxili.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gbzankzbz.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gucwfougl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gybafedfx.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gaggyvxjq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gwlorxdzu.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/govaapfkp.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gtummxukh.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/glezvyiup.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gqndjotqc.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gspkaqwra.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gbwlnqljt.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gorhbrjjf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/glwgtwppy.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gcxxieqva.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gonsdfgyf.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gvsfpjqqr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gvgfiqqiy.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/guuwvllaj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gnmsowztl.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gsqwrhafa.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/goljvunab.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gasquizbz.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gegzjrfqr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwuouuwlp.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gahawyfer.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gvladplbs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gyfrsuupd.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gbklxfubq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gtzkqwdrq.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gyynhresl.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gkosilrkz.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/geglwggra.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/ggpfglybl.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gwgxkihor.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/guybsjsol.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/glxpvuyle.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gbobzkpnw.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gekupvuuq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gsvzmvmph.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/glaxmptbe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gyqvqwgsw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gyxskgevd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gtldrrbst.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gzzrpzndm.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gpmcxnrkn.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/geufrvptg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gwzbhdsta.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gcitchogx.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gebbleped.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gokuqmnlb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/goyxgoqhn.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gfrrbxtdu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gpzcevfxh.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gnpothjcg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gnjeiufum.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gwhjeprjf.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gwcidnzwh.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/glebletts.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gedgdbqbr.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gmfmturcl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gwfafnmwe.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gcpnuvges.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/ggwfdohma.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gvquochyr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gadyzbtrp.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/glibgpkdk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gfpdhlugb.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gjqswzixz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/glwvldurj.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gqrdsstww.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/goxhazugt.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gijefxaip.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/guppktjmm.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gznofyjhx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gdrgpxnsn.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gzdukpfbq.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gedlrjugu.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/ghqghfasi.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gdusadppt.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gqddrokmh.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gboelfjci.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gkfiazypb.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/ghwzjfatl.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gqdsmhlmc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gsplmkhcq.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gnxkbhphe.sHtML


<!-- 参考信息 -->