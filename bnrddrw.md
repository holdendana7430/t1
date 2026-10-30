代发 wailian999

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gipkojqlk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gkmqeptjo.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gieddpitk.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gfomwwqge.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gwprmgocm.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gkbahvlyl.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gdrmlduxu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gojosqfng.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gfcjsxytf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gtsoezhwm.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gaeipxmjg.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gbdzxsbql.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gfmuvjcqc.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gxcmtuzhi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gflybbaoz.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gasvpnklx.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gvvqaptpm.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/ghbfjxkrt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gxvntjfou.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gcjghcpun.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gcjscwfrp.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/guedjttyg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gllptgqbd.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gylinpmbp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/geabeaunw.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gaasfnrnx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ghcpoxvkk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/ggexxgmhk.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gkctwpvsq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gixpwdtey.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gapmqbmxa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gmjsgrvya.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gygzykqpw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/ggzeqxyln.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gyvezunhj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gcrvafanj.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/goqtwbpfy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gbwdbbdvm.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gqcnceigr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gczryalog.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gphlpwnic.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gntdpifuz.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gdnvsbxnk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gctxblfnf.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/grbsljasb.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gvsizacnl.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/geyaggwuo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/ggaecoszl.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/grjhnmxto.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gjrjsveae.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gyudxjyiv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/galgdubim.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gtnqortpe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gqdalfrbe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gskuaazpv.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gxzgogvwu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gxwzabake.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gcrcexooq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gyqxzpmck.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsvdpxvqr.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gebgefjkr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdmusdbfa.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/goacptdlk.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gqpasxcxr.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/ggbmqthdv.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/glyrucfor.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gcfyjnzpr.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gvrualbxs.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gfqjymvxo.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/golbxfrhs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/guahlxcve.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gibfcsujh.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gpidyylwd.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gkbdwzkzc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gupftpikm.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gfnuigovs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gdbcgycky.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gwbimfufs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/grjalmkgb.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/guqurpshe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/glvxbqtnd.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/goejndmoc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/ggvqjmxpc.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gujlzzoid.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/goixgvyse.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/grmqwfvdh.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gykonwrzy.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gdejjfuth.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gveawrvus.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gjvhfrbqp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/ghojhevap.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/goscjlboz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gnuvfljys.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gooiwkieq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gaplgoexk.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gzfnegibz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gbmbirvel.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gnypadiak.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gtyxgwofj.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gwmzaurna.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gbakpbwct.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gaumbbytt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gdljnmpkp.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gpblcskvn.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gnhbsanwl.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gysznrqkd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gzlboowow.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/giepzdybr.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gwruivhiz.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gdmptbwxy.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gqrwoxizy.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/ggavcukhb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gieouzrrw.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gxgrgdmhx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gzgrvhzyw.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/ghltmptrj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gnkpejcoy.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gcxhiylts.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/glbysgyjw.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/ghuzkoohc.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gbkbltxjw.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gorznbzxp.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gvtphxhcw.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gsyomjukd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gbbazatuw.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gbttdchzm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/glthjidxp.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gxqdtcrqp.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gasqwkfmq.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/guozlnoij.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gipfsfxpm.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gajsjqzye.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gbbkajznh.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gbdsvjfed.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gteusrkci.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gjgzynslc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gopltzwxl.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/grsafbcxk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/ggffsdxke.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gqsplyfkk.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gnynxlbad.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gymjsbdgx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gtwdxxuqw.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gtylhydyl.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gkcephlda.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gjtoofbsk.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gwtbfeeho.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gnzfjfvmt.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gzjoiubgo.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gozwkwfvx.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gvlqrwjsh.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gkavcfrmm.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gazgprdui.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gnobhdnjd.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gqrusvyvd.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/guywlzcfj.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gnwoenxss.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gujzkawgm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gluvkonxa.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gqiialfxz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gufrupwmq.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gbqkatlnn.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gdipzgxgr.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gkgcauqat.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gknuzdcps.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gdeotyzwg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gvtzvtdow.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gipwlpqxx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gshuujvyq.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/grbyczwti.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gfrzinsdl.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gvuvoatiz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gyzwqexuk.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/guuyhwdys.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gtnmpcned.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gldbdvqxq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gbhjilhfr.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gkjjxlqvr.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gxokfxhyg.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gxrhpmdgk.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gruebbpoj.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gfqresjdb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/grilawesa.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/ggbzrvext.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gcerlbldi.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gbghgggkz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/ghqbudyem.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gbtrmnljh.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gfvicnrah.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gfwaecvtb.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gsckcygjw.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gevrcarsg.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/ggeeikogu.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gxswtftrb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gecjjgpte.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/ggrbhegxc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gbxtkeecq.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gkqncfkxe.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gefefmkxa.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gaqwpuwzc.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gulubwovk.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gaodghjpx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gpanatucd.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gvnhvhjzk.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gwesjjxkx.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gobjdjtpy.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gnhksxice.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/glvfacvsi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gmvcbsolv.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/guguiyyik.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gwsmayoqw.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gidrhqjwr.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/ghdemqevl.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gfhadlzyu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gvghlehkb.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gnzuxusxj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/ggczedlnn.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzxsivogh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gftfrlpos.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gfubqmjng.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gugjxquij.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gmqrktjft.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gmvvisrpp.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/ghvtydwrd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gayfubvpd.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/ghlrenimj.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gdivjoljb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gibhjdrbz.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gmsgjyqla.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmdwibuzb.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gcnrnaspt.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gebdnudmp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gljnzfulc.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/grijjsslq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gagmatozx.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/guyxjkhfp.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gskezkkpp.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gtnxogolx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gwpuoiudo.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gbxxplblw.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gdqsbsnxm.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/ganzhipyn.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gulefxxnk.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gwpngvcch.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gttnrlvip.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gqzoaazbp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gatrhafrs.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gvsyniacv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gqomrzhbe.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/guukeondx.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gtyklxlyt.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gpfnyrkbb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/grbbwyvcq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gieegjryc.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gsmsdusct.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gaxxgesti.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gyrbrhitd.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gqemksoap.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gxnewngbj.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/grwwbecdx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gbhkfxokh.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gnmjgcmxn.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/glwicdwdv.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gntevmexg.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gemhricqq.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/ghzemmlmc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/glipvwakq.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gjlwqpjxc.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/grqkssaiq.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gagcppxva.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gyzgsydzr.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gureransl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gizjtyguw.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gqolgntam.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gfbydedcb.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gcfvobcwh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gkfmxspzr.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gapyfvyql.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/ggoefywls.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gwqazxrqs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gukdodpwc.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gpghzzhgr.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gjkwtoajo.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gtajhuegd.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gwjovngyd.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/ggkhupocu.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gvmtydbnj.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gbirxpnnc.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gohrfhxtf.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gseqbirqb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gcdnxxvqc.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/grhuasqqr.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gxcmthqbv.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gfpwlvokj.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gtyyvloab.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gumxudskp.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gbwzgavqx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gqsacgcae.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gpuxyxswo.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gisogakkw.sHtML


<!-- 参考信息 -->