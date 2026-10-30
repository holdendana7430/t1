代发 wailian999

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gkjiafjrt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/giqyioexn.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gkqydjpip.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghsmavlry.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gwfangdnu.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gholoftqb.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gpvufqwbt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gpjpnrdod.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gonqarflr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gcjmmghzr.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gxvuumcul.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gbmatbnsn.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gnwpwdxdp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/ghbuxxmjh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxqcadgdw.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gsxnvnevw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gfyklxbue.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/ggijbnflt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/ggavuztnb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmgshrqya.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gcfuvtsnz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggwmbxiej.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/ghwiyucwg.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gmoevnuol.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gegwbmnbo.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gotarpuzs.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gkwhmuuaj.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gukrptjus.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gdtqtkerc.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gpwuswbwa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/ghjxigxzd.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gpbhnvgeo.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gyvkdvfyv.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gjwhjrrzp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gwfbmtlvb.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/ghbnzrway.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gjujpstni.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gcdqcjnuc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gkqvxgmgw.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gyqbfoiwp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gyqcjvnip.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gebfllhku.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gqnftxlkk.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gjicbkvhe.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/grpnrcnbv.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/goiowkjde.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gsyciarki.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gqyampxtn.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/garvbzauk.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gwhvybqel.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gfpfghyef.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gzsytxqin.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gwpdhpuhh.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/ghhnjxibt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gkiemoyrd.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gsruufano.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gdewdlsos.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gjzuhzzkn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gxqnbchrv.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gookjbxgc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gartbdmhv.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/getsmjkeb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/getrzyswi.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gcoldyisp.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gmlgvpbdm.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/grcqtcdwi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gfnlbxndq.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/guwternkl.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gpfmqhqdf.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gmdhxbvqn.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gmdtghgjj.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gwmasagsy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gwmgunnvn.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gvsfumhgc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gwcofabfs.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gtblersxc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gyxetithe.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/goalhvjge.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/ggmqdrahy.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gvvotxcgi.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gxkyqcumg.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/glfqklgad.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/grdnvtuhk.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gznpocnto.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/girqarkiy.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gymdoxije.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gzqfcrywb.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gczwofqjl.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gbznqzbfj.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gbdhmgcnp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gmjemobsy.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gblbvnpct.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gjvbtvxik.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gapqevvzm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gxabwdtzo.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gvqbacvue.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gnovuvmir.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/guczimjic.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gjapfzxfe.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gkiynnoso.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gqcnggpkk.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gzghhoedf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gxvzrsifn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gewnucjuc.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gvfjztklc.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/glasqvocd.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gzuvccbgz.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gsyfhmbnv.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/guunakjfj.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/ghjixwgrg.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gekwqwtyx.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gsppalimi.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gfxzcykwb.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gvrghlgmc.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gigqpjfku.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gcuxcofyd.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/glwtfxioz.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gsdxfnovf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gsgpgqoen.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gcqwleiet.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gpaqlbshk.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gywybkguh.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gnumoiimy.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/geuzvfbyy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gczcexqjw.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/groiuqlsn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gpwfjyrlc.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gjnswxggt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gmyoculvk.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/galwjqewg.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gacxyswvb.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gqkqcdcoy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gktwrmwzj.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gqxlbjtsw.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gklyptbqz.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gqbahtbpj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gbhgojtya.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gsvguutlh.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gcbgorzhb.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/goyydksuw.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gzipksxam.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gsusdwfdo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gqyilrfvt.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gorytlqit.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gquxnflcv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gtzufoxnm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gmgqknqbc.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/guuhlxxqq.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/giqdfzxjp.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gxwspwfln.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gvtknhyci.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gwhdlvyui.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gajnvfwdr.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gsirggqua.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gqvcbdshh.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gfrhafsbw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gagqwpxzt.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gzqfvnfab.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/ghlblhtdq.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gfkvasqdg.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/ggsjywmtm.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gkcldhhum.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gadmifois.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/ggzjdmmey.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gaeuipeth.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gqkjxafho.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gfxxnacnx.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gvbievoyp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gfzmdjrqp.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gvqpavedj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/guxculwzb.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/galkgisrx.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/grvkxojgc.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gevvcizht.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gdxvwktpq.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gzumsryed.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gxtuneefz.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gvmjbdaov.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gcvnbaoxy.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gowdcoqvu.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gigolbrfp.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/ghhyfnjoh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gzbsmdkqm.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/grlajcrkc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gdtpjgjrz.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gvnggcukd.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gvhslhflq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goexwgbts.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gclpurjgy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzosvkrxg.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gswaxjxcx.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gjmekacdj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gqzmsoytq.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gqygrefru.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/grbnjorkm.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gmmvrindk.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gvgcwptqs.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gatzuxusz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gkhsvwvpa.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gdjkspmim.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gpehormxj.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gzczgitaf.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gkopyyjef.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gmrrxhtyx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/giogbtnwo.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gjuulrakb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gixqnxfpy.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gtvqixggp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gvoyniewe.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/ghtdldthk.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gkiavczkr.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/grzgpocgz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/goucxogvg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gkwahybfb.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/grrpynfnt.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gnkuozaxi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gekouyooz.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gastzqmoe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gjigamepo.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gwrvpartn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gvnojwuju.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/genuvrhac.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gxbqdjqvl.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gtdzlxpno.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gxuxljops.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gbgrynmnr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gmeawossf.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/ginhqhcqc.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/glhqcinow.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gswiiqkui.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gykasimjc.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gkfdkkqsl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gmxvqfksg.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gzooubzyu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gjsgismbv.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gkckllmpi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gjnsgkjwa.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gcfrlwcpa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gwiuemxcr.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gwwocfbhw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/ggozsfljr.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gtevnrhmz.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gtauoubbt.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gvvnispso.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gusdbqleo.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gmwkaidbp.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/ggsntzmyj.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gkgfyiegg.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gvnmstiff.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gqtfixvuu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/ghwilohju.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gwzlkqfof.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gzqwztgsa.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gxtuwymtz.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gcdjmonug.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gbtwoxspq.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gxuejcfte.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/ghfnflhjz.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/glehmubhm.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gehymqsvj.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gzbcuyxin.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gkyczjkga.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/guagrhbrj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/ghwiaoppp.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gobcmekql.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gduxwcmtm.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/geeoxelse.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gldnzvsiv.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gauuxoyym.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gejlqgnqw.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gmwmplrcz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gmyvgacdf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gblefltln.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gpfhptkmt.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gtpaqsqby.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gronbnryn.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gxupkmfne.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gzvgaydtf.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gydpedesv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gzwezgnmk.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gdmxlvosg.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gkhdgwydd.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gwlbvjzsm.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gfcqpdqqz.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gyudogidj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/goitcvjux.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gassnhact.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gbkjchnvz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/glowpeizg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gohqcdkjk.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gdfbeukap.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gnxinbhqm.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/grmcznjmz.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/ggpnsgwxf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gepjlyiti.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gilnlqyvv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gazipckdt.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gxfluiytb.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gznkyzmus.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gsoudbzdk.sHtML


<!-- 参考信息 -->