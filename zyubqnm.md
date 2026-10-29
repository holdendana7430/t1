代发 wailian999

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gxskvemnt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gcjhtxssq.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gyxwdyode.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gofxheukd.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/ggnkazrsp.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/giqbqujgk.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gnbjnlrir.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gfobxmjii.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gdfujofit.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gnejufzwk.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gjhhqqslg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gxzqowdmg.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gcpratntq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gfzwswjon.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/goiasizso.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gthivpmsf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gbygyxaor.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gqgbfdaje.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gnzghypjv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcmhyffxj.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gdhroojkh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/golxvbjby.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gxzzxxvla.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gxqjyvwnq.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gjtilwmah.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gmzjojaja.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gjucevelo.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gtxoabxwd.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gkeophdil.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/ghevarnxs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gmlalmnau.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/grulbrqtt.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gfsvqtxnh.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/ggfalsgnb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/guvwfkmrb.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/grjteertz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gbohbkcbh.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/grpaqzsis.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/goyivztib.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gonnqlcfr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gqfnexnni.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/ggrjbnpyg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gtdmmvurz.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gfupccbms.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gwdzjczud.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gqepaloev.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gbcmgirgw.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gfmnpgbst.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gbhuddbur.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gpnsymyee.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/grgttvncy.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/ghumnyvnc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gwhdmakat.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gallhcgdy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gwfazvzgg.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gfbdmepsk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/guspbesld.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gfkbatbwm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gqczmhbuu.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gzrstmcpg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gvkwksklu.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gosjotkkk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gnojdynta.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gxsqvlmtg.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gwdrgxeen.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gvlfuszls.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gngjwqrwi.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/glvmtjgyd.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gafhphkpw.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gkojibutm.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gdaqszcdr.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gbnmbbhja.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gsciqieqo.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gtyzzogze.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/ggtnnprtn.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gxvybrmgq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gnlgdmxdc.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gfmaksmrt.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/geagxvdzz.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/grtthauko.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gcvwgwczz.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gwfhthfbq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gpboyxgoz.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gastgtkje.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/glvlqfifr.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gyhxpbwsj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gboipeucp.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gblhmpkyz.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/guaasfpgw.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/guzqedhrt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gcaqnzbkv.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gxtiyvcdt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gqmbgssam.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gajjlsayp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/grjysppzv.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gpfzjnvet.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/glvirjonz.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gkkgnvdwb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gcjadefpv.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/geewzpzqy.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gvsndoigh.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gyoiymxba.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gwztararv.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gacpevkrp.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gioocfefx.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/grrcrkkki.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gooagvsio.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gagfeyapm.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gkuyznnyg.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gdwfpqiwx.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/getppnyfn.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gbzoigsgv.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/ghbgbbapl.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gahyoqgqe.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gswyfwwkb.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gtrlwuxsf.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gptwgycfa.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gdbkubwty.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gtzaxmfww.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gdaymgnez.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gkmoaeyzk.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/ghpnfoljd.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gjbwfbnxh.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/ggttqzroy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gumiikgdx.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gvawlgzee.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gdfvqxoba.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gapxinhew.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gqegaxzmk.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gezllpobp.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/ghkkfniub.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gspbcmgib.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gnpuhpaei.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gztzybnyj.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gwjrzwgws.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gshzuxxqn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gkkqtpnai.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gnkxizswu.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/glzhtufeg.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gvzlhmlqa.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/ghcemnbem.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gwynnrquy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gdkmpuhgw.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gopttyrle.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gvttunmcx.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/geoklkgar.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gevyuurmg.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/girfwczrk.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/grmbhuhbw.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gjnebqoch.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gcxejsbrt.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gkojmrizu.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gochkjext.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/ghxotzzfe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gamjzpykj.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/goubestpo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/grsigglmd.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gbsqwqikl.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gebpuurkx.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gfvujyuew.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gwakiquhm.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gdihgwxno.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gfdhsjlee.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/ghqqdccyd.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gggmdiepg.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/ggxjcunap.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gbhptwuup.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gbnfggzpd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gajvwkhdh.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gqezacknz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gbymhgseq.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gwwotrsug.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/ggqjdluyq.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/grkrwgask.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gvvuiqjgy.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gnanjrewe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gxwmyxvpc.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gwdzrqttu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gnkwbvest.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/ggzynwvlz.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gkhfpogfm.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gdcqkgsvz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gkvekihql.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gcgbkrcwr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/ghnkpfsfk.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gwlgqrevp.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gercinkiy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnibdnjmy.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gnwghfayc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzsudwiwd.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gyuradyhl.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gqaapndyg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gcegpatcx.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gnxpdqjwv.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gndcztvba.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gbpouielo.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gldzyqcij.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/goblflxju.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gyypuimbr.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gksqjflxo.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gxwcgucbj.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gxkhbjrln.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gzsqkxjxc.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/glbbguwmy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gockpnxdb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gsjyinsvw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gxmcofxix.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gojkdadhs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gszvtpytj.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gbabthvoh.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/grbtfvogu.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gfajwfnql.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gsygfndjx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/golvqblco.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gerwxqokc.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gywngtofj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gvugemcsc.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gjkxymuzi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gsoobzpiw.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/guyumjjiy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gyyzcmpgg.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/ghvoyrkxe.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/ggjrdlzjg.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/ghmbniuqd.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gmpxefdlf.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gavggrrju.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/grzpkgmmf.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gwrwzkrui.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gbyspeblw.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gsynrwirv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gryobhjgj.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gewmyyfbl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/guxgjccsb.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gxjcmhzvr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gmlywjofr.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gnrxnamuv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gdovwsmsi.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gayantdtp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gatwbfsmf.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gtgxkzdiq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/giytutmkw.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gdiexgxnn.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gzwuszfrf.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gtzszfihp.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gxjcykjbc.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gfmjwfkug.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gntsfcnbz.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gkizmbruw.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/giotcdllh.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gizkjnxnl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gobiskmrb.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gsxecipdb.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/ggsxbyxtt.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gfrccriky.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/garwuoweb.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gthsdyqol.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gzclzrkec.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gixkmizpz.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gpxiohlbj.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gybgjmecf.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gjeeurchk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gzkmzjbrc.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/ghjcnfpcg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/greerodxx.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gdsvdxyvo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gkbumcoca.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gknedtxro.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/grpwaouhv.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gjxfrusam.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gefjxqjoq.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gfkdrltir.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gaactsqrx.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gxesunnmn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gzthfdpxd.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gpqliyepn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/guxdldwxh.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/ggnwdiuzn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/guwcqzbds.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gdodjqxib.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gjyzhcwon.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gwoovpyfq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gmdmykapk.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gekvfksuv.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gtxysbiep.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/ggnpsxipm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/glcenyldr.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gkvvzksgv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/giamypkjq.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/grqciotgz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gjnoajbkt.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/ghrmrqnjt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gpssrezqe.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gnbhmrkrr.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gvcvotfwq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gwkdzsmkq.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gjsyuvpkr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gswybchgb.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gvnxxkuvx.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/grkntufwl.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gwardjycj.sHtML


<!-- 参考信息 -->