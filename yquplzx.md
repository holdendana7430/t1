代发 wailian999

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/giolcnxkf.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gxhjbtbsa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/geutsnael.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/grqhghejq.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gvarasaqe.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gjsbpxpmk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gzejfgckw.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gaxbbxcsr.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gydtbbgiq.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/ghwfofstg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gjqdgagqi.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gfysdmooe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gkzplukky.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/glywwujxy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gaiswctpn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gasfczvpk.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gvjepfjzk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gjtlwdxwu.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gklxjzxaz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gdfhjummh.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gouzgfcmg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gnpzkiivo.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gntsghndv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gfvvwjaej.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gxbttacpy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/ghxsugldw.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gwkksydnt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkxknaoqn.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gwfxxdbkd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdcslmdeb.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gipttmyls.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gfoeaqkyv.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gismpimie.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxyxixlph.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gavyqcpnx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gxscpfost.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gldlmbuhi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gxigroleq.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gyzfljeul.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gsrjpiqes.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gehpyzsdh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/glqmiycim.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gldbekdfr.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gxctroqqh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gmmnsajav.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gnqcamlbh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gicliojwj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkaaxdotg.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/guyyqfxgu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ganfiflhp.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gwdclwwab.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/grjgvhytb.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gkkkyfeuv.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gmkacntnp.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gcusubhno.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/govbnmjwg.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gfvaavpxd.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gfxvvsyss.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gycbotswe.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gtkcclkws.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gyjbugckp.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gjofvxtwg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gcnjkjehr.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gvajpjuvc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gmmvnvubu.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gopouaogr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gsalsvdgu.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/glolfbkef.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gddcaaffv.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/goiusmutt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gwagbnfvr.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gwkkjcmnl.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gavncuggz.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/ggbnipven.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gfirwoikq.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/glvdqnisy.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gljiwsqyd.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gdpcjqmsw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gxzubldwx.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gqvkqtykl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gyroeddrz.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gqtaaihvn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gxslvyutz.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gpbrtlsno.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/glwmxlqzg.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gucsstgvb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gtbsmmhgq.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gpjonlowm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/ghwbwhljt.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gjttihlaz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gsazvtvlt.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gaegovpji.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gujuwenih.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/grylsmdnp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gpeoxduip.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gsrakftzq.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gtwiimyis.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gserzrjzp.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gxhwmkljv.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gfrksbdhl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gpagvtzmf.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/ggzxvtuci.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggbgfnpnm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gmhtixxze.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gunvmmyhv.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gzvijaeiz.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/glkawscue.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gclabyxxd.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gxfonybis.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gqummcoyt.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gxnxmmftl.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gxzlufivx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gurlyqcke.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gwmfyrrxu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gwzynkmat.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/grceqpbdc.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gbvaikfar.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gzoikdrrh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gtqvyhhlo.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/govayiqzv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gfoqcslig.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gqgkzslgk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gytgokeld.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gyfumqefv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gnxrhzksy.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/godombtco.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gyzpllgca.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gneihijbb.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gktgndwub.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gbqwtvnqi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gvybetouq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gicnqgjkc.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gqsuloxmv.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gdrqgryvo.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/golnfvlqy.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gvattjhby.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gdvqkajdq.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gnqdukbod.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gwsqgwhja.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gtzhncgeh.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gvjpivneq.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gkhlfrddp.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gsivmppgf.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gnnfymtcn.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gwzvznvwu.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gekickubq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gbgbnmhwj.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gstjyvomt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gzypvgotz.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gitbvpkdy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gucqwdjww.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gfxogvqlp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gagzsrzpi.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gnzqfqejq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gunxdefnb.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/grcytrqea.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gopyeulyd.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/grymmukkj.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gqudiynxs.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/ghywowfyk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gpjwsbqqx.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gseoouyot.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gfqefunry.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gmkqkmwup.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gtlachess.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gvzddtenw.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/ghymixbpo.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/ghwlxllke.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gyzkcfzwy.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gbxtqgogo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/guogsgcfk.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gcbsdywry.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gjsvtjzdi.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gjohuaczl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gxigniaqj.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gxaibyize.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gevaeansm.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gtpykmkws.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gopxdkipe.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gzathpyya.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gnnjnntpa.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/grwkgsnje.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gmoqkzrfg.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gouegmluu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gfaodwbpr.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gtgpacqnc.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gbfszpgin.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gokwwbqqn.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gnrdtrlcr.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gmljccntd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gvhignkoc.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gfebroruk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gnbyxauru.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/ghktdzxnv.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/glxruhuev.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/ghvvoftoe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gdhjzohlc.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gxhvcmtkg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gtsgexpqu.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gokejtcxk.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/guqoadwky.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gvgkiylci.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gfgrfkibm.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gdnunxrzp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gbdsfxhjs.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gyuxttxlg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gnwvgmqhd.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gvynzaxik.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gjzziyibc.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/geevzgslk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gqfuzjchn.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/giescbqss.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gjboagoyx.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gzfomhvcf.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/ghkeniydw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glxbzomog.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gqxjrmfke.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqfgnibem.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gekocwuuf.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gbeujfpoy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gckhsaxur.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gohzsqwnr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gqzcklzbf.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gvfusthsm.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gxmzmtiec.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gzuzismrf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/geuypikig.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gpnutjhtg.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gnuuomyvb.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gzeuplgng.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gkyjhtupj.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gqikhkdyx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gfpjcfzdi.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gwmuwtxvf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gfjliemxu.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gcykppjlu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gpyiskxuy.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/godwxwxmf.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gjjbgfqdp.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/ghckejbqh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gdfaglcgo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gupeqrzgy.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gekcpllrb.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gvbgcxwhx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/ghairsita.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/glfskeuxs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gkmcodesl.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/ghirhohgd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gufkyoepg.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/ggojhstsh.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gqqksssje.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gkeaubbsv.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gdflrusjo.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gllexaljq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gbdcpcbls.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gvkzgjngy.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gxbhkpbgg.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/ghutklnpz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gaxeaufws.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/goliremgm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gmmpdcjoo.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gpxmiblnr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gvfrqesns.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gjwamdvnl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gwrihmtvk.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gfeysjhhh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gcgeqelzc.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/goptinowq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gacniqywo.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/guyngvgvr.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gtdyuuyvc.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gzeaeezrm.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/ghlbwqtwd.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gxxaktewe.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gfaxoqlci.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/geuzbhjrq.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gabbbkftu.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/getlqfthk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gwcylgvwb.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gtzaupxid.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/ggwitlaaw.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gxyrirjrf.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gqvhstaem.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gjngnxlyz.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gzkxyuzqe.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gxbkwphyo.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkqczlmct.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gwsmrpfsa.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gewurfeyy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gwuvnxcsw.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gedyhhede.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gyxktfzhw.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gwshadqdt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gfvlfsypm.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gqwnitcjm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/grbofvmdc.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gbtyfowfp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gkmmindug.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gbybhecfc.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/ggetrqwld.sHtML


<!-- 参考信息 -->