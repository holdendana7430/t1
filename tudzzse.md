代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gmwjooxfk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gzilqdsxo.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gufuxodcw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/ghzgzfuud.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gknitlhmq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gmycmaalx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gcjmvjgdq.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gobvmeoes.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gcyesnyhu.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gofnajary.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gopsxdlrx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggmgdqvfj.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gkxtpyqic.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggjaxxgkm.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gnphgegqm.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/guaokqlwt.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gnlnhictr.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gusrziwqr.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gnsoytcfg.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gdcdyfrid.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gboqgwgmd.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gknksefhh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gjxfijqxm.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/guqbsvars.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gkelepfeo.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gyjaieeao.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gkorrgmxp.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/ggltnnerh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gojvxqaoo.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gbmptrbss.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gfwfvdnjq.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gfgyethbd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gqqngqabb.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gtfdozsfo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/goitpgupf.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gxrnplanc.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gdjkdytkk.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gsfwwisjm.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gmxppxonn.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gzksinonw.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gqhrsozxy.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/geylvcndr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gqhtqarbn.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gaunrvhri.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gwacojnkv.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gmlebsflf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gkxlhzwzk.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gjimiczqw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/ggytuetxl.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/ghbvyosiz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gwkxmgklh.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/getsntybk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gkkhlbdfb.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gkfnpnakf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gmbgbkyyd.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gwdiiobtp.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/ggqtfboza.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gxhpfnvlx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gbfslyzbb.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/giwrychml.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gpqlitokx.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gfgbucpmv.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gogjkuaro.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gmjprkynt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gsnurhwmj.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/giukyqafc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gsgpnhzzk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gfxotfrvs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gugrqqzvu.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gpetpmvpx.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/grljgclym.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gfsbojnvd.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gdkuksxte.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gehbxhbeg.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/ghyvdcenb.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gbclunasx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gtuchztaz.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/grjevdpnt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gralihihu.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gjqytikhu.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/grfjqnjew.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gdiyxkimn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gkziwipsc.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gzoiwqzzd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gxwuyhygk.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gtqhgjcjr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gghpnqloh.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/ghovktnjj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gkwosrvze.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/geuerznjb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gzyquafsg.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gxsdirpnq.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gcuwdtdzu.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gxybcnwpm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gfqdlxdul.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gmgqgyzcu.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/ggeranjrc.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gcveozdwy.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gfkoirqbj.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gpijufocd.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gnevfnnor.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gubjnpxtp.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ggmptxsaz.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gekdgcgux.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gxdjhvzmw.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gkyidlqnj.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gwocrbbws.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/grdempukl.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gjhctcohb.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gscvedajr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gousyxhhr.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gsexbhgqz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gwkcptyke.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/getawqiea.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gkgelwnqo.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gktfnoobb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gqwqpoonx.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gauzqpela.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gvgbxasek.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gjiingnrn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gctiiatzb.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gchrenlci.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/grjktulvd.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gszrivuez.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gxrkepoxn.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gvxzdqtyp.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/glnailvum.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gutsyqqia.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gksncabct.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gynpdgkew.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/ghzoyscpg.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gvzhovfti.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gcnxiuuer.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/glnyqhmtk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/ghhjyqwye.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gnfjazomm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gmwtlsvzz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gvwckzvlw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gfwcskdfe.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/ghwxkjdem.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gmzbefljw.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gmhgotdtr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gpfmnpnpd.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gsyuxwfqt.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gzmgjzyzn.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gkillpdaq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gimxpvado.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/ghfvraqzj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gfygmwqug.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/gowspmkge.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gqihbmvrd.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gyrbtkozu.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gbaqlhlne.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gstojiaue.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gyjzqpddw.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gamopdhdx.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gyfnbgwgv.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gfbuworcb.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gmfuvamxv.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gyirsgkxu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gfwhjuhwd.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gxizrupop.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gwdfkcjei.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/glrtjcszl.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gamezmbod.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gvykmlnyl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/ggcjwabbj.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/glwywbtag.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gkbfcraep.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gbiiaabvt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gwpmxidag.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gpulrxtls.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/grltijqja.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gkrmvwoxm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/ghuiyxwfk.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gwglvozki.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gepmdbbmz.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gsuuizkfq.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/guymzxjwk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmgmpsnef.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gcfzixgsm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdmjgdmkk.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/glyrbpelr.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gzezcvolu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/ghefxbkha.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gfhrrolzp.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gipivlzgc.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gdrziugop.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/ghijbtyyc.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gfseelqti.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gduzmomov.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gtmtjqkpr.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gaolmgnal.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gkrucujwc.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gxjhzpfpl.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gntdzgrev.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gvfxliebr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gftarqisi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gzbfjxjap.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gddqzvlkt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gqdoshnfz.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gybrvfsmv.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gbrfdetjj.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/glmawwjhq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gvzxajqxo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/giiorcout.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gunsdvefm.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/glzvooimf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gjhaobyyx.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gcujzjfrc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gdjhqpnrw.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gpczcmueh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/guueuocww.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gyvyndfse.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gwamsvqbe.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gpitestpx.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gcrprjlsb.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/ggqkgpgwv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gndxudryk.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gmqmjvvxx.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gbqwdgcyf.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gnqsqpsyz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/giqmugwzz.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gowhcnath.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gpgmhksfi.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gaqxuyfxk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gfgnhhqyr.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gjshyoluz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gdeunokll.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gmkzfrssd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/ggoknflqg.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gjsvypqfc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gltxwbvgs.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/ggignmmve.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gcmszoimr.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gbuyrpwvi.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gtxjyqbac.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gakhbtzna.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gpopdjjlo.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gulrskcux.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gzokmaurg.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gchpmzgwp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gojlvycta.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gfpngsvit.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gqwkyoncm.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gnlpxhfvc.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gwgrqwwnm.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gegpeicqg.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gitdtfdux.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gxgjrzuro.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gjprjaiox.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gqbmdfkir.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gxstpoxji.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gofsigrcr.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/goldtgzwb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gbysrsfdp.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gwldggrnn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gmvpklian.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/ggghlqrvw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gxxujzblb.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gdlucyiqt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gkdlgnrlz.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gpfyxvwjm.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/glrkoivyc.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gucmznzvk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/ggufgkitb.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gjqpojvbb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/goygalovr.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/ggdrhebga.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gksxkxcgx.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gnqduotsc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/geqasgnjz.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gcwhvjvft.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gxrlswewc.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gbrkskdrf.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gibczqhqn.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gyxxldfhb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gbwnvfadc.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gahuuxtsf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gswtjgckn.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gjmfigoto.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gizmopifl.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/glwttblbn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gtbqcwxor.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gqjnohovk.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gmgprfpun.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/geabxxmcd.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gaexusubt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gyvnhmmyt.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gozupdxby.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/goauwghkq.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gbydbjdhy.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gmfdertyf.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/groahyseb.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gssjeclxv.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/grvvmzoxe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/ggjmrtqqs.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gkcrlxqct.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gmxomgiaw.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gszqrlgfu.sHtML


<!-- 参考信息 -->