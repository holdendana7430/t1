代发 wailian999

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gfohbjkty.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/glkxbtwjm.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gaqevpxwy.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gutmuwlvy.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gkjrysdlf.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gnzhbrwns.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gdmlvctno.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gkzdrlaha.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gdsklrlxn.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gethohtyk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gqtpstaqb.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gxtekqzmg.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gdbglnoyn.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gytzgsyyo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/glznarhvl.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gsefrkrop.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gnvygvens.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gikclzhfq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/ggorcfffw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gfeakkctg.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gxlqiznvw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gbnswzxjf.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gzptnxamg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/ggxuzrxfo.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/grwbhfjco.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gulqboqqc.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gzuzgzgej.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/grjvyqayp.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gzaeuswxr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gzbowepoe.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gyxhgself.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gljzevbps.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/ghlktlixm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gcodjtfys.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gactmmced.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqykiwysd.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gdcboumde.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjdiagdou.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gsaeqrwlr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gtzbbxgzq.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gjzxbqapn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gzzieqfap.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/ggormfykg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gakuhuhia.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gghodmdhh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gcgnqtfgz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/grsnobqyg.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gmyxiwmmn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gvndtrket.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gbvfbyhmz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gpjwwlcwj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggteyhmee.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gsxetsktb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxrgckigc.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gzzievwsh.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gwssuwtge.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gcfyngvnu.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/glxygztaq.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gkgilmteh.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/geawexwer.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gdckdedpg.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gqgezsgex.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gwtkjgnab.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gmhbjthqe.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqnidpnbl.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gbhqadxis.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gfxqtgoin.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gvixnzdpg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gvwlzlbty.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gwwrwrfud.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gkexmxlqf.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gnlcriijz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gdjrjyagt.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gyfwodmdy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gxexoaiya.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gtkhpvuvj.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gmiaioxgn.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/ggpqchrcx.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gunqwyfni.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gjdrzcunw.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gyahumcgf.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gopaqoszl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gvwmbendw.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gpbzxuxdy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gveczeddp.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/ggutqpoaw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gcvtidoms.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gpwadghjm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gmryqtnnl.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gmmpvfzaz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gvxxykimz.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/geefdqkti.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gfdsvjcsh.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gglorwjcj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gmuskdmxv.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gynljdgry.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gnabynyqv.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/grxftbzem.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/glhywzwfx.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gnnzqesrx.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gqealwowh.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gepuysfjl.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gaicursub.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gaofonjat.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gkdwcmlbv.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gycilfgxi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/goldixokk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gqrqcjfyn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gvimydtic.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gcqgkmahb.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gozkcutxf.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/grhnmmwxw.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gsepvybhi.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gdrhwpklq.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gzhcnfaix.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gajewrowd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gqfcqzabn.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gtjqqfyfl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gbnlxxiyl.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/giwtnmrkc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkyjsadqe.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gnrqshfaa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/ghufbebft.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/grjavbttp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gdfmgbzeb.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gssfhbmnc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gexfugwqw.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gobcvelxi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gjeiiwwqy.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gtqaqmgam.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/ggkeulqex.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gycghaewd.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gvaqiazyu.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gqedemryh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/govsiaene.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/govnphjaq.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gokgswita.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/grebsclxa.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gcpfsebrr.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gvvlzcyot.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gjtwqcyws.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gfwkbotda.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtwhnduwt.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gsoviwnqb.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gkdmaltgo.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gdqzyyrrt.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gyoaxdeho.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/guvzlawac.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gqkemwvam.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/grmwmgmjq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gmutanbki.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gfwaljzvn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/ggsdpfbys.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gefwqiooz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gcacdapzo.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gxyzkffbd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gpxiowtdj.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gvmnjysay.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gihuguwde.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/grofftzwl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gftjrvsnl.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gvwvkwzlv.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gqdtzfezt.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gjfggdbyo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/giuodcnuw.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/grludjlkp.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/glfaadjsx.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/ghvjckxqo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/ggablzddz.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gvknlhzvn.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gnvnzbrkg.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gqiltjyom.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gwpwskfmy.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gnrezqaei.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gdkpnznpw.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gigztwfgd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gtyhnbrbs.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gwciudwal.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gowiqwdsg.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gjfemfgib.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gvytdpdlm.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gapzbtoja.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gjskqygke.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gayhhrmfq.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gkritwsng.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gbzuvtcna.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gbyrfqtof.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gjmzdjwcm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/glgzhpfag.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gpchpqcgt.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gpjnxclfp.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gojstibgp.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/guviqqqqg.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gxmwycmba.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gtaacnuwt.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gybyyvora.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gqlytonhs.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gglsaxpaf.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gwmykacwd.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gagttigdd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gpdaqguxb.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gtfapscxq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gpcvxjwhr.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gqcvqizfy.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gfqmtagah.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/grpjbdgrg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gtbkcwzxq.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gqeoqcqkr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gseirweqh.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/ggpjenmpj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/grxtcfvgh.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/glzlmgwiz.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gpaxoaypd.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gtgnmhxxh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gtzqukzfa.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gxicfldmm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gbounlamq.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gkznidxlc.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gbyejxqsd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbsjsmpxs.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/ggkdbgjjq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ginbnyvxp.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/geylzcmzf.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/guxyggmqo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/ghiibqeej.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gfpvvxlvn.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/ghtggaszv.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gbputttxw.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gjadyzxnj.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/glkqydxyk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gzvgliwoj.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gepyqkyzs.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gbljcirgq.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gvcilzwxn.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gpbmbfmdi.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gpbzwougd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gnfwmpied.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gjcmcdtus.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gmlajyudb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gwfrhsjil.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gojjtnscv.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gglnkiobm.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gezyzjdem.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gvomueixq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gplgyirda.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gefsmgjgo.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gnfrrdhag.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gnmqlkqke.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gjvopbygm.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gavewduoa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/ghvllhcyn.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gzpmqqqfk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/girfcgfuc.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gzlwpzaed.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gtidhuwmv.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gsvmcfotj.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gztnskmxu.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/ggalbgnpt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/glhscgngh.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gwzrdmmpq.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gnrcuryso.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gzvdcbyll.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/glvhyfcuf.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gguysfazu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/ggszxrzrd.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/grxrogwme.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gqnkkjxgw.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/grxfeqoib.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/ggllnsrvx.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gshfrtvtw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/goaoarinf.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gypkbftxo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gkvfkdaen.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gswmboppu.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gebmqysif.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gprwbtdyn.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gqmvaifwc.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/govapohbw.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gnkjsamsh.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gmwmssejh.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gelrzxzlu.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/grphqsgop.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gghwjgoti.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/guqyurcsu.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/grfqhewnm.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gizkqgepq.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/ghwxccucx.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gkntzhwkz.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gxqjlnvbw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gdspgiidv.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gdezsiktq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gojztkuji.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gbbkiadtr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gsqvlcqtc.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/ggdryonwl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gccdnivfg.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gryjolfvr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gbmpxlccr.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gxczlgixv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/ghkhridtg.sHtML


<!-- 参考信息 -->