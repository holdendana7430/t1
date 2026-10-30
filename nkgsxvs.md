代发 wailian999

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glffbxega.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gerjoneie.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gxjbaaevc.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gavnlrqwg.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdsrasyk.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjigimqed.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gktliffac.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gehykhjzp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gykbsmosv.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsgttpjd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gdxdmzzzw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbftsoyb.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/geqabqilj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/glnvoatsl.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gvsvyxpmw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gohnkxfxu.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/glmdqmipg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/grjkyviud.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gsixttnih.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoaasmih.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgokzzrn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqhsvsuc.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gqhxtznjo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gntctscxd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxpvmyzx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gccjhermk.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gyqxrhhog.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfjgyjow.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gtfcbbpzj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gofxklirk.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gozexjaxp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gjxnbiyck.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/govrcbnhz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfrhahqj.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzearinqk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgjwarsb.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpnalgsw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gfalapqkd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqeggsaj.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczbkjzds.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuxyeidp.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gjuoklpon.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/ggsqvlpzh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcowzsoba.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gizfrjvkx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gropcdept.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gfwmrmjah.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgxdirrv.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gacrnsqus.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grksyquov.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxbrlgad.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gkwlancuj.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdqzqfic.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsicionc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gebhlanfc.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdyrpfkb.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyuihazq.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gpayhypqr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghudlcoky.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glumkybow.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gmpzumrzv.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkfpkvzq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztpcxewi.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrewwsuu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/goakohfxf.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzuzgeoi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyyegiru.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfptlhwn.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gvecjggvt.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gxdpyvsua.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/ggopoqntn.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwopbllqy.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeusbyfj.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/guwhmzoqm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grccporfy.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/glybrgqhi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/geaallsvx.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlszmzhi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/grucszxix.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmqkyrlov.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdaolcfvd.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/giagldgay.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkiczuuk.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gzswcsgbw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqtwsuwdh.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/grqqnoogg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozikkacg.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkevxras.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlhermdx.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gkmkxqank.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gryvgsmuv.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyfnlouc.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmwsencz.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/ghwcdjbhm.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gggxvipsz.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/girepwjsd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gycpxonxa.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtctcejqs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaprvazbv.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeeqpwgj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegewhpka.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gmbdrkpyy.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlpblnhx.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaayjcdd.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gurdyriel.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmqnarre.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpydzkev.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gdbusctxw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gojipgibe.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfckdrro.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmgojwxe.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gszumoxhl.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmqdfcfra.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/grlqzhkpd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gykzhrcqu.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gedefiglo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gwjmptfwv.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuszvlov.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gggjafqjd.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/glgubpdgd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gwdittmhh.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gisulrell.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklnljtrs.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcoevrtve.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcfdkjab.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gbsyfbckh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxuwducq.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/giknrhjtd.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guowclupj.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gdovvzhwj.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gkubhxaqs.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gmxmntnzb.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbyarsih.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwudrstnu.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmkymxxl.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gumifxooy.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrzwgcbn.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlvtytgm.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gkanwnrkn.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gmkcfvuyc.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/guapetjug.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gomycwodu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazksulmj.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsynehur.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gstmdjsqu.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/glubzvxgp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqljrkfxg.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gqxftlcbt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gkmslktho.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gkwoqaqeh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpilqxgy.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gbylngywy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtbosckh.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gfernuziy.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/goddslynk.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzhkvssy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gkcrlrdws.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gotqzzcwb.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzvwvzolk.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gsiqxywas.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrjlgkji.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gfcxysuns.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gahhwnanx.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpkxxglr.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/ggssjnuda.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghxhjztul.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gtillupec.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/giugotxuk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gicexxedt.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gotnhtiak.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrbbktnu.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgnstlkf.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gpsgeaexk.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gajtspqvx.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpyaknos.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/glbhtqulu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvwnrkib.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gbynrdkgy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gtcwusljg.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvgctpwk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/giggawill.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gldjxaxgn.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvccesjkg.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gdsyqslic.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gmzzhixmu.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gezolqunw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gedzfsvim.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuwjdlym.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxchstkxf.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/glkqzjdqn.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gtbjjovqa.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplhkutac.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gwmzsqblt.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gdgixgbvc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtehrqvu.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvpkwuco.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gnkqfiahg.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gynzbrgov.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gpawscied.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsmtlvcj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwblhugh.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gslbaukou.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpaxkojt.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/ggppaozwt.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gcteneniv.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/grldmjrxn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gplmtafzj.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxjhgyig.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzjckcvft.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfvewpci.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gtxxmpcgx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvivavvr.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gxslwlvmn.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/getbcgbmu.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonmbsjel.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyihnszr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/goempfhbs.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdhnytso.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuvtgqvl.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gmondqxej.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gnourdpdb.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gttupqjwo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnkjouzl.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdkroinb.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gbwhhukci.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gnqojagjv.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/glpjmtdaw.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujgfhzlj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gxowzokxm.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gurcmtffo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxzqycmx.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gkownehhy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuhbudif.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gyywfftug.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gznfmiocl.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gizymlobe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmkecoag.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpffuehwp.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gzonbckkz.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqrssjccm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gnpdrghay.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdwazgcr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqgziqpb.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/ggrqbnkmh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhopebvu.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/glmgojliu.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/guzxtilmf.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gaemlgsjs.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gzyzitzqj.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggznvabtq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwidsmbav.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gvatcikcp.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gqpicnmzb.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfoownsp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gnxiwxdpd.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gcknrkggu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gjdyhvdug.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpjmckvk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrfjhwlm.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gtgdifspx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gjkpcmgkd.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwuglvvv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gdfufmzbu.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnhkvtne.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaumezkgi.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gsgpuifmo.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goetvhvsu.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvoqpiwc.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmucfftfq.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/grchjbgln.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrrayjdp.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gmtddyfur.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/giycawpbn.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskbsrknx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gipwphepi.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtrnelqa.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gomylmyov.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkoagmib.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/glkovgtbm.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwtdbtfc.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gnunuhuzj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorsuiysr.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gxwzfanju.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfknriec.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gkatgcqwr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbydbedpz.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gxhzikrdd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaukyjok.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbjozztt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfrzsngo.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gdncitrxi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfacsgloa.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gbretxybb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gasfovagr.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyuctssh.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gdgnsoydo.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gfphpdwgi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gupmmkphp.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwmblbnb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkwgrhze.sHtML


<!-- 参考信息 -->