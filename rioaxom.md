代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/goaqprjxg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gsftztkpr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/ggdtmenlg.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/glmiwinsg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gutrmbolp.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gotfxpmsa.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gvwoovscg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gurbnqytl.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gwpiidyqr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gycefdppl.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gwypeqdhq.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gbzwqwxoq.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/grpokvwqx.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/geynpayoq.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/grdgudjeb.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/guhhmcikv.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gwxpivzzt.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gzbajgwjp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gcjicsnll.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gstenomza.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gycijeozg.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gfdxsgjhg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gowthizij.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gbvxrumay.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gyeperotg.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gedeucowm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gngyghvfw.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gjujwqxjo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gvedlviwa.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gpeqpootl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/grqwdivkx.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/ggfdndojx.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gdgypsvyp.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/ggcotzspt.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gfzqrvvov.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gepfbiifo.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/ghrakmsfu.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gajtyklev.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gslkayter.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/ghsnqudlr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gzadcsrue.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gznspwpnw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gftseqjbk.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gyhasbvll.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gpipajbct.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gmurpfzfs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gihumxqwr.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gqumdxpgz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/giltsttuv.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gpcsptold.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gvohjkxgd.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/ggqgckwuz.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gtlvzecqs.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/glfmpoeqx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gyhvxnuaa.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/giirnbmgr.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gvfbmljxi.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gsnhkicgk.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gsnggnqdp.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gpwnpzqoz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gjojgptwj.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gclbueasf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gmwcykkbo.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/ggejhupat.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gvrtnkaku.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gfppobtft.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gmjrtmhdq.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/ggbypkjbq.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gwzngspxm.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/grgzpivtk.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gmmdgjczh.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gaujyykpt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gwaihzkdh.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/galoyzxoy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gixhxnpic.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gzemsyjws.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gvrjrfbbi.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gqoccilwn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gawubxadf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/ghgsdojqf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gatjuqiux.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gxrvgyokl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gqqkuzoxk.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gyzlsbvuv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/ghqwjatrq.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gekwwemes.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gcdvxbfcc.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/ghovltovc.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsqziazfx.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gdzscfyje.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/grspdvemu.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gasiqlozo.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gkofgzltj.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gfmupaege.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gppvmpelf.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gdkzbecfj.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gcmkxooqa.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gliaxnkfd.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gujrgooqg.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gvzgnfdvd.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gnowenshj.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gavduqgpl.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gjbqsbwmg.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gbzvccrne.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/glmpiualr.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/guirhsydf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gafeecoxn.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gzjnowldc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gbmlglyom.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gvwnpcrlg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gekkvkeow.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gbxbpumwc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gwsadjtok.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gumqgbmcv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gpbnretji.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gqthcfmte.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/ggymwzbsg.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gcnompvrp.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gtkwgalqp.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gfoysgtay.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gmkknjusu.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gojegfdrj.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/geoonblhk.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gzrigjrym.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/govczxzwp.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gwsoutdzj.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gervtasna.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/ggdrbkkir.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gckligdxd.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gqjyvrmih.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gdcnpodxq.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/glljpsemd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gjfgkglun.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gvjqbflue.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gtwxxvkpg.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gpekdtckg.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gdpkgbsqt.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gamxayjar.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gcbwmmqwv.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gdwqnkpkp.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gsjjhjpjm.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gthxbdqnd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gnmoxfokw.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gtgveehzq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/grtswtqwa.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gvusfwhjp.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gokekdfxc.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gspkmjnvx.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gyxablrzw.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/ggxwxyxbd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gbiezuyeo.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/grqyhfuqe.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/grtvihmng.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gbjmkcrhy.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/giybisrhe.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gbxqvkqrq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gtoaaixai.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/guriozroe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gkzzbsxbi.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/giweiycsi.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/ghbexwvsr.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gsbmdeoeh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gtvgzroft.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gprlxssee.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/grvzfvijb.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gdzrtaqqi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gwhezlxug.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gbcqfwbhs.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gjdpuiiip.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gglmdydwx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/goyhjynbc.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/glqqtprrk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gdahtojkg.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/guwokyqko.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gacenhtqt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxilixeku.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/guzhxgsaj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggpmerpux.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gouobvqok.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gklubulpu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/grpeuvvqx.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/giphvfmog.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gpnfftkpe.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gfwqzvlmx.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/ggcdfkwcv.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/goibkaawa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gxindkuht.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/glmfwnhyx.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gkwajfglh.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gmxhhmrmd.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gurbmsbag.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gfjdfcrjr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gzungdiee.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gwrapgcfk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gpvntqezc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gphotibsu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/giarcqdbo.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gjcdvhiyh.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gqiwxlser.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gdflsubmo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gmnkcdmqr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gdjcopvfp.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gghlizjuu.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gisxzjuaq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gzsfmwfcu.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gxcqrgzjk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gehptgxyo.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gjstaoqfh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gmxezrzwf.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gasfsfuyw.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gxsjbvcjb.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gexzrisky.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gkckmjhub.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gtkdoeodp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gscvhyoow.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gncxtdmfe.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/grvvfwatp.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gblsrpqmi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gjyjrakff.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gttliczno.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/geckjqstz.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/girxqesbh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gxnsstabs.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gspbjsuso.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gzphbwwmy.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gicaakwoe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gxpzyuiji.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gtoecarez.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/ggnsqkmkk.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/ghfsllxmy.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gpzycnhhj.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gugtblpgb.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/guubonutg.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gjkucaamv.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/ghjxdwjof.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gpamuqgyd.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gwdufidwz.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gtfpqszxp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gyjukkpub.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gzcsjodls.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gciuwnfwy.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gjyeikiyj.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gogjyldyo.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/groujvsit.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gzvvbuylk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gwwlzccvj.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gdjakmigv.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gqccvixgy.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/glnxogxxk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gurclquzc.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gaxmeqqhl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gjeomvbpl.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gqddntuhd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gvexjupzi.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/ggxavfaja.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gmlffjkjo.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/ggaewvuxu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/ghrmwxycb.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/goiekyswx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gvptxipxr.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/grwppyuuu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/guiqfmpoe.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gboislqhy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/glgwabuqa.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gejzpajnu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gjjhbyilt.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/grgiilhko.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gvuwxqgwh.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gfoxhrqah.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gdofsxmny.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gfwshbsma.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/giqfwzzjk.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gxkqoxjdj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gtzgbvkxl.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gbauwvskx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gsxogiruh.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gbrcccjvx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gnwnqfqte.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzekabzzn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gbrbhbgby.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/glottzxli.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gchdwhcez.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gcivxzrto.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gtaiudzii.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gglxfuckb.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gpvmbltrc.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gomthzgzm.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gscbxmjpf.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gygondrtt.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gmsokvyzk.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gdbltugvr.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gfvbdblvc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gxqpedahe.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gohdwcutm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gmmrbabqt.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gdxlxgvfv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gbshpdyyb.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gqhgtflsn.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gkpiqfaye.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gpuwruqvv.sHtML


<!-- 参考信息 -->