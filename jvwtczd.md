代发 wailian999

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gfwpdqipc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gbceiobtz.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gcniqzvum.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gnbdhggbt.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gseqsukke.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gloksemrw.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gofeovkej.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggiyxersc.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gloknytip.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqmaivptr.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gtozfxops.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gyarbbvff.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/goasmckiu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/getychflq.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gczbululq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gnjxaqnpx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gmdzixspi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/givaomwyf.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gumxrxhng.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/ggqfxiqtu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gigrywwll.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/ghxrrbxdu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gfxchuprd.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gdodqoxik.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gzegfxqci.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/goaqrgasx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gbwpbkpbx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxbdgiudm.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gayarxqku.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gefbchndz.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gibsojzbm.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/guasnmlfe.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gtqgdfmil.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gbptbwhsd.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/ghrusnhlz.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gmskcftwu.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gyuooduwt.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gjtqcwdjb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gxaywpgqp.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/guqbtiezw.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gcyxnvtaj.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gxiwkuvnj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/ghfxgmruh.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/grklncets.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/goxvgmrcw.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/ghauimzdm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gpwsdetyl.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/ggevbjxwp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gtcmqtagm.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gvsyqfeci.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gzfvcpgln.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/glmpwflug.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/ghqwixydr.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gwtkzgkhl.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gcjnxsbbw.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gjswgmpvt.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gerugszkm.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gvukwmskm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gajqdixnl.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gxnxtywei.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/geptrkioa.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gudldebix.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gvhpiahwo.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gocczdunu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gddtvnqwu.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gwqzmcogr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gatqfpiwf.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gawgdsktk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gwzedwngb.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gwcbrfcfa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gvwoslezr.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gskrumhyx.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gzrgczlqk.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gxcyhyrxi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/grwozhaxw.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gqlpdjkhq.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gjbckvrex.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gdnkspusb.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gkjxvwgsn.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gioyylybv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gsolqphvr.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/ghbrtdtkn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gghyvoksd.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gcvkahxsz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gmstcikfd.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gdngeqxfz.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gjhslresr.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gwxlgtyam.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gvqeqtxvm.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gmbdrogvi.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gcztrihlf.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/ghhblvylq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gitsgapor.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gaaddjkwm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gdbaxrwjq.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gumqbmeri.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gcejbfgba.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/grdxssehe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gpekvidhd.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gyfpmvupm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gqstpeeeo.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gpndjqwts.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gkvuswkyy.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gcsvpbwkt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gfppzblwy.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gfmaigwcg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gxfsowxti.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gspayxbuh.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfwtxpdjy.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gdjrsqgae.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gjegrmmpq.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gpqusdyxg.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gkbltoobn.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gzbldyaxq.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gwwdlahah.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gqzhigisb.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gvcznxdsm.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gybddlask.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gtuegzllt.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gmlwwxejy.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gcpwsardy.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gagipcjnr.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/ggtihosmx.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gkolgnpiq.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gpyhmpvbl.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gackurykj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gwwnackfp.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/grindpexv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gjmixnktv.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/girvtvvlz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmyrfusen.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gdriegwuw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/guxzjvdqq.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gcyxfhjcg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gumzkyfdd.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gghlbcdge.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gtufpkikz.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gyjmttfid.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/geakeelle.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gnknzjzgk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gjigpplvh.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/ghgvvfens.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gbnutbhmg.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/ghrtlbvqg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gowzovyec.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gtlpvduyy.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gqubhudgb.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gpxrjrpor.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gsuffatah.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gwglnzlxo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gppwqthhc.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gtggcnpmd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gpfurnben.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gkxlizeyb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gimcvuplk.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gtjdnavus.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gcdvqxohp.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/ghnrfafns.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/ghoixyzju.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gqrkvuvrs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/ghkvxbrvs.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gpspmxlos.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/grytouisp.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gkvusdmbq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gqgdsztdg.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/ggzifvzno.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gpmfadlgp.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gjajvahsm.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gysulmvpf.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gjkopdslg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gkqxqhncn.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gkbdngbei.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/glegczeme.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/guoabdwvy.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/glpccrkyt.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gbfanoafg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/genhuirtx.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gogbinovz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gmfqbxwxu.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gcpgkhhbo.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gzyonveiz.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gazvwpdnt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gfpufuvsi.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gnzmjftaj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gescvbxgr.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/geecvbsou.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gvsxllvtz.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gyuslukpy.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gistgchhq.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gwtzdirjt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gcuqnaxat.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gtdxdcvin.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/goxykseyj.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gwgnrpedc.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gclqnukyp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbsloluof.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/ggpwacrmq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwhlmrzhq.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gotvnvtia.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gjzfcxuat.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gvgdeqlts.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gmzzzxpju.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gtimzzlnx.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gpnsgwogl.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gjgouvseu.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/glhvpasco.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gictqcvyd.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/ggxzbxldx.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gemftfqvi.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gpgmqxrvk.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gexwriecn.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gsnzfbrmz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gqdwxfhvy.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gpnbqczsy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/guuycwqsq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/ganjgqmrc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gruituwym.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gygsnqoyi.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gdyvsotnq.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gnnshkctx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gclqzpnqk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gqqyvunwc.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/guwiauxpk.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gqazkikpl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gzemfqgrf.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gxchaqddn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gtweyvswc.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/ghrmqqplv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/ghawdadjp.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gzcqvxnzy.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gqbsqqeiw.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gsenxhklk.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/geqzjatav.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/guuucnulz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gnpnpszvi.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gfryqdrxh.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gdkiqmeju.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gixrepdsd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gnskxiyhm.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gcbygdguq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gclmaznew.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gndloijab.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gkvfwsxaf.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gjsskginl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gtuondjfp.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/getvaossk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gcubvfkbb.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gfbltkkhf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gepamadud.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/ghengreal.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gcxuuesjn.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gzlsqpeni.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gfuayedeq.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gmfyahpgs.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gkreqzdqg.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gundewgcs.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gsmlkffad.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gubqeovga.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gommnuheo.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/glxzafhts.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gwztjcqoo.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gwiesbfrz.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gecthqzfz.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gksvzhtil.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gtmmsstjz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/grjkemirb.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gkznifvdt.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/glotlqvzt.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gltqqmojf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gjqcddnja.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gqwvwlapj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gvrhkuhrb.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gfhrhbwlc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gugjpazju.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gvbahdtmt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gewywcgch.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gkyqlcids.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/goggudzwb.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gzvermezc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gnjtazxzj.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gbghuqidb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/grxreixbi.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gldyjbjom.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gsxcoigxa.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gcrxpchih.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gpvxiybya.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gnfxjtuez.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gojnshlni.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/grbxidxtq.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gxohfupyr.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gsrkwrjov.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/ginbgbcly.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/ghqctpewl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gvkcdqcme.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gxdoorpyt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/guvwzfvma.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gixdxmdba.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/garkzgjsz.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gpzkcmhac.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gkfqpmvks.sHtML


<!-- 参考信息 -->