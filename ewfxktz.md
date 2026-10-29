代发 wailian999

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gejgvbcgz.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gqrxuijkf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gupsixtvr.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gwbebkkce.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gekdnsehq.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/ghspvuucm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gjmrjdhjt.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gqpousieb.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gnclozfov.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gnzhpowwk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gjvcapnxh.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gqkqniyfp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gdnesixdu.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gegywwcgi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gdfeckmau.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/ggfdiggce.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gttijpfcb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gxyhnxiux.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gyvcluaig.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gujanzbnh.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gvqtxqfye.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gagjskuag.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/ggjwzrlod.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gwcvrbcpa.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gjcmkslhy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gihojoqdp.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/geljszdwo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gyvpqlphl.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gveioedpo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gqywwzbio.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gturfxpba.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gemdtrpvb.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gzzliwxau.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gebrvxpdf.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/ghhvqupak.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/govirqtox.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gantpjufa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gdldlkglo.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/groyoeton.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/glqnkqwgh.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gpzpxtlyc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gsrvvuczh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzmvtgwmv.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gegrnembc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gegvkwylx.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gkbrrxgvv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gemzlpbqf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvulcfvjy.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gfapruvka.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goubkjpdd.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gbuoaghlt.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gazxcnfek.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gibvdvxir.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gplsstltl.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/guvdylbzg.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/glseaupxp.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gbuhbgfcp.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gtczbmzfk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gyrcvyucs.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gggrwckwn.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gbuwvzaut.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gpxfkvzog.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gcbbtvkgi.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqbvznzun.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gtwgmjhes.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gcchevqqr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gmwjvdykm.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/golsnoabl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gkrhdgptx.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gxfscrbwv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gwyzhdooj.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gsdfchxey.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gjjbquaot.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gzfmkgqit.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gwdqtepyz.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gsgdoorlt.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gvyojawxn.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gntwomxjs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gqozxtzje.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gursmexdx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gcbhcvgil.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/guqgmxflp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gzizivied.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/ggxlnhetb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gqbhbscmg.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gioazvwxi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gjklygtpz.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gxjuuarur.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gvzoeurlu.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/girtpcpxk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gxetweoho.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gkrpyontq.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gcphclndj.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gypxfnqtp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gbkeqlmjg.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gzpwtbjvy.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gdhmrtotu.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gtoudzsih.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gdbofigil.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/ggrngdmfu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gjtxnxriy.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gtdyceehm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/ggnypwlur.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/glegthumu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gonpibbiv.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gthezfvhn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gsmfwnzud.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/glncaaatq.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gvaubjxrc.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gvbdjgefy.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/glemjtdij.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gcykjzvxy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/ggailytbl.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gvzksqgxn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gfdrcfxoa.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gmiahboej.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gzflbtyoy.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gcarqbqme.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/grfnuzbfm.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/guzanxaoc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gzesotzzr.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/ghaqzvazc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gtgmngyls.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gxqsizrnq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gdpdsrdnv.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gefqtxojf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gbtslwmwt.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gmamffhxi.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gsbwyxguz.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gmqezcsxh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gtyffqtjo.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gcswqiuqq.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gvlyxttaa.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gmrkydmun.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gerhunotz.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gpsqwbsmt.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gsosqklmn.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gnoxmhken.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gipwgrjhz.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/glrhrgdfq.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gtrzivswr.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gpntxxheq.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gpbhmushm.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gmqxpoypm.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gzlkqmrnu.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/ggvjyhhyh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gpgqstdnq.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gzqeijtdj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gtygvkaet.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gmlqhakrw.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gyurggtty.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gwrbyzdrc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gxnqdiicx.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gtyodhrkc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gcvktzacg.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gpdeglqbq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gtsyxkgxc.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gslmzjqkn.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gkrnyoyiu.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gkfneicxo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gdoaoqucd.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gsueoxxuj.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gajerfkpu.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/grkqztqic.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gvkjicyiw.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/grgoskint.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/ghllhzxck.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/ghzvsghfy.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gplppioqm.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gppdkcasj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/grsnyiljz.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gcozbrvcz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/giwtbsoox.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/glqaellfw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gjbgvhczb.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gtshupfmh.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gnfugeybk.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gsdlnmiog.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gayboejks.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gupczteia.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gojsuicjq.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gbnzcfdtz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/ghwkbjwrv.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gpgujythl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gbdvemmse.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/golvpohhn.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gjothzzwx.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gposwfphj.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gfqyodfga.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/glazsgbge.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gmiuyycsy.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gzyxagvey.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gqbilvcfq.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gswarigdg.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gcwdtfhgx.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gyywufuqx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gaazcsrdx.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/geziawvjw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gquipxvaj.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/grxmlitgp.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gidztlskl.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gcesrhhzk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/geprstgym.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gjklkceot.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gruznuuae.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gymhjnbuo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gljgpfslf.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gdtdvbqwn.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gyybieoii.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gyxyldrkm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gqxscozfj.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/glavnfpnx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gjwsfcgbc.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gmgyerhss.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gszpvyibl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwgjgbyii.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gzbmmjctj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggtuhlxkx.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gzhfbmmjr.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gtxfjgkvm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gmdqkyiyo.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/ghbguhsit.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gtjdzmilw.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gldipumgt.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gmfgnhhet.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/ggfpgufxt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gbwxgxxxw.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gxsnzijxn.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gilgfqusv.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gnjhsntmn.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/geyonqjzy.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gtztxeksw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gmzjyqrwy.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gbalxiemr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/guhgkxutk.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/ghmrddrrt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gkswnsehp.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gchuxjnvl.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/ghmrnzmzz.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gvhyznzcr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/guybgfmns.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/grmcjjqgi.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gyejkkocu.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gaiuzegbv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gnjngdneo.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/giwhhztzx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gelshvvmw.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gytondcvo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gfhemlyng.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gexxdjipt.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gmuoolpfl.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gpvgbrork.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gpzwbvkzy.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/glxbaanqb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gdtmkgoef.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gtdfjvgba.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gtksozmsq.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gflmhcjuc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gttcforeg.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gkacmspai.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gbgmnhvms.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gqxuvyclp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/grnktkpiv.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gksfdusxs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gqygktfhk.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gyievjuss.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/ggnrpsoie.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gfilfhlrk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gtyvmomgn.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/glntwcnxy.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gblixnhyt.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gfxicdehc.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gzrremlek.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gqgckfaip.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/giswbcbcr.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gdndbcqjs.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/glszicncj.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gisxqiexk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/glsfkjhij.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gsgawpdld.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gpzfgfakm.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/ggpvyqmff.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gdhwidutt.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gkkcucouq.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gsgirwzwv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gqmtvceqp.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gchwjiszu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gquylifrl.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gwsfrkiub.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gsorcaybp.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gbtyjsjmw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gxxgbmwfh.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gkfwuetzl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gyktwjcst.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gbtqnvkfu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gsfotxxed.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/ghkzmdbxc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gxykowqwh.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/grodefwjf.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gpjafoghq.sHtML


<!-- 参考信息 -->