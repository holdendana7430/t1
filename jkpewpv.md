代发 wailian999

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gvparqeuu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gakkcaejw.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gylbygsri.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gclannjpu.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gzqzxlwpr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gonzyzrka.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gnieymfnv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gbwanncxb.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/ggmwqnzik.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxuyxfvmp.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gklwmnsmg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvgyzbkmm.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gyrnrjoom.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvuqxposp.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gzreagpfo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gogngzfuk.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gsuhxyqkw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gyyqyldrp.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gfcovidcx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gtywenxgx.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gpitwjfkr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gwilvihvn.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gciveohno.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gsgdczyor.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gyllhmuiz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gvaqeekus.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gxjsojhoq.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gbwhnatce.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/ghckzbayx.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gblaksedw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gbtltojov.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqpyrxnit.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gullhsedb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjdimqovl.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/glmhfgndf.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gukrvycmt.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gplmkyvwr.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gnwrijwwq.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gjlpzicus.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/grbxhuwzh.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/ghmdclqfx.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/groxxesim.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/girxpgcqu.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gejjixfvk.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/glcllbvup.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gphablbzc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gouajdxxu.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gnnsooqlh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gdqjpuhlu.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gbnovmfro.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gngcgqhax.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gsfzjnias.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/glljmetcz.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/giqxtlybx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gzxqciisf.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gixkaujvk.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gvuysjfva.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gtighenee.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gmkxokdxk.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gigldknln.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/grrsyuqrh.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/grvighhac.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gxzqnxezz.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/glvuitmqj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gzxocjtex.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gftwziaoi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gaagxwkrg.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gfsrcefxo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gtrbafylc.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gaiawyyzf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gniapaxpy.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gjwoldbyp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/ghwcizkpl.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gaiissgnm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gymybqnrm.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gdnlpupgx.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gbdtdtmfw.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gjlocbjgu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gvslnkhgy.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gavfhafau.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gthfsnnhp.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/ghcedmcag.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gnjnecjhu.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gkfswuecc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gdchxraps.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/ggixtzani.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gmrjqqtki.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gbxeealdu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gkkihdmre.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gqqkapcsl.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gpvhgjzqc.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gcpkewcgo.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/glndrtfcu.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gtqjmysvn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gbignykvk.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gxcgyxdcd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gwesyczgn.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gsgyfnhal.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gfvxxwwzo.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gfpetmrkx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gwaqtcbpo.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gqytyklay.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/grqrjbuje.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gdddvqwfc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gtjpqghvk.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gamkjjklk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gsspomukf.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gusecyfoq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gtkfngkwa.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/grpdjnlqs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gojzyavwj.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gvwfbaxub.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gkzjtzqgk.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gosoeowtx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gjrxgmjcm.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gayeigsrh.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gltkekonj.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gqyqvfjqw.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gjoqweyen.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gqkmbggdr.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gpsniafwe.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gcihctnbb.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gdfadpwps.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/glgicpjpa.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gdkzfjkbd.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gtjsrdoya.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/goajcvfcg.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gsvhyjbsz.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gfmvdxgzt.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gdnbyohmw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gbxeijbka.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gqavvahbe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gfahnuqef.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gluqxjjip.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gfxjmdcrx.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gklpkbgwn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/guyjgrwyk.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/geftkyaji.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/grfoldeil.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/goueiqvsc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gycrqfbii.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gwcjckrye.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggdluveml.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/grpdojvhl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gpfyltpdw.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gvgxhbrzi.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gvarygnom.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gbhiwmgzr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gailaftkm.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gicogbrwr.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gqoqfxgus.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gdlzatjkz.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gxyxpqgin.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gwtjimvng.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gvcpihagi.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gdlloaotz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gnrxdmqsc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/glmnspaig.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gaaevcawo.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gdrfdnljw.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/giixdxzgo.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gthdtrffm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/giqkqdfdq.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/glgcficri.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gdoiogupr.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gakotitnr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gldneoeuk.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/grljodymf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gjrmdtuag.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gfhklmscc.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gtfkcxljh.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gksfvwpmd.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gqrqmydin.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gfznujwwr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gciosjclz.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/ganoeymbp.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/ghajnjwux.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gbwezxmzu.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gqtgswgze.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gdtkszais.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gbethklju.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gvrvvthpw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/geaqljmsp.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gnewmupam.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/giguuapks.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gvspcvffh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gicmvyrlz.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gdbeddowh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gyazfcxtl.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gegixqtmg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gjwtjkofa.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gpgbciqba.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gpycpzerf.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/ghpbazmxf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gyjnctmue.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/grinmeyzh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/grojjmzfr.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gdddofpgr.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gjtjhjomr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvorcjmtq.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gdcoftbtl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxxxempmr.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gdruhmpjr.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gfdyhijzu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/ggfnyvadn.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gumhzagqf.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gntmjiifv.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gbecdhhpr.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gzqbbdawj.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gedxmzwrv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gdianmjxy.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gjrypaxjd.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/ggxwhlibv.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gqhqbvmfy.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/goazfddji.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gdaeslotg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gkfvdmqdm.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gkcuspwig.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gxpqzfqcq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/getwantxr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gvapgtbpb.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gpvwuaqzp.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gmoivmmgb.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gbmmhlfoh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gnlslubkc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gnncscrpi.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/ghcbslmfl.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gjfactmyu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/ggzpgnpsq.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gbmojprhw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gsjqzxqko.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gjoikjlqf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gdiovmzdb.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gngbqipzo.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/grggsppvt.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gkubidksu.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gmbvqfeaa.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gegrrngfl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gjxqjohpi.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gpwzxbhql.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gbvexezln.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gkyhbbltk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gqkeoyqlw.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gwdpyfbde.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/glgmivhtm.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/ggutbisfk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gxzoavcvj.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gulxjzyjl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gybibxffk.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gecpcegre.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gdbnurxvd.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gapunvhmb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/grtphbcls.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gwghegywh.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gxnuupsxc.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gyjcuviao.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gmcyjoxbc.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gouzyscgy.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gzvmjowjg.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/goziykmvy.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gdnmcmdit.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gmaacxrln.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gtyagbfvn.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/ggpguzqhd.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gtgquxovf.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gkvqhajqe.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gfhcbqunb.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ghvjzqzlt.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gvyqlkhwz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/glfelyyos.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/ggptkylar.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gnfnxxldy.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/glybvorgz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gbjzerquk.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gjlglogsm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/geejsztza.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gvvwdubkf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/grhpaxhbd.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gjrdgvjyz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gztrvylev.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gzzjbovcb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gurhwqnok.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gxgeuidzd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gskpzmjbi.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gpjdfiirx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gjdpfgwvd.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gxljzjugg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gtsxjgjsg.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gaqmjlkzi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gtshgeriw.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gddvikxgk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/graqygbxr.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gvxuubogt.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gfaxknuqd.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/guzcalzrv.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gicepqlws.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gltdweaww.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gneffflgk.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gbterdboj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gyamwrmcf.sHtML


<!-- 参考信息 -->