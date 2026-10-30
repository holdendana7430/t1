代发 wailian999

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmspbuyrn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/glkriltnx.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfswvubx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkzldprhv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkdciknp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfcjmfppn.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gevabjneg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/geeaptwdh.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gezpgfimf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/geiokibxv.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrbayioi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gjagoiojs.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdvuwyat.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gwwaxyxnl.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghehfhpui.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsqsttck.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gndfllueu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gnnotalnu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gsryxtlwo.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxyfgtfr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/glsrxudqh.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/golzkgggx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbpstzhf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwphaquka.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/grshowgxl.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqvkvljj.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/golkpxggu.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gufqbabdv.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcevzlvp.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giiijeagw.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdhglxiy.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvhlxuwvf.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gzmhzsome.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnklxjzj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gpcutgbcw.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakdrkybu.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvocqkold.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gtgctvzng.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyotthoqf.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gajymmuql.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhdgujim.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gzajkofyz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhhxriou.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfojrccq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gaebbynzl.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurmnnkfu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtavhegyy.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgcrgjvi.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gghnlbkcu.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/glrxprzsw.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkedgknwm.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gpzmzuria.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvrlvzsw.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gelljclgk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gomrwpzue.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gmpxuphzf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyggxrqd.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gtvjpnnsp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbthvhjxh.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqafoxnkb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmbdlugb.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gavirsnwr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grryhdnkf.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlamiadu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzfclczsx.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gbdjlekom.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlqprjnr.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqujkedl.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gheutrehh.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/grbiwtcvj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gdtycwsfx.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/grdxgsgcj.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/grkkqtwna.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gnosthyxu.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/giyigfwie.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpndtnoy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerlggbab.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/grzkbnxal.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/geajionso.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/glnfbbltw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvoxielqp.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwnwsckw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnimaexbp.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gbefcjmoi.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gnyemgyvy.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskwffcrp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwsfyjns.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmqqdztyb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gbcxnfkmo.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gaplitnyu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpglnqzij.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbtzkesx.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcwonrfne.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gwnjgezlt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzlkuymec.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/ggybhanyv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/guvygsepz.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gxfvdpqma.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gcwrccrxt.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdfjmeoe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gcnpdomic.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/geywnijor.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gdbfdtynl.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gadrbhdlw.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gailgzzto.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/ghdqmlnhe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gkesnwpot.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/geoduvfjv.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gkyafmorc.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/grgzzgwmv.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gwmzvcpvk.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioydbele.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/glhlsevsb.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmeoygpd.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gylgtnimy.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxwrevtx.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaylgqpjm.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/ggexhvkbe.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gtkcvhxlq.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/giseevmfi.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gttkemjro.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/glzevgryu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gramudtic.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gngppaxoo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedsgzxgb.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glukzikjp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxzyepcf.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/getlamzse.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/grwnzhggg.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/grqjaktxm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gepnwoovg.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqoyadll.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gtchmiffw.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/glkvrnflz.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gskwdwtdf.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkmuvzmc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrypsdtn.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzcipxjja.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqvormayn.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gmrcigcgr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gnddsrtqo.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkljtqbg.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gudgmqoxa.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gzkcskxjh.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyzkverf.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/glvrdsrfj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuligmcs.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaodwnuu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/ggukmxpzx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsotxeun.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeerhtub.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimbxuucz.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gyhcwylcc.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzdyxtxf.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxgzvvye.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxnocqfc.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gjudjlemb.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gnyzukavl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gsgtgpgsw.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gkknxoncm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gyopgnpzz.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwlrgrth.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgudgzid.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gdnfzydbl.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqoziavz.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gvoojkwbd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gkdflwpas.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gcbrbxtzr.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gernvfgce.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmadrjps.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gthavjnbc.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgknbrxc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiroivwo.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gcklsujfl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/glpvspmvg.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbchbvhn.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhmzdeso.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guslvmcua.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjzgkmdv.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gutrzvyme.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmrfkdbq.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhpnjvfh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/ggovedyct.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/geqnsgcgj.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gkcylyknj.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqzcpcrt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gymqrmtnt.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/ggionzuci.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpbdhimv.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gudhwgerc.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gygfjljxq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavhmrzqb.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/ggozdfumi.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvhpppzd.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoovclxg.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuvrvpza.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gejtwicyl.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggngxesx.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyyldwdz.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqvmbosh.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gualjsaua.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gnsducesp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gwvzprjcb.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gmokxwoka.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkfjogbl.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsbwnlka.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gajxjcmuh.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxroagref.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjznvacb.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gcrbxjulz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gmybcymvv.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gnowhjqgz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/glqsyeyeo.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/grnfvgfpu.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gptvhoqde.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxaliyzpe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gaijrnjow.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gckmtmsbm.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/glubrkvan.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpftrtce.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gckgvrpbp.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/ggpclbkty.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwkiylck.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcybpedl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkczvuceb.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuseixjm.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpvvmabo.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gzxclqcmk.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gixwhjecp.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gljahgqio.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gzmufxycg.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmljnxyog.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcczzhmoc.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gejwfcmtm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gbyxriavk.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/glqonotps.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjocwwzd.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtxxmibd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gokmpqnup.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gwfrtrbic.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gysupvrkx.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwmqeruv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/ghwnqmbpn.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gtclqbqpi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyphmrqb.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfblloro.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugeqkyuc.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gwzczblhn.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gelqayojx.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gffoepcdt.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuaahvvz.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqdqpceb.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxdlfskf.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gnbiohgmk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyfznfnw.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gamejzyqv.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gxogdbpcv.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgxnmrla.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/guzayypqv.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gafjqkccw.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gxyepwcfs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gikdetpqa.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gotislewh.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gdwkagvtp.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqgtvhod.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/guladaojb.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsaeigkw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohdwsqkf.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxbzwivg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gvtzmazgq.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjgnwjyk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gvasocesr.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gkrfpbaso.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gzwbszklk.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gwlazufto.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gwyefdive.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmmfmwyp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgocmreu.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwtqvcdx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gmxmxqdio.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvicmjfs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbxyodph.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gzswzrugb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpjrgszt.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmqzlnve.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdeuibhr.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gzvpjrymn.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/grwwgokis.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojnlvubq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gclasymph.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/galpqjblh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqdboxbn.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gninjrgkb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glfwhcixu.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gojcogtsr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmuennzq.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/glrucgxsi.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpwqgyww.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtyfshlu.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyewvihqd.sHtML


<!-- 参考信息 -->