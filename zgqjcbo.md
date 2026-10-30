代发 wailian999

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gyfowrdzw.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpnddiaw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gjyflwzxb.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gubvkbrms.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkjknuhf.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrloleek.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuuvdmgp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoxvuphg.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gkurygdwx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gxlbbbwim.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/ghwqgmcyp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gwkvjbtxh.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gmchjyecz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytvamxhn.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gobxxgyxk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gylxgqynk.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/grhxiafsy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjoxduth.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gotargagk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwbqsxujm.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkvxhdik.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gynstuuzn.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gpylurwbr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gamojmlpi.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgdeyeyg.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjitquuyx.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnxvuelb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmlushrr.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gbnbnmkkm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkasjfrn.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwrlutfj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gfwkhtdqr.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdfrdnrw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gsrmzbthh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gnvecfcyx.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/giwdepzrp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gzpxfvfmv.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gfygwgqqu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxairwzk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmemeesbq.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/ghenyhnls.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgudeeqi.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavnbyqpz.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfvqydfm.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gqjooelcw.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnipbjer.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/grywcteam.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gscutpjnd.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuzjemew.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gotqqepcc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghasnhctk.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaumqoxz.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gftteioer.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gmikmzdtd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmdiqzacz.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvcgenxi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ghityilyi.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtaqpxcc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgggbeei.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gvaqizbfj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gqklcyyja.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeabwpnz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgkrbknn.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/ggsnfmdur.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezpiorej.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdakjwepc.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gzapuyfbl.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpronmlb.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgkfiivy.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gprwtnrgx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbmirtttt.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/ghdhuxhoa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvpytiwm.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gtekzxoad.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gfehuqdla.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbobkuec.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrepbnde.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/glbfhpaas.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gnmychdmp.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gswyglvjw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtfwxhiyb.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygbjnjvk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gybweaglg.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohxwmtxf.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjuidzdd.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiywdkfa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqajxyor.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkfybrnw.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjcwbrypm.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gyutbzeqd.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gsuwkbwfn.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfjrfpmu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gcligqfja.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/giiiopquw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdhjnbgzv.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gmawawhcc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gassvsqnf.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjrqnevh.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgpvviwx.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gzeeulsii.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/grsufqmxj.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtquyzru.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gzwkafkfx.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnovbrcm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gyrmygkto.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gukazmhns.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdynctxmn.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvumfjrrv.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzrrnjhqm.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gokadbkhe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnmskshbr.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/geuxxsfha.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gikgtkgvi.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhuwrmqh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gebjoszts.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gkkaedwnd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqagjqeod.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcdddfvu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gmscphfxa.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gelcsgmzb.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiwlndqg.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfxdisnd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gehxuopnl.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/grgktiacm.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbmtcdoe.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/glycldxsk.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkkedzxw.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdymfwuuu.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkhsethf.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gotkaande.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfomybikg.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkokqvdca.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gjttqevqf.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genixjbjz.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviophpeg.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gsquxawew.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gwbeqnbxc.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfrxjink.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcdhofwt.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhhjjcit.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofdhuhtd.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsgfgsgd.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdetwzdya.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtruasnj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gotipxbic.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gebdyallb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvicznoft.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjoawytt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/guvwexjrv.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gbsmyqyar.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/giudgrmuf.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gadqvyybh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvgrufje.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gozhjyeun.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gaezvxkvw.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmomjxgnk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknkufivo.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/geigmzprk.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gttkahsaj.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbigdxwk.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfdhrlrk.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gombyurjf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnlosaxl.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gsathdpcv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gucooqfuj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gatkgpmwf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/guvoewjjm.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/glsdrzopc.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gdvlzbjtt.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjpdjgtke.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gcghqliuu.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/ghgtpmwjy.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gdkexjxpp.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdpedgjo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnowjpom.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjgfpkuz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gualuhezn.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxcgrema.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/ghyxtfqok.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gujlehloq.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvikrynwq.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gswiwfzyb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjersmyhp.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmmczdnd.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gyiwmufqe.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gktakuctc.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gktdtbrgz.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmzbukxs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gptzrzchg.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gixhusnji.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzjrifkn.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gakwujevp.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gpjwdtcnx.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhtucnub.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbwxcpyjd.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gcidnqljy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwemympas.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzblhdpgs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gypvhoaoo.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gfdqakwde.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgksgdoq.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvrsvjjk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjpyoxicp.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyqreout.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfcvinwc.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gcqifrhyp.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/glxidubhk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gclkkgmls.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/ggrhvrmla.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxcrytcky.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gprgchrqp.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsztwpvpv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gohvuncgc.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gkldmfwer.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/ggsavpbjr.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzkemvab.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrvzkcfz.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gksdefycb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gzboyjqtu.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gpirkhaea.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gcykfyrfl.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gofftnpzw.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gnrcsdktt.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/grskzyqvc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gszamwjxg.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gtbdyburb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxngquqoc.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/givatqwkz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxddqzfg.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyyyvyug.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gnakszjrz.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvatihhe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gjuhchujq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gjjudapfc.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/glbpzegwy.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmzebhqoa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gijxnoimj.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gbnfibyge.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gslpaiyym.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/guysggqxq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdohntcu.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gubgnswov.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gshozlxpl.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpxsvilk.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfxhlnvr.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/grcnrgaeq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gmwcnrwcv.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/girfnyaof.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/glgjxbezw.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxovjncf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganwrsfdf.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gnoulkaca.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfualckjj.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gfqxmghay.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsijiopy.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsseizbo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/goigcmjrt.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/grlhghcbv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gczoyukam.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gdjmdevmk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gelcfdeds.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/garxyuuau.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtbxxnlq.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahpxmquw.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/ggacvcejm.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gohtpjlse.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gfcyyvuam.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmsrgsqm.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnusjowny.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmasrgmxy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gperjadjg.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gbnmklxxy.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghumfutfo.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghtbsyoq.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/glaemhtap.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/grxzkjzjr.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gkmbjovkv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gefemxedu.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gispjdyns.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdygppeb.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmjqwpze.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gigwccqem.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhzirmuv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjuphjavl.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyuyazda.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gebpzaxpq.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigblfjro.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghepckgfg.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmhpxjnk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqyutyqs.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gvklgqfoe.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/ggwqtyqir.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gmraviivt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/grvqfdgsa.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/ghvszzkgs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gxgenfhfz.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gtdempvmm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gbwkqcrvs.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/grfuucjsg.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiexuwfx.sHtML


<!-- 参考信息 -->