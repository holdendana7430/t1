代发 wailian999

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gyugvduzq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggpyvjpbk.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gejhcsqzb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gcskfeabk.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gmvlqtuwi.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjjgebkfc.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gziqvjsmh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gqiqkpwfj.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gpixlppwr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gbndxkirp.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gvfvxdhtw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gsorygjvb.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gewiyazkq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gultqzblg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gcjbsjest.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/grftufdtd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gytyqawrr.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gccrljnqf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gcyhngbqh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcjznmqfk.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/glqtixbpc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqfpeysch.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/geahppclq.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gqgimayzy.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/glybjzfwj.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gkhqgydjb.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gzsfiscjf.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/guqfrfiue.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gkflkkjuq.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/ggjusxuvl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gxondlaiq.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gncfkizix.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gvdnomccf.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gllnddanw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gxuchcrtd.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gakcmzlow.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gdesossni.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gjwjhwmvo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gyntxcvwl.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gidxcxckn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gzimkdmxy.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gwvdgdzrb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gtlreucfl.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gmlkuuhwo.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gdlweqlgj.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gyandpzrt.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gbvwqvmnp.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/ghytjirvj.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gpfqyetyh.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gupmojoee.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gjcewlnfu.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/ggvspmhfe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/ganudnnzp.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/grnoqmnns.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/grjxsusmg.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/griwtwimo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/geaqinqkt.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/glyshvqcb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gzskpmeed.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gmnaeegkp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gyanjfdgy.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/guczhlruy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gpvhjookr.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gpfewskat.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gabayepcq.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gvszbnghf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/ghdrtqeho.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gaobbusem.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/geysueoqm.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gjyhaorym.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gptjifurk.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gpbigncxe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gxflsseqz.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gteiltkko.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gmtwlgmxi.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gyydqcect.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/guaehbrks.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gyrsjtdnw.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gjwzgfziv.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/guzsdtyjn.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/glodmfmwo.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gxgnodhcf.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gmkscvbey.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gbpnzpsni.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/ghlzkemes.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gahkcqpvn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gmndomrct.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gcwtrqlhl.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gyvgpmhic.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/grwcwzjfz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gfvhgcuzm.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/groqouqbi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gafvdpenr.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gbiedfsrd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/grwohkehu.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gjhlakhuv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gwgjosdoj.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/ghagftkoy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gdyfytnxb.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gyyrsytxb.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gzixmkpzi.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gdxxrlogi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gempfhacq.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gsymsxnda.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gbafeszmc.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gtwoxhkpr.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gebwvdnhz.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/ghmywiilf.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gsekgnzon.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gomiurkdq.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gxdlnavla.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gnxyendrj.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gehdsrmzh.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gteltexia.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gfwmkdvgh.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gbxynczvh.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gdllbvzaz.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/grrwpdfdm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gysmeeufi.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/glrdioutx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gspmughtu.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gxkhpywfv.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gqhzkublt.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/giplofnue.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gypvnbzkj.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/grjftdfzi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/ghbogbddq.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/guimbyjsw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gcfudapot.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/ggqlwrzfu.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/ghopzrnal.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gmnkxulnc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gdhbpsqjq.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gyzstcvyb.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/grrgidmbo.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/ghrjmchpw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gubkhbtrr.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gvnjimnme.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gjfdwpgov.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gvgkyuziz.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gtnezobce.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/goywgpksh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/ghgsjccji.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gkjfhbnhf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gfztxqvuw.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gkvaeucxd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gyhqzyyct.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gnonlijgo.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gutryfurq.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gggkpkjnh.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gbrwlpoga.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/ggcqfxfvd.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gybvjwioo.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gepfknflw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gmcmkvbme.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gnftkufrw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gtkehgqve.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gqwnvnfgo.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gurckwkbe.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gftmsiqay.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gucmtyfgt.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gbvfqflpz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gpxsiflam.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/guegshzei.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gtnfxwheg.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gqladjtbt.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gzqifxbhd.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gwxyboiqw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gtorxqwvs.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gynhhaehh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/grzpjwqce.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/ggxtxknyb.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gqrgxfhlp.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gtnwqdbvq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gcaaidisv.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gfcmbjdwm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/ghujumadi.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/ghqorixvj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gxywmerht.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gzmdyejhe.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gyxwqyhih.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gsxxqyauq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/givalxpjf.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/glwihgbnq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gfqhqhntz.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gkhpwdjwp.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gsctkvktm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwqgxpmxa.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gpojzznwa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grsjjzxwo.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ggexuppfj.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gjdnjkwis.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gjiafyzdm.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gdjhttoxx.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gkwysgagt.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gbbwharcl.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gpmfzgfcq.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gwvlotkpa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gyhkzjlee.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/ggjunhfpy.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/ggqrdhamw.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gbqyaapbx.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/grghayazk.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gdqfpyifs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gorzmaaxa.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gmhiwvapo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/glymjisrv.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gnxfqutid.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/ghrflhcbh.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/glayqsenz.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gqfexcfwb.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gcjeigsfg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gaxvtztgr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gsuuvimyr.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gketniasx.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gdtjzpjwp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/ganutwatb.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gudyzyzfc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/glmugijeq.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gkqxemwhk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gqynhtllk.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gnpromrvd.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gjnvmnbbf.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gzuckegot.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gfrvjysbh.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gycifabqb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gazjiazhp.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gzswtbnyf.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gfsnhydep.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gqczwumgl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gpfxvkvbr.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/ghzdkmnjo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gxbyvtknm.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/grabzpfgs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/grhvwyfna.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gyijaehtd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/giqrnulrv.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/ghwolxwnq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gazfyxajv.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/galtwbwuv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gamgyoaqb.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gxieptrjw.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gzjrqtuis.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gtosyjzhi.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gyodcsgem.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gpdkamgfx.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gkhwrwzkd.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gdoizkhjh.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gpyykckdd.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gszoewhxl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gvsqplplx.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gssdslklt.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gtiqsyahl.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gtlqwbxus.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gvgyxdbfx.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gefprsupa.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gakyadvuq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gdpwsafep.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gxcxhtkww.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gxspioeha.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gnicawerm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gyzzphrgt.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gnjbrcjdi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gletocymd.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gdglhbdog.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqdvjwuiu.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/glndzphhv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gopikhrfm.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gvjsqfevv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gxftayonx.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gdewyshgg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gfjaxvdqi.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gchagnefq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/giehanwkr.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gowqmhwol.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gpgvzoowt.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbjapctzk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gsbpdsfey.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gprtqudlh.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gbbnvnwuk.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gerfpyxlv.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gydgnpgbj.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gjctcwqdb.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/ghypjkfhd.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/glgymaagp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gpvzygbkp.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gqpvzmrkl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gceoeyxrw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gmfkpqxku.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gxxjntqyr.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gchkcpdei.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gsgrwupbm.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gkjmlkssh.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gqypbnlvb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gmxpgdxqv.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gpbmtunlj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/ghrskrbbw.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/grswifdcn.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gvacqwalu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/glvqucyma.sHtML


<!-- 参考信息 -->