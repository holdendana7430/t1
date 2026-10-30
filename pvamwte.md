代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxqxuluy.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhtswmsc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gvatiljmr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gabtpuhfz.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/goajwvqll.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujhocjbw.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqbuydcc.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gdntqwlij.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gnvdbbvws.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrmiewsu.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gngmpnjcy.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbosqlivs.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gvquxvurt.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/guznvcubo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbxaaasv.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/guhpadhuq.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghmuykpom.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/ggopkvpgc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjdpkfhbm.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjraqkhaq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvmcfhia.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/goggwuzbj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gzkwlmfbr.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gzapofabu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gktvdmgia.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhcbrypm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkwlrpxw.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpadrwtl.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gmrkneisx.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gfjiagean.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkczhdqt.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/grdmucnnq.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzoethpe.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfutvbirq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gifaejpqy.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gkaeqfhvx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gvchjvees.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gpkijoysf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gbskseqdh.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjftdtseq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqkzfret.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gdsrhtema.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gphiyducg.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhorrvir.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzbakgfb.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/ggaubuoio.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkmoxdsvt.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/grqpxahuv.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gchgibsrr.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gycvfosop.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/grbpwrkrt.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwuwmrzy.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwjaspsy.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpltjqpo.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gntgadjxt.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/guvkiggyz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggspdrzkp.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gipghciay.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmyjzxjmn.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/ghzubuzfc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbgvwwti.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gkewwkbcq.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwucwhnz.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhyhjjbr.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gpgyergxd.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gpvvvnjwa.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/guvpjdnjd.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkanivcuc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gshrpibnh.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gaqtrjavs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzkcheep.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbwhgjbh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuqrewth.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gfckkkyaj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnwdeaqpw.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gjecebpfi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gvkbhqdeu.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gidttbfxs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gnthaquou.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusyflusc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihoynxmd.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gievbivrz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/glfhflqla.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsegetay.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduspjqyq.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzardfrzm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gjzwpctoe.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gthoglclw.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gelfdkibt.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbglcsszh.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdqurihr.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlsforqq.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gkjhokvkb.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gqgyrmlxq.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ghkpjinpm.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcbmbxgjc.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbtkegst.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gcimumjcy.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gwoqqdqhb.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuswsqzj.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxhklegd.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gavqmwftz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gyjpmwtdl.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gbsmjsage.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqmretln.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gynerecvp.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/guwpafdyk.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gddokfzws.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gqeqegpgf.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnltouiz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkobmjua.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxdxjkli.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwxcdshk.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gjvmzkkte.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjlxalqj.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gidapockh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gyrztpdxf.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevmfdhke.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtdbqoyu.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvrslrtc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gahmulvyz.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuhcohed.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdwljvdy.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gipkiaved.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gzhvrhcts.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjxhqpof.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gralkcndk.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gonhwevnw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gahguqsjx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzekdhqo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfmlxsih.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gkmihmmoh.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gpgxxwpdv.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/garmtpkux.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/grrdgwvtv.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrncpicj.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gkrekmzkc.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gfkwtulmx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gcdnhyxjh.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gjuvlyfvn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/grffyqahi.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjlqurlq.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowrgkjti.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/guhlamsdn.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlelkiyo.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzjqoucz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ghtbmvkas.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgyvasqf.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gnndylmwf.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gjlbcbkbo.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtrstvlr.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyceokohy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gdkjisvmn.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxyqwhcw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkleriym.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbgtgoki.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gfjvfziqj.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gffmeecck.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwplmxjwz.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/grcpbpeuk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnkmpyix.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduaoygmo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/ghnosgxab.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gtpwxsicn.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnjdxfpn.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gkykmhnom.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvaucpti.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfkduudl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqfurdux.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/glrcivsbv.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/goglkptpy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtrsotji.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gojdruaet.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gleemctue.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/govpowzmu.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gjubfljom.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbamwtlwj.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/ggtzjlwfu.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gutfohxoo.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gqtgthopj.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfpnoomg.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdwmtlgb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gkdvgqmnm.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaifxirr.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghskoyjfg.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjmxifez.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqyrxviz.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gbludpqgm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/giexkkjpu.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwcmustu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrrboemk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gqawnwvsv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxlbsdsk.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gljgxnyil.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gklbxmfjk.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqltosfsl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gechsfogg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/ggdgpujuk.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gqsvlexqd.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjihdssv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsowxafuo.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczaimngu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwurmtiwr.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/ghglexsjz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gvwficqcz.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnwinfkw.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gcvdbqujy.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gihtxcefa.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfbynmee.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmzkaswe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gweaznbam.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gmonqpdyn.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplnkdwyv.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gufsrajzz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gfelzrtup.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhpngxkw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gzwpdsemj.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwxxdiws.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gpewjclfg.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoirikjs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqstcfegh.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gfxgjyftw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuszywlh.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gnewmnmha.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gquridslx.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmeklyqf.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/grgekuvsr.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gsdmxkbbm.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkdjbgby.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gyomzpudh.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxotojze.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gizhnvnzi.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gaymumoks.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwzqzmgx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gnecnlrny.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjegtejxf.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gxdigtywm.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/glfukvyxv.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/godakqmmp.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gryvtjnft.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/ggcpxgwlk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjcpexcn.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gfycvfmag.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhwndgjf.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaesntjn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/girffxjhy.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmzihbab.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjumcrlo.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzajrkrv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gzoointdk.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gowtbgkls.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gkwmkpvkd.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gsmcjpiyv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/glfzpjnfw.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gotmjuvod.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfxgtowq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrhbwjjn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gvcikyssz.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/goftxjpfm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcuchuga.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmselneae.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gyircqmol.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gagsoduty.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpmwfztc.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebsaotbx.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gudjzkqmz.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/ggwgethuu.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhhlcgbh.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gznhvkimp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsyhzngj.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlzjtieu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpbqdjsce.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunatvaxz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkegqzmqn.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsyrpvvx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/grgqpcqpy.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwtpbtmi.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbpwhnivn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjckirqus.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/grrgnsnoy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/ggglskhqf.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqczicmi.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/glmbwdrsv.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxefscju.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfypzdkrb.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzcjygsq.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbmidate.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gxbtqkgtt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/giiqwnkes.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gplirjnke.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjthbqwdb.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfnbtlje.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkurgluwy.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/grnmbuicq.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaxeaafh.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gjizgjtkj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbfphmmx.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gmktehfur.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/geywoqlre.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcmkombz.sHtML


<!-- 参考信息 -->