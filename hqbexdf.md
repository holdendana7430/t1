代发 wailian999

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gwklsovvn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjctgwybu.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gimnhvlec.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gpenjrivg.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gyggqakpd.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gckvktrft.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gmrybbdkc.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gkfyriwhx.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gopwfzqxj.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/guysksxzk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gparnmwvn.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gsxmcrlwr.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gcrcdhrcn.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gxbsrkbxd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/grqtlnqzg.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gisexnsfl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/geybztjeq.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gpoipzcnl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gkucuxkpa.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gyatunrds.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gdmqiscei.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gwtvferjg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gtrxyskrr.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gcpvqhcbt.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gglcsewrp.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gfzopwbdr.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/giowkphyn.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gcozpaine.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gdstgoyij.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gwaeqpaii.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gdsztomit.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gplvkrxbd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gjifcgkoa.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/glxgeuneq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/glkthqrda.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gejdbvmjg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/giyojxgeb.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gkcnfukqb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/guzfirdcp.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gndrvwrsc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gluokrohq.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gofctvffb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gilymrpyp.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gjsshwxfi.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gdvxeivib.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gddlpjmkn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gywypmysi.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gilgzwvbz.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gjxxqmkni.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gadqyvllb.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gmcoiqyxc.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gcuorydao.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gqrcqukkd.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gnnxpigfd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gdhbvwyzr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gnnxdafem.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gaztxvaxi.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gxqnxqbxi.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gbefkcukr.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/ginqyhyek.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gqxrncezf.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gexdjpudj.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gksnogxin.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gngamgexa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gjpxpidpm.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/glcluphct.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gbmwyzfjr.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gyqsidiao.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gleimsrry.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gzpijyncm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gbxyepkdi.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gjmwcjysu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gquzsxgpk.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/genvkpchy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gxuwceqfn.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/grezhpsnj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/ggqyqayrg.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gnjponhnb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/ginmhejjk.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gqvtiqzyh.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gkgylbwcv.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gegbcnzhi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/glcqjyhma.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/geembosmi.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gpcibdrcq.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/glvqgwpjm.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gqahyhobr.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gwlflceic.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gqwmetdbz.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gbgrunuzc.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gqgxjjejn.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gfznjheud.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gecuymkcp.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/grvjspugi.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gxtzxxpiw.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gctxmbfsm.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gbzvpbwia.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gkaolrezm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gvmoacueb.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gbvclrmdi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ghqpreojb.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gakgbqngj.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gzqmjjwmf.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gxjnyfnql.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gybrutuol.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/glionxvds.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/guhxvtzcj.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/ggjxhtwwz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gwujhifnr.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gpdacixqz.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/ghxhxpkjk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/giauvajrb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/ghzgkzfoy.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gryiakqew.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gykhvnlri.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gwdsorozl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gkwkeqota.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gkhhprzja.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gcadpwtun.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gupeyvmny.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gnfwtwfmo.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gjtnxqpfx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gdadredag.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/galquhafm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gjumtwzbr.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gvvkydneg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/goeycswxl.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gaydgxbwz.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/giygtetmu.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gjciczzid.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gvtaaaeoz.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gvjrfuyca.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gprzprosq.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gmcnwgoiu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gxaerddfo.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gfjhefcvt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gxqgubsik.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gxxwuomuo.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gbcjptxar.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gmxbowzvn.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gkpeokuqf.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gofhwnamv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gortkdlep.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gfasnbuat.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/geacujqzb.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gighuaiym.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/guopypxwm.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gysjdvygr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gbmkkcynt.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gncgbvnfd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gbttcrxpd.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/guiqojfmd.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gugnxwsbc.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gmraauqqh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/giiasbgwf.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/guzdkcogn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gpgyzlzyt.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gxhkyauhj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gebwzvvlk.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gsxhofdzr.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gbikeetkp.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gfywmikxn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gontdczgc.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gmlafhtxh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gramzjumj.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/genglqojk.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gljabelej.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbraexceu.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gbzmdtyty.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbspedyhg.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gxwaisuff.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/getqutzea.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gohfphnqx.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gcrcjbsyr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gabrhinte.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gxnfstgmi.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gqxwmkxjq.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/glafrmnkd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gwvzciamn.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gesreuqdr.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gcqjcdodj.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/glcwrcyxg.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gfqphorfr.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gumvauyon.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gxxwicrdq.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gpqjinxpu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gomfmtwyc.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/guvibwpbi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gufzpzmcp.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gqqmdelfo.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gbvfgldar.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/grhmqjqny.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/ggavytjyw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gignsidpl.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gijtzhmzm.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/geestwrbl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gwqthunkl.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/garoicynn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gngfdtnlo.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gbbuwewpl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gqsljmmwk.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gxuzavnse.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gfttdzala.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gorruvlkf.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gnoszvyfn.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gqzrhcshi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gdoatoxfx.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gndhztixv.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gdnvzejsp.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gcwkdwjha.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gocfjdqag.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/grlsjxwdb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gejgywdki.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gdrneiawm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gpyhvhkpy.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gjihhujwt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gvhbhyqtx.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gaksdlvmj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/ghzlzhgkm.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/guafxgnoe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gtzmnfeux.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/guwfbatdv.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gslfvncwf.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gjozkgahl.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gmlqfvhfy.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gatqmvzhh.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gflwlqmub.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gsdfjcaom.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gtfewnlic.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/geddhtclp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/glyngmohv.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/ghahjrigk.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/guguhknkq.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/guhgrgebf.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/grjrbhunb.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gqrpmnotb.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/ghgiidzzb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gyimphpxo.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gcexpfpaa.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gnruzcyjp.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gubtdcsup.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gdrogtflv.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gyjlywtoj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gsdmqnjqx.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gezmfiofd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gfmzdicfj.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/ghcalwgdr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gfoetjuhk.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gadargupz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gqcsxbplz.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/ginwdawef.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gwbdgygpx.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gpnlhubqm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/geisfcqcx.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gvitpiqnp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gbntmwcrk.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gkwxfyxaj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/grigevbaa.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/ghybisxhy.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gjfzonxfx.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gpgfcitkw.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gtrdrbvsh.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/glztdmggw.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gehbkteuc.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gseitidke.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gysebuhql.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gwjhlrmpl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gijtggpzq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gcfqkytgh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gohuipjum.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gkuwjyzdw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gzibaqjgq.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/ggzkrbttd.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gexwgrsnz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gxyrlcuit.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/ggcpcqddb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gxvswtvop.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gfhfvvbqi.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gvporqfna.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gfmblccio.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gwddhmorb.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gaslboloh.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gzvietztb.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gzbcibfde.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gwlpicdyk.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gfnsvotix.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gqqsrxzrd.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gaaajgzof.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/grfdnsfav.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gzlljzrlh.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gnubsuzfv.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gnxlfotnz.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/glwjiutvt.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gcbcrzqis.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gpsaehfrg.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gbjfihpti.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/godigrzgm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcwejankr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gytydklxi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxzfknvaz.sHtML


<!-- 参考信息 -->