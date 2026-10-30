代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gvkxligrw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gxnsrtdwa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdvkmeoxf.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gancqoeyx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gifmdsjmp.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/griufaujs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/grmherodm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfndokkrg.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/ggfhouqmr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glfnennzj.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gkzlzwdrc.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gnynkmqtb.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gmyhtlagm.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gccbmylrt.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gtkioqlzb.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gpjvfrstl.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/ggrigyovn.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gtmcpfrat.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gbfdpuwlf.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gqtkkexnb.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gaggsnjno.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gvisyevhg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gquxjjbeb.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/glgjgjzxd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gextopbua.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gdqyluyfr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gkmhgdqvb.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gbhccxulj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gnjwsyxua.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gekexezqu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gfcrgpwnx.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gnpuudgvh.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/ginhxcvjt.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gaiiuvutn.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/ghtxhzoxs.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gcpchlfvd.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gpbvlhudt.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/glbohfiwk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gjrixglps.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gqbbojjiw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gmbboeepz.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gkbdyqqtc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gcvlomyhc.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/guxnbvzky.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gciydwmlw.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gkeackcsd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gzmemunln.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gdcjcwsxi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gqawceyof.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gztedrjyt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gbvuvzvhl.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gtldyljue.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gpgzotgza.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gasbyhsxa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gorhjkgrq.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gchibzilj.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gopzjsnom.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gqsqnciqm.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/grutlulyr.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gvtmjobqc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gtyjqyhqj.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gbcegfygg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gnxsrnayv.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gxwqlhkzk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gflvrolit.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/glmxbstzn.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/ghixxhyll.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gxtgzyjzn.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/ghpanplcu.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gllegyiur.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gmrxzdefw.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/ggukrutyy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gbmskmqcm.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/guxfwgdrj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gyxcqokbd.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gjlxddexg.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gvjjuabgt.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gbwuropyq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gklpajree.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gilbpgeri.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gdubvzxjb.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gvzylslbl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gcefwdvaf.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gglbuxomi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/ghizgahkm.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gagsomybl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gkkxzefsi.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gyeflqpeh.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gfveagska.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gztvgoiij.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gfyobhslo.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/geyjofssr.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gvicdliui.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/goitdcall.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gjvhjvpbl.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gxydfjjzn.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gonxfxfnf.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/ghgeqzvox.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gtajhobez.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gscloiqny.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gfeolbrqm.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/govfyfbbc.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gufbbejum.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/guaoakhzo.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/ggcdkwpbl.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gmtqrhnvv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gldoifppn.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gujflfcpj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/grhhtuwig.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/geinjvqiz.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gztkhxbyn.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gduxoirzb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gfgzbdqri.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/guqngwtdk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gczfofysu.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gdsjwfyht.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gjgwgyodx.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gxcpfzald.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gcmrnpbjm.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gnfxdkxqq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gfubpnbzs.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/glyuvjnwr.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gbckxpgpz.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gzbkwqsoc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gcefesjuo.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gmykaebtn.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/grhwfepgh.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gmknnylzi.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gmwpqorkk.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gdvliegqw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gbemfaxed.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gtremefoi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gxlzuhcjy.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gkfwlomir.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gsrwnarxj.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/glyjxkfgr.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gvvcwahny.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/grdmlrwic.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/garrbmgkx.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gwljjlkbh.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/ggsllowbm.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gsadueuce.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gvcwxcoen.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gwkstxaoj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gpfcdgtfd.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gtlthukyi.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gerefpgih.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gibrkmtsj.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gyowgdyyi.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/grigwhnvv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gupsevcss.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gyincwnjl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gqhrjjsfg.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gjlegzueh.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gnxzsvqqs.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/garyvpoqt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gvtvgbnft.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gjgnxkbok.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/glicszgwt.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gearmzypf.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gnbsuqdpg.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gqpvxzuux.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gudbspncd.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gmzfwwkfx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gvsnroruq.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxqylexrx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gyberktqb.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gdwfkcpst.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gkzmifmng.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/ghybundiv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/ggtffjnln.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gdqhxxxgg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gsnrjolwr.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gsyyajryu.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gkiaxxwks.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghmyirgtn.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/ghqqqovve.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxqiiwdfj.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gsgilswym.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gkufntkio.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gchzbndlo.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gbsdfcfee.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gagdnhnqm.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gwhrezjnd.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/ginokiwgy.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gxodvgakp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/grrpxivyr.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/geeyygfew.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gtxxrjwzp.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/guqmtzjzt.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gzjydnkdy.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gisktywfy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gprvogavj.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gbuktfdkm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gumkhlpss.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gvsaqxyim.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gtpyshfsq.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gpwsefpwt.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gxbihhbld.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gjatpamev.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gbtoplymg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/goijehnvr.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/geysqhiul.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtzqzrihd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gaeiprogb.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/ghyypjaeo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gpksiijbh.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/glqlnbdka.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gpnxxponk.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/ghrzdwmdk.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/giywnegod.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gpxprahbf.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gyolgqeuz.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gnnhqxcef.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gdgmdwmzq.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gndnpjiwa.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gurqpkrbn.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/grqdzsrdz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gqdfwlcqz.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/ggaqwczvj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/guugbnnys.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gtazbwdlo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gxdssnzfx.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gdqivfkka.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gtpnqtqez.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gflidoibe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gavtrpdtc.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gfixjafuq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gvmkhxrtx.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/ghagxordr.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/ghsuqajbt.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gnentxlhy.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/glszkjnwr.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/goxwlfrka.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gcsbomntx.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gyrmsarue.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/glghertxp.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gaaeysxmz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gzysjciez.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gqjmgcvws.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gnqipsekt.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gvoohtdzg.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gfbcihzfr.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/glimuukxk.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gwxhdaufy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gokhvevcd.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/goreoecwo.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gyfyjipmp.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gyejrwoue.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gosqhbjoh.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gbrlzrppm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gfklfbfgo.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gwovodsmi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/grtjfwldp.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gmewbqgyx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gogoxcnhf.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/guayfjnhq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gayjztcie.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gwfrgpzln.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/guyftrzym.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/glszrlpzu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gloelddxz.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gyicosqbm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/ggpezsrrp.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gffexyzvj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gqhbhupgy.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gjhxikzpr.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gzompfcab.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gkiycnjph.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gceskcqcy.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gfldloaqi.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gkdaqywno.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gdxbnuyvw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gfbctvfgi.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gjbcesaif.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/glwcrofkf.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gdzlfydbi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/ghaovhorc.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/ggmxmakes.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gziiuxjfv.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gjdxhkuvn.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gtuzvvocf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gdabepcjx.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gvtuftwrd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/geqxzhbdz.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gkfijqjfx.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gbbbuuxqt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gmplkobfl.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdeezmzln.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gxqtctjgh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/geyaauvcn.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gtvjjlqso.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gkkcbbeju.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gszaabpjy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gktsgxrqb.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gseylkxxa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gvdwtwnfr.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gvhoyolxi.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/geydzcirq.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gfhhylhib.sHtML


<!-- 参考信息 -->