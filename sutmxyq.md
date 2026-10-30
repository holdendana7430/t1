代发 wailian999

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkaqdfxx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghbdjhvw.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/glwlewujf.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmarehnpc.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkgadxet.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmyzbgsn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gspohltay.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/ghxkarsro.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gomqlegod.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gdihbpqot.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuyfdhne.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gvlavuykp.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqowcysca.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaghcboh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gtitpscid.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxkolwks.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcilxdva.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudkomsrw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbucqivuq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdpfvnmi.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gmpqamjea.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/guemwcbex.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gyacybxjf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/glijxhcdo.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gvayheeov.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghuasoei.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gwviqcobe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gnhtruhrh.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/grrfdphrv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwqtjhgkc.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gnvrfazjf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/giqwghpeg.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gmqpsflmc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gegjtzdny.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpklirlva.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gokxwnwel.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqrluhmx.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggujouvde.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxlervbc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmurfqypf.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gyxrnpjae.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnkoeaaf.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbzcuakd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjygweki.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxapjiwk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiwqscqj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfaymmjz.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gttnvgeko.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gzpqbuiwy.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiabwjrd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/glzhpocuj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gaetqmpyq.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gbucpwsne.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvupheuqz.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gqggklzyd.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gwofcplwp.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyfjxaoh.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gyywugtic.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnthurop.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtsenstvg.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezrrfojl.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjaxgxyp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcjohhxo.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuavfymb.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcuwezzo.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/ghfnvegsq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gscmlypey.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrcypmrj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/ghhpoqgwv.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godbrldva.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemsdmyzu.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhhgcwxq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gxqolqjja.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gkunrtdik.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ghjkszlxt.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/geptdrlgg.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/goemimjeb.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/guolqoiog.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkyxnkmx.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpytuxrhr.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafjvwgkm.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gypgxupsz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gpyrperkb.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/glhmcakko.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ginhqlcuj.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/giunhlvmo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqdpgtxo.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkhrtmahz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geigogoob.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gozcuxwdf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gnteliodx.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gnjtawcax.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzepbzpvv.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gjytbeosm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gudgwjwxx.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjhrfccm.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gdmimchpd.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gkcofphwe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjimtrlyd.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gwuizfrih.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbxcmvdx.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcosytigy.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gelyfltjy.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdesxuff.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoppvdsc.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqljtjda.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/ghzktvkjp.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gotjzcqjv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govsithlu.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwfjwufc.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsycrdgad.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/geuyozfzk.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjknddlw.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gtjcctdmc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddvdfhnz.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfnicuql.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gvocklwew.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gsgvophca.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gyvbhawjl.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvjefjyi.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkrgonqj.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyjxhujx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/glfidsmxa.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/ggohxesey.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxogidgl.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhbjebsz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgknhgbx.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gzlutlekn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gpmgavaus.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbcsmqqe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gsguwthzr.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gkpdhdksl.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpqwhszw.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxjaslla.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/grvnjqtmy.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/ghhraknxd.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gxodbtoos.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfheosea.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkmgzuzh.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/guzmcgleo.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgmcbxtq.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/glgoujceo.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmgofovj.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguzrsmfi.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gsicjgtan.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioswshbw.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/ghskgzthq.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gfgxrlffh.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gooabrgoy.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkhrktmj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gmhpueeni.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlngvtin.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/guqnhoitl.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyaamuqg.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gfxthigte.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/glufjnrcg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyqsjkyr.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflijjhqx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gcidrfcyd.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gmuzgpvti.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhougbbm.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gyghgwjrv.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhmsbayb.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gwwltmxby.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gsaqxmjej.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/giimsdxis.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnddxtwy.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gvkisozeo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/goaezhntq.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/ghqqvjxjd.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlozhouv.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmgsupga.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gqbriysjv.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkreoqfwp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gedpuseno.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzdcanuf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmumubetc.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyfasona.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gvygdiiuf.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gqswovzhb.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/glgkycujg.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gookdapgm.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfyazvcz.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gaixnifxf.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/giguyqjqv.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gqzoejtkl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gasxxsjeb.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/govcwawwc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjzqhtyo.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbqiegii.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gjdrhckjz.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gocnbavcm.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/ghinehacd.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/guvztkgno.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/guhhbxlhp.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gsrfzstwk.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gnetajpwu.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gkwahnimj.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gmzfrpdyp.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gzywgpxau.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpfluwfk.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gajjyxfgv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcpghndin.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpticgqms.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gquauizfg.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxvqkpka.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnflimjfs.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhqkyzjt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/grgicmpgs.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/ganvhflur.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gfabhobvo.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfhyncmu.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gmseyncmm.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtuhvhtx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwexindez.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/genkgjqbc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiibawlm.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsdwbfcx.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzqcemzy.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpjjkelb.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gxngixdeb.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/goyoitbgx.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gxjsdwsxl.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gkftaytjv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gweodgszl.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gcenpgazc.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gccfodqeh.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/getzklcar.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauwxwzoy.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxjselvk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gufwcpmys.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gwrziuwta.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/goszhkhcb.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gdisuppys.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebwneyoq.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gabzmzhgf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gaashmrai.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhvqvqam.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwpkzeyp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/grlvzjfwc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrzdmglb.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntfrhkbe.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfomqeiy.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjlndcjno.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gswgojnqo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdqqurer.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqblkfrhq.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gasmjkbbv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gabxwitfb.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gkqqlsiqv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gwtkblbyq.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gpwfdjwuk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/garenpnwb.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gwcrjtcfn.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/ghpaczkdi.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmwgjuql.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfetojxuz.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/goihzisik.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjyiyzmo.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gegrysooe.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gankzaqwy.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusfnexmm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/glochifig.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/goycwdadx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gnthdyzfk.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gazhuvhwi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyfxaxkk.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gslgywbuj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggauthwcw.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/geoiagobz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gwpupsiby.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gzqypifny.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gooriblfv.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gkufgizdh.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gexfinsmv.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gbgfgjjwb.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gnhcuzixy.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/guqiwsafd.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsubbwbr.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/giamnplkn.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqmaqlaw.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqzjlmrd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhjcwfwq.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/ghfpsivax.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/galspdfqu.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/grgiqxbxv.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvylsruu.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmmphqen.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlvskfmq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdylbbnah.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gzypzkzki.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/galbxjudo.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvqvmjnw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhnjcxhs.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/grvelhvdq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrkuaimr.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gkhtixxld.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqipekdm.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gwnspwlhp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gseiuyuna.sHtML


<!-- 参考信息 -->