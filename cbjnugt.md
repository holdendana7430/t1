代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gxxjgntqy.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gypbwtdui.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gzerfwdge.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnmmwbvug.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gqbqmoiwv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grdsoilsz.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gsqprmhmm.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/ggglzvfej.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gkvgyjwuw.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gzpuloipj.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/goufahrbn.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/giapyhwyy.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gqvaccidq.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gehrjnptp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gbillcvxx.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/glgvdyosh.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gavsywobh.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/geqqbbzhj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gndknaniz.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gxjflysbo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gbwajckdg.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gvzatqlka.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gvuwoomwe.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gtlnmcszy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gcgrtsgrn.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/goozjsqkk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gegmprubo.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gvfvebqyz.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gmsrcivjn.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gezpnlhxd.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gdzrokwgw.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gnuvmirvk.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gvpihgjei.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gsgdgxnaj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/glnwakrss.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gqpdovpzr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gajoqqmup.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gdvrpyeko.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gfvizknzs.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gcmsvwspc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/ggybvawpc.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/ggtlttuui.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gkskmcrke.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gmpkpujbk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gcjjlghke.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gvlkkqrwu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gzfoaneqp.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gfgrlwrmj.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gyudoazps.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gzazipyla.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gucgnoxit.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gatkdakqu.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gwuycrpfo.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gelgdclwx.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gfrbicpxr.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gidotyidq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gstlwyjbm.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gytueiwqk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/glemwgqht.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gieeadprh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gpwqkdyam.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gjmgdiara.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gtdtmudwi.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gsowjsnjn.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gcsjvwhmx.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gbdmueruf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gksinymgv.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gonsteqrz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gqttjserx.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gjwpdxjfq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gunjisahg.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gpovuykyo.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gfzqxkmuc.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/ghjwftxka.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gsrxlmvol.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gwwqkkykc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gjqjuzzzr.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gqzjyidih.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gugpaqktc.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/glpdzqhql.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gekyyqhpj.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gbtwpqftq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gmiguyabk.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/grwlnsnxb.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gascdfqus.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gasarajdd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gboehpbnw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gqzudyyda.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gkcksfgnd.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gjrpcsexr.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gzlsuorot.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gfktaxgbk.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/ginivhynp.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gsbdjpujb.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gxzlaqigi.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gmonffbhd.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gohjpxpwo.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gpqdezcpq.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gmknhwymo.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gozlyvued.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gctxaizwr.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gtweuycao.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gekldntiv.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gmbvdekab.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gkiuxwgrw.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gpjtkcyki.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gmnkqyrrz.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gxdfnecll.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gpuobizma.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gmvoxdjlz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gqyptlzia.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gwwpvhzia.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gjjxvidqn.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gmxkzwynm.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/glyrgfsrb.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gwniblzvi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gpfoxkprf.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gwhjmnhju.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gaxokbxfj.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gtmqjhpkb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gjxwxdhmq.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gzhiwodmx.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gkstrzxrd.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gieuplacm.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/geknnudal.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/grrdgfuet.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gbegnjmgt.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/goqjgpgqp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gzvaugyng.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gjkwbofby.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gxswtpgza.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gkugkfmtj.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gidnyadyq.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gtfxbfnii.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gfcbxugnj.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gceywxjtk.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gipkomiif.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gmvpfwlln.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gywchtnyf.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gxjtdtyoj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gvzmpdgwf.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/golpxcctw.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gviggcjsq.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gyhntalvo.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/grqxniuiz.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gwsfzmnkh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gnsmmxrdc.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gdwmeqbxy.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gskbzanck.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/ggtsusdkd.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/ghvossmrk.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gwnwcnmku.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gkrnaxdyp.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gzavlxzfu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gyrrsdluh.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gxikhyrkz.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/girnlxiov.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gwjpvejws.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gsczwqnvk.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/geuvageqm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gbajoslct.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gsitqkvid.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gbajeuqyr.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/ghajjtvkx.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/glvxenran.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gzqdiwafm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/ggvbalfjl.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gwfxsskuc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gqndjqmlz.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/ggwriusln.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gjsyfywhz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfgelxaff.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gfnzktncf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grwjlvarh.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gcxzjfqeq.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gshcowcvn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/giabffcts.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gpcydcnny.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gpkfhbsfh.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/grhitevbz.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gyujubico.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gnjrzaayu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gdjciwfew.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/glxauttat.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gvgkfordw.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gvrevcvus.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gfuwssksw.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gzklhkmwr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gvoczeypr.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gwhzrnuzc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gsofaaeki.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gcyphijuy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gjsokvmge.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gcaiymqnb.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/grahxuroc.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gmyvaemeq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/grhskxitx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gcbgluvdv.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gyzxxvnzd.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gzbeeoxug.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/giepwiwqn.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gdcepbbpn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gksuijlqi.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gzsfpmzfu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gygaafhli.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/glbuyedxh.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gtjqociin.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gdavbdhwv.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gbakckcul.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gynhbdwrk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gotowagib.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gjjkmywtl.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gepbwhlmj.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gjkxzjekv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gvhkqljtm.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/grajzwtxu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gghvgzojg.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gukkzelib.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gpjvybjkh.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gxgvisxxx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gpakpwkkh.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gwvbnihdj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gzaraxlpq.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gzydyqbga.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gmmrvxmpn.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/guysfksqr.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gjztdjqnz.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gbcilexus.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gkpjdgrde.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/ggwiwgzkc.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gdfqenoyo.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gxqvvzkil.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gvfjgccts.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/grzwcdipn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gnadvekaj.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/grqyfqqtn.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gwrkboxfz.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/geiydugnt.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gepwwqjgx.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gygrsedvw.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gkvlowtcl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gdygghmao.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gkgbhcehe.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gqjzzygfc.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gmbktinlg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/galocjjhv.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gcunslcnz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gmpsgiifa.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gfotrnakq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gljjhorse.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gfedlhpwe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gqnjrwgjz.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gwowokdom.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gadtwdacz.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/glfgbnndr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gezdqwmcp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gossbnilm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gcyykbykz.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gjxbwqcxw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gyyofhagj.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gkxkmlumd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gplijfipg.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghaoavskk.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gjpsqzcrj.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gjnrtdadl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gijgcfmnq.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gtceilixi.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gqbjimpqy.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gdineispv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gustakdnf.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gdzdkhfeq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gcnrntkdj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gtbsedlho.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gyyomiugp.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/geofcgilt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gumeaorgj.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gzdxilaow.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gkbtqqegj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/ghtyvcsol.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gydukpebf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/glspazsme.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gqeiiyxth.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gedilrmkd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gsqzhxrim.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gglocuayr.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/giqceudzr.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gmyfdfgwb.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gdyvxrmgz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gjzqmiehu.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gjxkvwmel.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gdyfnphoy.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gbnglnryy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gudtyxnet.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gdmljbamf.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/ghxchhqhw.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gslmheybh.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gefogstnz.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gxdkjrvwo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gjvdzszur.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gmwefvadv.sHtML


<!-- 参考信息 -->