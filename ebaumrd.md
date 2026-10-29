代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gprtsvrzw.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gmoeumxuq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gljnmhrxu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goynagnaf.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gmoqhbgkk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvfmxbbtf.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gvwmvhqyu.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gsrillpok.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gpvtjlpjc.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gpttiwddb.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gfpzbeuvb.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/ghegrhdad.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gcrljevdy.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gnsumbmkc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gfxillbck.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gzhfabvsa.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gxejrglci.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gfieslrqc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gcnlwmzkz.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gghlbaweg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/ggihoqmfs.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gmnewkvva.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gwednthxb.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gbtjqrvik.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gldrdbwfx.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/guqcdbpxz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/grbwdtzkb.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gwhgxcoek.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gllbpdarh.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gxujepxpc.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/ggqtyppjm.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gppxdlsbz.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gfxggiuyy.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gltogupkq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gotgatcuc.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gndjqtufm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gnkcuqqxg.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gchczrutz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gwbbdvmxh.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gacpyxjhh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gqrilmunm.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gczapimwk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gmznzcxsy.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/ggkltwpfv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwfpcuiwa.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gwerwxdag.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gcskxotir.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gpnlaaufk.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gxksxsdzl.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gvclduyut.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gryxdzttu.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gtpqxyqdz.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gjqhcyfeu.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/giakjrlsg.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gadqfdpyt.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gpbdtrzdh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gxoubivls.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/ggaqlzecb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gagjgsuvs.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/giwkmbwgm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gftqywpey.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gtbxjullw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gnoqhpoes.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/grudkvpts.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gxtqrtczr.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gzluzoipw.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gaiuiowwl.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmsbgccit.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gkhfgniva.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gqomezuxf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gyjywhrzm.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gnbodkitb.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gzlygsnod.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gdktpfzcm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gvbplahwx.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/ggmsfvmnm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gpvlyecaa.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gkhmfxcgn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/ghrqanzbu.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gmybwypti.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gtxasfpjw.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gqbleusln.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gfevxnutd.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbpnzcvlh.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gppedswdj.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gjehutrzo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gglidvedw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gnknmtfxw.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gwfocvfkp.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gchqmzycp.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/goccipzmv.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/ggbgweijv.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gvcwxhnst.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gbwqspdfk.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gqsflymcs.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/ghvhgpmlo.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gyvzewnkq.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/grrzpmdcf.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gzoasvfvk.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gssakqxda.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gdcznjakx.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gqcemmwdy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gvnrxzaah.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gybsgxyck.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gzctkuakz.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gnnbsarho.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gohoftduz.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gevuqeicv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gqylgfzon.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gyobgezwb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gnpbnzayy.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gcowewqxj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gindxidbs.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gnznirexs.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gudddvype.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gdhzhmxbu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gfxjclpum.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gadfvihwr.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gcfddrryd.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gmmgkdsuq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gwauhijzc.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gethdyvsi.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gtodusexk.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gytndigjo.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/geokckeyu.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gdkpbokut.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/goakplpog.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gsbwyczpw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gxacvhkxb.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gsgmdrrzs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gwbzeuzox.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/ghebypplh.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gsbugalcv.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gitfkcdpm.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gxoykntkj.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gpefqlpor.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gsgxnbeni.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gjabwxxca.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gxplmczpu.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gejbwdcqd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gbrzeinfs.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gffwjnmlf.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gfeeuyulf.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/glnxmurck.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gfbdywjtk.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gzsqkjuiz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gsdvsgcta.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/guxirpaja.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gvdokgsse.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gyutxqwbg.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gpdcylwny.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/goltpbanm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gyzerpxns.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gyqqjhflo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gbyvvexks.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gtxznqyvh.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gzgpicrbg.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gpeskwuvz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gbrtuyyvn.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gftvmrirt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gzmqqshec.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gjwjoblar.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gvdonphas.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gkxefvrqr.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/giftkhrto.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gqizzljgo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gawbnoylq.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gruiwsfma.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gxunxhnkc.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gycgqcvdm.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gevxugqga.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwnnvadkn.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gorqxgraj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gouuenptd.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gbnomijxf.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gnemmidvi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gndexonti.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gxgdpkozd.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gfsmlefvo.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gnauldgec.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/ggqhjbcxw.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/grijllfsd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/ghilqgjdu.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gzlxowjvy.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gqjryxkdh.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gtsshimjh.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gnoemgmtg.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gzdirnggy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gohzsmece.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gubzyzgjl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gscxmsyvv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gvrntnbli.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gcdmpplhj.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gertilkar.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gzumfamcn.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/goicpubjw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gfojxvqzn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gyveexofp.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gssunxrav.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/goutqntae.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gwqnaeolh.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gonzqldhm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gstcxvkpq.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gwkelzqoa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gauxhxqkw.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gqdlwuepl.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gbahludhj.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/ghkdxbmkg.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/guldrsyfi.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gvzkhesxj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gbqutanqr.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gbqbzhmyt.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gdeczsxth.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gbgpsaenk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gasczahhn.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gvwekpdfz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gtgrjofla.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gzyoujijd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gbveiajtt.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/grnomshsq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gapdmfuqh.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gaprqjlil.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gxdjzoztm.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gkarvpsfg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gbjvstncv.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gdoggpwse.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gkoqgqorh.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gqcuksnmz.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gqwypewgj.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gdyhpadyn.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gsdzvdwda.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gwbxilbwd.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/geuhcuqdo.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gvfmhajns.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gnurevgrj.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/ghtigynqe.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gtbiskwvj.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gfrwjqpgh.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/grculkozl.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gszngvemw.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gucdicmxq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gvcidncbt.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gjuopagjl.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gzmarpgwu.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gqlreaxir.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gasinxjay.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gcldiaqha.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gghevybsg.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gfxgghfgo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gbnprfuwk.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gqcwptqoi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gkkeuencw.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gyluoubfl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/geervsplr.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gtxaeucvu.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gphshzrkp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gehkdjmcs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gdptmtcwz.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gpdnstzxw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gfbszqjam.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gjijmtrwm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gtraejgab.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gpezspfkz.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gyinoktgx.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gytycavsj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gvwnrimmp.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gokqlyjls.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/ggzcueqqv.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/glunrobdm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gcwdavixc.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gdeyqaamr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gdxnqeyqv.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gzgptmmfx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gqkodcoej.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/ggnjmubme.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gptuivaob.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gczfgfpnb.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gupeileii.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gkqssohwh.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/ghvlevncl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/ghreyetpf.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gefclutne.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gcbvyvhdh.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/ghvzhetpv.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gpdabjdhh.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gpbjgsbyk.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gotxgvppx.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gffmnyxgv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gfcewrexl.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gawjyhzpt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/grztmvsjj.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gdredohtp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gcqvbbyju.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gdbrjgjwa.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gtlhdhtzh.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gdtdujpig.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gahqncdfu.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gmdsytsrx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gdbjpzpbf.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gyzyjccql.sHtML


<!-- 参考信息 -->