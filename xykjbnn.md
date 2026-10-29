代发 wailian999

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gtfuovxxd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gtehlzgzn.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gizbchzvr.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gemtoggrp.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gvczbggik.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gkurlutda.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/godoqbtkp.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gwqihexmt.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gpmonnrkk.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gqpqeopie.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gmwuyadwm.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gfnpczpyn.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gvxnwrxlq.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gcuhmjsfu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gjlikazhm.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/ggcmpyurm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/getozbiiu.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gbwkxgvry.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gzpevujfu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gczpoexpt.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gblkusela.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/ghgeepakh.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gtqukgdrr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gdgjtzmiy.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/giikewlar.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gmdekphzp.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gscoaqlvl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gnpwahslw.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gpadapmdq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdnauimwb.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gtqgoidsn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gknahjnzw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/grfjuxike.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gobuuojrw.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gbmjpksbb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gwtrdxqit.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gatczvuso.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/geiqlzpib.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gaouuzfpd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/grsxyoxvc.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/giwsbfbft.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gsauymctv.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gqmxkcdcu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gbffsyqmb.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gzbbyvauf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gsisqxoqv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmmewdtse.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gtggsdxpe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gyjfzajgs.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gfylovrnl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gkhrnrmli.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gezgcjtmu.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/giumgkpbr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/godbpmlqy.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gzjqyysul.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gzhfmlsis.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/grokrgssr.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gvvstwzal.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gdusibmnz.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gtymmfzfi.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gsotkgzsq.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gttxsuuid.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gjckbngiy.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gutkoclzd.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gvwlqyjon.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gnxuqkrio.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gkoluycjg.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gjlclnrsw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gslrswsaj.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gllamnfek.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gjbxpuatd.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gfzyfxocu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gglqhngbn.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gglrjdxng.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gkmjiujje.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gvlfdrwfj.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gxceyrech.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gwtbqpnnc.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gilpxkdpf.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gtyjuxpiz.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/guxhwaeqq.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gaykeyhlp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/glcuwkhja.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gmbgqaxvs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gwfkzuafr.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gpzzhjizz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gumnazxkq.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/grbleeowr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gpicwmpzk.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/ggvxovsow.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gurfqfhmg.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gzxqbnyah.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gvptfdyvz.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gelfszmlr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/guketdfoo.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gylafzntf.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gadwucxkp.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gmnefqlgt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gbajbawwi.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gntpqxmmm.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gpwdisfin.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gltrgfjhs.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gehebuslv.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gjxsodleu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gdrknbmaa.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gubkxxdpr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gbbvirjop.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gzmdwxhze.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/golwuqwtm.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gtxicnwmw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gcqgbzefk.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gfrfslhfv.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gqqatmjpq.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gotqevsas.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/guzvwrvrz.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/ggruhrqhs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gbprbiyoi.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gpwvxcdpq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gvyhgamvw.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gjfhmsmtx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/ggyiuunjf.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/glzmqhiuw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gllyapgji.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gnetrwzlo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/grbkhbqxn.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/grrgqyfgd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gzyczxhoj.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/ggpkrvdvi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gsyvkunfy.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/goevyqqmi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gejbxukax.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gkbwcebth.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/ggdypdyes.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gynnhwfip.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gcmpqyule.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gfctvfwmm.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/geiyvqwvm.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gjurqxafa.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gqdtgzztj.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gepkosaew.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gnmzgczqs.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gsvrlqdyl.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gqpelcnlx.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gbrwlzpev.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gkhomumqh.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gloprjsyq.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gnzancoiz.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/ggwfovkcq.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/ghqjuuejb.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gfbsbnqvh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gpaxbsjzd.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gdbrpjitk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gmdencqqt.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gfxkxytuh.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gmlfcvkfj.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gzplyjtcx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gwfsnuvcz.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gtzzvplcn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gsxzvbhhz.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/glzhqjtjq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gkzxmjzbj.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/guloeffxs.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gkmpynndx.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gvyauzurd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gxzbcnwag.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gbbnqxngd.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/giklwkxch.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gldusynzf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gdudyzycx.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/ghwnwzyes.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gkjgyfgah.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gqprtreaz.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gtkhtsfaj.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gavxwwgsc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gnnrpupmw.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gmkzezwpi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gfuunngwu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gnhiztanz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gxmlutvey.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gqcrccsbn.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gbixazssw.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gajyhghga.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gqwkhmqgh.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gmlrdxvwy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gmwjhspis.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gwtztlpjw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gizjoyjte.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gwutsrmfi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/guxtaglaf.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/ghljjpvne.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gzcymfkik.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gkssjzsts.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gccwlzogr.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gfhgjnnxq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gurzjuxhh.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gbvjjiygy.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gkqpkfltd.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/geakjilqx.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gzadkiggk.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gbymnisqs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gibiyikcq.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gzhgqjoks.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/ghpypxgwg.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/ggylnsuth.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/ghgqihkcp.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/guuvuplom.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gjbcffyzh.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/geadowmfv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gmupdhnhy.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gerxdmqsv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gwqrhpulp.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gzihxzsrq.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gevfbgngg.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gilpmjkmn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gqlotybkh.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/guqmehqsm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/giisnmjpm.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gbiunhiuv.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/goiblaqrm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggkskdckp.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gbspdwjif.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gflnwnrcu.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gzffqsyyw.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/grgmzubpa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gpttsepzk.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/goagraenb.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gvbafgvrv.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gyxjpivqh.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gepcadkbn.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gjtvanxyh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gjpevfdmp.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gltccxuvo.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gpzhucpqi.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gtwuaqvmv.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/grehwahvt.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gllhulgme.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gxfvclegl.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gftfxxdaj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gemuedkix.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/galomybtt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/grqnfqxjg.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gdlvxnhau.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gqwfxokup.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gtejleasv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gulwqtlwu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gknxfpgti.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gfkzcrerh.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gkbocavff.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gctpxvroh.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/guykaqzbz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gbfirvcxl.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/ghcddijej.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gmbyrjxul.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gsiybfhdd.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/grkjbzmlj.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gxcjvcorv.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gkdclfjwn.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/glnxlyzoq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gcbvkzihx.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/geiapkpzw.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gvxcycuqe.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gzewgomat.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gjncjnrus.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gfvhwdddp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/giibenkxn.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gikrvcnhf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gwjkhptkx.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gztxrgalx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gtrtoynew.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gpgaumrsd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gsgmfqzzi.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gchsohlol.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gdvmnwrnw.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gmhgrjabq.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gxpsaczeb.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gkrrulwsi.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gbdgfivgm.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gohiftemh.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gtvrqhamx.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gvpsawbhg.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/glzkbjjyb.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gzwbeqikq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gvxswqatb.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gtfbunwyf.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gqrxdggbr.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gxkwbdrtb.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gbhbgqxhc.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gpjobvwhf.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gzqxwnthx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gkrkivfns.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gqcolmabb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gjtfqpxqf.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gluplubqc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gpzlmsphs.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/ggrfwifdz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gncxrabsw.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gubcsawuf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gribpjxtr.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gleqelwqv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gfcefheuo.sHtML


<!-- 参考信息 -->