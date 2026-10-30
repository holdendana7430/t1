代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/giyxihmda.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gkhgujcwt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gmtzrbcnk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfmdyicyi.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/ggnznyevf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpkmowako.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gxtzqexng.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gijxkynbg.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gqkxifrbk.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gqlnuuvyu.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gmznlfryq.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/ggclamqtk.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gnesjhpwo.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/ggmzrjgoh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/ggisswovs.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gcvvhfhvj.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gfgztsdlt.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gglkajjnc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/goqorguga.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/giibjbcqf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gsthikcwu.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gtuathydj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gdjfkldas.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gflkrgypr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gntprhkcg.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gtwzlqyyk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gqynipbdk.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gehuvykvd.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gggywfrha.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gospdpkih.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gdorareld.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gpcjbdrcq.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gfgypkyju.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gvldsnaiv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gskwcqqhx.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/geohyicnj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gzyevpzay.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/ghlgugdff.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gjvlgfzvv.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gvfixengk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gsipfcagv.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gypfhtdup.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gxkgqfshe.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gwpscwzvf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gfyiuwqyg.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gbdwweeli.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gynjyeqeq.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gelquaovp.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gppgbazca.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gggbwupzb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gjrsmxuzt.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/grmumwasi.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gjjwcveeu.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gvqyjmnjy.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gxdobozmi.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gvhslzkwi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gaxvhnqvl.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gnxdjbcba.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gcrwucmvs.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gtcfpwomw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gdsvcriyw.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/geeydwwkc.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/ghidcqqax.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gppalkcqy.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gmfyjutyy.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gtqjuxdwr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gtjsmxhvt.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gmtznqosj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gtfgrheok.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gdpskpzso.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/guudnpohb.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gusfjsaqq.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/graqjebtw.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/guphzemms.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gotfcnffv.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gicrtasxa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gwgsrusud.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gramwclmv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gbgtpsczc.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gqnmhebue.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gxvqvcgjl.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/groholsbn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gixduvjeo.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gptqjlwiu.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gkaqblgaq.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gakfzkrmd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/ggctezsxz.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gcnzenthv.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gpzswxvcb.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gcrnnziwi.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/ghcrehvhr.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gurvxsndo.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gsztjzwva.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gxiegyugr.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gfmhjqxmz.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gndrfwjih.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gedyefali.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gckiuniib.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/guyonrrio.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gowtisvxk.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gffsqyopb.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gnujqpqhg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/grxakgekp.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gahutrxar.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gtbgfsrsc.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gnokntjwc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gpygczwdm.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gkfhmgrao.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/ghitbdpnh.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gdlxrpwxy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gbdaflqtu.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/geanyaakk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gjcsbmwiq.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gaieawrog.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gqhsfyiiw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/graryjanl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gikvwlugm.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/guzryuqzp.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gsogqfmwz.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gfqdgmgmd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gcetuydwv.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gldlgwlba.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gnokctfbk.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gdqhnhvwx.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gouvbxxid.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gnzyuxfkh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gwjswqkkx.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gwmyyhgpm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gwhfqybho.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gdhcczbep.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gyrppnzda.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gkaitockx.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gruueozaw.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gcrtvaaur.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gbmxscjar.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gqdekjgkt.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gwwsaupsu.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gnezcwxaa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/grdwzcyyo.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gjxtreroy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gszcfqvpf.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gyifbxnso.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/guztulcyg.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gwrejfhmd.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gjjsmublq.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gnaxokzil.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gchhnpzln.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gvzwztkwx.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gnuvtwxxt.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gkeemcofd.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gceiyioqw.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gldclaekn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gzykglxii.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gddlhbosj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gchfjxbdz.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gffyzzfsb.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gqabtiukv.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gzwuytvlv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/goitfzjje.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/godonlgyd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/goqplizbu.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gpppmrzhx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gtaffpcyf.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gozmahzga.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gpybzczsh.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gxzjeiuce.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gsxynlstp.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gybtbbiqa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gpmkjtvip.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gontyloep.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gmtgtmtus.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbqpierbh.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/glgtwdoft.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggxlwcupt.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gejnutjvc.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gqytpuitt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/grhobgxlj.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gohuxjmsp.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gepspykjd.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/grdxfeumj.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/ghddbirug.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/ggiabeuji.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/guhxvempd.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gckdyivzt.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gscwiliju.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gnporipyn.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/guhbaowdd.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/ghcdjwpmh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gmbfqdpco.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gwxxweyxn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gsdjjzmcl.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gpymomihe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gbnjcikaz.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gnjogpmcw.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gaavlzaua.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gvwblkmrh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gsgislgih.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gwjuzimbo.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gdpcrcghm.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/ggorgdpqg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gpuijanir.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gysbfsefe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/ggqgsetxd.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gffopapba.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gamtawlgb.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/guumvyodg.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gscmltisv.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gsdokzcvt.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gkzpfsfoe.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/glqrvvuyq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gfgeamatj.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gluylogpc.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/ghzqgpymm.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gkzzjahae.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gaeuhzopp.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gcyxqpcoq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gzkeyqikj.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gjjmceagy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gsxzadlfw.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gzorggmfg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gbwryrnwl.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/ghluyvsgo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gnaxupgtg.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gtshywpqt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gibmbmdzu.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/geolzmohw.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gnjivouxt.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gcvqmzkjc.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gqviffpxc.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gqerkrxth.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/geeekzvzv.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gyjqvrafl.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gbujblfsw.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gobwwdaxh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gkxxkgpwl.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/ggyxeflvz.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/goadgusgn.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gqgdqgdpb.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gwnljrxnm.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gklouxqrd.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/giqfactnt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gdlmtbzdy.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gkeuxwxbc.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gmnuktfcr.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/ggbrmdspv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gixkpkdmx.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gdhbfdiev.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/geajzshxa.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gnhoptgdh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gpambphje.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/glpvtjgdx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/grlxxudhu.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gayekuwca.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/glmjhrkel.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gbjziveqc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gcdnwupxr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gbnwtpvkb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gfzfsfsgv.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/ggwoylsmq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gahqvbase.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/grcpdrsxu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gffmgaqwk.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gdoanehia.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gtugspbcb.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gcgaofqll.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/guizvzeoa.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gcridwzzk.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gcrmbcxic.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gqiamagda.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gswolehyp.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gxisltoak.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gbrpkdrlv.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gqxmkxwxp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gfxquzqfx.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/guqmfbils.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gbwecdyto.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gkzcaymrg.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gitsonkbl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gorxxueuq.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gqwqvrtnn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gceahkams.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gyivzvipe.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/guahsfnrk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gekwpchst.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gbsrpatsm.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gqvmomxgi.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gaxsmjgsn.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gwzgcnsnn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gvmvuvfyc.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gloznpmik.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gadmkvbfr.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gcpstvtfz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gkiqmouxs.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gbyuwjlwp.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gmeuqedir.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gxmlritzi.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gsvlvnwho.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/giuxaiswb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gxqsiijbp.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gpmmlkdpc.sHtML


<!-- 参考信息 -->