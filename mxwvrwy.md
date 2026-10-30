代发 wailian999

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gtcjrcxxb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gemaiiyyx.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiksaird.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbqjuvjz.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gysosujxj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gdwlqhcjb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnostkuv.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gawmemuir.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/ghexezmbg.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghttjibwz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaffuzbtd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gezathkli.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gtewujcfs.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gappkxvxw.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gvwajqyrl.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gdbnftkxe.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxkmalhm.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwpwiypp.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrpyests.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfyhtxhp.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjstkpul.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gtdmhyinr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gkegmtsok.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/ggfhobykt.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgtpiooy.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gspljzgsz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbgjhdagh.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvzbobcns.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjymnkfx.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gmyjvzbud.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gwujlogjr.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gunkpvuzm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gqwllyjfr.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/grybehkbi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gcxuhgegx.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzoiukgm.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/ggedwrhul.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdciwboj.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gljcfzfgh.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gmjqluuaa.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/geznkyowr.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkaedieb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxdriktds.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gllqaxhwd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtasswark.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuxinoss.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/grcnfyely.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxlpdsxl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/grqveypga.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gxrxjxjsz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grnwkpvgl.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gwamptfud.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gffnjwxhn.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfmgbzff.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/glwiusnam.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidyqsdpw.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/golujwruf.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gdoeyxfto.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtnzjftb.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gcgwsnnca.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghadpsmwq.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gjwvjjdev.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/grfthfshi.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsxqcwzd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gdlpobkoq.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gqsuplplc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwriokkp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeyfkstt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gnvskqkvu.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgbcxxwa.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/glemxbwfe.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gyxjbcfaq.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gbsxdxlrc.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gjyahjitc.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gdigqvtpr.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwseibfa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzgympaf.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvcpfqim.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhinjlsu.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/glmimnloi.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzecpzczz.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gplwllbih.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzojyiyp.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gbxesdmjk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoutuoyw.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gmvafbiio.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gtdfjrgfe.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gollicxih.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/galfynbtr.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/glmthgrig.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpqzjthc.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/growbxfxb.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gctbheyal.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/ganjfgirs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtopjrfms.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeorrhim.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gvsnkfdbu.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/grlsczytl.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gjilhsrve.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gocergter.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gaffmpcoa.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gpncziaji.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoytakvf.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzjpckfv.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/geazkdchu.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvukpkxg.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmtscirf.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gbouesqds.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcctoxjg.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gkpnnwjbi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gvskapzfx.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/ghoskssoe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcnrwwui.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjtnhdxh.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzrqugxku.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnjmimih.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gtpektggk.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gnluvybcp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjrisvel.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqtsjhij.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/grokldgvc.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzfthjsr.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gqlgfcnvg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/grzpqgiqw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwhnwldh.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grpbxltnc.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkbacxlk.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gqxhyotym.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gtelsefay.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqihmxnpb.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gqlsazajq.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiiyhcnz.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glayahjjx.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfvvsemj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gayvcnvfv.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjagsrhpm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gjqbqbiqs.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/guicwiixb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/golzmefyz.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gunasfpds.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/guoricmqg.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grswxighr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwcpbawl.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpupsbjk.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/ghialehjo.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gsipswegr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gqxteyuta.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gppxxnuce.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwjjsglr.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gnikhzkjx.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gaepbqqle.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdhkrvip.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpeziiew.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gehjtcaaz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdfbnzkvg.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gghtppgcn.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gejkffebx.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gsnicpcen.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gstkwwfaa.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gzjdgyubq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtniqsgii.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlxaqjcu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzpwmpyn.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgxofylw.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyplotyi.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gtqrighwq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gvopksblz.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gnvldufud.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrpjpxiu.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghloyesgr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gaykuuwja.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqkmfsoj.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjveanza.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/glhdtampr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gpuoeeaby.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gqhvwdgdh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gvrrlioim.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gzczlgsrq.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gjtjqezim.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxexzeycg.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gvurdboiz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfzsmhbi.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwfmjqdc.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gtogqfxmi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfipinxyj.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcigddtc.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gglozqnoz.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvriboufu.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gmuysyiwx.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gsspovgxq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvugscmf.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxrnfeko.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gtrgiqawg.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gekopwupd.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gwjtcihxi.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnkilrgk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgwrfmla.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gstnhmrcr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnciztozl.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/ghshoomla.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gdvjagajm.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjogfwok.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylkhuonn.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glelxtryh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/grhkwlrff.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcyskchg.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhdmhkyf.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxlnakpj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnhdxqfj.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gwilkdkuc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/ggpsgnftb.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gtmipwyxh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/glboiswog.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/glhtalyxv.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gghkkamkp.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxfvomhl.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gwrmcilar.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglmqzcfj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gndpxakds.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gpaaznqzr.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gthsakbic.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gafaxrbdh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gkqrufssy.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gplhzanqs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gejfvsyqc.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsizjwsxs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/geqjklvcj.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gglbyguyd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsifutfs.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfahozfnx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gwiocbyxk.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gswkmtdrs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gigdjsqhp.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gaulguaip.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gtzcogtwt.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gjiahuiuk.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhilphza.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrdpttsj.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/geayrwlyf.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnigqxfh.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gnnrsjgxl.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwihlcrpa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gjtrcnzpf.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gmrbbdwqv.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkukzrtk.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcloolie.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaoefvyq.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwqijsxb.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gppcbbplj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlfvqurt.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gizqkhseq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/goszvyfkc.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjqykiiz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfcywyup.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gplentclj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpjbcixqh.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/greqwhlti.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmeldzhb.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gibmstcss.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurckherx.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfwlssks.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/grezprioq.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxlnfrdp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdodrglkc.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbljwtnm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxwyqgfn.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gredulglk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocrlwkdd.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcccrdof.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gtckfrmpy.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gozmdjpyz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvedncom.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gpljwbznu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacjsijmv.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/ggaaoopdy.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtimzanpa.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/greczynzj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldymbjyz.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcnnwhyl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwhcacer.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gtawmpcqg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gicqmnjtp.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgugpwfi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gcvrmdueo.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gytkjbrgr.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqzjnfpso.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gqysdwnwk.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyadjvlfc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gggxiazel.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gyztvyeic.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gotmsusqx.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/guoebadaw.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/grymslpny.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gmisrlzfi.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gqjykplug.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/ggcsplwon.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gpnwwhgpa.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/goexqqxmb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqgqiybm.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gpemqzynj.sHtML


<!-- 参考信息 -->