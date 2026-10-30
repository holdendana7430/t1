代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gufvjbpow.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjikodqc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsafxpndc.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvrwfifjo.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvdilzpp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxcsfczu.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gklskfjnf.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdywgqpfz.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwjtxxwx.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/goagntzmg.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlhczmdy.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwrqzyqtx.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gwvexqdon.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gcgujcaag.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gvgsgomsd.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxswnrdu.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmafrfgfq.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsvnezxy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxffygmuc.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbgbqjeg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxfqwtph.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhtqhrgd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gfbxhyoby.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/geachygcu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gxojsyhkk.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gmgkqaihk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gktexslgp.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gihmvgisf.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxozeodi.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gsndrmgvr.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqvtzswi.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyumywwv.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/glchrelol.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gsmwjyrnb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gopkckzeh.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gladdbjws.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvahxbbtn.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/grdifqlcr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gczazrjlk.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwdtckvs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ginnxkiou.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/grokjauyv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghdoeeqhp.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gnfsilkdh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gvquvxdzu.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdfyeast.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gunghuzlt.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gefczglne.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibxdmpmp.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhusnbhe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjumpfkwe.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgdzsdhu.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvfttvuc.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvlxkwzm.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzyfcpyh.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdgubovp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gropkgkxy.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gygpfnatr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gbsezxgbv.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gjcdspfbz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gcuxjvday.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtngupbhh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumvxirle.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlzntrdt.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gginwhaim.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gkfyvegnl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvqlguet.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvnnjipay.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyawigvs.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gcmgmiqic.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxwibljf.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gfpbetflc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjmolcuc.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrtilxza.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcmiyzzh.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gqpcmwxcb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gcetgndeh.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumcyklsw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfatobqy.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/guhqblsjl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gjddolezp.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/grhmvfcjq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/ggysycvqv.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqgshklr.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/geircxafs.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gleusozxf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gpspylhnt.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwtdbbkn.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gpdmzdbxa.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gnezxqrhn.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpddxrgo.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmpgpzsw.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gitemijyo.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaxcozec.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ghyzbxpwr.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvacmafnp.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcquzigt.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gayyamzcx.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gwzfmggkw.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkteuhmt.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/giguunmsf.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjseggwn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gedkakvon.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdetxlaar.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswutlwwp.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqqpkojl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlfvrfsg.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gdountpbv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdguvpdms.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/guwvhwovy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlttlmwm.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/geknytgch.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugcxuxlb.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnojvnvg.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdjtgdrp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/giydtiakc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/grukraotw.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwcywozd.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/giqeysqhp.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gohsefjhx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gygljpmnj.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbhggrfy.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/grejigkxn.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfuwtenu.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gezwdnbnx.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnoilyvll.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gqrmkmbdo.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gequpbnfw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gpupigwmc.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/glbcubcjw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/ghgxaoxdi.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gthxpogax.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gwxrqgcpu.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiblnqfu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gibmpzite.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdpsjblm.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/ghulmyxfa.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwwnspgs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrjyjqtq.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/grngcfoet.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gfnnvdfod.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gltumuaxd.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gngblknno.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbqxyyqe.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhvclorw.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkqlgvha.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjxvbhsc.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gpvpipksc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gustekpna.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gxclilkhg.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwaneobi.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgcqylyx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvbttivn.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxtlrlky.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gllqloenq.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gndsajchx.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzpcrnmx.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gohazbeds.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gkejkrcnr.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlrwluad.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gagvehswy.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gknmzscdt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gtmddxjmf.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwapemihv.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepumhcks.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gdeygqcqv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhrkjoqw.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gbmhqvssm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqoxjpmno.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gvlgzkjif.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gftsqnmet.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdjssiws.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/glmxxotmh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmqqpfuud.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gqhyiieoq.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gbzdrwjks.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdobqjyyd.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltqzsqir.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gtrablaer.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmpuxhwe.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/giqywmjcs.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuwhepxu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gozthaznu.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gvyxmzuzg.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gecadojmz.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gmctbndgo.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcrmiqoa.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gfqmeyuum.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaczpugig.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdtbonne.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcljrysuh.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/ghozkccpv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gcomdhkve.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gfufuddko.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gzdjnnyfl.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyucamtdy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptghswwh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyffjbbb.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/glclbjjqt.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdfdrhxv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjauygluo.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/grkqsuitz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaiggdex.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehpyrlwc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gumltcrrn.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gmhefftjx.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gvrutiqfw.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gvyegpcds.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrxptqag.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gjelpeiil.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsawvjnq.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvutytmz.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyrftqsg.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/ggkaqgrhx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsejetna.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gguidnxim.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gclqdnaar.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gskrcknif.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaiybzpw.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gieaxferq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghimmxwwy.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkufjxys.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzbsxyqr.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gtldkbnaz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaarsqyiv.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsbomgij.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gyichczwg.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gpsrudvmz.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gdmuudixq.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gcgcwagfr.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gxwpafoyg.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ggojspxyv.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrmfzrsn.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmyobybww.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimdrfkfs.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gbmdnzsxu.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grakeghou.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gtswcmkum.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gqbonmsqy.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvqzovhp.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gijpdliyw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuvcwfpf.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gsdkrnsfb.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpmsvhza.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/goyhggxat.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfwtzpbh.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgtugmmm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gupybxkxd.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/goyyjdsnr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczarizrs.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gbgekrlmd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxozvheol.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gherhnkbv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gjdvdfryb.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/geixvbbzt.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gvsrxiomp.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvugtwev.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/glcpmvknb.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gspcozkkp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusadjbhh.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/giznzvswb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklujrbyq.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzfnxbmo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glafsmkje.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gqdabwxbz.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcnbjubw.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnbxtmyy.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntanjizx.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/godqwzukw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/getwptebp.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gavsgdigi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/greoacgcg.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyoiechm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gswkmjyuj.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwzhurljq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtikztvut.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gxkstbbij.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkcoisrlv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwhnzsbt.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gcadpykqj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gyiwgywqj.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gatepdyzx.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/goadhmpwi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkozgoyrc.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdahnnwxv.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/grrmbwcqh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqtuidqc.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdbdmjts.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghltgdgjc.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gvrwgezhd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gnpytohnc.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gyfkpylsb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezegnmvi.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gllgvmsyf.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gisotztyb.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/galtvqewb.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/grgwrzjme.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gtascttes.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzvmnfbv.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gpauexdmk.sHtML


<!-- 参考信息 -->