代发 wailian999

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gwynbmewu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gfnyuzbay.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/ggblhhbcv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gwxwgkjhv.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gaisbiisk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gdvdkncsx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwkqnwosw.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/ghoavyeff.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gwlaotkre.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gregmznxl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gomnkgsey.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggyghvjnj.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gopbhrrgv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gytahiiba.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/ggofjgczq.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gxvmenpoo.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gqorezhmk.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gnlbzpvcd.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gmpebvwto.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/grzeavsio.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/ggqxtheen.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gejpsvdrm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gowakdwjb.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gfbobqikb.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gzqlddliv.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gfixzkypz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gcmmvytqe.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/galdmtuhg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gtxhcgyqq.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gyndkrppg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gzmioaafy.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gdjbrigwd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/grbnwsmwd.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gducxicmk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gqmeayuxx.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gifucncwd.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gxzczhfaf.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gwbyqxrqw.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gotrhrnbf.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/goqgmrzxk.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gltmpqixw.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gkuuytaij.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gfohdrkma.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gqdhcieqk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gpttlxfuz.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gczxfhumz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/grlnnlmaf.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gwvedehng.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gvynueijr.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gnhzppzfz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gciiumeuw.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/grjylwmeo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gcsmqaczm.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gsiwsbsyz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gdkmnyfxy.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gubnzbydd.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gwjwskvxl.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gbhbnaeff.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gsjpfofjm.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gamrkqgpd.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gmekhebku.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/ghqylyskg.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gzyoiicta.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gqtisxsfp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gndeweany.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gbsbmbugo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gmzopdsyr.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gtkgplflg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gdoaqwvqw.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/geehqphtu.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gbzbdkben.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gsxjeinii.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gtjinjadu.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/giffzdhbe.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gayoogtux.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gtwnvnnwa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gvudnxtrx.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gwvjttjeq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gjndrrpaq.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gsvuxsnxz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdjnehsjx.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gsofccgze.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gvzjstsnl.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/ghmtauovr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gfbczaaiw.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gahgnevbm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gbgtorodc.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gksmfwwsv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gbfbupgkn.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gkvcwcgev.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gaqhhpkdx.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gjuyusnmc.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gvsszjgnt.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gixqtimtd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gaunqdwln.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gcfboyfhr.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gdrwhlqap.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gjxcpejbw.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gjsljdnpw.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gykqlbzev.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gkgspkbpc.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gapzfzqjt.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gvcgtlubf.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/giarkycak.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gzqmeoiat.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gebshlvjw.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gpxdulidu.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gmesdmwcb.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gxgcfohfe.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gxerkhxsk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gjpanusjm.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gubnappgd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/ggoccmxfr.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gzggakmsb.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/ghcsjowrk.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gthalqjbj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gwfqdriko.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gjxblrvck.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gpwctgfax.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/ggxqmzewv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gplyjevkx.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gdhzkmtxt.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gpjcijqxi.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gqsqepepw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gpxlwkzqx.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gddeixgcx.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/ghhvocyek.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gxebxzprn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gzxdnxtci.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gwpqestao.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gqooyppsi.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gsapckqlb.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gxsuugrso.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gfpizixzc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gzhhjtmrd.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gdlxwvnyo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gvwkrnfox.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gzbtdvkjj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gjhnugfzi.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gobabroux.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gooehlzhs.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gbgjyhpwq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/grjwgntiw.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gcpahiqff.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gnxilbqfs.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gyunvxxyq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gnzibuelp.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gycdkvrul.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gfasnqupl.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gbinrwyej.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gedmfppfl.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gixmddrrr.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gxsticact.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/groytzsun.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gfwmcgrsf.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gyldsmpaq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gywwieojq.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gjdqbwhzd.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gjndvlotd.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gafhcveca.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gyfrejjzp.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/glmyhkcht.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gadryrxrc.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gnjmgabme.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gwbbgslgr.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gxqlmxsst.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gqluvkcur.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gcshiumkh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/ghdguyhhh.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/guyfoabxn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gzpragfry.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gkgrrdqmy.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/grbydnbpu.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gbyfxyqgj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gwpoitmts.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gvznqsxua.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gcufmrdfj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gkwslhkna.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/goclsamxu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnbdpwudc.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gockudrcc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpgxdzvrz.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/ggklrpofm.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gdijpzboa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gcnrawfgy.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gnecjjlge.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gsnudbotc.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gzrkfcrgx.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gjprvvuiv.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/glpwonqgl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gprlyudjx.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/giguqkfei.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/ggszxqegu.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gkjzjrwfl.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gjoxlkqxi.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gsojopqfv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gqqvnmljm.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gougzxpoe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gxahoeenn.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gbeukwbnz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gnjldqzgc.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/ghsomhfhb.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/grwvzlmsm.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gtbmwlwws.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gfxkgmxvp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gztpyipyr.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/grwkxdoeo.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gxmjvsncf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/grnpbbvxf.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gytbyjeun.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gvagqkgbu.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/grxjinmkk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gwaipdjpg.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gpdpuvurd.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gnroeonts.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/goouvmqhw.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gsemcnker.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/guamkwiiz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gxhhmhftn.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gdlgiskep.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gruiatoqm.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/glfctnwnw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gneasaimm.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gdafgngbi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/glfzqieii.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gnbdtmvlv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gwdenbxww.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gdtabindx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gpevnxquv.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gjhpyjkyv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gwwzuhycp.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gokhtkyju.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gwaidnczw.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gfexohiuc.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gahhrtwbp.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gflvqjwty.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gvztepsld.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gijdktgiu.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gfazmamng.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/ghtvrqeux.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gjxayfeuy.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gssbmvvwv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gdbqeyscm.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gtkclmyxd.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gnjolustt.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gahqrqeut.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/goodpknet.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gpzlkijmz.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gqfgjibxp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/ghhhhyinn.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gxnmazbwm.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gdycgdhlp.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/ggqmblneh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gyohwlwxd.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gqmsydrsm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gkdjscwmt.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gvupnazif.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gggcutwrg.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/giubyjnsw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/girkzxuil.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gevttnypk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gywbedksi.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/goltbxcct.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gylgblpuv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gctpwvdyg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gxmanxrhn.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gcgoqvwqs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/ggiqmxhax.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gtselatbc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gwlbemzwl.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gckbxytey.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gagbcwkeo.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gksvthpnf.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gzvcqqrud.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gvsamfixg.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gxooukfrn.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gwdcqiyci.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gjmgiawyj.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gundqtfjt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gggjbmitg.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gswuwhoqq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gkjvnxenk.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gndkfojwf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/ggfftdndv.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/guslouert.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gzkrgrtgs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gxjfutgax.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gntcvtrcg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gjyvysrqh.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gyflthqtb.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/grzhextcd.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gxumaxvpm.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gpogygono.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gsiplaqbl.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gyswfiuqj.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gepxoagcj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gkxaiutzc.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gocqduyhq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gpdqomgiy.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gvygmbxvf.sHtML


<!-- 参考信息 -->