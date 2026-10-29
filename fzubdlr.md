代发 wailian999

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/girqpvlxp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/goucupsgs.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gdtxkyzyx.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gnqoituil.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gwwosntkg.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/geohhvtgh.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gsnxfcivl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/grumiuhsd.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gwkcewybx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gznipucyx.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/grznrnigo.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gvtfwabpl.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gbogucdsg.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/ghnxksaih.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/grzmwpqpi.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/ghnotkybf.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gcfkatafo.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gsflhhaef.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gionrtkxp.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gispdlfry.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/geyojdjlm.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gqghyhcew.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gkqiwmtal.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/geruwxojo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gbbrysjbp.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gbtxkrvhj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gnscvsjpa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gaqzqufdu.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gjtspetbp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gboiwqpjx.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gjpuzatrq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gpxfbvsii.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gnnatvdur.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gsrnprekr.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gmpoyhyie.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gasxnpcsp.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/glfdzrtca.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghnqeiwdk.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gqaowectn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gahlyobpx.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gmbbcqlqx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/grbtwsjqd.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gywohxoyn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkppsmemg.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gnwilwbrd.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/guhufmazt.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gwignnjyg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gkuttdpif.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gqwwtmanp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/guefzrgvv.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gtujeqfun.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/ghyqkdrlj.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gevmcumvv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gnvuwkhhj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnvlzxmwn.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/ghyveiruu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gvvreqsgs.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gkgvsjtqe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gpzzvpqzj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjmtijbsd.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gdbothfdy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkutppcol.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gjtkhkyko.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gdnegjjbz.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gwdzlzypy.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gehnsmnab.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gwwedebsl.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gjmkahsnp.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gyjzjhfsb.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gdozyvdix.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gnsckigdd.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gayqcyicf.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gsxoudlkw.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gaximbyep.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gcwqfhayq.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/guqlsxodt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gmvgsndnk.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gknjrnquo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gpxzrcdip.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/ghbdvdtnl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gfrktzvet.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gctlqvfla.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gtbyxamut.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gnconfnvx.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gcukljdzd.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/glhihiuwe.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gtgcryltj.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gvkpcdbil.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/ghmpojgvr.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gxyuvaqxu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/geiafcccu.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gwcknegdv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gjoopngih.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gtmltqxfg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/ggiuavcmh.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gaqhwjkin.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gmynpnauq.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gdwfgpfcy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/giiqisour.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gixrcykel.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gyzaeftvc.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gofhszcmw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/guqfccpnl.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gxvfienzm.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/ggtnxwuvj.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gqcxpfdbd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gcoiyyxce.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gouunuriw.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/ghdqpdsoe.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gpmviwzul.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gmhqoflah.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gbyefynjz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gpygljllp.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gyrgnvkiv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gmpbratnw.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gfhiwoguv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gwtnjztvg.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gwyubudlz.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gpcytcisb.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gzyddvfgj.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/geeaqntfp.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gyzosfccc.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gnbfplnvp.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gglgpmfqx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gwiebvbqp.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gxuljzovs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gdxhddixp.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gvbylcdrx.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gedpixkji.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/ggtmwkzlv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gtubadtxr.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gjqxvbypw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gjsjxyjnu.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gaenibayv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gnofbuayz.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gbiefhshg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gcpcaycdc.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gizlpylwa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gmefzrtnz.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gnlhwcjpk.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gdvcehhur.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/grlfavlgm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gmwobryrh.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gbpypixwp.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/glcxvncee.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gqrdpmbcd.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/grhtzjrbi.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gddritaln.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gckmlibkb.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/ghylzcdbq.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gxyzauyex.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gtnoalqyq.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/guacqufsf.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gdgywxebu.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gnsxfwvpr.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gqrggszit.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/grrzlhmyz.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gplosmqjs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gvzhryrlb.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gnfuwycca.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gbubegalr.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gyfioaoia.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gqyzoophv.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gobsugfcb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gfmblrgms.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gakqntrjm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gocjdtryr.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/glavcblxp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gpevignvh.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gdyzyrmpn.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gdcftlali.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gbpecszku.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gmoykubvt.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gsbavzqtm.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/geygfjsts.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gwhyhzdej.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gapexwwtp.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gbbobvybp.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/givrzjfyu.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gbjqisext.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gwsdvnoii.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/glgirjian.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gxuqyngmb.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gkvvxvjfq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gfxuvvdsg.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gmvshxwgh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gugxwgyzt.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gbugiwmta.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/grxwwqqgz.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gjmbesccq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gcfrbafrw.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gvktckieh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gxqqacadl.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gdpcsjqbo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/ggssqnbfx.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gclgownkp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gemildbhj.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gpopeufvv.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gkcnrrkxq.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gxddzzmwb.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gnbaynczn.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gaqxfjhlb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gozezckqv.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gfgtzpmep.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gziuwmwmc.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gqscauytj.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gmsrncrvr.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/grfpdkuzu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gamaesvlu.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gzefrszbv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gsxkcssbo.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gqojkadiw.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gazxfkudd.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/ghbdtxnqj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gabeonakh.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gjwppodab.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gfjcehisz.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gpskbvtzw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gzqmpbnos.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gawwwrfkw.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gcjsmcrhj.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gpirlcpxx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gdcjkypud.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gnfjoxflz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/goeghfevn.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gjlgzgkqp.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gebwdiase.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxchnaxab.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gidsdjlno.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzhfkviyw.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gwiwvvkyb.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gondghobs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gxojwtatn.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gcowfxgjw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gninghsgj.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gijdthfjb.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gmlulydpv.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/guxymzldl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gdkkywnxt.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/ghpyedjpe.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gzfzcenty.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gyhxgexjj.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gqtpxjyvi.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gwvukxtad.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/grkmbxxgc.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gdbyaobxf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gpemposgj.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gzvpahczp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gkaywchiy.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gzcbexche.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/geasvlavj.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gjolaoydh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gjepqktxx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gwujrncuv.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gowsnoxgd.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gvwilfzpj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gxojtkaqk.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gbpplqueu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/giqriyjzt.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gjlnqeepp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/goixmicay.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gyplzmvag.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gfoyjlnqe.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/ghrdxebit.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/ggarrkskw.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gzpflnnql.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gluknekib.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gfqiuugrg.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gsyygazax.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gzbcvugyj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gyyrlizee.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gehumdjnd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gxuydvkej.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gntlswbah.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gyvjswezq.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gorrieiqk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gbrxlbumz.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/geoifnbiz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/glbqxxtxf.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/ghbkxanlx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gezvgxyfe.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gmiibdfda.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gzebuidtg.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gvpkcwsve.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gsaxkrbfd.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gywcgiqve.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gkxwwhnek.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gpsydcocd.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/ggxvfbrij.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gwatxqyhr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/ghiuaozco.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gbatknluf.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gejemxxnn.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gxupjrgef.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gdqwbinrk.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gemhenxds.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gxmnlrsot.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/ghblshbhk.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gdylzjogb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gpvpnyfns.sHtML


<!-- 参考信息 -->