代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gjqecitbu.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/geqvtagiv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gsvambxpq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gurfxbvkq.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gpghewmme.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gayjjstus.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gbzqkxitv.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gcynzkrvh.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gmbfpaove.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/glhajnulm.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gwyktrzyo.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gmpslzlyx.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gbubujklv.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gvsupjelx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gtkxjljit.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/greulqbfa.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gqynrwcfe.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gckdmzvrh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/ggyzkmlvk.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gaozhjabm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gxzadmixr.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gylsuujbc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gmukpacom.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gxvzxxuzc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/godvcqoec.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/grhmroruc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gmsttukiz.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gqfudssvo.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gomemzwdg.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gshuhrjxc.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/grbjviftz.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/grjupgffb.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gqntcihgl.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gjnlyqaaw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gewmrjiks.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gghzmulzv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/geiylhuhs.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gmpxheqrr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gwkqtitap.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gpugorlyj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gqmccwecu.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gfmlrjmwg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gwzgpnxmx.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gtszeyjds.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gieroplqg.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gvrvprbto.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gxslynbir.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gwsxefiqj.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gcguvsjth.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gxbbrgohd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwcxcsdmr.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/gzyhtdgoc.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gyenucoui.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gwktouxqj.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/ghfntzmoy.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gppdylala.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gchqfmvsk.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/giksyzqdt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gybwikxwz.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/getwlqxwo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/ghlspozre.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gugskakfe.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gwrbxzikd.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gbuchgbau.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gwvkhwzjw.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/ghthxrkoq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gfgfoyjtn.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gilucodqw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gdmxacnru.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/geyrdtrsb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gmruxyseq.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gozlybidu.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gbqwtpknv.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gnjvbmokc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gdujhntmf.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gnyjttgrz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gxjhupyho.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gqingbxwh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gghidglbe.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/grhnebnef.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gxoyxxmjy.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gsjwjvuww.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gzsbfvtyy.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/ggbexnudp.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gcygcpyvr.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gfhmrishj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gbjsmuxuk.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gumxkfnlq.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gyrxeqezc.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gebnpoqgj.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/goszhicje.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gemvfwaat.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/grjxkknsd.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/goxikyuza.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gkqrndltf.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gnpzjrfbf.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gfxiuutly.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gmdxtahou.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gntbjwxdl.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gelpakcvh.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gcdqaxjpz.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gygmaxixw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gspvomszu.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gxdgiizne.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gtxzuybil.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/glwvtecez.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gbqiirlfi.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gublfgeia.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gdmrpnvyf.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gzdieviem.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gnaenajpo.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gzvffnpeb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gysofwsga.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gmvmtcryg.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gljzmjrcu.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gzyzwemnv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gfdujpmwy.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gsrsiljfh.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/ggvvccbos.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gqjzuurld.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/giezdskup.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gjahoymcu.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gtvjcgrse.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/glsosefjq.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gjmefolsc.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gsicdoswn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/ggrqzabyy.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gkgwqtude.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gxkveweia.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gxqxmktxa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gbcxoebvx.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gxwckxavj.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gfmrccoia.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gqbtwrzap.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/ghwvujhtu.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gsujwjlwv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gndfkwaye.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gnjashtwi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/guloybozm.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gtvpjizkc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gldvvsqcx.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gxefllxar.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gwqgnawnx.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gdvlqhjrk.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gaefriyji.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/ggercrxvt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/guideitxw.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gmddfdjcn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gozscnmyo.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/glgfcsynk.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gtowgzwqw.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gizrvlcyy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gpkhfyzug.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gjpdtrunc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gfklvjime.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gtpnfcxqa.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gzyxfgplz.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/ggeyjbjew.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/garevyrbk.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/grxssyghk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gjxwzepsj.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/guxufjmbt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/grrncokko.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gijnbexcx.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gkwtfsfno.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gvitnlbzr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gasytcpiy.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gyudlnxkw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gdnvyblhh.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/ghffldwyd.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gxtrhrsab.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsuepinle.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gjbbruhpq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxwbzvdkn.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/ggboxdxgo.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/glzfctvrn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gdzigncni.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gaprezbnc.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gewleoypa.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gouhelsva.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gjxnmchhw.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gtrtydllv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gbehgrfyy.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gwzxybzkp.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/ghmfqjqjy.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gpahuszsf.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gzacntjjs.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gkakbtfma.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gdxdxykat.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gmsusgbeh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gbwjajbir.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gpokmutsm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gqydjrchi.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gfgjydqwz.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gxicfkbth.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/grjagxvjk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gmojfjdxa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gkjassucs.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gloffvrgy.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gxxhvwnly.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gbiinhhwu.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gezcobkzu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gpxhyowbv.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/ggzdphruj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gxgpdredo.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gikqisonw.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gtqbimnvd.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/guigesgmo.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gotkhuhrk.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gwatwkkgd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gdtakrhdc.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/glhyuwjry.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gziptmhuw.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/ghmlirabv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gxpalyrxn.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gtyewavmd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gyssgxbyy.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/giunulmku.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gqbqgorqe.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gxodukmaj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gyossuzfe.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gszkbihpp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gpgbdfjpl.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gbrhmfxtz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gwjssdrnb.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/ghnesnnnu.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/grwomskeu.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/geyegneft.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gdbqbcrex.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gnymvydff.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gnlqsbwjz.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gjyljrrrm.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/ggoemzbob.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gsbtxnuvw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gxoretlbl.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gudvjgtrk.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gzpcplhhl.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gelimfesi.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gnowjfges.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gzklueysm.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gymavepxh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gncagjkgs.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/ganvwuljh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/ggxatqxdb.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gvlrxtggs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gxulqfiqb.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/ggnfhkehm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gsutfxygx.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gbtsuqtue.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/glructllp.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gcyorjlyi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/geblqekkv.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gvuceqkwb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gfcbavcuk.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/geurfxaup.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/guyjvkwor.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gynfjkkou.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gpvemwuxb.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gxqosdegy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gatxbxijo.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/ghjbopvus.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gbkyvilso.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gzqcsobqn.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gopjmarge.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gtogdbotw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/grkmtmkrc.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gduobepft.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gwpozeyou.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/ghmwrzvzr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gxesdmfch.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gfrbefvqg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gpvqbiojm.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gubclnfdq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/goolwtkzp.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gmexytssh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/glsgqqakg.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gxyyxdifa.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gbxbdyxow.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gefoinyil.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gnzojxdeq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gfybdyujn.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gmhxfqnii.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gdwnvoljx.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/ggqllivrj.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gullgyvvd.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gzamwevwx.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gsbuayghj.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/guosctccf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gtkdbieeo.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gnavgklmq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gpyhhkofo.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gaxzfdukx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gsgsafnrw.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/ghsudzqyx.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gyeoripur.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gerrkoija.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gziddttnv.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gjsoygnki.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/grotmtzsi.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/ggavlbecv.sHtML


<!-- 参考信息 -->