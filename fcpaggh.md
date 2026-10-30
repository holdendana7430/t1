代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/grzgnjokt.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gjuowvfxo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggycjoafc.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/geqtdscje.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqchqmra.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gsnvsedjh.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gmyayarkv.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gqowikboa.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gpouncbkp.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/glevdxlyg.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnmixguf.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gzprslomg.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjdajwmc.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gcqqeaipq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gszrsjfmb.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gwfpcrspc.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gvimkbaxw.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwrltgli.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthlrpotu.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbdegmfxw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaolchsx.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gsasxukhu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/ggywyagxm.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuuqmpnn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecfsikjh.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gkltusigr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlgjsgri.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gwvidltem.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxabzrcoa.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gooujixjk.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyojytzl.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gqxgrutzm.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gjorpksvo.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gekcdlwlk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbzeujtd.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgdajvhw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gdvtbeeaz.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gssvcduij.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvojycwcq.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyfdyotfh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtybzncar.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmdrfmar.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxepameba.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/grkbauijj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gbjmryylf.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbksrnhpk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmanepovm.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/guqutsubd.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzmtaasv.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gejwaavhi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuopjvnz.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gykqzhwyr.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdltsrtf.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gjefnnuej.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkvnhtip.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gaycbajwc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gazmkajgm.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdpbfezz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbcddmcr.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gejtskkfl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/guenghddc.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxzrjvlv.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gnelgrsrl.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glomjouqn.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guemuxguu.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgkecrwh.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gwhupsbsj.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkfdlasvm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbmfkjdv.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gegimfbys.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzckxlyq.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghtzldrye.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gydoyvhfh.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/govqhlndc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/goysbzjar.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmnqwpfy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnitorui.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrxvdjzj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/ghrdaoauv.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gpemftgjm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gfhayhbdk.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/grapegssj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgebotph.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnrgrwvlw.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/ghoyeylgj.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrtxcqnn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcunnqeja.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gvcvjbucs.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gcrmdrvsk.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gdyzzhktq.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gvtfxqbox.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/grvuxfazl.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwqhqnuj.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grferelji.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfinywnjy.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmntptfge.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhzkajqq.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gfeuimafb.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gvdipmzwy.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkehefjg.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpchvgesh.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgkonndu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/ggltjhxpq.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtsmvjyp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/geosloqmb.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmryxwoa.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxaglvol.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfrrwsan.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gexgvmypt.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gqlgrvnpo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqmuqqjp.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gpkyzzfyt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmfnzoon.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtyaabpv.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbnoziiup.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaiqveev.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gvmcstaqz.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/guwrlbmwl.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/grahbcspv.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gviefxjqi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhkzwbna.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoplhbzw.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gbimadvgi.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulpmkfaj.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcvhuhjp.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjsleusq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzeguqvn.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gwmrfaigv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gszobqlyd.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdlppuwu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwpgffsy.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gduwfybmp.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gxidxnqhf.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gidlhijgc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/glzuwtvuz.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gyswhbsot.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gcihmhcyq.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gypabtuqe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gxuxpkgbm.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnipiqtsd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeemyggy.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqfjuyqp.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwirjgvr.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagjdlvbu.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmfynoza.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqinhiuh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdqrqrmdu.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gpgepshnx.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gwpkwfmkz.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/glifeyruk.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/ghurviqsk.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gafkfqplp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gbfwtwxid.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gcjrmzzao.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/glbpucumd.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gemenpgkp.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gqcdzvoxt.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmmczfqr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxagozsn.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/giatldfww.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmalmvgir.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxcaoltg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gsqyufjlc.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/guawadigp.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxvrpdnx.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmhjjqbb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gorstlgbw.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnltbegdx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjknjnefi.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuoxkgvo.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gezzosabu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfoxrhvs.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gialqrdje.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gntbfqmge.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gghchwrsj.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gjassmqnx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsmivvolp.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gehahguop.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhvdeeqm.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/ghdujmhml.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/grwzfwygg.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gqwycifsk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gskhpmeta.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtodbbkgo.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/garjuvzjt.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gnmfvgpvu.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyukesej.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gdeujuhiv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gvppowbqw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaiqkkfg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqybwull.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtwsnmvq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdfawjku.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikxgmfji.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/guomwntia.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrctrbxl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzzyywxk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/ghjiltqrm.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzteyazue.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzwjhwrds.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gpbusjhpr.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/grixpqiry.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxnrsxti.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gvwzvwkxa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyburfle.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/giroctanh.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gxnsungnt.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gsolgtimf.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/grakqhckj.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gjieuzfnt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoztzkag.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzfeqvpl.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gwexpqgki.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gbdjowgws.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkndagnl.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwuabqkg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gllymabls.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gmniroqux.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyimigkhl.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gocmeamdm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcuwjbog.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gyztbhznk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaqhvjfa.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/grnzazani.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqebxwvt.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gquipjzrg.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmftgdkcf.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gyamhbsqv.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsaearsv.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxwtkclq.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gndxsbvsc.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gkuquxogw.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsamxumkn.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gipesfkxw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gleksxvmy.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/ggpchoxqd.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/ghmlgdxsr.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gzdmqzwcd.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/grtgllqwx.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gruyghlps.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gitvabdqa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gymzmflrn.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gfjfcexkd.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiywavgn.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvtnesgv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/giiyazjiu.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuybefsx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gocjsgkix.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gysdxayot.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gvvontbpt.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gxepxvpew.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gndfxeesz.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpryqryi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcktmvax.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gzypadquq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhlxkyfb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldzrtfln.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxrlggzo.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggofdyile.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqckkuje.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbkoldghl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gwfqtihvk.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gphfgilnj.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gzvtnszzx.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gducklosc.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkldyqvwu.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gpixbvval.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgufgkvu.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gvajudflr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/ggapyyvcr.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzicswys.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkllydyjs.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gtxqrjpec.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfoucbyzf.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwzlhqwum.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gncgrwnbh.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gclhxolui.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gruiokbkk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gttaurybi.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwhrxaon.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gmjvztayq.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/guyxbmcvi.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gwnstyyii.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gqrsvrhka.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauvyjxxp.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiwiqhcx.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkncrimc.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gyhccsolg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggopiqknx.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/glngujvip.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gmfffyjwt.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyqyduuo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnnqxvgrn.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkayhzciz.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghygoyudg.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gxeaiolzp.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxsfappm.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbdieqrq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkaymsks.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/glokolixl.sHtML


<!-- 参考信息 -->