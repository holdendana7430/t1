代发 wailian999

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gkfislism.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gcsvepcah.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gbeiiifso.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdjddbikj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gaslxguez.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkxghacjb.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gsddlboif.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghpwidppv.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gpvrisilh.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gresdtkwu.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gnsbpynxs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/guoaklxbp.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gfuvixcmq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/giqsynigd.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gaecepioa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gpcqrbowp.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/goccmuqiz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gkzezbyzf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gnhxidbkn.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gimhysrgk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gtlawbrsu.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gcatycekb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gegaxpleh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grbyuaxvq.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gxhbxoprh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/givavdtnc.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/ghpgoskxk.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gfpvazmhr.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gfnpspucx.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gckzyukta.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gtpslgbyr.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gjliwtecl.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gfnmfexwr.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gadblvdhk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gngcelqln.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gtwiybqqu.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gquouxjkx.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gjqzggyih.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gapoawhre.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gvlpuohll.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gxgmtdwyj.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gnxfjwfgv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gmkxhyvel.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gweqruers.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gasdksmzf.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/ggtwpifss.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gnskclzph.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/ghmnzufcw.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gdyoewhbh.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gpcbpwgvv.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/ggpemvfgb.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gekooubiq.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gnnqghvam.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnaburvqd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gedpnqvul.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gguiqmqsm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gvkzfbebc.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gjuphaklv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gdacqbkga.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gimxnhtju.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gkdulzhfw.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gviqhfzdc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gdrkmsphw.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gyasbzwse.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gfpsyibhy.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gbhrdfwps.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gkhkamdjv.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gbnhwnmxt.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gmicvhlxy.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gfcbqacaj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gurvgotui.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gmzdrbggy.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gzljhvajl.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gjpsqsouo.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gmlbusgmw.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gbsworeso.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gvrtgfylb.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gdnbhdwxd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gswlhpcyq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gsbovltwa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gyijqexfy.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gitzdxjyw.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gidxjomon.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gkylnaenp.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gjhbovkvh.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gqwdcnowj.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gytaqolqb.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/ggbyhjuyl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gqpzvhafi.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gpnepxucb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gpypztppj.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gtckkpkla.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gfutueveq.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gmyolklzf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gigsooych.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/grhpsbluo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gflyitawb.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/glcpiennc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gqyklnjmj.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gaqzhrmgj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gkgtwhsrr.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gwdwwbdoy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gcpcnpnpb.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/geqipylxg.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gyntvprlp.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gogjnqxhd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/goffybyqh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gshendjlr.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gzgkkkxqo.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gsvnwbowp.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gozhjjkio.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gdfqfpair.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/glgperxjb.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gezporptz.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gyfveuvrr.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gmoaxdfzw.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gtcrhzyfz.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gckpodjno.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gtkhgeylk.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gvumtrxte.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gbpcggxjf.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gwvahbmit.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/giipjcfpx.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gkoxfxlve.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gbhumbmfk.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gwfibcims.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gauzeehxu.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gdyeshvkv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gozisndae.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gtcyciypp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gmmhpzwqh.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gxocwwzgd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gtjutmvhn.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gnqfejztq.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjecynwwa.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gtoeupcrp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gaetufaot.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gsezhbdoy.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gnlyrprpj.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gpkxwbneo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gcpddqish.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gcobtztzj.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gvmatptfw.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gmbpfkkxx.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gkkdqptby.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/ggxpuenfo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gbzdowflf.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gqhhiqnoy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gtuzeyiwd.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gcyoahvrj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/giwcolono.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gwhqfibod.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gvlpnpako.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/ghcsqiuop.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gzuxeagqm.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gbjoyewbb.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gzvqzhhee.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gchmihitt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/ghpmwmbcb.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gsvstlgxz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gvlxygvhe.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gcsqfdcqx.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/ggdiesrnz.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/glvtlocux.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gnrnzjjtf.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/ghijpcbwo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/ganfxqxbj.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gnyvtfimu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gjnnyldwc.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/grsxolgnh.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gokwpwtol.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gwowvxfid.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gdlvhusat.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gszempppn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gyzwxigwa.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gspelvqlq.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/ghylukgaw.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gpvvsxhyp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gmszcuslt.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/ghegqrrsm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/ghxkhpjah.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gnjyckbnu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gguluopsx.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gznlflieg.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gwakezacb.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gjiftvfnd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gasewuhvh.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gxfjtumnk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gjobrrrrg.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gqebnrfby.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gwiufawng.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/galpnlrub.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gopzktofw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gozlegonj.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gnwowymep.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/grhhlimcw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/ggazpqmxq.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/grhmqpmbw.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/grjikerxl.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gzrixpsjx.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gnpacvkki.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gcmdtesxu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gczmiyjmu.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gggtjqdgl.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gkiozzkwf.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/grgxdovca.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gnhfaexui.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gaktjvnyr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gvyqevocd.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gpisymfuy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gawbftsgz.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/guxtuvehn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gwavxycsu.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/geubhkgwu.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gqkffpjfh.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/ggnpphrwe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/ghcwbgrzx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gsdismpbj.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gdoajvbce.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gkoeoiyfp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gyknqhgxk.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gqcgeojyg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gjzsmewaa.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gznhxevfy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gtyikelff.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gwunpnbxi.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/ghkxdrvwv.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/ghyzrklyz.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqseptlhr.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gpifaafbc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gcbhblhtf.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gkviahffh.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/geiorfeou.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gmowmvarw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gkcapcukd.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gyizvzigm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gjcseubui.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/grtwbpxjk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/grtcmfkbq.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gzipxpaja.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/grsmzebns.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gsstejzah.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gcekuvcrk.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gpjumzbmp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gsxedwjti.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gfctjxlyk.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gtkvvuzid.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/goypbaltv.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/ggvwxymlj.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gsvzhymcz.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gmglbquwp.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gqclwlthc.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gvdlahiav.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gqiggpjtq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/guolujqzk.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gteasavqy.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/guqvqjeao.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gjxsbeepq.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gctjydeuw.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gwilwxhop.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/grhnndzjq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gdyptbvmu.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/ghykctrzz.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gnnjsgzrs.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gtiaxccem.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gsrklxukd.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/glbyuoyfa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gkmjgdqip.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gefmttgrl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gqjtxvbis.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gscckncuc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gadpripqp.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gcniixutg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gypssasem.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gxwdgvalh.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gragegapf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/grpajykdj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/ghsjsnhug.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gtiezryot.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/guhypntod.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gcxlmkwlb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gwuctsmlo.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gyitosyqa.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gopmixdiu.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/glvuglhwh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/guxfmejlk.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gvgsmmymi.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gqkkddylp.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gssxfwpaa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gagrzzjwj.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gtwltovsx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gnglcrzyz.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gpeqcksil.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/grakhfshc.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gbltyzzhi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/geikkvcyk.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/ggsurbifs.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gjvduccji.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gjfbxkqmo.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gsrhciclx.sHtML


<!-- 参考信息 -->