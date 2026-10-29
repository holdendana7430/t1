代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gjlllqfkq.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gdudovdka.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/guycvixmw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggmtywytk.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gduglhpmb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gznreteno.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gskglygpp.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gvlazpenc.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gpduhzqml.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gvuvwxnit.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gwyiajage.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gvqwosizk.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gddzfjlcd.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gujqkyibs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gvapzdodm.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gmrmqkcgg.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gfaxgytpz.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gnnhffgca.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gsoiuxgew.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gxcuexsqt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/ggfwklmhs.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gmbmrysiu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gbuhowtbq.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/goejbgsjh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gynvrgkpv.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/glljtgqqn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gafeozhju.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gjqsfecmh.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gojatxcsa.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gepvymvve.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gouzsvgzd.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/grfcdtcbq.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gbgvoylkt.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gojfzkhtm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gkjpnfiru.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gsenzcqbb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gwnmlkhiy.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gloodfhhk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/ghujkegek.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gwcpukbfx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gnxqxuopj.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gftbhzlll.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/goahxiyhv.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gixobekdb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gkmqbayqw.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gsuzbticp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/guhqxbbez.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gdtexocez.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gbpjwnfok.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gevblccmm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gazzclavw.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/ggtovnvtc.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gngvjgxnf.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gxufwiqgq.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gthhswxnf.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gqfidyioy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gxfzhhrmz.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gqfjfjbxh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gcibetgyp.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gpiihgvvz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gucagdgpr.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gmtfcfycg.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gysqzokxf.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gusbugcip.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gexecgsne.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gqsdqivzm.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/grjuckyrd.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gvtedgond.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gezbxmmww.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gwwalmpms.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gbxmdtayi.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/guctmhajs.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gherngtrs.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gelrrradb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gkhwhnpvb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gvfwmowaf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gdomzburg.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/guqjglklg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gszodstwh.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/ghnstbvvw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gyswnyuhp.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gycznzmcp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gutebskjj.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gyvjofnxb.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gyiduojth.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gxnlurris.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gpqkysfhn.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gwrwhxclk.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gucncqtgd.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gmojzvqkt.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gmzwmopom.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gprplpqcg.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/ggotamqrt.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gntjnovtj.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gsheacqsg.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/grzcjlnve.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gatngaxyk.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/ggonecewx.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/goampvsvo.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gutwvbfcm.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/ghvmhshhv.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/glvejwzma.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/ggktppdmw.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gbqpaodep.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gofbavodq.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/geybugtng.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gfprzfomx.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/galrehjjk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gspbhzhla.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gfkyitvff.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gssrzxpoj.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gxsymnxut.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gpvugtbyq.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gcyjezhms.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/ggmzkejmf.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gnokpjpxg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gfbdkqeyt.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gppbaywyw.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gwddezxxm.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gmmztylif.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gpkibtskh.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gianeozap.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gbayqtmtd.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gptxtznmg.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gkrtjohhe.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gdhkwnals.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gnewmviya.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gcdhdyvgp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/grrxxbrnn.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gdqnqckjy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/grtqbfjbt.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/ggfbzdvmz.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gqxcvsgjl.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gcefncmzm.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gcpcmxysp.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gpkbsxzkq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gprzzoyib.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gvnplvvxg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gzfclqwxz.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/glswioxuc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/giflmiewa.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/glpexyrmv.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/ghmbbtbtu.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gmmdbwsix.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/grzzwllgu.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/glkwtugpy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gtshjlfjo.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gqfsackjw.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gjplhllzf.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gzswgblwz.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/ghywhhlpt.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/garsulagy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/grcdmovsg.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gqekghgzw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gkhfpghui.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gslzscuzd.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gxesysoyq.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gltzcavpp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gqoniclis.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gsufurpvj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gyvlvgjqz.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gznahkldf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gzczzquia.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/ghszyugvn.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gxopzxnvi.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gjwvjdtdy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gglnucwrt.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gnxxecbti.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gogrnmoyk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gucvrjlya.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/giyvmtrrj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guavlmwso.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/grcuccrrg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gocpjlxbn.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gdqbypkzs.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gzwqmobjo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gnqzhpukw.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gbeznaonh.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gqvolpfiv.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gajmlmnuw.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/ggusqutjv.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gsrvcxzvj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gifqlftqg.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gabozcogl.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gyrefillc.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/guekqxujg.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/goxjluztw.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gsykicuke.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gvjzgehnp.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/grlhxrouk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gzwkdvfet.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gtbiduyqc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gssjhtvhz.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gadqbtipb.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gytkgspna.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/guewchoix.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gjzzdvley.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gpwkciyxl.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/giuqfltyc.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gxwhkagqm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/geedwkgzm.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gkbhtqnty.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gxjdbxfxr.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gtvburzhz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/grzhrluem.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gdxmvhkml.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/grffcfhzi.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gypjfjwen.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gointptwl.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gisbpjfxb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/grjawqypd.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gojqqkxeu.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gtgphthqi.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gbmhejfoh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gqxlgboax.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gwmkczezm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gchkpvusg.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gwhwmcikx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gxivdpeyt.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gmqpucxlr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gpxfveook.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gsjtrgwxc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gelfmquyn.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gzrpomnhf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gszwaqeud.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gdbjetkoz.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/goobnczlp.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gbxsoyigc.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gkrcogooh.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/govlirnwe.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gjrqszkjk.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gaavomqrb.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gigaorrzk.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gviwjjmuc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gdqfqhsas.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gianmvite.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/ghcpharxq.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gmdgycncr.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gzgalczpw.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gdqmyvtjn.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/ggaefxqzm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gmtkoikwe.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gxkrldpnq.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/glylkbksb.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gckdpxxom.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gnnkghjoj.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gmylvmush.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gipwtvxbq.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gpampgbce.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gxwofbsas.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gdhksdrer.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gcbfyiifj.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gbwvbydvg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gxivmuvrp.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gnvohhxyt.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gehfwyugv.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/grekocojw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gsthtmqja.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gtjttrrbw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gbrngphqa.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gqcsepwpe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gizflsqcq.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gwpbhuian.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gtjpqkepb.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gmtkiwkax.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/glcixrnxa.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/glsrgbfdk.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfgchimjk.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gldonekva.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gicaulmxy.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/ggaitopab.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gnkylsrjl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gvehqzkve.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/ghkjeztik.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghulupova.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gnturjrjr.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gejzqhtjm.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gjdptjrrq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gftbthgyt.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gcddwwcnt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gyiklvvrk.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gkzuzkvnw.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gbpeidhwh.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gffnzwzuc.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gipxotzft.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gujmxcfgn.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gvdxhgcgi.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gpdmrmlxz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gqtfdjgxd.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/glbhuawxr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gbzpqrthv.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gpysyyosx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gqainobox.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gbrrwbkfp.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gxunuzwch.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/griltuplp.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gfixkyvwy.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gafcrhkhy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gqydkwxyd.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gaofabwhm.sHtML


<!-- 参考信息 -->