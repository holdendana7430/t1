代发 wailian999

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gojalfjhy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/ghxwoimot.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gzhpxynln.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gsywfxjeq.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gwkzshonq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gdifoughd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtgolvgbu.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gmezymfgv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gfhlinzqs.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gqivvhfyu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gfpyyfcvy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggjwumuok.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gumxkrrvk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gawigubkt.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gjxljjmmu.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gswngjxbq.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gsojhnczc.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gwotkbuhv.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gbbuhdqwo.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/groegxooi.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gdgpffuxh.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/ggojrtmlq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gkqoasrmx.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gwadyboue.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gyocfjkyc.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gooovipsx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gcbdnywnr.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gtkvrxgmc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/goaykvtha.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gensrpfbq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gmfkmdevr.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/ghiiukpun.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gmagrielq.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gkrlckesl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gqcogxfsb.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gagyhbqeh.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gdqijsysj.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gdqimsryf.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gmgwgutpi.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gsvipkoek.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/glkibmjok.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gpidpjsej.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gmeawxtdf.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/ggqqtayul.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gpjaeyhkg.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gfiapcqdr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gumfpjrrq.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gkvtnvdim.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gnhpwzfvx.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gqjrwimpt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/guimccelv.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gfowohtij.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gkqbynqhv.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gbtkmtmhj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/glzyomznk.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gjgvncggg.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gpgxcailo.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gfkgrlwqt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/ggujtmhrf.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gbemsuvsi.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gigefxuix.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gkzxhenqy.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/grawtgjnz.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gshelhtyi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gfjqxobsa.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gteifybmf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gwmgfmxus.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gmztuolcs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gtgpztykm.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gbffevrne.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/grerphuis.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gswurvggb.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gmrafhpwq.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gafxmftbj.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gslgtkobm.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gzjgcgbix.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gghzknmqv.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gnfbkzxvm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gzsmhhrux.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gftnhewjf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gryztymjh.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gviqnnipn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gxydncgfv.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gfiycmoxi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/goiojzosv.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gjmzdrrsv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gknkkrhfl.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gurozybpu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gscahalew.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/ghsaqqnqr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gfmlhineh.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gbpkzvacg.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gwmblxjhp.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gvacbstqq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/grhpamgqo.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gitwtbdba.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gcqzkyiws.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/ghhtkohsp.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gwmlypxdj.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/glumqtqtr.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gxwgeqpqa.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gfvwhurvr.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gwvqzgblm.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gdurylpvu.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gcksxbton.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/ggycaazjp.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gkchpdhpq.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gzzfznhfu.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/ggpflxxre.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gzlemtgzl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/grrydtxyq.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/ggwcrjqdi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gwnzuoamx.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gleyhmyjw.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gksmjtawi.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gadcfgydi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gvznpljqe.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gbepwmuam.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gsoucyonx.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gnajojvmj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/ggwcltfno.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gjupahclu.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gydxjvqmq.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gqxqemjzq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gzmadhzxf.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gqkctdasr.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gpknyqpyg.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gulvhzgxn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gvjpbxdhb.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/guwudznva.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gcnvzioff.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gabyrzare.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gkcltepmm.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gtgjuykta.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gwgdfpyvu.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gsdfiexjc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gisryylea.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gvvaapprd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gwcbgttrm.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gfausvqot.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gjyenquga.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/ggquvfuuz.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gpsfdctiq.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gzeugbpsk.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gxixvmbzr.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gyxtidltd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gejupjlkq.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gmoirozxq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gsfiarkuw.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gecyysnau.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gxuiofhlh.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gorvgnily.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gxzylfrij.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/ggfkeujlb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gpjdtpsvz.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gicdrjvbc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gwtiytjqm.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gpnsheshm.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gsdujmoul.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gcmsciuqb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gxzfmwenu.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gbiobhwia.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/grzkiwtun.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gzdloyued.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gqrjyukok.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/guksawmgf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gjrbvvunr.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gfulbvokd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gdhpjqudj.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gctcliikv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gvifgqzlz.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gyekvlrsl.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gtvrdrqdj.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/guvqemckz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gmyetnciv.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gjbrouuio.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/ghwvkvuro.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gvfnykybb.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gdhboeook.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvjsfaahy.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gdkcfzero.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gunaxvqrj.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcaqijaml.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gairvwfaf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gptnzthfq.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gbomgkodt.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gowqdboch.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/grqrcdoph.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/geoxhearp.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gcquphspy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gsnztyimm.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/grdskrjgf.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/ghlcpnacc.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gfyrjnhwt.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gdduiaulk.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gvmnmjfov.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/ggbnykysh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gkhguuyyc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/geawjwlvy.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gusokyvhm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gbqypjiau.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gavfjmfrh.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gcsypzdmj.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gwrphvpdd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gwdlvdrlm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gonqwbzdc.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gwlfjmppk.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/grkgvzgss.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gnqgytkwm.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/glhgvwpbw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gkgqsyyoq.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/godgbvfct.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gzswfbwir.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gwxcofqxo.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gsgzzpgoa.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/ggofsoats.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/ggjpksath.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gppigrsfq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gdesoeknh.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gvyqrfqvy.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gyroocoli.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gjkcdhsxb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gwuxirqig.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gsqmewbuz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gwrgfwkcc.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gcjwvdyws.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gnirxtlul.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/guepgfdtu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gcakzljyd.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/guxximjpb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gpeyjoocx.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gkcgbnsan.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gsziwbnvd.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gusoqkacx.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gkcuzjhdc.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gzahkjolg.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gcrjchgfz.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gpogbbemx.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gyoerhudu.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gyvlrlnlx.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gewizggqz.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gsqmyrbds.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gomgtbsjg.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/ggobwikin.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gyrkmotta.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gcsaebgmg.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gynwxixqe.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/ghifloyrj.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gqsodbals.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/ggrmzzfel.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gsbemlqdq.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gurtkcwvb.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gblkjkyim.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gizqkafwk.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gafsyefee.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gwmpklmea.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gfzwqotqu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gzudicqhy.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gqrupwsho.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ggeuzovbp.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gempgnepa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gtlhphtet.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gyzzhtofe.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/ghlkwwuvy.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gqpbnekbz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gkzjcqkys.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gsdrxscma.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gnndjbgcz.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gjjdtcuod.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gwkwkrgul.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gpmtpzqqa.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gyyjoynxh.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gzgzruyyz.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/ghzmebsjo.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gefbwkyps.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gpohnesjf.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gbkqwklzm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gvjptgxub.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gcvsjwdgb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gnwuiskgk.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gkbbwngzq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/ggvfciorz.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gcemgteql.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gmmuouqdy.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gtwvvmani.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/ggzhihcjy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/ghufgktoq.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gwasiqrgv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gluqaajhe.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gcgdttobq.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/ggxbclftq.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gsizknsou.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gksxfjocn.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gxuxkecep.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gmkprcefj.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/geuyqxwwt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gucocxulv.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gxiyqbwpd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gpogsqlaq.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gglapycyj.sHtML


<!-- 参考信息 -->