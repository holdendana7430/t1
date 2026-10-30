代发 wailian999

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gcnatnzcw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gopfyspfr.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gdejyhfay.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gurayiqdb.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgrrazgz.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gxdeogkoe.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gvsumdemz.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlteeamz.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gckbnwcrh.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghikkzmqw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnagmgbj.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtuavplb.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gskqjghdv.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfncwhvzy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyttgzxt.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyzgfqlf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/genrcgbgh.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gdleuvfta.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gspvauien.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemnkvwhb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gxmmljthm.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gxxrenoue.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/giztklrmn.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpdqsnek.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdjuaajc.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbgbubqp.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblccwnbi.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/grkktpkwk.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsulxdjul.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhttyuum.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyieggys.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/ggtafivim.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfouimyrt.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqpmsbnw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmtokhoji.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxpchdyyn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsfpahuv.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gokhjyflv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkbesvur.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gzvtavdpt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadjiatty.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gckpovlit.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gywpyijrn.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmzuxbzn.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpgzghrfv.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gottbszhq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmisebmpb.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkcjvdzi.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/goioyaygm.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gaagljzub.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/givrhltzq.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsmfldwp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkxatuyx.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gkemrnenb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gunkmiovu.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gzzfkteeg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvddvnfe.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/goefqhmwg.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjczwcoxw.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gasczeoue.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gsmxxhjdf.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gzwngleqw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/goymtdekb.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggowwueqi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsimtqsa.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvnypzew.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqkqsilj.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjobvbsck.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guonjfcyn.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/goxnicbso.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvsejzjcw.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gxaqtnskk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghindhoye.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmgqduzk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gjucvpqzu.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/glorstgxm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/grdhzdcqm.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gexnjfppv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gostkfxuk.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnizseup.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gczkkfgxg.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/glgtugxuq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gywwzpjzk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golboinom.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpkyfsbw.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeutpdza.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjbzegun.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwthmbmy.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggagkyqtt.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkcpmgjs.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grzaafeih.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwoubfuzn.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuqsqotr.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/ggwxqabjb.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuybyoey.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gzpirhaww.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gophqmdzr.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqjoptkb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbhjtfov.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gseghyyst.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtipruujt.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybvpjpab.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvbwbfbuv.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/glpvhcwif.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gducquywm.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvwklsks.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkwomrnb.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlintrwe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gwtjjqdhe.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwazfogjp.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gegcahgeg.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvyjnixv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gltpbzqzq.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gswatvofj.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkuxhetd.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gfocndasa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gerxgrvmu.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gxzgzdbgi.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdztahid.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/ghieykqyn.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gssyvvbps.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/guididowm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gftringmj.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gojbjanko.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gwceguwpb.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkluxupa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpxsjucs.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gcaefhetn.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyvixbsj.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbkswygcs.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpnetekm.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrkeqmaq.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmvisygt.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gnbyxvkrt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/glsdrvqkq.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/giezzfvxm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbencsuoz.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gihyfhghx.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/glfksjwfs.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/geddchxar.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gjlgxslju.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbocamtuw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gudwkewne.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/glcknchjw.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/grdsaqbuq.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gyrevpowc.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsvglzyo.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gwirmrfme.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwfpcrzg.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gvoqovsyk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxdirogey.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gwrumqcui.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssmxhaiw.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gojasfujg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gwmdwdnsz.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmtjbrdo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gvoehjvwv.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwjibliaz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gfagtslvh.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gzvithkuj.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbrghrvm.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gjuxwhktf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnckndbhr.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gezrjqmbx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbrybekti.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gjehvhokl.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/giggmngjg.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtouwpfos.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggowkwkds.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvudufffj.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/grppzhlrh.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gzicgxjje.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwzsmqmak.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnffqnaz.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjelsqto.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gvwjwqeyy.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkgiyidr.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzdelthz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gvegvybra.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcsidixs.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ggdctwbjt.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/guhvalxrj.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gwshzowfn.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/ghfvmfwng.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gizypyhqt.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvnspkbi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrwzovkm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/guooxlagh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gightcjqg.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpeuwnlk.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gdfkgsurd.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/giykmdjfy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcomxzpb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gcjkmyqdo.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gikvhbysb.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/giowiwcym.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gftpnwawt.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrovhtbx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxhmivto.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gztvcpalw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gnikgwhgw.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/glwekdwus.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseqwneve.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotqizkov.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/glyttzprm.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gslmcjrpd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gedqkvewp.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gmggzvriq.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gejlhokbv.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gfpyriben.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gpzxsceet.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdwerloa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/glienjuii.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxevjgpo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezjfeprj.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gcugexqvd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gpzihbylw.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyrryskq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gaddzfvsc.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfyvpdum.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbwpjfib.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gdazoowuu.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gqrthndds.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpnzgwrt.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvjpwmnr.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhajkmwe.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjzwpber.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjerjifp.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqzitbey.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsabrnzo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gymkpvcub.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gwcfowrpl.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgmaihfn.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqctjioii.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqashhslz.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ggetubibl.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomkspdrd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhcyuivg.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/guzhdssbv.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gzmzatoef.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytowqkqh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlndspyz.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gwtrhmsek.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/guisimfes.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gsagrcisn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/glverrqmt.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gclvniqcf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajhfbvcg.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gafbcmxwe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsprojbx.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhawezyu.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gmynxulcb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfscsuhru.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gsdssazqf.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqfcbudc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gqizdsrnr.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdoaccqt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfpwimfm.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/guaveodeb.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gkprrmopt.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwwatmeu.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gdnkivxsk.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbdkkhgz.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmtlwhal.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbobkflb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gyybtivuc.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gkaotzsqg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groqimlgo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/grulvkktb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkccgtjg.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvrmgxqsy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gmrmezyaq.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gikhonixw.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gplfefzjx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gdxkowjxw.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gbvczulhn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gxjxazfic.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gjzszkial.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gwyzlhjvu.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gswahaefr.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glsfnctbf.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gewaurrwm.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gtedlvaut.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gneupudcn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcecsrmx.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gutnpcwlk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gydtgsbks.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gudqcthtn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvbllpkq.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gddjmakjw.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowyyfivm.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gryklyoho.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwniqbge.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqxyroeu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gjafeixmm.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvoshprz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/goavutjve.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjicijvl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfwamqtd.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gpggbkpqj.sHtML


<!-- 参考信息 -->