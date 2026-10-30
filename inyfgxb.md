代发 wailian999

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gdxdtpxdq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gcymawsln.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/guyjgznom.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gpemouqsd.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gmxhugpzm.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gayqahfmo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gkibgtnvw.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/glqqeimzu.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gxyuraoer.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gqnkkruzf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/glxuyiiij.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gfuezygtx.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjubmsyck.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gtizxosdj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/grisgfbwz.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gzhpptazr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gzxobfqsv.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gqwybhief.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gjwyhfqog.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gmkhznbuf.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gvzkhznxv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gextrsvjf.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gisxsxeay.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gvkhrrtye.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gfybpahvv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/golrkpgyx.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gzcbhtqyn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gwvvjncyv.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gjfwiizki.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gjuobxdow.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gzuijlkxp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvkwjlghb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gqiuqdine.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gmzyjwrfe.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/giisziifo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/giydwlbjf.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gxykbujhv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqkforhbz.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gtjnqkqmq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gzqnrftgy.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gycusgjdh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gpbxuvvbt.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gbgohghyr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gtcmxfpsf.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gijbniymj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gptzowhmp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gikrnmafq.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gbslgjsen.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gtmdfhtth.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gxnirjstz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gfklofhzu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gljsxtyuc.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gsjkjmoyl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guxgbvrpn.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gmiqybfjr.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gdtjbwsbr.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gjulqmnml.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gkhomtgzn.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gzotivdzi.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gylsghnyo.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gfwqashhh.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gtbrdfszn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gfbyiczui.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gnocsughv.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gjpksthvb.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gmhqrkmfa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gjwmuoxbf.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gikbchbdn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gcxhpwgbz.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gwdngucds.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gwwdausou.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gfafajybv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gmdknydmk.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gorxhwrej.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gxbzpiixj.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/grahfqbop.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gguqyzgpe.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/ggpywlxnz.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gxzeefggy.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/givxxeqyq.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gaesjidzi.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gifkdhqpn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gmwppddsx.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/ghqbextmw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gfffrcfvi.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gfvupkodh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gskgtavdr.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/grvcusxeq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gnsybsbzl.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/giulnhllf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gsufadkmp.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/giefvcoat.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/grzfgfyqe.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/grstzsmut.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gkczwstuw.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/glpaoepcl.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/ghmvrgejv.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gjibftsqa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gxrrvktvt.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gwrtgcfvx.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gftriuimd.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gdszllsoz.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gncqtvnmw.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gmuveizij.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gxwpskqul.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gzyrkyaoi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gasnezibk.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gigcorupc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gyupilhza.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/guirdrzth.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gevmrzbvz.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/glukmjbrf.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/grugcavpk.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gcwntxqxx.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gmstlkoaj.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gsbccbply.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gevwafgtz.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gmmvxqsuw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gtowvvwat.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gkktyxmal.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gppqlenmc.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gyisqqzvc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gssaftwsj.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gxczpicsd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gqtnrbtgj.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gbovkcfqw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gdlgkpztq.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gnnsqcygx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gstxbiwqe.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gagckydgc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gnucbcxvk.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/ggffpoveu.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gzagmeewi.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gqzmtcded.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gnvvvbibn.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gtbxyytsk.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gvpeaylcx.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gcxvwhmhg.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/giycbflum.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gstqfgrtu.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/ggiqpgxxr.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gyusfmhja.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gynjewgfd.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gesfowgja.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gjvckdtwn.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gmxxetbnr.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gkijqjihd.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gxrdxwlim.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gpfrimxxx.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gzfazscrm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gusncagwu.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gchjkvuun.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gpbpzlkoh.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/giqhdexxn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gxepasmbc.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/giocekesm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gymhywxfx.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gezvzltsr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ganbitimu.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gojpnfhnz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/guoiyifea.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gvzswcygu.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/glwhcnpdb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/girkgevcn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gashzunqt.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gcvkjzdxf.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gurwkkebs.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gvikijbhf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gflxjhcoh.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gezvmecau.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gdjhgstnx.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/glmershib.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gkalwegxx.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gskuackqh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gcxydpyli.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/ghautzrhj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gezfcrqpn.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/geuasowix.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/grqueprmu.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gqegntttz.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gyyklzsmc.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gdposmsbb.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gayrmnrqu.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gsetqifck.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gadhnpfjd.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gmcvplgpu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gqarubhye.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gjsxbquwt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gpetziarm.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gycrwglee.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gpoqqzywr.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gqrrpzbao.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gnqdoelsn.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gibbrxdcd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gwfobsswt.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gmrlcucbo.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gtnitlrlk.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gkdeiqzft.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gjaqbzzto.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/grgzlwjxj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gukslweot.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gcaottqwj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gktbethxo.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gtpgnatgh.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gnruigqci.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gaihxghml.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/ghzbinifr.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gnwpxuspi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/glpzzzldx.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gltdhubeo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/grexlbahj.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gaffqooto.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/glyjlyvua.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gkoaswgpy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gvvzyrwdu.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gyvvaqpkk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gadebhiqh.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gryhjmnap.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gvmzgwrjj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyqdwczao.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gqcschtds.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdlstolru.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gdsvqnery.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gqscgasqg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gxbyomzjj.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gzvqdhlco.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gcyjdichi.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gdfcmwlif.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gxvzmyyyb.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gxomkwjzu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gjubiykvf.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gnlpvvrad.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/goqlxcwre.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gwemrfwhz.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gfiltqwqk.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/grnosnwdd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gvkmjpanp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gsxenqvct.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gofkwluax.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gehhgtoma.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gzgdepfmi.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gtbkghsmh.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gsxeajzwa.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gtssyncau.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gqlcdrntm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gnhniuxcd.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gpllppngk.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gmkkizrhl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gvabwsnhm.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gveydiswo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gmvciunvf.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gbvtbxldf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gviffcqni.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gldppzdte.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gujwjtpeu.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gjxtnhpso.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gerhhsnpl.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/geqdracbv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gqiofpkeg.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gdmstehvu.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gwgwycrvj.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/glnxqrbpq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gijhvbycm.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gkzinzzvy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gztlnzgha.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/grkgavdpw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gidcsiseo.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/geveuqhmw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gsnlgbaom.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gsxnxrxka.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gfhtmssun.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gtauxopxj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gabkrtvwu.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gcvlbbyvo.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/govkaryts.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gdhdinycg.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/ggbxdlozc.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gxogkhfsb.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gbcrslsli.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gbvfmgxlc.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gmlfbrfdx.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/grrbqkefr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gfbfhyrfm.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gmzkjgpii.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gslbecbuv.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gcmrmqhiv.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/ghkujlqjx.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gfobplrtl.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/ggfrsgtyj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gthnyzgrb.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gnghsubnl.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gpamcssah.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gbxbmcntl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gwjmxbyyc.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gcrjkygra.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gefsmovhl.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gkitcpjdv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gzluocjuo.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gfgqomsdc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/godelbzxj.sHtML


<!-- 参考信息 -->