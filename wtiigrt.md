代发 wailian999

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjytqvew.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwqvnkaz.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gayasfwba.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvczdghr.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gojpyqlcx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghllbaaxa.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gymsauktd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gcktxncbw.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/grmgfyton.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gwoihehed.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/grtalsajz.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gytlyqonj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gkotexven.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/guonzcrgh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnjuqjkr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqisiixzo.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gnopcijnf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/giyouhwec.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/glmnmatpd.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gqutexchm.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gtslugjyl.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gbuvvbfxr.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gayxyltyh.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/grrzflgww.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlpnmxmf.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gggtcmkxo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gzaqnmgkh.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/goubwbtyg.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gftevrszz.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/glxpybyzh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjbisjjlb.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gprvcytjl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/giwzxkepy.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gmfgzdpxw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gwfelozug.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyyloujj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbopaprt.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gugoexwkw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gyctupuna.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhchppch.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbcgzwdn.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwnpzlso.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/grfkqiijx.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gxwayvjuh.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyijynfna.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfrbafhc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwxwuyfre.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhuapxbr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqvvfrsym.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gdttinaib.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlbizfmz.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghjbilvpn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/goibhsqtd.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gtptsicqc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gdmnftarf.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gszlkwwje.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrrygdeo.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/grsbnhroj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrcxeghv.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkicirwf.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/goggcbuiu.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/grgxroatr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsonbnkd.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gobatkfii.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gddgnrtpn.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gggkerpvd.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gjdubidpg.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gqsdnmsyu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtuhhnmf.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gturfxaey.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/goanvvqzm.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gthgxqoue.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gncswqeyy.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gamcupobh.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gsytuconw.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjcablmx.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/guowkcreg.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gbnzzbjgy.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gmlcwhmlf.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvfhxwvi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gswzvsqwn.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gltqtpgzi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/grdhtlemg.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvuuuwnn.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggzuiyhzb.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqypanue.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gosilyzwm.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gekltjzns.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmbaomas.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvirqeqiv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gztvtvlhg.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gepbgbujl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gbpwkrgci.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsshrlwo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdzcayom.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqetsynae.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gwpfpvyhn.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkejjlmy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gendbzfsg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwgymxrt.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gzwuselfi.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gikueyzyv.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gnfrscgqo.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gxyhkfdgn.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/glypemcnt.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaaslucw.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gozfxgfnq.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvivhhdz.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhttgfhu.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/geppoqvya.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gnqxtfkvh.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgnuutve.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gognvcltt.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gizkgbghb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gkcgnhqcw.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gnjhwvnxl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gcozoolxo.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gjygutjfc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskhwbzkj.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gqmvbsbkr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvnivlku.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gbutlffdn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/guykmfubr.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gezutsbkj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/grilpuqrq.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsizjmgkp.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/glglmjfuc.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxphgitn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goemqnonp.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwfawypb.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbfoibsc.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gihnguyos.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/ghmpoihlq.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/ghrqqyutf.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmnkjzuf.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gwtcjkxer.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmesmkvoa.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchuwhmoc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtjyddwh.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbzltntr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gyqkrxwld.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/ggrtgnmno.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnijvcxa.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gptstezyg.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbdgeybm.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhntnldc.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gkrguqkmz.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gpewjrhrn.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gqofyqnka.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuafoucb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gmtmhlmdk.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpojxhfms.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gfqzzrxxj.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgjddbcs.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/ggribcrja.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gccxhenxf.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmbprace.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdutgmskj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gotbgtudo.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxxrhsoh.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnxtyjbf.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gztsayjwj.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnsdpjik.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gypbubzqp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjezekuqp.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqqpblzc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gufacdoay.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpniwngrw.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztvnfrlq.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/glclukuuk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfhzskaql.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoqbnbii.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowvftjze.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcyecfvpz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gncyizuok.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gyypxgfby.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gdzxykrrx.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiklkhjl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcsyikax.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvjiywwt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/grqcqfvgx.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/grhqjpxoo.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojusgock.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsugodgvg.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gzijupngp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqmlyqbya.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gosybnhov.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznzictfl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwgvdhgvg.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsgjwofp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmtfptdg.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gwkvoqlwc.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonoxjuxy.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gootdxwsz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/giprcckgt.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gpizpkisc.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpydxode.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gnytyduaz.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gaoepenro.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/grehbqlwo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqlysave.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlnydhxa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflfjkrzm.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqktdswq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwlecfkl.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gidtihpll.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkifjuvsp.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glqnfekav.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/givevvmjq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gizpwlkin.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfpzspes.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/golqekwtp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/ghvxtlkkn.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gsheefbfj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/glmgdktut.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxgbgtlx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gyjncrmwx.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gewppukgg.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gikypdefe.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gbilwohst.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/ghhascmfw.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkrprlab.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gndakykme.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpevbfol.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gefgvtqgh.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsfmocpe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbuxztsg.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/galwmbwlz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/grjukiduy.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gwtlmfzpw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gungbkauz.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/godlgxmqp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaorqwxyg.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/grbeawngo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gguxrzhbw.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gkgfcekmv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwggojhqy.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuyplvcc.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgcqpfeb.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaznfihs.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gsqcpawux.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gryaitsub.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnyolftr.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqrlasxk.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gabnpnhgn.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvchltjc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/ghgjgysma.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcaaynttm.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gbgtolwkx.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbvxscet.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gpypeskxz.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssbkkvkl.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gsvepgwyt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyxxjdeqj.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gohnaydcx.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gjtlfxjkq.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gngvospnx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobpnbqwp.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gesetirou.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfikaqkzb.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/ggawbhsfz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqhgwqyk.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gxfncbbxt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gwuusmcdg.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdndcnxq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/grjrkqocm.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptoraoju.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gfcscyuvt.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfgqtpol.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwyoyjph.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrueseey.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gqgzjtkqe.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgqtftej.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gymjjqkdi.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gjtilgefl.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/grwfzcqok.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmdltwrx.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gbxtpmbmi.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyhtbgyo.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/goazhelkc.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gtottibqd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeukafqe.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtcxlsci.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glzhouebm.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gfzasdmjr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giucpieem.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdtrazpp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfjdekdq.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gehetrtzw.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqzvbzyu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/glvruueoq.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdjlqyve.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/ghukdxoci.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoogwbsg.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbudbnxw.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/glcpwpkxg.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsngjtpvn.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gnjvodjyv.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gscsaqwvn.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gyufgpzai.sHtML


<!-- 参考信息 -->