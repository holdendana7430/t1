代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gzkzqzpzk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gdplfugjy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghtzqvwbk.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gvabgofnp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gnhzntbul.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/grdcnztnq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/glwdcxcul.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxlitwxmj.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gyhsptzve.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqsmydkpu.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/ggzwnhprd.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gsdjeubaz.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gqqkzazjw.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gxbocitxu.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gzfmcqnxc.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gwnffyngk.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gfmrhbcpp.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gmkfsxuud.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gxjvzysfh.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gegqhktlq.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/ggyatquqd.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gibpjcvup.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gfgroknns.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gjfggqukc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gvgiaaffi.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gjbchcbru.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/guadnmoui.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gsgzqhqzk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/grpspujqa.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gekzqycou.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gkipcxtzk.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gxnuzxaba.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gpzheiiyo.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/grivyettg.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gyfbxukrp.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gfpbnnegq.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gthohfzuj.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gcophpfod.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gpnxgrgll.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/guoxhddqt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gkmcdgymi.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gequvgedm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gtzktyhkp.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gydmaauoz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/ghuiusflo.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gweulhffx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gpuznfxol.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gobgcmgdy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gdhyyghsm.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gowrvrrvg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gpqplflly.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/grofenlrk.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gzamscgay.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gtudkkwma.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gkkelqtyt.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gttoqzlvz.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gqdrqgsot.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gtbglvscz.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gryzgcglj.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gxpbicegy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/ggrodjook.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gyibgyakz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gygazxumo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gffwszayj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/grnnbjtxs.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gvepbwhdc.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/grfdpmjqz.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/govpeknqe.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gdbyvragc.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gyygdvvwu.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gjkqsgrvt.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gonlvwqgb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/ghwuaxybb.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gefvjjvep.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gszhucwfx.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gaqciitwy.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gsjgmqfvn.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gzzgnlxmy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/grnivwsgn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gwcjujclp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gtareuuse.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gmfnmmcze.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gdpifvidk.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gunrllmqg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/ggiwznczm.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gjxuwduhg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gkovbwbfi.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gphohdlrg.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gkvlxwutx.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gpjsrvgux.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gnkwauipz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gzdgteqkm.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gfpjplobe.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/grvexczlm.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gnyiboaox.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gxfdnvzmm.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gwhmypfyz.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gqkyculvs.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gnjtyctpz.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gkluxmmtw.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gcjftoaja.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gblnfqupm.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gzmckqgoh.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gizpvmqia.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gnhkynubk.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/giknqfuwr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gtkzylkjv.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/geejjcfjs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/ggqqsuwtd.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/ggvtnnwws.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gtpkxczje.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gvwfqmzde.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gopdrgdwh.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gksfnpmjd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gpxuqqwaf.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gbhqtpkmh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gsyfpdpyk.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gtxnfrewt.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gvzcegrlr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gdgyzmcrx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gyjmjwtko.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gaictxtvd.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gzoqpoeaf.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gzayaackm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gxqzucumd.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gczekhycy.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gaiczmjpy.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gluejmeiq.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gngffuwqo.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gtqyzoapz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/giwthqnwb.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gtftwtacm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gcrneliyq.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/geuqqpqlm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gkhltizww.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gdawncxch.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gbiiwceil.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gqjfgqipz.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gswjcwynj.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gyyosfqbn.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gizcnsbpg.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gnjvjlncx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gqubfcysq.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gfmdfnjky.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gqmkwatnf.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gmtycmidf.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gjmowmqxx.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gfdsovywv.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gasfnngwi.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gaftznaqd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/ghajbwnmu.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gtqbxdlpp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/grpyuyzfc.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gbkgjtjwb.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/grlzakrxw.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/ggpobtbaa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gnquuxqpn.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gpugkdxet.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/grbmtvbnv.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gxfenihdr.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/ggryfjgfq.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/ggfsjxtxr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gvajndjxs.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gzywlcdew.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gpuzslgzh.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gnbkpiujd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gwlvtwvmq.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gslpnabpr.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gtyviuehc.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/ggrvbzjco.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gcnhkxnfa.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/ghgzoduje.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/grdycyljx.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gyjqvplgv.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gbepnjbiy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqpctfcfb.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/ghpsbdanr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gstxtlciu.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gkxhruitk.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gnuowjgzp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gsudzirlg.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/goszvyvcf.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gdjiknpge.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gcdeysaaf.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gvrvyrkhu.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gkydeupar.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gjajssgfd.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gakrqtxfl.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gacllconx.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gzhgngmbq.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gumzkwrdq.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gympwxbks.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gztrukzhb.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gohoayont.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gszvjcdsp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gncwoqumx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gstauhtkp.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gbwphgrqd.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/ghzgdwtby.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gpbhtefji.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gtcwczorx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gfrcgdmav.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gfaipfuve.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/glezppkcf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gjmduunvj.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gonerkkow.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gudiiywjm.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gcidxxzvl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gvfzxfwnj.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gpyjzdzsw.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/glrlivmzb.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gqsdiyzfh.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/ghkjnxuly.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/grqljfhcw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/ggacocytf.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/grfctthcz.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gsnvdzwju.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gpwarjmfi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/glertmysg.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gkcvpwgbu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gdxopocyu.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gvowkgbeg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gruwyvdfj.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gccstjumw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gzuqfxtak.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gvukzvksg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/guxkahkil.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gttararrn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gilztycju.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gswdvfghb.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gdgdizbjj.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gfyfmtuxp.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gjehykinp.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gulqtumte.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/ghrqryayn.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gviealxqt.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gaeqllvkc.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gjzeqwgal.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/glaotrren.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/grpaocpzj.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gmodreohl.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gjkoctykl.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gcncfmgrr.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gcgyvrjvf.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gkdfrdzkc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gebjnbdlu.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gekwmluau.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gbdevanxz.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gerejmazi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/ggoozbxwq.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/grlwuuatz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gbrcnanlv.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/guyyyrliy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gyfrbfgff.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gpscldbhw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/glcvbggwh.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gvhjatbtk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/glkkuchho.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gyqwtaltm.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gxpsfjcoa.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gabelsngo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/glomwloxl.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gxjfxcdlu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/ghghbbscj.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gabdohdqs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gkovjhxrj.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvzsomhtb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gfsulvgce.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gkftbrsgj.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/glgdhpjkt.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gejlymwdf.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gjzkjrula.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gaqbcgyao.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gzpnkljjz.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gwvpzdbft.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gwdlgsrpv.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gvvnmpdgz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gmvxnyscx.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gwnpgxaoa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gwjtdlqil.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gzmzrlpns.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gbrttfvsv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/grswqtfwi.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gdswnjnjw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gdpxkfxxl.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gxxeakthw.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gzvppqikf.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gjelhxnxk.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gydjfrsro.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gkiarmlbk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/grytkvvfv.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gvoiqkbth.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gehxwfdxo.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gbaxltgau.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gxnglzetc.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gwfyzphel.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gjqsaftll.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gctryitbr.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gunybkhlw.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gwhwgangd.sHtML


<!-- 参考信息 -->