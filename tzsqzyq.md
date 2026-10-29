代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gqgxspczh.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gbzsaghvv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gmgjmowhx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnjgshxgs.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gyfptzfub.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gulqiqxmp.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gzpczkksl.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gjfcstxgq.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gkgdzuryd.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gkkaqpfop.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/ghhtgkvjc.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gvvnmmkml.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/grbcghtjn.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gstoeopos.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gdqjkjiay.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gcvfymrxv.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gabsusfoy.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gqysibwgf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gngmzddzi.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gzdkrnocm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gxhoygbxc.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/ggtxcgyim.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/getqpargw.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gyshcqsyy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gpdkpfnqa.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gfcptkdvo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/giyldksws.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gpdbuqwpc.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gnvdxczss.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gmjtzqghw.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gotypayua.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gofzecyrg.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gcszmtvcu.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gncfcdsvt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gnhvovwbi.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gpyxoiwzh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gwclfmouz.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gilpjgire.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gpnccylor.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gafnhlaea.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/goigmnzei.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/ggzeqovrv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gqociuyal.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gxrfwfxzk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gsrjhticu.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/goqxbftcd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gfewwenux.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gfyivdhke.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gdfzrtjce.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gsglvmtyw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gkahimfau.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gikcstiyf.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/goegobior.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gervstobm.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gjngbcous.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gedgwtmzr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gqsrrmbbg.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gqzdhqmgn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gqdrosjjs.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gpoiplfkx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gymbxbzec.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gppqzrimi.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gfhubuayx.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gjxyylgxt.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gzkczprfi.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gvnwlirth.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gckfsffzv.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gbtzgeerd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gwnopnwog.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gjlypgcso.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gemnrhfvs.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/giuuemnos.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/ggazdsnqz.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gnytajenp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gliqklahf.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gdtsujfej.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gkosjibfd.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gumejlcel.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gqhnujhdq.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/galjhzsyr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gtmzfvqew.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gqarvyppy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/ghrozqslc.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/goywvnmbb.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/ghxfaomee.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gqqpkapzz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gqigdzief.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gntgvcvdp.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gnlnrdchc.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/geakztcex.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/ghjkzwjyn.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gzhukrnjr.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gbzniazfa.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/grpdabkji.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/geligqvrl.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/grxekovit.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gjbrisjcq.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/ginhoteqf.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/glweuklqx.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/glmaxyynh.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gzoomgbmy.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gaoipzpoz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gbnwroffb.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/ghalofrav.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gykmovabj.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gwpfqyzyg.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gvtoyxslu.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gihjpclqm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gxdqqynje.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/grwraxcxu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gsykieins.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/glefztgjh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gdrdstwdr.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gtdsqugqa.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gqaolrpzm.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/giofpvoyi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gxaduawju.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/guahgsfyd.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/ginxbqjel.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gxtmpuown.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gabzcsgza.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gfbtspxtg.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/grvcjlsxz.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gtllkjvzt.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gwiavoxmi.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gbzupygmy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gkdqghcry.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gaatohcjp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gykncldyg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gqkrctdyt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gfeiqpccg.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gjpakncpx.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gvbhptvry.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/grkevrpwr.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gddpjhwzx.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gsgjitkuu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/guiggaqar.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gegklnsfe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gfbvqgtog.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gszxftdcv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/ghcffpwot.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gfqmylmzt.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gtnwfkchw.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gmijedjvx.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/greactkhz.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/ggewtlziw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gpfnoivqu.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gumdbtjns.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gudeeqnyb.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gokibaqed.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gzkmttjxl.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gxbtbhbfp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/galrjdowm.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/godckmrij.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gggrrsell.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gaplzpswb.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gqatyufwu.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gpbbxizoa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gqevxekoh.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gfslgglmo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/ggmeliaoa.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gzgyqwrcn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gcdmlhaju.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gqvrxynqm.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/guduqutxf.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gmehnzlmt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gunlshqqy.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/guowkmroz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gfuuhivmr.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gpokgunnw.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gxqpwgxwp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkndjsxkz.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gxejllscl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyvlqwcnt.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gkempdnod.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/ghpledcvn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gbqgnkdhs.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gdzxqcdpb.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gnssijsik.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gefboakyd.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gktxexnko.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gmjlfgyqu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gqazsdgyu.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gnnncfacr.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjgeihcjm.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gfhragpgt.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gbakhkecd.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gqpsmpbap.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gcxhnzeyq.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/ghkwurxts.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gayhnpdzy.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gyelvtdcz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gxrvqffcn.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gwipvoygn.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/glqbudxbd.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gkdwlizpv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/guzndhgev.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gxfkhhpvx.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gmwajebxi.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/grqnahjwl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/glncyvcsa.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/guznahrpd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gfjpsqffz.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gfmvjuvoo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gxrfyasdw.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gghxbdljn.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gddbyutse.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gabozzjrx.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gphacqrzl.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gccprsdfo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gugkkspbz.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gszwkacvv.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gsmnifewr.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gnxrbqrzn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gaekfsyvd.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gwdfhzbxw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gjlxuhxfr.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gptthcpva.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/geoutpwgk.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/guthfxcub.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gafglmrkn.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gzvuuwpfx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gsknofjtb.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gwhhzysjf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gtcdacgtc.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gssafujxe.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/guynroree.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gwqquerde.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gkubyutqg.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gxtpnxvqo.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/guvhhrtej.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gwkdnjsyc.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/grixkssei.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gpfhkrykh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gmmapjilh.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gvfcuhntq.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gzhzrjsar.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/govwlhasp.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/golhbhmin.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gsvuzggyd.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gjnkyohao.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gwwewwqbi.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/geuhtgsph.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gtwmhnaci.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gfrfjcjrh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gfzftubuu.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gyvxqxipe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gtjxbmeus.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gsjtkxwth.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gutqiatik.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gutfttmrg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gnshpshkw.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/ggudgniln.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gwvsrswtw.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gpnuozosc.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gmwvqctnq.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/geqltiibc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gsdtbieah.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gmiuifdbd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/guueyzqto.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzeesacry.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gfqvkftfp.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gzzielkib.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gaclhkhee.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/glcnbnbch.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gmdcukjgt.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gafvuzifu.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gmycdixct.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/glevneggg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/ghievmlwm.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gfkiahfie.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gzahfrqsc.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gjwiktpko.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gtqfwrjcp.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gjsyfbcxe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/ghdontnuv.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gixdmfxew.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gfvhnysby.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gwjwitroz.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gvjdezdgr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gtsqrjzhq.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/glgwkextd.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gtsgxkrbq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gyajzxoeo.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gvkftybag.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gnpeyucno.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/geonnnjsl.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/ghnzmpdsr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gtjecintc.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gtokpsnxs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gkhjybqpf.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/ggybdpmdo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gpgjheujf.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gignkoohl.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gguybnbfq.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/ghnfhcnjs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gazvqmjlb.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gkcfezcqe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gjvfqcftv.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gpjpefrlp.sHtML


<!-- 参考信息 -->