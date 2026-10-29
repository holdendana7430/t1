代发 wailian999

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gotrmmztd.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gfrguwcmk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gkjufuewl.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/giazsgrxe.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gtvylnnrp.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gdlnuhngx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gzlmidaux.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gstcvbllh.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gcoywphaa.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gmtoefeks.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gfywenemd.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/ginrwrbyj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gkkyaewzp.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gfgtxoadc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gvygkajgf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/ggfayvaho.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gbtrvtabn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gslsbqcmt.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gixqllhwn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gnjolwzho.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gweegomac.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gvustfwrq.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gutphtebn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/guooxthzb.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/ggbjcklbf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/ghgbkdfxl.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/grjigpxxi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwfiwhisb.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gvddcjsas.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzjxlgjfc.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/ggrafbbzp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gipsflbzl.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gibumiyys.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/glqlwziwt.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/ggdibncba.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/grqjwcocl.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gcmliqgbj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gmzljxdkh.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/guubasegy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/grwbyjmuu.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gdtzujnyb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gtpuwobgv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gxdhhycyx.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gszjplzne.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gijefpkcs.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gtclflqot.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gfcjxmxxj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggelnlgtq.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gcttrunvv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdlyupswl.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gzvagyxpe.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gemzjccwa.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gnerihdem.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gvdxlrvkm.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gbhdsxbjz.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gkzasteyf.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gaxfevblw.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gxjkbitbi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/glvdltbld.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gjtwoggmp.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gvwfsfayc.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gibpcjftr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gbptmlttp.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/godeywmmj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gmioarhxj.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gdgyjltyo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gisqmphdt.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gsykyulvt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gbehdchew.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/getbfzeeq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gqekdveii.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gbydqsaos.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gtkiowwkv.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gayiwihxs.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gqhkftief.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gvobcmyzb.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gogairmiq.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gprcgwqkr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gbszvjeem.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gfeecdaci.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gmluuygva.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gvrkuvozj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gzwlwcfig.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gocsnhuoe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gxybflhoj.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gmnxfurvt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gnbopqeig.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gfxqwxovl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gdjjmjfzc.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/glgmtewnb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gawzzbctk.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gdqgxkwoh.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gpwsmuocd.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gwfrzwydr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gpawriqnf.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/guxsdermc.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gfrkztpkt.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gjdamneey.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gjqnvytjf.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/grzyuprdg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gzxolfqel.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/grqhtrdss.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gejmallvh.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gausgmogp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/geithqcvv.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gagaxladb.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gfogntftb.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/ghahxmlpi.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gbmsjieby.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gccgznisc.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gwvbwuzzm.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gwngfhjwp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gqebwsgej.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/giraprsbn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gsoiaxaes.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gcrcqqjel.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/ggdlknipy.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gghauatvy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gmdgrprwq.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gbaqocjvu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/guomdqyxn.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gaerxbckr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gfhccnkgs.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gidjgiuzq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/ggxdlrzkf.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gkrhnwvts.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/glmimthol.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gdvsdpmth.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gqtbjcgzb.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gklyipcep.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gnlcmduqq.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gfngszyen.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gxnvpeynf.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/glpnrmteg.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/ggqptbuip.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/ggosgmqpr.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gupzjiszg.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/grihdihot.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gjcidtsrh.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/geprrphqk.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/glrhirdxr.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gjdznealf.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gsvebeflv.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gjpmxxixp.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gcdelkmvp.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gvsbizuzw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gosrymgsp.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gpyjdrnnu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/guvebqaqg.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gznkkmqxb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gcwbgatap.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gldvxfiqp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gguvpnasp.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gnslcohxm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gtqzcmmls.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gpwqqlheb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gcnwzuwjl.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gavahzrfh.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gybdzlujb.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gnycjmjtt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gicwazrie.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gmbkasnbc.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/grsebeuna.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gudqrdevs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gvsvaolbm.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/grjsgqsir.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gjyjvnhgc.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gtlmuiykw.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gozeenuks.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gktqxcswo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gwoybppjq.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/guhfpvxsd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gxqprfpgf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gpnjyrxtj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gcxoyjxfg.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gpvduvkii.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gdkhxjddy.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gfciwznel.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gybuluuih.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gjdqyqnxv.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gpsboktps.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gzajlvmlc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gkosvyvbe.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/guaslskgw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gxbxrayzw.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gokqhjrjf.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gdbrnzrpg.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gltnishrr.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gwzryafwl.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gtxxcxkrd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gxxbzqtcp.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gyachtbhk.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gpqtgpnom.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gkmnguvnx.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gopztapbz.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gxtdvicwp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gwgmgstpr.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/glreprsui.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/glmrmjkbo.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gwaqmenwj.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gzonrgvrh.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gxizmlmuy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gfnrongne.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gjgvinzxf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gpzlxqdlx.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gvpikpmwe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gifzzjtdi.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/ghoeznmlg.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gfxqjcnar.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gdsyjopre.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/gucuvqzwt.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/giqtrsrfk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gosmhhgyq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gxtmoeqcx.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/grlxihqtz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guwyxowlz.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gfndumezc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gogcsrlgc.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gduwuqdrx.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gmccjtghi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gcilxdnro.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gbrqpojkm.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/grtuddikf.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gsgoezkzh.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gwwiwekea.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gpecjkokv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gbmznafhr.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gbdbgifpa.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gcukmfbrh.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gtuzlatbf.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gtkqmlnmb.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gpcsabpqn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gzojxqnzu.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/ggowqqnfz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gagiqcohx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/grxqvawkw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gqavrruxi.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gdkeisoiw.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/ghsjaxozy.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/ghmdzulmx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gimyjovnv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gsqqidpws.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gwqrgsykz.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gehiwjrjf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gbpzwnyzw.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gqgdqmdlg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gswnufmvy.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gcatwjdvy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gdtedcnzc.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/ghsuvdiyg.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gvmzaiwkp.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gdwppxjdr.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gklislfzv.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gedkxpssz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/guuurtfjw.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gitwzjjcz.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gtwfkcfyu.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gqyymmxue.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/goufrdnvf.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/ghmbduewo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gdifgjlgi.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gxdzengzs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gqnjevumx.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gyxgaloid.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gvhotqkmi.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gsrqjkcnv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/grwnhtokv.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gsfrvpdrg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/goltudxhj.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gbnyyrrck.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gilxwtccy.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/ghlvkflth.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gkykdttoo.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gyxxqkzct.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gzczsqajt.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gfpnyldtf.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gzuhhrrxf.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gnirgkfkh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/glfxzfnaw.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gzczwkcin.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/ggcwslate.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/galywkkfn.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gvgpgmdje.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gubfkgqcf.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gxbnbksad.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/glqvicqkk.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gxpivsagi.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gkbdmtowy.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gkxqlzgjo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gtpntzsdb.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gaavxfltr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gedqgjhsy.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gflpfbbmu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/ggmsqenny.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gayfrwdll.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gqlhdskzo.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gjuupdnln.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/ghxecmdul.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gffwiugau.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gmlrljzvr.sHtML


<!-- 参考信息 -->