代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gfputwcip.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzkqgsla.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizmaptyq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggjxjhbpf.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gavhyjqvx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwzxxbbh.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtafxxnjj.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/grwhfgyse.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/ghpsevjvf.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/goyrxquep.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gnigmimqz.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtidguml.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gnvdojkex.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjywusinr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/glgwoveps.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvfygbxx.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gbgebtatf.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gkpujzwqx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/girfiaawk.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gamletrqx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gjrfmblzv.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gprhtglsd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gpshgqgpj.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gihthwwnd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/grsxsnxab.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzskldoz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gaqpqsrym.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/ggjgmuujf.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gkponjdxt.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrjwmrki.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeijknjz.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkigtjajd.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/guymzbjhi.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrlowshp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvofvzfgw.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgrsdbsf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmpwjqxj.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/glnpqcxly.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxomiyllx.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttqdbevo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvxktlwb.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/garvklxxi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggwaxbgvg.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gngdpnkjr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gsrvnonwm.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gdindzifp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gpetjjgvn.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/goatzrjym.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwidrnwr.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwgmzzwy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gflfylwfh.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/glvlljaoe.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gucsqevra.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/ghzofyquc.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grftpzawx.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbthsqlh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqvhyyti.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glswgknbr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgnbpacc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsbnrdlq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gktfiofar.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtadgktka.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gpohrqjoq.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gbqpbrgiq.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwtcxxwu.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpebwbdt.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gafrthlhc.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnogixzw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gunpaiyui.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gbtyuaheh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrnkeohh.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gigscnjsz.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyndfodte.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gikjmivti.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsymwcfzd.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gulobusfg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gognbaogx.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gyymspiml.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gsroolxpq.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gxmyinydl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gmwiqowpm.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvpkjtey.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/grrhdcysp.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gkuvurqsp.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjvtebrk.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/grcfioysm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvozpzfbr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfoguvko.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gthjhhkth.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygjvrzbf.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gqqohhzif.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gslnhttww.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkmwhudj.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/guslrchww.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/guichiqyn.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpksnfslh.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gpsbdtuke.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gpfwlxgdu.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjfzytmv.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gwgxxzpzq.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gzwqtxaus.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/ghijoclsd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gammwegym.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqcfipga.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrxavufi.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gjlpunnvd.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvobmfdri.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdssqgzy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gykzomlvl.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gjsyikazs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gifydinqk.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/glxbkfdme.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcavrkht.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqmmfnrx.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxebgoqx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrowkvgm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqcrhgnc.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gloxucxfp.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmpswlint.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gatmeofpd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gvxikhxtl.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxaucmhz.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfnzxyls.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gtzmfbjjv.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktjlsjht.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjtehcmyg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gzmlstymd.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhmtpzwl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gnckftpav.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckbdjtob.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gcqyysmxc.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gwxzguakn.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyvkbiza.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxztapqt.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gnnvmqijo.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwgxggho.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gfekpatny.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gneblbezr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gdfovbmyr.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gxidoqvei.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfitapzy.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/geehkokhj.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gogmkmxls.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipgsyhqe.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/goklujisg.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gwmagaxzf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnifrfzsc.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/grcunothv.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/ghibsodec.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gfyfjsxtg.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gaiggmdjc.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsktpzhx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqoisuac.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlymiucl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxdtqzhrz.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gebhppzus.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gavwemuui.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gzxscrajv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/giinsldea.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gporgabyu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhjeldng.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gstfjzoql.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gyyvutjqo.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gmbldtkjy.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/ginmqrmne.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gfyosktbn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gdeiamizm.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gekrovrul.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gfexebrpx.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/geutubvha.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynbohwlt.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxpfcplxt.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhkydmin.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjosottc.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gnchsqudr.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/goakhdjlx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdfmxqvkd.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjyasvhv.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzlmlmzk.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfnxzvlw.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvjtlivr.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gjflkffuw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrazmodt.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvcehdpc.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdotirfy.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gfueyiurg.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gjmfavwmo.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzfqwrzx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gujnbvvdg.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gwjwiiwoi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcevvvrqv.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gzjbhpbss.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfxdctsh.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwukntbig.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gepmtsbun.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqbxqctvc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdmpkvjy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbeohguq.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiduunwh.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvkypbcun.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkonfszwy.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gnbjyiahd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnvxxmpl.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkrzschs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdipookbw.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbisxyas.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaejceph.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gjddqzhir.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfhjmxjy.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxvlpcln.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/ghdpbacsq.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/glokkxzun.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gwrdgtzos.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gflddwagm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gmrssyyxq.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuqsfutr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsevooju.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuvqgpes.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gstfwylxg.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpmzsalk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjqxcgho.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gllnbelqn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzekaxflo.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfoeapui.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gzrakuqnh.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gewbtkalp.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkfncsbg.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqwvevfd.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxipxeqx.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdtlatix.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwocsibp.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/goqwrapif.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/ganyshynm.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grxpgaziq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxizsgbhi.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/giylgguuj.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gmkgizjxa.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzfdewws.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gpkyvuppc.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gwkfykntt.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/girtksqnb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gobeyaqyp.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmmxpvjo.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhgjvhjp.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/ggqwdbnjw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeubeuet.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxqaieln.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcitrbekv.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshtyveuf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqiylzgm.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gugpkyfsc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ghrryjmgf.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/glnpdhuml.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbvugctv.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzugfwwhd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/garvgljaa.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goujeumcp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnaabhvt.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/glzckrbfb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gqccdkzec.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoahstuu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqerwfsu.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gpmjykwlj.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbezzkse.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjmwrnhg.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/grrumqtsy.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gfodawlac.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsslbdher.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gxtpefdty.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gocoqxkzm.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobsrncbk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/govyrmveb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouoawrup.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gujkjvjrs.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gccwwloso.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvmqohtz.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gatvihyok.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmthczvvw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgurkmih.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtbfsxtw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gglnoqljg.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gsydgpqpf.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gadrkseuu.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gldffqibp.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gddgwthyv.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gblreapkl.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/ggxarpiop.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/giuckffgl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqoaguai.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltpgtrdu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/grfssfkam.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gepmlpqem.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/glsjkqsbj.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gwkjwkpkq.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdhjwwcy.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/guxghjvqb.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gvxaytmdw.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gjriytdgp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvfkujtl.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gxipvmlra.sHtML


<!-- 参考信息 -->