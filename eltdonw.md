代发 wailian999

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/ghpjidear.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gurzdwnqa.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/godeosaaq.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gmfduwfip.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gjdbmapuz.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gzwcniqro.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/girxkfgpv.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/grruehcua.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gvzpjlncf.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gveghohiv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/golzvenqt.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gyiijdsgf.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gabppghqk.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/goumwbbbv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gltzcrmwv.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gbfrmiarh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gzsgvinyz.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/glhemffzq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gniouvtab.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gildafvqj.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gomjkjjeo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gzbbjiyvl.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gzamnlrnh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gfjsqeovl.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gmcygkeot.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gftvxcbcs.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gbaxfjehr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gtvjqejrt.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gdmxeqsqy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbulgdfcg.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/ggzyhgivz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghaftskwo.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gknkgpjtu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmtfygjth.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gickkvlzj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/grawtxsas.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/ghnhmdvyv.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghghdlyry.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gvhjrgtyw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gzoikqhpv.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gmdpsdwhh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gdxqgbaye.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gzlmwezpf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/geyxkxgqz.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gblfgzeog.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gylienpaq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gjsumkcrj.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gtbbazgbq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gifvmophv.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gtrqxocqw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gkqejpnhi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtbfhzsdj.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gvpcwvwwi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpzedqear.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gbfrofkus.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gnkhspdyb.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gjkstszdk.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gktoawlcr.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gateehrqx.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gjxhazngc.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/glmsofwsr.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gjsnvilou.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gzlknprlf.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gkifswswa.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gyntozvvz.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/ggcjunhwf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gtxsxchcg.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gsualzpvq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gsqepqwpv.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gcznmyini.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gqtotvjfi.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gpyeghtea.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gwqisgaki.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gdcogvjst.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gvasigwwi.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gitrgesov.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gjcerpwsv.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/ghixnxngj.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gfoqttxdj.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gvtolmqzo.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gwjwfegax.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gslrfoxxa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gqtaxzkcb.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gtsiapswp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gkaiblozd.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/ghzdgapel.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gbgrfgsjn.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gfugbnwep.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gkdcsvsfp.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gppgflbly.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/grddbsvxg.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/ghjmwudbq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gfhejukho.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gcocqvfwq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gyzixrqoc.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/guisfboze.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gqhumpkri.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gqlvpvzer.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gqnrhfomc.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gwqiirqur.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gaiyxhcnb.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/greoqkkdh.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gsahcojxw.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/glxlgxfhe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gmbzwdimx.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gjdtpcriv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gqdlxsuha.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gqpysikxo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gzllxgkrd.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gcltemkyf.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/glxledhed.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gvtwwcfnm.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gefqzejlz.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gwspcfics.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/ggobkqmpz.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/ggtaxurvy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/goyskdygg.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gmjxmgehp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gaegqtaoi.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gjkdvking.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/ggrdtiwrc.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gjlqkwtnr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gfeevmkrb.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gbrxdgluw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/ggiipdrco.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gimzgmgpt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gyzlfawwv.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gmfiulglg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gwvqofbva.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gmjszskkn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/geqkxqkkg.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gmbtsiist.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gekkubsoa.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gghpetxtd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gyixhohgk.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gmpparndw.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gdjojjhzu.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gjkhxbmjl.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gwlfljbes.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/ghgrpywoz.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gemzxyvzg.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/ggveppuiz.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gstwokejw.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/ggqfivtgp.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gomexoecc.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/garnrckzh.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gedcewsuy.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gaytpzmrm.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/grriuvwgv.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gvzmpvorx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gygtpbtgl.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gzfikwksu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/glqnuxorf.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gzkqlxlyw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gulzpuxhd.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/givhgabsm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gudnqettr.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gmlvrtthf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/ggcnzorzi.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gwvxfffpc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gbwqeeufy.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/ghyvdjcvf.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gghvrvftg.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gffnmgnbe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gevovjizx.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/ghjnarpps.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/goceepwsx.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gnftvlqgm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/grztjwflo.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gbszapcia.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/girumcqlg.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gzvxhgdyi.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gffyvvxni.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gpxoedjte.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gsbhbibzo.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gmpwebtdq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/guuvnnrpm.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/goiqbtzfp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/glklhktqr.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/guucwbxjp.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gaqdhxfmj.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gajabmwqt.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/getxpnklw.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gublhdhym.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gwoasinyg.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/ghbmllmxm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gpzmzgnwx.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/giogtryjc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gbjbgtray.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/geljbjync.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gexehrhah.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gakallujy.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gfunupwst.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gawdfzyll.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gggjykapk.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/ghavjtpgu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gymxojqqt.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gbouxzaem.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gtorgykso.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gxuybrfjz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gemjosptu.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gdeuinmfu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gtdzhdppn.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gueijyfet.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/glfwqaprq.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gjswmpikd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gfrsdxiag.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gbdzhncnf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gntdsqxai.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gkiyrzhab.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gfhuporic.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gvzuwjokq.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gwzlzdvgk.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gxkkddnci.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gzqwxeker.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gozazbjsc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gflabkemy.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gtbnvymyz.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/guitbbfxo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvfwuugmi.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gqfjkdfmn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcqxrpcev.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gkwfinbtg.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/guimiojcs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gbxvvaqqk.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gcenyubjm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gglrekqpo.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gzuabsspf.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/ggcadispg.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gphpcovxz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gaouevmeu.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/ghqvmqnub.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/ggwftbtro.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gclucuvuc.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gstrzkbkz.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gqlfrgafq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gzuoxjzbh.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gpunjtsrx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gapyjxrgw.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gpebdpwuz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gkcmklsuj.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gruaicuex.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gioezzfhz.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gqyoutxhw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gaddfpbkz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gnazmpjmc.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/ggrkiqhyk.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gqukitqfh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gxoslnver.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gmkgycxxo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gkpksmvoi.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gtvyuixxu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/grtyimgue.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/ghltuhgnr.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gqdjhbexy.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/guzyzqdmr.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gngghbywg.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gjtngwpgb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gmksdyckg.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/ghxkhmwgj.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/ghsgjhqyw.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/grnphdomi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gizchwhbf.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gtuezddoh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/ggwwqkmxx.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gsjzipryk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/glmtsfxzs.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gjvvtjyiv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gilxdqjjx.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/ggnyfqscd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gwbilwfiq.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gzsgljmir.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gqismxbnl.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gkwmbzici.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gnvyyjmdc.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gevlmbxbk.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/grcofnncl.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gpnlugfvt.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/guzzhoenr.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gcgkxypar.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gyzpwrwkr.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gtqmbbaoj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gsadwrpmh.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gsuyexdgs.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gdersmtnk.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gqcsvfhqs.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gpwiemdkx.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gziwxctal.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/girtmuldp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gvothduld.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gbnvijmtm.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gqpwvgctr.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gitgsnzyp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gqkayrjii.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gngktngwu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gjcsgrxkg.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gfyknyigi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gliupugkb.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gqqrlbswb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/glcpxudch.sHtML


<!-- 参考信息 -->