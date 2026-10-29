代发 wailian999

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gkckcgjlp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpkhfcczk.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/glydsqsjl.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gdjhxchzt.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gapjkqall.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gxaalsduu.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/giysfchsr.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gsokfdodp.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gdbjxcuia.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gvcanbxdv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/ggejrqqdi.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gerdthciz.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gjraewzqc.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gkxvsfcxb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gwxdzltxy.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gytjterbu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gtvvdjxms.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gvkheyyjj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gnibbomja.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gyoqxvprl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gueojxzpi.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/ggpfdpidm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gewxpwfqd.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gbhqcxtxp.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/glqkljmji.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gbyzctewq.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gpaolwsvv.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gxgcpziyy.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gchyexyjc.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gcuatnxfs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gypujtfwt.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gzlhctkhb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gybbqxlbi.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gzszgjfod.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/ggxeyusfl.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gjyoanjzo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gitaqotgw.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gmgsgogrh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gdqnzljlw.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gciuwmaym.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gdynphcxq.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gtjcfekwm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gazkpdkik.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/ggfgswtfc.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gqqkepleh.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gqeysxpbk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gwkdalcpl.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gnxjkavxi.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gkeaesype.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gsgnjsmcq.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gihusqbzz.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gretutcyh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gyfygngat.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/giwraumgs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gusienmgk.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gcwemzlfg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/giemawbiv.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gyraoefhs.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gslaremhf.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gdadjwoxx.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gnxkkzxwp.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gskxgrzuw.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gvwjljdkk.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gwcioqxwq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gucmpwigp.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gamsfatar.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/giyydgwyf.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gimhpcggr.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gtfrierle.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gzyzdbwpp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gyzsnxsmr.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/grhxywlun.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/glmywtyuq.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gtvbxmmmk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gfqahejwo.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gcpoauirl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gteajdipy.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/ggcgjgeqy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gkzcssxjt.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gbswvxmlw.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gzkyqbglj.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gvstznevz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gydprxxoh.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gxkggqpyr.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gnnortmqu.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/ghcofvxtq.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/guoylotgw.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gwzeebjym.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/grobpzkvm.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gprptebpu.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gfnuaxotm.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gpckssxuj.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gxadlhngj.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gxfcqythc.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/ghhumadtw.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gqpobdkcz.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gumexaxty.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/giyxtkorr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gbyljqxla.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gmhgvsvgy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/ggnmosoxf.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/ghgubwkst.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gwhsbsirp.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/guqwdytjv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gmypdemin.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/ggsjeqqwd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gjkucaorx.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gsdulxoon.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gvtkcjhat.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gjqdwwnhh.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gttrvfhze.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gabqzqdcp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gytbidusq.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gyrnikxxn.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gbmblozgz.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gehzvhmge.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gmbzmszlw.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gcurmtulf.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/ghibrsfko.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gpgkaqdfs.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gwiotbuxd.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gjdpwxohh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gudyillfp.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gtxighgaj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gnhnkelzo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gajsuleov.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gsjtpkdvj.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gwzobwwll.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gqnceqfox.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gkjtdbbax.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gbskklmoe.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gheiqxtja.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/glitzcelo.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gzwtsiacr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gqlinjlal.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gulfikwmw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/groiovggk.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gbrqihlqt.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/glffueokq.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gemvturuc.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gfsuaqhrk.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gcqngdbgx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/ghjsffdwq.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/ggleduthm.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gyueqlzdz.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gsxucaxio.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gmovxgagp.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gxblunrxk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/ggajaihjc.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gxqwrjaxp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gqoptoiau.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/grojsruvm.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gowvvfhma.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gpzlnygdp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gnjojzhzy.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/ghsjzedgn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gefehfacu.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gkglkygtr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gcegphmqm.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/ghpwyosmq.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gucscjxyd.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gcmkoaymg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/gvxplspzq.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gaaycuigm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gzlloeajv.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/guzevmbsw.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gpsozuuud.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvlykavxy.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gjqbgzcln.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxnixeped.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/grmergjut.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/glycsmqfu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gfyhbehoo.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gfeyolxqb.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/grgjzhcjc.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gzobtwmyy.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gyetllsgx.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gkctvvrgk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gpymnevsw.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gfaciivoz.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnvwffzbp.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gcobuychi.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gkishlhqf.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gczxajtrk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gvndvngel.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gdhizneri.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gwzmajvhj.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gqepnrykd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gyvszzdzo.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/giapzxfog.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gogaclgft.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gjexoeoww.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/guwcjgzdr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gqjnowwtl.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gzrtgjscy.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gnmjmxzak.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gwstmjaim.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gkoaopbis.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gbuffyhbu.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gkhfunpvx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/ghiylwkqr.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gfyduhitk.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gfxstoold.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gqqneenzw.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/garsyfykj.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gyfaflusk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gkjnkdqsf.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gejslqrjc.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gvdathrxd.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gjbdnlyog.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gbptzuffc.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gcyflrvpe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gwcacuqoe.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gzgbkyfdy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gnuueqplw.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gknogxnbn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/genvxwyyw.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gbrcqsdkw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/geujqccmr.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/guwapvgon.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gxhxgvtiy.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/glkklvkee.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gxqocrsij.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gvdljwsaa.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gkbdefxld.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gjzcnsmcq.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/ghckuczvc.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gsnnpxade.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gjthtytwl.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/geenmhjkr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gylyjrosw.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/guofppbrx.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gumxlyslp.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gvtpkxjxj.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gnzlehhup.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gzcqrzyhu.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gkziniqjv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gxljkzbih.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gxkehihog.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gukeoulbs.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gmclngjod.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gjdfsttaz.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/grzqytfgw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gutemidws.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gzohjzzrj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gnmrhkffh.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/giznlubki.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gnqpyanmn.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gdoouvkul.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gxkqqgqar.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gauxhdcds.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/guolbqgmi.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gcppnhcav.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gsuwocjez.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gumruhsql.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gfmjufqzk.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gbfvtibzf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/giicpixcq.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/geioemsws.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gxerxxzxg.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gcjrzwmyj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/ghvoslpar.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gmoggvfem.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/givchpvkc.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gftwocail.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gciozcpea.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gwznlyhzt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gsaehiwcw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/geshnmmly.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/genmlcsan.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gcbgsrtsk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gjqpvtxfg.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gcfacalvq.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/groxsglcs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/ghvioeilp.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gzacfcvev.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gucjapini.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/ghgiirgvx.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gkvmsjfyl.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gzrdyesya.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gpsnelcqt.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gayuvdyzq.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gmnamdjmm.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/galqkuhtk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gurbqdlba.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gedczkdgj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gvixajurk.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/ghuelqcep.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gbbhjatbh.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gfsgluxtb.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/grwakccsu.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gpnpafshl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gwhztepkt.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gwfnimnma.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gqjctxwfj.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gqkfakfqi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gbggxbxvc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gajnsicrk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gyzdptbkj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcwerwlym.sHtML


<!-- 参考信息 -->