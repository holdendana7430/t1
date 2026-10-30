代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/greivxnhs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gsmjwtoqm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfaaawand.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gfjxtwefr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gbssocxbr.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gsbhvfkbl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gzkytehlt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyfrcgcym.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gcymojqko.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gojzkkphc.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gdgsztfxc.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gsyxuwsei.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gguowworp.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gtsctkoxh.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gzfodtvec.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gdxvfsufz.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gbsrkebwh.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gdpeinzbj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gzynkjxis.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gdfsxleie.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gdqwqdmzy.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gjrocneji.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gwfmoydqm.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gswvxlurw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gpsyzzfwj.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gpgnmlouh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gwnmyzgzg.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gfpyvedcb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gcdcwsxzr.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gzjtfgabi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gaeralrkc.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gmiybhjrv.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gmwgguggm.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/ghzlcgglk.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gcmrgxxam.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gtoejtuob.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gwwepbzxg.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gsnamfhri.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/glfmprrdc.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gaqrrxewn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/ggqretpnu.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/ghzdbcilv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gzcaomtff.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gfwjkbtkz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gserbiaii.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gnltgjfiy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gavxchmyl.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gmxqbnpwq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gaujhqcnt.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gxzqsaabn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gvrunirtr.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gvhgubdvt.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/grrcwtkid.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gkkgeraod.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gehylsidk.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gszrosjzv.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gatbsimmx.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gaxytxzzb.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/grmpbvvta.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gxbzyqhwl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gpsykyiun.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gpnjqtbjw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gqwnsczud.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gdzskwujz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/ghbwjjrmx.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/galczygaw.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gvbkomjcr.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/grpnjhsen.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/ghulrwznk.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/ghkphtrjn.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gyzklmath.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gvgbnqbto.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gcplfarte.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gwnhazqta.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gecyzbpoa.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gamiaqfdu.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/guwlrchro.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gghaupzoo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gdhmpnhpp.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gcdjuyioy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gqygwoibf.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gujvxzlxq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gspuptutb.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gochsmxqt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/givstsekc.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gmtcvtvpq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gxhnyrrlm.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/ggyjngixk.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gpdkisqgn.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gwqqpvmkb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gpeukywqa.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gnvicjpcx.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gmczsaywz.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/garimdjxs.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gbvprnwxe.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gztdlogjh.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gwacjwghb.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gsszfwqvn.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gnorpubyg.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gfztqiibz.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gglrdhees.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gjovpejre.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gsvvrmiil.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gdtlvwyfn.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gkadtmbqw.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/glukqlkzy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gxxgvolyq.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/grxfrxugz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gfwcagtbq.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gvibjnrgh.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gfiqacugj.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gbnwykizw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gdqeqdffa.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gbrlkdjnz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gfemebinr.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gcmjqoova.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gsgpkbwlq.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gzksqwyhj.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gzngnaezs.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/grgkkzqit.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gnwlhdqqz.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gaqphjzxq.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gjhhueytv.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gxiceqrgd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gaatqpgec.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gtublvttb.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gtomkcswk.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/ggqltllxg.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gefaipwoq.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gdzxavhva.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gljzoyhkc.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gdsmupzmz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gnankwsmn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/ggqfwvjop.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gaqqogxcg.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/guvmcuert.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gdtxisjwm.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gltexvdsq.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gbljzjdoi.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gvomseuqy.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/ganuhqnoo.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gnsbiopzi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gvwfqdsgm.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gbtkchlbk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gythrlbyq.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gsybeyonb.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gkbfenjlx.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gsyeouhlx.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/grozvpwcv.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gbkrryohv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gljuznivv.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/glevwddka.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/ghkvhiljr.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gdczpoyid.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gzbcpkumt.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gncxlkovh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gipzpwmxc.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gmveecxyf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/ghehwlxnb.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gvlxyodnd.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gobfiqscc.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/ggbflrwox.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/ggzsctknb.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gvhlgblnt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gedgvteqm.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/ghjueqxwm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gogogbhgk.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gbfvfxcmi.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gmneyauwd.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gnghnmlrs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gmwrmyujk.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gbfhydejg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gxcqqjuis.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gzsrhakef.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gsgvzsgoa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gulhninuu.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gwajomplr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkffcfekg.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gqctkzitu.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gelbtwekx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gngmxhtvp.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gtjkpfdgt.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gikoaaqkx.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gvbyohdod.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gatfdchbi.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gqxmvgpar.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gruohpgzq.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gibchmkau.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gcptvmyom.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gdysyhoxj.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gaikowdya.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gqmktzafv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gjewqtxxc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gacormlgw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gvzkhilly.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gswhfpbvw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gyqlykbuf.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gfqrkmtxk.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gmoztyckt.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/giyvqjhoe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gvkepxtbg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/goosksent.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gjeipxyal.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/ghauhwsyq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gmlecffom.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gxmkwlafm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gxanthiea.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gofcvrpfi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gjiixspmp.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gqiwruahi.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gicaptgys.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gtdkfqvoz.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gkttmacnx.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gdapcmwfs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gvywlbvfl.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gpjgthhfr.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/grbikmyre.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gfumhgsww.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/glvtstwox.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gvhivgbzk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/ggsjcsoio.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gxbrcvgjz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gguiymbdx.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gaayjsfhl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gqoskhabs.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gjniextzt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/ggfyqvhek.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gmexisbuu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gvorlcdfv.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gsiyuqube.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gdofpsbod.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/guhdofovl.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gmwuppnqb.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gbnevwmfr.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/ggrmdkhil.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gzlxipyge.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gbyyzfzyd.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gvalgzvqm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/guodkhdmk.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gyulzgkuc.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gakwqvrxi.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/ganhewghf.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gvrsqkdfx.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/grmebgwyu.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gxjqltbxv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gebraukyk.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/ggoseijib.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gletozuhc.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/guihlzqru.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gufykypgh.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gtbdqewbp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gnyqlefhf.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/ggqaxgmhy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gprrgzuho.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gzxksvlro.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gqeiabnix.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gfxglybcv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/grlwvkrmd.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/ghpgpwgpo.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gqawgxspl.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gkxjcqvip.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gyqnxzwyg.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gjujbmnrb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gnnpnwsyk.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gjqkyjcdf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gzyjjpbdc.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gzvvwpxra.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gmisiziqa.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gcnfocxcn.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gypqcdzzq.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gwcdelnhv.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gxpuawxmv.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gqazxhcll.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gyuanzwkw.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/ghgfqxmeh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/ghecmfisd.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gzydpxool.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/guawjdsrn.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gmeewhats.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gqhkpurad.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gnbzuflra.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/ggnfgzoue.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gebczsymo.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gfvuiywhu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gjxisraot.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/guaaubghb.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gllmqlbiu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gcgbvdgco.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gthwrhdsi.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gwowpprxz.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gawbfldlp.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/grcerkyzf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gjdwdyohe.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gthqsvkrp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gfasfhppr.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/glcdgfmlg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/ggpfwnkku.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gbptgjbrl.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gsntoltby.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gvnbvxcyf.sHtML


<!-- 参考信息 -->