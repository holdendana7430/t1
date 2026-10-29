代发 wailian999

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gmdkhffxo.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/getxdkxel.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gjjxjxlfz.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gytsreenf.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxlwydxni.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/garzbqjjg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gexnnclsa.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gjbindwnf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gjsujbmun.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gcesowmiw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gykppymui.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gnctynvct.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/ggxczpxsg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gajagyprr.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gsdzksrvn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gnvffyufz.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gvczozjge.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gmfbffkdm.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/guhtusstk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gwloepxxq.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gqmivdolr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/giwjsabtz.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gdwovgpbm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvfpypjlh.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gzooqkdbh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gvjuyujue.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gxebgykly.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzwddzyip.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gxnjccpyr.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gpinvltoh.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gntwijszs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gzpszqfgg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gfmxnbaql.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/grgkpwelv.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/glmbxitbc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gdsbhhhkb.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gjrzzirjb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gvosbdrcm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtaeqlply.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gxasqrnrv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gowbalnjk.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gpsdjwurw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gvhcvpjkc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpeseurcm.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gmtcevknf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghiarcbbs.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gjofdrwlf.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/ggfpzvtut.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gviooktlx.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gurgywgor.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gbjsrmmzj.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gngrilrna.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/glpvwywjn.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/guwkyciqv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gkijrpvnv.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gkebdpspm.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gybymiyub.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gqdhxgfga.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gyqyvergb.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gpjinajvz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gbguewhtk.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gnjldhkcj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gupunawch.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gklxxqbts.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gkameqkbg.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gwdagpyld.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gvyxencpc.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gmweqjeyf.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gadhbapuc.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gfkyhxubj.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gxfdscgas.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gvmrlducp.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/ghvleakru.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gqebjrlgh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gyhkbrebw.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gikwzqcop.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gwvxlktff.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gaowndgap.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/glztmyxtf.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gfknsxzrp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gxwqidkpp.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gomoplywy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gajzruaue.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gbukwqhkb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gdjwxmujt.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/guevpddio.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/ghpvysvvb.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/getdluzhh.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gjzhwzpld.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gjfpnocum.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gbkvpvvnw.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gtkzqfhzv.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gdwzreguj.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gvjropymd.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gzkjtspgt.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gdhkgdqlu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gbzeljlkd.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gtfsuxxqv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gdicvslhy.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gyhjajwmi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gfmrbwkum.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gcpbyjvfg.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gpsywpnvj.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gavezepri.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gewkgaegx.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gthmrfqct.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gtrsmeetz.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gofldnchl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gevctrkve.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gaymoftji.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gugigzoqg.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gabpqygpi.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gliizwhls.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gpkuobocc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gukqpzybi.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gwiczpkgz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/grtaibtul.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gibzyaurt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gbuzavres.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gzydiotwl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gtstfjjzq.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gwxrffqed.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gxutuaemv.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gjovwlgmp.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/ggpldrqte.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gsjxeshvj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gnvdwszsu.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gdyfuybra.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gsvbiqbif.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gnpqolmfr.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gzapckfhg.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gqttpgkmx.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gztxltjjs.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gnxebkwme.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gwefrqshm.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gahxhxhah.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/giprwtjsh.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gunmrxayw.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gkbdkiloe.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gifodxery.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gzyoykuxi.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/goooeafxs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gmramvjrj.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gnldsgzio.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvebtsrdk.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gngbjggjf.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gvqyrzaqg.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/ghiinmour.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/ghmovojql.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gihqetagp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gdjrestch.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gqthiplxx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gpbabunjo.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gtoqvaicw.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtaafcjmf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gxbpgzkhm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gwniizxng.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gsjeqrrux.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/ghyqqkfkh.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gwsbyuhzi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gfevzktni.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gqhfigafv.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gzdkliyjw.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gwsalrotq.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gstofjkud.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/globgkycs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/giuweqwgj.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gsaeukdwb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gsetvmnoz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gzuzouobz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/ghhpcudtl.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gvolpmaxk.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gtfevskzb.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gfxnaiakk.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gpbhluhfl.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/geszukdip.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/ghphclbpb.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gldtkdqll.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gbjospwih.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gqrojumqk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gjkzmfxci.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gllsejrzq.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/grizkmhei.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gfufmajlr.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/goyanrumj.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gssmcmhmn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gglpniiol.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gjujnvoha.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gmmmlaayr.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gunasjmhs.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gsnuuhwxz.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gaoxdvgfz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gmkudjnhs.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gaewnuwug.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gigutevmf.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gvdcdiesh.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gyzcrihzx.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/givmeyndi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gvtoxrakx.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gdlhfyamv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/ggmrkpfbr.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gqpychyiw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/giejawqju.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gepgxqitv.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/goglwirpz.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gnmpugbaa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/ghexuywny.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gyjequqme.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/galevived.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gaaapwfer.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gbueyajys.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/geguiboaw.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gkezxkmyp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfavmpkwt.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gplzrlkjx.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gsluyoxof.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/goaupmbqq.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gsbgezegp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gtutrjwhc.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gfnlcuode.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gnusdldyk.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gjrgpevcl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gnzuueckq.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gznjierzs.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gccjazbju.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gwdqcmwdg.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gudusafcr.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gsnvstejd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gvgpwdzdg.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gbnqtimsn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gcxbbxcxe.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gwnwlzfky.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gtuspngvg.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gzquyxzfk.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/ghkyezmvq.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gzifmkryc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gyaxgjhll.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gfamcixzd.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/ggxfiytov.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/glguskgip.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gpcajpyik.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gfodoaylv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gqcbjbngm.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gmfrortcw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gtvrddfeh.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gzevhwvlj.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/grrffdgwj.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/guktialsg.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gxrgnczhg.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/ganogzhkx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gpbfyscit.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gijyqvktk.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gqnmniufb.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gwbhkbzox.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gemwmymao.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gzjyxmoxc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/ghuehvhrg.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gwxcovwvf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/glauvswbb.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gojobglnz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gifmklyzp.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gtzqhxbde.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gxhbezlcd.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gdegcguxp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gixwckmas.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gbqdzeilg.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gdajlkelq.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gvmobtssh.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gievyxflm.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gvfvmqbab.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gummsurgs.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gcoakuqjq.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gweqyycsc.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/grudaptzj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gvfbbyhkm.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gczdiiela.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gnnsvojvd.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gyuaitqmk.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/goncntgtv.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gfejgmkrm.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gxvzmabmz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/ggbxrsyft.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gjudrlniy.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gstonngem.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gcldnjthm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/ggagnngjb.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/geyyfrabg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gyuyrmjeu.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gjnoafgju.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gcaywvkmb.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gwfaavaor.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gylvxtair.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gbivkwjze.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gnlhroxul.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gmfdwnomh.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/guivdhbag.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/ghkbqpart.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gwhtqiniy.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gjabmnooc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gccznclvp.sHtML


<!-- 参考信息 -->