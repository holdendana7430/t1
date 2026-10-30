代发 wailian999

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gflajyerk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gylqixfvq.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gukyziyau.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gtesrrywi.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gyxfuhomg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gdgbrkfqr.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkqpqink.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/ghytldepq.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gkezradlt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ggjhacoju.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gcteyzkdo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbebmbchi.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gprbwbtap.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghgiutraj.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/ggnmpqryn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmisipkbs.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqdrqbtj.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gundkvhcl.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/grvnsoqmq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvebbdehs.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gqsazejdd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezdojvgx.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/govzpgflv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowghwnbs.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gvuelfbsz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gfjfxxfny.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gsacjwfit.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/guzooxrjp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gqffucpyt.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gweaamwuz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gejuiewoh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonuyfutz.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywggquto.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggkbcwwc.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/giqgrlhvz.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/grnfppnzn.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhtqljaa.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gcumbqmwf.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjvnassg.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjkragoyg.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbxawrst.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gmnzsclmc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gfvyghfga.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcxrgtlj.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gkukyyzqe.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfgewwbm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbjykoizo.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptemroyh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gsurwwlqe.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmsgetyz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/guiwdimgj.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/grmwzunqc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gxaodrdvv.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/glduotclv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gslozswki.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gvpqjfopa.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomegwohg.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gacnljylm.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/ghrnppeiv.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gcsafvuts.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gpihrkbnp.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhwgealv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttcowcyq.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaarlhmc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gxctrkwwk.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaaruifu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gefvdmcmf.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsenwxwbk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmgxkbit.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gstiyqtch.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpajqhdms.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gavqkinfn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gyhkfhmjj.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gaczhnuns.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdlrnifh.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gffzzgyaz.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtqyejdqe.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/grxryjqwx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gyftoofyf.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gmytfuzih.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcouuzfpw.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvaxfykc.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gabkuxxws.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhaqalam.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gmhwftppu.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gtntaxakv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grkyuxuxj.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gtkpojmbl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdglrwtin.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbjnsupt.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhooures.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbnleexe.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gtmbcmfhf.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gtpdjvgyb.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnmpnyys.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnpcyizd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnanozvy.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdtutfry.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwmtkvot.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqiogrce.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gomcqhxjz.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqjcbimd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glgnemspg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtlshjfn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gwseoxuzf.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gvczfxlhr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqykavum.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gnabdmopp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuuetkhy.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gszlyxudm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnfgttef.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gskgnhqwj.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghshuvtbp.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmitvhbb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gsusrccca.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvudidpzd.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gubcingsm.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprfyspkn.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyhjpvxf.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpiciusc.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqaghxuy.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewwclnui.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gojquhboi.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmtcjdpa.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gdykypfja.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gabjqkmkw.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gzifzigko.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwdfssis.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gxhmhkccq.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gtfdtpsgq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gvxefetpl.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjqkafee.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjhoulbl.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrchpwcj.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/garuteijm.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtygdhbyl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/guipmvdki.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gilsyvkyz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gyynuigzq.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gayrjbgkg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gpduyfsew.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsrbppgd.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtezprzkd.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gosnjztqv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyhdxnng.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqwpqjfws.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpsxdlep.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/grqwltkap.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpabfcgl.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdmrulnm.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gloghamcp.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzmessoa.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gqcncmrnw.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gagkwykvi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gcnxafwgi.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/geywfylje.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gyxgehenv.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gghhpkojo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gqojbxeyi.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gifhkvwjd.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoumfjop.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyrghtme.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/guvgptuex.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrfytylw.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gxohyssak.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxwjnvoj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gmrsrhbuj.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gdgstmfjz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdezqyjer.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/ghumeepmm.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gmkbecmnl.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdszeuyfq.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gnutfflcs.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/ginxfkdjw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/givcnhzwu.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gkbvpynkl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoeiccxo.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gdcxdrvfp.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgggpnro.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gbnawncol.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gdimfncsl.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrtccxiq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlxfusnn.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/grogclake.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gdarpbwra.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtfxrxqy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurcvgjwu.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gruwfvjzb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gutqyqgje.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghisombtq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmhabuyc.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gkkrxdpsg.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gfchfqqcy.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobcjpjzq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gauikvngh.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbccpmly.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gksobbfln.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gexafjhem.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqjbpips.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkxzapqj.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwyftdsh.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gttptfcaj.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzuctiov.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gghqcwtov.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdbbkjxnk.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gjodjafki.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/goxaiaorz.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/guwbvvaxq.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gnzxiwioo.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfquaxgw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqsifelc.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gplbumzmo.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gtrzdedki.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpbzhfnf.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/grlsdfszm.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gpcvxxany.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gajicjqkt.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gczfdlqhe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guprukyrm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxxdboah.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhikkaaj.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gliplzpth.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gvgdsmpns.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvzpqcitq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gllqqwbjb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdlanmax.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoinybgb.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/garkvjczs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gshljcmis.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgjscbeq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/giciicyfy.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gmzesvdpw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/giiqtxjwj.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuopjjjx.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnyczozg.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gtduiqbft.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gbdjxeucp.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckvvoegb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpjgcdhq.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gbmolrpma.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gewqqliay.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdblqxer.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqxtrkgx.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytaslhzw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gkfehnptw.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gtorapjzq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmjcgpyy.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlpnrxkl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gssjifqcm.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/grumqpvfw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrelsgzq.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqvwwkoi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gqinexeti.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/ghafsdzby.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gelqmifzh.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouufsyhd.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpquieynj.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkvasikh.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/ganugjput.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gykbwuzgd.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/grtwtuelw.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gffsfibfx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyskpukgq.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/guahxytpd.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhqscklq.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gvvykvbut.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmtjcjhp.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gaoruaucx.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzphpggz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyicyvghw.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gaoznklrv.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxkzlfjb.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gdsiqbauu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gbqspymmf.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/guwizhfhz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqjrhwfgb.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gcclephkl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/grormtjwg.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/grwxpaxpy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gtlfvsteo.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzkuqatu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/ggszdftye.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/goqahiqcg.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gpswaiimv.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gxehfvjuv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkcnbgra.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgbuvilh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grotoztnx.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gseaplkkr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/ghsojxdun.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmgpgxok.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gkrxvagqx.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gipfnlzpo.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gehxqcpsi.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrqudbwd.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggprwxdim.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/grhxxtbvh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboiouhkx.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gmghqkqkm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfufvvkfe.sHtML


<!-- 参考信息 -->