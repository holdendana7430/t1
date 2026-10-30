代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gjgjtjygi.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/grpiawgro.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuycqawf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzscssfvn.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gjztcstlk.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjibhlen.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gwafcmprd.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gihuhlvfx.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gvkaiqtkz.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gxdxkifni.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtdrozal.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvnbzqxuk.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gmjnpqjws.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/geebhflrn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gydwivoif.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gunutcarv.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/grlnyznjq.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfdlpnzg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzebsnokx.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkjjuuaf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gybtyadqh.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gusksmzbe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gnhufbnyx.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmiyvrrs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/ghgxvsfsm.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpxkgira.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfqgtbrn.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gbefuxfiw.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gvdyzamdv.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginxsxrjb.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxygvnik.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gscoowqkk.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gdtdplkyo.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcuiszcye.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjyzjiwn.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gwjbamgyl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/guqrfnheg.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gfegirsgh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjxsloeia.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gupjfssbd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtnizbxj.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gzrbglznp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gaayyfsxq.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnjlqoas.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdlqutkj.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpgwgiah.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnpulprp.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gloojlvrm.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/guaqwnzao.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gebzvcjuf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvudajpzx.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlreeeep.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgxnuogb.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gkolexxzm.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdksfpfo.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gvwvmfime.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gsnaltbkt.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gqctcmdyg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/ghcuncsct.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwnurrpt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gnvsfsjjt.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/ghlntleis.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gtjhshmjh.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/grqbpofly.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/giqjipkgj.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/ggodvbzou.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/ggrjcgydk.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejguqtlc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvnqeylw.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gwenkkzvz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/guzhkxpen.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxkkmhpj.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glicnmnyq.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/goxhwwpwu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvkjthnym.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/giblvpfwo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/giaffmkqa.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmhxpahm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gfukgeixr.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnpgkziy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjlhkyyy.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyfokhyq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gniugsrgn.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqequtkfu.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/geamtuaok.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtycwbxtt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/grtuzngtl.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlhjearz.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcrflgqh.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyvugbwf.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/glqtytson.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbjzfkxt.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gmhebetde.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gyofmmpgm.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gyajacbex.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkplixde.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gxkflsbaf.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gqdcubvja.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gjsfsbkxb.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzqnwysg.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gkaxuvvce.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gspulbsmd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gqgtlnqla.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxdjuxac.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gshcpmpqo.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gziatcwwm.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgrjlbej.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gaapdbjtr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/ghfymtjjo.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzoegafst.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmdqbbsw.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gornufuzu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnfacuyx.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gynfnehqe.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gowcltmry.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gzaxbwsgj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gygipzwhz.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkbcdeppk.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtvhgdvcb.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcmqkcri.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gusvxyamv.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gmhkbatlq.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gxwrsivqc.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gakbippau.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gdygxrusc.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvvfojnsu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcppahpao.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyfvaueu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gvfnftkpt.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbgimutd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbzicoal.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxwipxyu.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gxiyahyoo.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/grucxravu.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyxfxkta.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/goodsvyzk.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gazjruvcb.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfvqypus.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gesyimehk.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gspsmlxhb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvxdzttb.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gnzzxijhe.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsykhnms.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/giuaclkyx.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gwucxahiq.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrfcizox.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gruutxsjh.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtutmtbl.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gedsxvdri.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfyasdfj.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqqxdxwi.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/goqggwyvs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gonygyyau.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gbfwnlkdv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhcxvada.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgnpfsqa.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gwralcxsm.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/goeyyszot.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/grkuupaaj.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gixmbmmqy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gohdtnaqb.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/grfbkknjf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/giqxeqhum.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gulaesrnb.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/ginxcisfb.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gpqrmcwxw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gueznqyra.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwaijaxi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsxoeqjs.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/ghyeifkxk.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/ggksizgsy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzkvveoml.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gkyaomxnr.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieoluxma.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/guhcxztwd.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gdcvnvhua.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvzriggou.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gkdncupoh.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdfngfdm.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gepqyfjko.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gtkmaujqo.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxptseqf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiyqyrfa.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gsztruvkw.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gliegzfrb.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/ggucshqfj.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlguwqem.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gyzybfhzm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gyyphpqxb.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gfklvwmxo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gbnogiaur.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gyvjieqgf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gvraoyymr.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gttqellgg.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/garorjcmp.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gljdpqjdh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gljyuncnp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gngqqtsdo.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkbjielz.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqxyqixq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gtifisfmw.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/getwaedhx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzaelsxw.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gdltlkhge.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyjvzfxs.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gakpluuit.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/girpfewnd.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvxcdmmo.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbibruvf.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gxpizjdxr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gwrtqsypv.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gijiyfeql.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzarqndaf.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gjdhyrfzn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnttzxrof.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzzfavpy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gbywvhqeb.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwjyyjvn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gupiyagwm.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdpyihkk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gklqjfpur.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzzlpotc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gxqvvwtbm.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxhzefmq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/grzkxwhpd.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxxfjuiq.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevibeodd.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdankjpyv.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/ghcggxnxc.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/ghmyfmjcn.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gqwqlbdbi.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpudzjyzz.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrbkdikl.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvxgafuv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gfundlhyk.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmrrcbtg.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsngdaum.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gkjyjyiud.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gsyslniic.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gejuaimmf.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gescgfgtd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexcdshpx.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeitleiu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqaghdsk.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gijploela.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glabgfhbk.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwvozjeh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdyjxvwfm.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gbriktqqc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gfiplixoy.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpivrqyd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojwzjfrs.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/ggiogorbs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/grkttycte.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gvktupxew.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gaziheqim.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsmcqwap.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gebmltbdn.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiehglvd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqsinfuw.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbevrsbtu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gashzywyv.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gkxnjlzel.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxwoehfy.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/glqhwpyze.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsmnlext.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeeqbqhn.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavgxlxds.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/grkqqgnvp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/galtdcwnt.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gxfmziels.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfornpjb.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ghragwpdx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gaubxqjmy.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gioijonei.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkuxivgk.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyhmvrpf.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbhlytka.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gsynubtoi.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpclbmawy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdntkjph.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/goozmqoik.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gstlpslnp.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gajnyfjnn.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmruufpse.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnzxztxh.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/ghyvbydff.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdgmuczs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gykpmvcua.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gkjzqzhev.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjpqytnk.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gepupmhpj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruotiggt.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrhapmhd.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gwevvzocm.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gtghowjmv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyoadiqw.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gccjukcgm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsvfdjqk.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/griwxyrnz.sHtML


<!-- 参考信息 -->