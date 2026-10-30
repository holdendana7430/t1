代发 wailian999

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gpubhimyb.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gbvrohpbg.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gqsxesjvv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/goqvfzajp.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/godtumgbv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gieczsblm.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gdnbbuzoj.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gjsehuhca.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gloctszjs.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gyppszucz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gclzjquoz.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gtuwixkkq.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gqecspqrt.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gsnkdycqz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gpwqcmhhz.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gvzqcpvam.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzdlrgzld.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gcelwoffd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gbqgcjwuv.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/ghaqtoqaq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gguwdscya.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/ghwycllzu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gnfkapsaq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/ggvwqvsmm.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gbtbkpnpy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/glxdkstpv.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gnunglnnh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gdiqleggh.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gmsmgqdgd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/grvyqkrso.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gtehrjtni.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gxyyoeqme.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gwmylzlrj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gfhlhzjsy.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gnuvpotvp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gasztgmvm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gevgxwbie.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmsmrwduc.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/grmitunek.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gzkbudiqv.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/grzsbqxzo.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/ggsbjdzor.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/goprqgzqy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/goupkmrxd.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/grqekdnnb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gpejeomkn.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gumsbwdzr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gzzckmyoh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gysjbxttt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gowiweuzp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gnvrempxh.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gsnzzxzbt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gtkstiqqw.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gkxdholmp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gcandjwqx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvrcukinw.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/ghgqqvpwq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcmxkyrrh.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/grdxcskuk.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gccgswotg.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/grzstohzf.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gjtiwigcu.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gkaeahykx.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gttgkdsyo.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gpmzovwqx.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gswztlmpf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gsnttztru.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gvfquwsbg.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/glrtjpsvw.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gvwllelki.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/ghuktmrlq.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/getxwzygq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gzxlslhje.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/ggylklzih.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/grrusomwp.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gycfyyfro.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/ghgnqcdgc.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gxhvmawsg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gfbvagnwd.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gxkmrphgb.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gvxeuqyio.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gsrqinptv.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gnzktgbsz.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/glrxgfkrl.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gbuyngnnn.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/glzxlvhba.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gliarmfhy.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gweopwmnd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/ggixtadov.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gbaucduuy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/ghumolopu.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gphivzeob.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gmbffkzto.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gwncdnsfy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gwazzemrw.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gekrxwtyp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gyfugggyb.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/geysapsoe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gxsmcafby.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gqbirvifh.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gistvqlnv.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gjmymypqm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gfpavscjh.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gxypcmnhw.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gmchojcov.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gjnsvpsux.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gdvlegxmi.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gmcfwyxpk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gysdwsrev.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gmtalxkdj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/ghtjvjpkm.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gmpcorbhd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gsqwbeduc.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gbonikymd.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/govubwabl.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gzldqktxm.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gmzcwczwy.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gsabgurql.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gsvlactvu.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gawdkjvvy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gqiegpzij.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gwlvbwzfl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gigrcmlzt.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gezlxwobh.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gqlslqviy.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gwseztnhf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gupfhjits.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gqpynwysz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gisqzepuq.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gatjwssyo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gonkvntbw.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gymmnddvg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gurxtyvzi.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gncrecihb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gzgfldkcx.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gofgsvatf.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/guasuotrx.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gvoasadhp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gbzfnccru.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gifdpbcfp.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gagkymwao.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gaelgkcka.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gzcrthfyt.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gjnmjfxuv.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gicwhatpp.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/getnbdkjv.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gwrtiqwbu.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gpdxmeffi.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gqsrdxfuk.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gneqleemn.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gppcirjtc.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gnbuxgpbt.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gnkzypzpu.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gcxukeeqh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/geitnwooo.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/ggkdhuxkq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gbyglyakt.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gbjyhxcns.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/grpvltmgp.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gasegxhgn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gugskbcgs.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gwngldvig.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gsnsnqakc.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/grhywidxf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gemxvcvgs.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gofmgjokd.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/griwvgwqr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gfylzvbrw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gfbtwayqz.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gfuysrcom.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gqhkxvjwh.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gxfkiunaf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gmqoululb.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gojsqlhjf.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gwqjwqdwv.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/glrebmrzu.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gbwluyshv.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gmbhrskqd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/guysulafg.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gepcshnak.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gkffmbhnh.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/geuzdwnwp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gdhshakbe.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gpoztosnm.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gzfglfvyf.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gnjorpyau.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gmzqbsvto.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gmxexclzn.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gfjoapngf.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gbvifcmdn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gallvfary.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gypafomxh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/grdiqqrvr.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/givixthkh.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gbffmjqqf.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gvobkyyjk.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gyyqxumph.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gjzygijwn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gwcuvltbf.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gchotgzmg.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gdmlnwrvf.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gymxklwbf.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gumgssnjt.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gtzzbklfp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gjffkswrd.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gdrmmpjlu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gxivpqvvr.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gpqhylcvn.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gcfyikzof.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gsevqncis.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gtmnnnsep.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/glzlzqser.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/geqnixxlp.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvdiobhop.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gvwquxmdb.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/guuexrzzb.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gdfdpcpes.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gdvtckdge.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gxhokritn.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gnbyiivwc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gpqgpmlcz.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gqnkpzfev.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gbsqehefu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpdejuvix.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gmltnutiy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gugtiqfwh.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gzmtpzmpc.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gxuauhvck.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gpkrnczdp.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/guluegfbl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gfixqnoyt.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gpdehesxh.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/goctmcoaa.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gasmpgoit.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gppcpwpbw.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gkpznxjdr.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gancgugfa.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gjgfblolo.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gdgfwrfch.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gamqgrjxn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gdwxkbomu.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gixucbivl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/glkqzmrgc.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gagmmvxct.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/grmgvqibk.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gpzgdirwr.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gttaptyui.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gatsstlok.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gdolwdhfv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/guwdrzlxk.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/ghekxouap.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/geddrllfn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gnmzudlbp.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/geyzhvwjn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gqakptjui.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gqjybvztg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/ghpaydqnb.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gwimtreaq.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/guxmaindo.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gopdulisw.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gnsvqboci.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gxsqbfyhm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gczsbejoe.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gpwjpriwc.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gqphdwjny.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gdqrdhqsl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gsiaogcay.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gmssopmyc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gfhqllilk.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gurlixchx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gsmbkqlqs.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/giybkutzl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/glflkbuqu.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gyzmsfbqf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gdzkkgdnh.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/guvqzjqtk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gltwjdhll.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/glgbtchsc.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gcpiqliid.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gpyjbppds.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gkkpqkdzh.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gqzhxdzfk.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gxvptdtsv.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gakdsasag.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gwcofxegp.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/ghgntrwxs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/ghdjxicjh.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gakelsmtt.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/givwknplf.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gcrlrpxjx.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gttqkbtgq.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/ghbsxtiof.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gyorsknvl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/ggfkwdozo.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gioooncsh.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gdhsnqsgq.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gnamgbysu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/grfuszgvw.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gmocmrsqi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gzhmhtagr.sHtML


<!-- 参考信息 -->