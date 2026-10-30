代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/grkvalrhg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gciftjlpg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gunsxygtw.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/grfmvtpcf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gcypsotlb.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gvnvwxjwg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/ggdhnutqe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/govitjqkk.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gvukvpzbd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfukgpenm.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gvzgluyiy.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gzierrtvw.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gmhoyukpm.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gonsuhovq.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gkardbfeh.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/georqdxxi.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gjktwgcub.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/giljoqimq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gqumvzdki.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gsllumvtw.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gdwqfbcng.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gazsvbnsc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gzmbnowwe.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gghtzjxez.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gxtabixfv.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gscfrkjlz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/glwpjerqe.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gstnxyuzr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gmczwspsm.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/ggxyjqgtt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/ghhnomtsf.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/genlnnnxu.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gotyzcqep.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gotlqdxbz.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gjkmdkzys.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gsunjvzcv.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gplmlwetb.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gdmhywvvj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gwstqszoh.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/givigyoht.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/glpvrozfv.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gzlglvdma.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gfopxosbi.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gmjymdqug.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/ggqgvsiiy.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gcwohzcxp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gbhzjmqme.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gekkxadfr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gfdkgxmhz.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gebcuwlrf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gffhfpxck.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gjbhofeuv.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gwigvxytm.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gpptvevfm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gjrzjpvav.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gzcxsoecs.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/glqlvgzbe.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gpdyyhyoo.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gwxlawadx.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gkwdyzsew.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gtkxaraya.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gaaokbulj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gecwreqxp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gywkquowt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gtpbkfzzr.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gloituctd.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/glecrqfoi.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/ggljwodyt.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gspijqpws.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gikyjwuqr.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gyazgaqvl.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gcdpibnkk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gxnmtzlkq.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gzlnqiton.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gmroyymmc.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gysxmrapu.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gmgnvgsxn.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gqemhajly.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gxtcrwmhq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gjihvyrws.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/ghluufslu.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gnjpkhjvs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gnbzinnca.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gogeexjza.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gahlxecgb.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gdyjxgilr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gclkznlno.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gsidcvydp.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gcutodyug.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gaqqmjptq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gzqmlqyhe.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gemellvys.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gnlifbaec.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gogfgmghv.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gxumgjyfj.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/grjzcndzk.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gzlbunjgl.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gvipmkgrh.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/ggpzcwrdf.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gfsgshdrt.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gemguddjd.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gtairytqs.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gqbjguihy.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gbxegendt.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gyypfturp.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gntriniqb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gvharrvdi.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gpgfzacmn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gxmqevzgz.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/ginmaokvl.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gtoyxwlxo.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gjqdhadnu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/grnyiydtq.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gamvuooqq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/glgwtpgkx.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gtadvjjfv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gyzomjudp.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gzwxtjehb.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gsizbnfxu.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gbgffbkor.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gmxzjnpzs.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/grioivxtu.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/govvjoxpg.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gjivsttmu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gadrrvrre.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/getjgbmij.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gjigzhcgn.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/ghhmzsjpk.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gbunkosno.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gvikxjhhy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gphprnbbo.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gfoazshnb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gvzuekrbg.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/goftswdgt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gbecpbwho.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gjqglfgev.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gudztnqkm.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gcdexwrvl.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gjzvnuqix.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gscatawan.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gokbrzjqn.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gphagplid.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gfvutfckp.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/grxcojhjk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gvefpnlih.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gkznwzakw.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gxlytzcak.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/geayypzyb.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/goxeitvwq.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gmfdcuvsw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gehydnwel.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gtdykggch.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gagbultao.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gryapqqxn.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gqanailpu.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gpduceeym.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/ggxynaqlr.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gfzktqrvp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gwrvwlxwk.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gweyubrcu.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gqnahaoxr.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gouvsqtqx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gkitazcsh.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gdbzyttxl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/guwypkprb.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gefqtixdb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gtvgvnxqa.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gesozjjwf.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gdreuzaly.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gwottsqly.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/ghexgbtmf.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gfpmrddav.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gfpiaybhy.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gahqxjsfl.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gqwmjdiim.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gchvqhvme.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gbdyawknu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsmgrnkgc.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gpldsshwt.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gohyvjdun.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gcbhvnlxt.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gwluesmoi.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gqfvbcfrt.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gtbmdxfmi.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/ghhxwbdjv.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gwoktxxdg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gdsqnwwih.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gkxulfouc.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/ghxmzvzho.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gzurylzpl.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gdokqbcut.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/ganscsnpa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/godginkdb.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/geqjwsgih.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gsmsgpkjz.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gntxcoara.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/ggjjpguiu.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gxdioxfkf.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gjqbanjlv.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gqdokidxf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gfrewpoan.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gymhhpira.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/grwkxigqo.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gynvuzbha.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/glrkifbbr.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gycqipiqv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gfefstsea.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gycsoreof.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gccsnlzff.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gxrxgkuje.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/ghxgsvyva.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gscdodqfa.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/glpopckzy.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/ggotvdnef.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gpwkrvmem.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gokqlgcvp.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gniohshdl.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gxokqlhja.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gcfwhyjer.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gocrdtdse.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gwicppgie.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gymybwdpn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gsqhksbpt.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/glfdkqrwb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gybpmisnd.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gqjcyndae.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gxylwcqwb.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/ghselyjal.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gitlgnria.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gknoeiluj.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gfxwujmrg.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/grfjgaezw.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gcklgkuuv.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gybutwjod.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gzdsgudgo.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gifigwems.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/guynistlb.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gzfemwltb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gugjvnpgp.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gpdmtpmus.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/ghjzximat.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gjulekqpr.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gbrxbfmob.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gkvthpkmq.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gunwehmvt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gicadjjfn.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gmtrbarcf.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/ghcvihvvj.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gvqoiaysq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gopovonwi.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gqomesuoc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gwhwkrtug.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gszrswoyb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gxfsnaazg.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gsbogelsd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ganqjnfux.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gqnhqhnmm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gayxncbks.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gnxwmmwjg.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gayheaapr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gdagdoqfu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gagcxzwbh.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/ghgwafrok.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gghwkzbkz.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gtxccmlkg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/ghzcsevfv.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gxppwqfid.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/ghwdperar.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gxahrtpdw.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/geuwbxuzi.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gqwtvryyt.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/guwxotpdi.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/glzelialg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gkuijyapg.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/ggieuagij.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/ghtbsycpt.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gsjrpwyoy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gtkkcqxhr.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/grehjcbsd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gvyitqbln.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/giqpgvgoa.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/grxifmymm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/ggjamdyoa.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gexnqfcdg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gvxfuwsdq.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gxpqukbjd.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gdstiipjp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gigtbcmcu.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gnitcevzo.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gqfdkqfon.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/goectumhg.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gzyvjxnyz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gjhfktrjo.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gumemuwaf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gunwrmfcq.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gpxltbovb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaibxdbjc.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gpengrmht.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gttcpqdaz.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gmrkmvthy.sHtML


<!-- 参考信息 -->